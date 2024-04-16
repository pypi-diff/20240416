# Comparing `tmp/pygamepal-0.3.0.tar.gz` & `tmp/pygamepal-0.3.1.tar.gz`

## Comparing `pygamepal-0.3.0.tar` & `pygamepal-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/cameraExample.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/fullExample.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/gameExample.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/inputExample.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/particlesExample.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/spriteImageExample.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/spriteImageShowcase.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/transitionExample.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/transitionShowcase.py
--rw-r--r--   0        0        0  2811327 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/gifs/particlesExample.gif
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/images/character.png
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/images/character_spritesheet.png
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/images/chest.png
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/__init__.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/camera.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/drawText.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/flatten.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/game.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/input.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/module.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/particles.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/splitTexture.py
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/spriteImage.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/textureList.py
--rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/transition.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pygamepal-0.3.0/templates/gameTemplate.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pygamepal-0.3.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pygamepal-0.3.0/LICENSE
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pygamepal-0.3.0/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pygamepal-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pygamepal-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/cameraExample.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/fullExample.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/gameExample.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/inputExample.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/particlesExample.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/spriteImageExample.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/spriteImageShowcase.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/transitionExample.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/transitionShowcase.py
+-rw-r--r--   0        0        0  2811327 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/gifs/particlesExample.gif
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/images/character.png
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/images/character_spritesheet.png
+-rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 pygamepal-0.3.1/examples/images/chest.png
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/__init__.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/camera.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/drawText.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/flatten.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/game.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/input.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/module.py
+-rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/particles.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/splitTexture.py
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/spriteImage.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/textureList.py
+-rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 pygamepal-0.3.1/src/pygamepal/transition.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pygamepal-0.3.1/templates/gameTemplate.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pygamepal-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pygamepal-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pygamepal-0.3.1/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pygamepal-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pygamepal-0.3.1/PKG-INFO
```

### Comparing `pygamepal-0.3.0/examples/cameraExample.py` & `pygamepal-0.3.1/examples/cameraExample.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/fullExample.py` & `pygamepal-0.3.1/examples/fullExample.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/gameExample.py` & `pygamepal-0.3.1/examples/gameExample.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/inputExample.py` & `pygamepal-0.3.1/examples/inputExample.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/particlesExample.py` & `pygamepal-0.3.1/examples/particlesExample.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/spriteImageExample.py` & `pygamepal-0.3.1/examples/spriteImageExample.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/spriteImageShowcase.py` & `pygamepal-0.3.1/examples/spriteImageShowcase.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/transitionExample.py` & `pygamepal-0.3.1/examples/transitionExample.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/transitionShowcase.py` & `pygamepal-0.3.1/examples/transitionShowcase.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/gifs/particlesExample.gif` & `pygamepal-0.3.1/examples/gifs/particlesExample.gif`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/images/character.png` & `pygamepal-0.3.1/examples/images/character.png`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/images/character_spritesheet.png` & `pygamepal-0.3.1/examples/images/character_spritesheet.png`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/examples/images/chest.png` & `pygamepal-0.3.1/examples/images/chest.png`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/src/pygamepal/camera.py` & `pygamepal-0.3.1/src/pygamepal/camera.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/src/pygamepal/game.py` & `pygamepal-0.3.1/src/pygamepal/game.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/src/pygamepal/input.py` & `pygamepal-0.3.1/src/pygamepal/input.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/src/pygamepal/module.py` & `pygamepal-0.3.1/src/pygamepal/module.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/src/pygamepal/particles.py` & `pygamepal-0.3.1/src/pygamepal/particles.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 class Particles():
 
     def __init__(self,
                  # emitter attributes
                  emitterPosition=(0, 0), emitterSize=(0, 0),
                  emitterLifetime=100,
                  emitterVelocity=(0, 0), emitterAcceleration=(0, 0),
-                 emitterParticleDelay=200,
+                 emitterParticleDelay=5,
                  # particle attributes
                  particleVelocityMin=(-1,-1), particleVelocityMax=(1,1),
                  particleAccelerationMin=(0,0), particleAccelerationMax=(0,0),
-                 particleLifetime=20,
+                 particleLifetime=100,
                  particleSize=20,
-                 particleSizeDecay=1,
+                 particleSizeDecay=0.2,
                  particleColors=None
                 ):
         
         self.particleList = []
         
         self.position = emitterPosition
         self.size = emitterSize
```

### Comparing `pygamepal-0.3.0/src/pygamepal/splitTexture.py` & `pygamepal-0.3.1/src/pygamepal/splitTexture.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/src/pygamepal/spriteImage.py` & `pygamepal-0.3.1/src/pygamepal/spriteImage.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/src/pygamepal/transition.py` & `pygamepal-0.3.1/src/pygamepal/transition.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/templates/gameTemplate.py` & `pygamepal-0.3.1/templates/gameTemplate.py`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/LICENSE` & `pygamepal-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/README.md` & `pygamepal-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pygamepal-0.3.0/pyproject.toml` & `pygamepal-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pygamepal"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Rik Cross", email="rik.j.cross@gmail.com" },
 ]
 description = "A library of classes and helper functions to support game development in Pygame"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pygamepal-0.3.0/PKG-INFO` & `pygamepal-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pygamepal
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library of classes and helper functions to support game development in Pygame
 Project-URL: Homepage, https://github.com/rik-cross/pygamepal
 Project-URL: Suggestions and bugs, https://github.com/rik-cross/pygamepal/issues
 Author-email: Rik Cross <rik.j.cross@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

