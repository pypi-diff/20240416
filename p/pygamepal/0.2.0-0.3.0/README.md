# Comparing `tmp/pygamepal-0.2.0.tar.gz` & `tmp/pygamepal-0.3.0.tar.gz`

## Comparing `pygamepal-0.2.0.tar` & `pygamepal-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,31 @@
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pygamepal-0.2.0/examples/cameraExample.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 pygamepal-0.2.0/examples/fullExample.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 pygamepal-0.2.0/examples/gameExample.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 pygamepal-0.2.0/examples/inputExample.py
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 pygamepal-0.2.0/examples/spriteImageExample.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 pygamepal-0.2.0/examples/transitionExample.py
--rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 pygamepal-0.2.0/examples/transitionShowcase.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pygamepal-0.2.0/examples/images/character.png
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 pygamepal-0.2.0/examples/images/character_spritesheet.png
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 pygamepal-0.2.0/examples/images/chest.png
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pygamepal-0.2.0/src/pygamepal/__init__.py
--rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 pygamepal-0.2.0/src/pygamepal/module.py
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 pygamepal-0.2.0/src/pygamepal/transition.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pygamepal-0.2.0/templates/gameTemplate.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygamepal-0.2.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pygamepal-0.2.0/LICENSE
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 pygamepal-0.2.0/README.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pygamepal-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 pygamepal-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/cameraExample.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/fullExample.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/gameExample.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/inputExample.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/particlesExample.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/spriteImageExample.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/spriteImageShowcase.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/transitionExample.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/transitionShowcase.py
+-rw-r--r--   0        0        0  2811327 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/gifs/particlesExample.gif
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/images/character.png
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/images/character_spritesheet.png
+-rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 pygamepal-0.3.0/examples/images/chest.png
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/__init__.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/camera.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/drawText.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/flatten.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/game.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/input.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/module.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/particles.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/splitTexture.py
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/spriteImage.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/textureList.py
+-rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 pygamepal-0.3.0/src/pygamepal/transition.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pygamepal-0.3.0/templates/gameTemplate.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pygamepal-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pygamepal-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pygamepal-0.3.0/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pygamepal-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pygamepal-0.3.0/PKG-INFO
```

### Comparing `pygamepal-0.2.0/examples/cameraExample.py` & `pygamepal-0.3.0/examples/cameraExample.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,114 +1,117 @@
-#
-# pygamepal, by Rik Cross
-#  -- homepage: github.com/rik-cross/pygamepal
-#  -- MIT licenced, free to use, modify and distribute
-#  -- run 'pip install pygamepal' to use
-#
-# instructions:
-#  -- arrow keys to pan
-#  -- z/x to zoom
-#
-# Image credit - Cup Nooble
-#  --  cupnooble.itch.io/sprout-lands-asset-pack
-#
-
-import pygame
-import pygamepal
-import os
-
-# initialise Pygame
-pygame.init()
-
-# setup screen to required size
-screen = pygame.display.set_mode((680, 460))
-pygame.display.set_caption('Camera Example')
-clock = pygame.time.Clock() 
-
-# add input, to allow camera control
-input = pygamepal.Input()
-
-# load a texture
-texture = pygame.image.load(os.path.join('images','character.png'))
-
-# create surface for the camera to draw
-cameraSurface = pygame.Surface((200, 200), pygame.SRCALPHA, 32)
-
-camera = pygamepal.Camera(position=(300, 100),
-                        size=(300, 300),
-                        zoom=5,
-                        # the camera center
-                        target=(0, 0),
-                        borderThickness=4,
-                        backgroundColour='gray10',
-                        # lazy follow
-                        followDelay=0.9)
-
-input = pygamepal.Input()
-
-# game loop
-running = True
-while running:
-
-    # clear screen to Cornflower Blue
-    screen.fill('cornflowerblue')
-
-    # advance clock at 60 FPS
-    clock.tick(60)
-
-    # respond to quit event
-    for event in pygame.event.get():
-        if event.type == pygame.QUIT:
-            running = False
-
-    #
-    # input
-    #
-
-    # arrow keys to pan
-    if input.isKeyDown(pygame.K_LEFT):
-        camera.target = (camera.target[0]-1, camera.target[1])
-    if input.isKeyDown(pygame.K_RIGHT):
-        camera.target = (camera.target[0]+1, camera.target[1])
-    if input.isKeyDown(pygame.K_UP):
-        camera.target = (camera.target[0], camera.target[1]-1)
-    if input.isKeyDown(pygame.K_DOWN):
-        camera.target = (camera.target[0], camera.target[1]+1)
-    # z/x to zoom
-    if input.isKeyDown(pygame.K_z):
-        camera.zoom -= 0.1
-    if input.isKeyDown(pygame.K_x):
-        camera.zoom += 0.1
-
-    #
-    # update
-    #
-
-    input.update()
-    camera.update()
-
-    #
-    # draw
-    #
-
-    # don't forget to clear the camera surface!
-    cameraSurface.fill((0, 0, 0, 0))
-
-    # draw multiple images to the surface to be rendered by the camera
-    for i in range(0, 200, 25):
-        for j in range(0, 200, 25):
-                cameraSurface.blit(texture, (i, j))
-
-    # draw the images (without the camera) 
-    screen.blit(cameraSurface, (0, 0))
-
-    # draw the instructions
-    pygamepal.drawText(screen, 'Arrow keys to pan, z/x to zoom', 300, 60)
-
-    # use the camera to draw the images on the cameraSurface to the screen
-    camera.draw(cameraSurface, screen)
-
-    # draw to the screen
-    pygame.display.flip()
-
-# quit Pygame on exit
-pygame.quit()
+#
+# PygamePal, by Rik Cross
+#  -- homepage: github.com/rik-cross/pygamepal
+#  -- MIT licenced, free to use, modify and distribute
+#  -- run 'pip install pygamepal' to use
+#
+# Instructions:
+#  -- arrow keys to pan
+#  -- z/x to zoom
+#
+# Image credit - Cup Nooble
+#  --  cupnooble.itch.io/sprout-lands-asset-pack
+#
+
+import pygame
+import pygamepal
+import os
+
+# initialise Pygame
+pygame.init()
+
+# setup screen to required size
+screen = pygame.display.set_mode((680, 460))
+pygame.display.set_caption('Camera Example')
+clock = pygame.time.Clock() 
+
+# add input, to allow camera control
+input = pygamepal.Input()
+
+# load a texture
+texture = pygame.image.load(os.path.join('images','character.png'))
+
+# create surface for the camera to draw
+cameraSurface = pygame.Surface((200, 200), pygame.SRCALPHA, 32)
+
+camera = pygamepal.Camera(position=(190, 100),
+                          size=(300, 300),
+                          zoom=5,
+                          # the camera center
+                          target=(0, 0),
+                          borderThickness=4,
+                          borderColour='white',
+                          backgroundColour='gray10',
+                          # set a clamp rectangle that is the size of
+                          # the set of images to be drawn
+                          clamp = True,
+                          clampRect = (0, 0, 200-13, 200-9),
+                          # lazy follow (between 0 and 1)
+                          followDelay=0.9)
+
+input = pygamepal.Input()
+
+# game loop
+running = True
+while running:
+
+    # advance clock at 60 FPS
+    clock.tick(60)
+
+    # respond to quit event
+    for event in pygame.event.get():
+        if event.type == pygame.QUIT:
+            running = False
+
+    #
+    # input
+    #
+
+    # arrow keys to pan
+    if input.isKeyDown(pygame.K_LEFT):
+        camera.target = (camera.target[0]-1, camera.target[1])
+    if input.isKeyDown(pygame.K_RIGHT):
+        camera.target = (camera.target[0]+1, camera.target[1])
+    if input.isKeyDown(pygame.K_UP):
+        camera.target = (camera.target[0], camera.target[1]-1)
+    if input.isKeyDown(pygame.K_DOWN):
+        camera.target = (camera.target[0], camera.target[1]+1)
+    
+    # z/x to zoom
+    if input.isKeyDown(pygame.K_z):
+        camera.zoom -= 0.1
+    if input.isKeyDown(pygame.K_x):
+        camera.zoom += 0.1
+
+    #
+    # update
+    #
+
+    input.update()
+    camera.update()
+
+    #
+    # draw
+    #
+  
+    # clear screen to Cornflower Blue
+    screen.fill('cornflowerblue')
+  
+    # don't forget to clear the camera surface!
+    cameraSurface.fill((0, 0, 0, 0))
+
+    # draw multiple images to the surface to be rendered by the camera
+    for i in range(0, 200, 25):
+        for j in range(0, 200, 25):
+                cameraSurface.blit(texture, (i, j))
+
+    # draw the instructions
+    pygamepal.drawText(screen, 'Arrow keys to pan, z/x to zoom', 190, 60)
+
+    # use the camera to draw the images on the cameraSurface to the screen
+    camera.draw(cameraSurface, screen)
+
+    # draw to the screen
+    pygame.display.flip()
+
+# quit Pygame on exit
+pygame.quit()
```

### Comparing `pygamepal-0.2.0/examples/fullExample.py` & `pygamepal-0.3.0/examples/fullExample.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-#
-# pygamepal, by Rik Cross
-#  -- homepage: github.com/rik-cross/pygamepal
-#  -- MIT licenced, free to use, modify and distribute
-#  -- run 'pip install pygamepal' to use
-#
-# Instructions
-#  -- arrow keys to move player
-#
-# Image credit - Cup Nooble
-#  --  cupnooble.itch.io/sprout-lands-asset-pack
-#
-
-import pygame
-import pygamepal
-import os
-
-#
-# load spritesheet and split into separate images
-#
-
-# load a texture
-texture = pygame.image.load(os.path.join('images','character_spritesheet.png'))
-# double the texture size
-texture = pygame.transform.scale(texture, (texture.get_width()*2,texture.get_height()*2))
-# split texture into a 2D list of sub-textures
-splitTextures = pygamepal.splitTexture(texture, 96, 96)
-
-#
-# chest (just an image)
-#
-
-chestImage = pygame.image.load(os.path.join('images', 'chest.png'))
-chestPosition = (200, 200)
-
-#
-# create a new game
-#
-
-class MyGame(pygamepal.Game):
-
-    def init(self):
-
-        # set window properties
-        self.size = (800, 500)
-        self.caption = 'Full game example'
-        
-        # create an input object
-        self.input = pygamepal.Input()
-
-        #
-        # create a player sprite
-        #
-
-        self.player = pygame.sprite.Sprite()
-        
-        # add a spriteImage to the player sprite, including 5 different states
-        self.player.spriteImage = pygamepal.SpriteImage()
-        self.player.spriteImage.addTextures(splitTextures[0][0], splitTextures[0][1], state='idle', offset=(17*2, 16*2))
-        self.player.spriteImage.addTextures(splitTextures[0][1], splitTextures[0][2], splitTextures[0][1], splitTextures[0][3], state='walk_down', offset=(17*2, 16*2))
-        self.player.spriteImage.addTextures(splitTextures[1][1], splitTextures[1][2], splitTextures[1][1], splitTextures[1][3], state='walk_up', offset=(17*2, 16*2))
-        self.player.spriteImage.addTextures(splitTextures[2][1], splitTextures[2][2], splitTextures[2][1], splitTextures[2][3], state='walk_left', offset=(17*2, 16*2))
-        self.player.spriteImage.addTextures(splitTextures[3][1], splitTextures[3][2], splitTextures[3][1], splitTextures[3][3], state='walk_right', offset=(17*2, 16*2))
-        
-        # set player position and size
-        #self.player.position = [160, 160]
-        #self.player.size = (28, 32)
-        self.player.rect = pygame.Rect(160, 160, 28, 32)
-
-        #
-        # create a camera object
-        #
-
-        self.camera = pygamepal.Camera(position=(50, 50),
-                                          size=(700, 400),
-                                          # center the camera on the player
-                                          target=(self.player.rect.x + self.player.rect.w/2, 
-                                                  self.player.rect.y + self.player.rect.h/2),
-                                          zoom=3,
-                                          backgroundColour='darkgreen',
-                                          # clamp the camera to the world
-                                          clamp=True,
-                                          clampRect=(0, 0, 500, 500),
-                                          followDelay=0.9)
-        
-        # create a separate surface for drawing the world
-        # this surface will be used by the camera
-        self.worldSurface = pygame.surface.Surface((500, 500), pygame.SRCALPHA, 32)
-        
-
-    def update(self, deltaTime):
-
-        # fill the screen
-        self.screen.fill('cornflowerblue')
-
-        # update the input
-        self.input.update()
-
-        # calculate distance
-        dist = 60 * deltaTime
-
-        # arrow keys to:
-        # - change state of player sprite
-        # - change player sprite position (clamped to world)
-        if self.input.isKeyDown(pygame.K_UP):
-            self.player.spriteImage.setState('walk_up')
-            self.player.rect.y = max(0, self.player.rect.y - dist)
-        elif self.input.isKeyDown(pygame.K_DOWN):
-            self.player.spriteImage.setState('walk_down')
-            self.player.rect.y = min (500 - self.player.rect.h, self.player.rect.y + dist)
-        elif self.input.isKeyDown(pygame.K_LEFT):
-            self.player.spriteImage.setState('walk_left')
-            self.player.rect.x = max(0, self.player.rect.x - dist)
-        elif self.input.isKeyDown(pygame.K_RIGHT):
-            self.player.spriteImage.setState('walk_right')
-            self.player.rect.x = min(500 - self.player.rect.w, self.player.rect.x + dist)
-        # idle state is the default
-        else:
-            self.player.spriteImage.setState('idle')
-
-        # update the sprite image
-        self.player.spriteImage.update()
-        
-        # update the camera
-        self.camera.update()
-        
-        # track the player with the camera
-        self.camera.target = (self.player.rect.x + self.player.rect.w/2, 
-                              self.player.rect.y + self.player.rect.h/2)
-        
-    def draw(self):
-
-        # clear the world surface
-        self.worldSurface.fill((0, 0, 0, 0))
-        # draw the player sprite image to the world surface
-        self.player.spriteImage.draw(self.worldSurface, self.player.rect.x, self.player.rect.y)
-        # draw the chest to the world surface
-        self.worldSurface.blit(chestImage, chestPosition)
-        # use the camera to draw the world surface to the screen
-        self.camera.draw(self.worldSurface, self.screen)
-
-#
-# create a new game instance
-#
-
-myGame = MyGame()
+#
+# PygamePal, by Rik Cross
+#  -- homepage: github.com/rik-cross/pygamepal
+#  -- MIT licenced, free to use, modify and distribute
+#  -- run 'pip install pygamepal' to use
+#
+# Instructions
+#  -- arrow keys to move player
+#
+# Image credit - Cup Nooble
+#  --  cupnooble.itch.io/sprout-lands-asset-pack
+#
+
+import pygame
+import pygamepal
+import os
+
+#
+# load spritesheet and split into separate images
+#
+
+# load a texture
+texture = pygame.image.load(os.path.join('images','character_spritesheet.png'))
+# double the texture size
+texture = pygame.transform.scale(texture, (texture.get_width()*2,texture.get_height()*2))
+# split texture into a 2D list of sub-textures
+splitTextures = pygamepal.splitTexture(texture, 96, 96)
+
+#
+# chest (just an image)
+#
+
+chestImage = pygame.image.load(os.path.join('images', 'chest.png'))
+chestPosition = (200, 200)
+
+#
+# create a new game
+#
+
+class MyGame(pygamepal.Game):
+
+    def init(self):
+
+        # set window properties
+        self.size = (800, 500)
+        self.caption = 'Full game example'
+        
+        # create an input object
+        self.input = pygamepal.Input()
+
+        #
+        # create a player sprite
+        #
+
+        self.player = pygame.sprite.Sprite()
+        
+        # add a spriteImage to the player sprite, including 5 different states
+        self.player.spriteImage = pygamepal.SpriteImage()
+        self.player.spriteImage.addTextures(splitTextures[0][0], splitTextures[0][1], state='idle', offset=(17*2, 16*2))
+        self.player.spriteImage.addTextures(splitTextures[0][1], splitTextures[0][2], splitTextures[0][1], splitTextures[0][3], state='walk_down', offset=(17*2, 16*2))
+        self.player.spriteImage.addTextures(splitTextures[1][1], splitTextures[1][2], splitTextures[1][1], splitTextures[1][3], state='walk_up', offset=(17*2, 16*2))
+        self.player.spriteImage.addTextures(splitTextures[2][1], splitTextures[2][2], splitTextures[2][1], splitTextures[2][3], state='walk_left', offset=(17*2, 16*2))
+        self.player.spriteImage.addTextures(splitTextures[3][1], splitTextures[3][2], splitTextures[3][1], splitTextures[3][3], state='walk_right', offset=(17*2, 16*2))
+        
+        # set player position and size
+        #self.player.position = [160, 160]
+        #self.player.size = (28, 32)
+        self.player.rect = pygame.Rect(160, 160, 28, 32)
+
+        #
+        # create a camera object
+        #
+
+        self.camera = pygamepal.Camera(position=(50, 50),
+                                          size=(700, 400),
+                                          # center the camera on the player
+                                          target=(self.player.rect.x + self.player.rect.w/2, 
+                                                  self.player.rect.y + self.player.rect.h/2),
+                                          zoom=3,
+                                          backgroundColour='darkgreen',
+                                          # clamp the camera to the world
+                                          clamp=True,
+                                          clampRect=(0, 0, 500, 500),
+                                          followDelay=0.9)
+        
+        # create a separate surface for drawing the world
+        # this surface will be used by the camera
+        self.worldSurface = pygame.surface.Surface((500, 500), pygame.SRCALPHA, 32)
+        
+
+    def update(self, deltaTime):
+
+        # fill the screen
+        self.screen.fill('cornflowerblue')
+
+        # update the input
+        self.input.update()
+
+        # calculate distance
+        dist = 60 * deltaTime
+
+        # arrow keys to:
+        # - change state of player sprite
+        # - change player sprite position (clamped to world)
+        if self.input.isKeyDown(pygame.K_UP):
+            self.player.spriteImage.setState('walk_up')
+            self.player.rect.y = max(0, self.player.rect.y - dist)
+        elif self.input.isKeyDown(pygame.K_DOWN):
+            self.player.spriteImage.setState('walk_down')
+            self.player.rect.y = min (500 - self.player.rect.h, self.player.rect.y + dist)
+        elif self.input.isKeyDown(pygame.K_LEFT):
+            self.player.spriteImage.setState('walk_left')
+            self.player.rect.x = max(0, self.player.rect.x - dist)
+        elif self.input.isKeyDown(pygame.K_RIGHT):
+            self.player.spriteImage.setState('walk_right')
+            self.player.rect.x = min(500 - self.player.rect.w, self.player.rect.x + dist)
+        # idle state is the default
+        else:
+            self.player.spriteImage.setState('idle')
+
+        # update the sprite image
+        self.player.spriteImage.update()
+        
+        # update the camera
+        self.camera.update()
+        
+        # track the player with the camera
+        self.camera.target = (self.player.rect.x + self.player.rect.w/2, 
+                              self.player.rect.y + self.player.rect.h/2)
+        
+    def draw(self):
+
+        # clear the world surface
+        self.worldSurface.fill((0, 0, 0, 0))
+        # draw the player sprite image to the world surface
+        self.player.spriteImage.draw(self.worldSurface, self.player.rect.x, self.player.rect.y)
+        # draw the chest to the world surface
+        self.worldSurface.blit(chestImage, chestPosition)
+        # use the camera to draw the world surface to the screen
+        self.camera.draw(self.worldSurface, self.screen)
+
+#
+# create a new game instance
+#
+
+myGame = MyGame()
 myGame.run()
```

### Comparing `pygamepal-0.2.0/examples/spriteImageExample.py` & `pygamepal-0.3.0/examples/spriteImageShowcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,126 +1,127 @@
-#
-# pygamepal, by Rik Cross
-#  -- homepage: github.com/rik-cross/pygamepal
-#  -- MIT licenced, free to use, modify and distribute
-#  -- run 'pip install pygamepal' to use
-#
-# instructions:
-#  -- space to toggle pause sprite 2
-#  -- arrow keys to control sprite 3
-#
-# Image credit - Cup Nooble
-#  --  cupnooble.itch.io/sprout-lands-asset-pack
-#
-
-# import modules
-import pygame
-import pygamepal
-import os
-
-# initialise Pygame
-pygame.init()
-
-# setup screen
-screen = pygame.display.set_mode((680, 460))
-pygame.display.set_caption('SpriteImage Example')
-clock = pygame.time.Clock() 
-
-# add input, to easily query keys
-input = pygamepal.Input()
-
-# load a texture
-texture = pygame.image.load(os.path.join('images','character_spritesheet.png'))
-# double the texture size
-texture = pygame.transform.scale(texture, (texture.get_width()*2,texture.get_height()*2))
-# split texture into a 2D list of sub-textures
-splitTextures = pygamepal.splitTexture(texture, 96, 96)
-
-# a sprite with a single texture
-spriteImage1 = pygamepal.SpriteImage()
-# simple alternative for single texture: spriteImage1.addTextures(pygame.image.load('image.png'))
-spriteImage1.addTextures(splitTextures[0][0], offset=(17*2, 16*2))
-
-# an animated sprite with multiple textures
-spriteImage2 = pygamepal.SpriteImage()
-spriteImage2.addTextures(splitTextures[3][1], splitTextures[3][2], splitTextures[3][1], splitTextures[3][3], offset=(17*2, 16*2))
-# simple alternative for single textures:
-# spriteImage1.addTextures(pygame.image.load('image1.png'), pygame.image.load('image2.png'))
-
-# a controllable sprite with multiple animation states
-spriteImage3 = pygamepal.SpriteImage()
-spriteImage3.addTextures(splitTextures[0][0], splitTextures[0][1], state='idle', offset=(17*2, 16*2))
-spriteImage3.addTextures(splitTextures[0][1], splitTextures[0][2], splitTextures[0][1], splitTextures[0][3], state='walk_down', offset=(17*2, 16*2))
-spriteImage3.addTextures(splitTextures[1][1], splitTextures[1][2], splitTextures[1][1], splitTextures[1][3], state='walk_up', offset=(17*2, 16*2))
-spriteImage3.addTextures(splitTextures[2][1], splitTextures[2][2], splitTextures[2][1], splitTextures[2][3], state='walk_left', offset=(17*2, 16*2))
-spriteImage3.addTextures(splitTextures[3][1], splitTextures[3][2], splitTextures[3][1], splitTextures[3][3], state='walk_right', offset=(17*2, 16*2))
-
-# for easily getting key presses
-input = pygamepal.Input()
-
-# game loop
-running = True
-while running:
-
-    # clear screen
-    screen.fill('cornflowerblue')
-    # advance clock
-    clock.tick(60)
-
-    # respond to quit event
-    for event in pygame.event.get():
-        if event.type == pygame.QUIT:
-            running = False
-
-    #
-    # input
-    #
-
-    # space to toggle pause s2 sprite
-    if input.isKeyPressed(pygame.K_SPACE):
-        spriteImage2.pause = not spriteImage2.pause
-
-    # arrow keys to change state of s3 sprite
-    if input.isKeyDown(pygame.K_UP):
-        spriteImage3.setState('walk_up')
-    elif input.isKeyDown(pygame.K_DOWN):
-        spriteImage3.setState('walk_down')
-    elif input.isKeyDown(pygame.K_LEFT):
-        spriteImage3.setState('walk_left')
-    elif input.isKeyDown(pygame.K_RIGHT):
-        spriteImage3.setState('walk_right')
-    # idle state is the default
-    else:
-        spriteImage3.setState('idle')
-
-    #
-    # update
-    #
-
-    input.update()
-    spriteImage1.update()
-    spriteImage2.update()
-    spriteImage3.update()
-
-    #
-    # draw
-    #
-
-    # draw split texture
-    for col in range(len(splitTextures)):
-        for row in range(len(splitTextures[0])):
-            pygame.draw.rect(screen, 'gray10', (col * 100, row * 100, 96, 96), False)
-            screen.blit(splitTextures[row][col], (col * 100, row * 100, 96, 96))
-
-    # draw sprites and accompanying text
-    pygamepal.drawText(screen, 'Sprite 1 (single texture)', 420, 40)
-    spriteImage1.draw(screen, 500, 70)
-    pygamepal.drawText(screen, 'Sprite 2 (space to pause/play)', 420, 140)
-    spriteImage2.draw(screen, 500, 170)
-    pygamepal.drawText(screen, 'Sprite 3 (arrow keys to change)', 420, 240)
-    spriteImage3.draw(screen, 500, 270)
-
-    # draw to screen
-    pygame.display.flip()
-
-# quit Pygame
-pygame.quit()
+#
+# PygamePal, by Rik Cross
+#  -- homepage: github.com/rik-cross/pygamepal
+#  -- MIT licenced, free to use, modify and distribute
+#  -- run 'pip install pygamepal' to use
+#
+# Instructions:
+#  -- space to toggle pause sprite 2
+#  -- arrow keys to control sprite 3
+#
+# Image credit - Cup Nooble
+#  --  cupnooble.itch.io/sprout-lands-asset-pack
+#
+
+# import modules
+import pygame
+import pygamepal
+import os
+
+# initialise Pygame
+pygame.init()
+
+# setup screen
+screen = pygame.display.set_mode((680, 460))
+pygame.display.set_caption('SpriteImage Showcase')
+clock = pygame.time.Clock() 
+
+# add input, to easily query keys
+input = pygamepal.Input()
+
+# load a texture
+texture = pygame.image.load(os.path.join('images','character_spritesheet.png'))
+# double the texture size
+texture = pygame.transform.scale(texture, (texture.get_width()*2,texture.get_height()*2))
+# split texture into a 2D list of sub-textures
+splitTextures = pygamepal.splitTexture(texture, 96, 96)
+
+# a sprite with a single texture
+spriteImage1 = pygamepal.SpriteImage()
+# simple alternative for single texture: spriteImage1.addTextures(pygame.image.load('image.png'))
+spriteImage1.addTextures(splitTextures[0][0], offset=(17*2, 16*2))
+
+# an animated sprite with multiple textures
+spriteImage2 = pygamepal.SpriteImage()
+spriteImage2.addTextures(splitTextures[3][1], splitTextures[3][2], splitTextures[3][1], splitTextures[3][3], offset=(17*2, 16*2))
+# simple alternative for single textures:
+# spriteImage1.addTextures(pygame.image.load('image1.png'), pygame.image.load('image2.png'))
+
+# a controllable sprite with multiple animation states
+spriteImage3 = pygamepal.SpriteImage()
+spriteImage3.addTextures(splitTextures[0][0], splitTextures[0][1], state='idle', offset=(17*2, 16*2))
+spriteImage3.addTextures(splitTextures[0][1], splitTextures[0][2], splitTextures[0][1], splitTextures[0][3], state='walk_down', offset=(17*2, 16*2))
+spriteImage3.addTextures(splitTextures[1][1], splitTextures[1][2], splitTextures[1][1], splitTextures[1][3], state='walk_up', offset=(17*2, 16*2))
+spriteImage3.addTextures(splitTextures[2][1], splitTextures[2][2], splitTextures[2][1], splitTextures[2][3], state='walk_left', offset=(17*2, 16*2))
+spriteImage3.addTextures(splitTextures[3][1], splitTextures[3][2], splitTextures[3][1], splitTextures[3][3], state='walk_right', offset=(17*2, 16*2))
+
+# for easily getting key presses
+input = pygamepal.Input()
+
+# game loop
+running = True
+while running:
+    
+    # advance clock
+    clock.tick(60)
+
+    # respond to quit event
+    for event in pygame.event.get():
+        if event.type == pygame.QUIT:
+            running = False
+
+    #
+    # input
+    #
+
+    # space to toggle pause s2 sprite
+    if input.isKeyPressed(pygame.K_SPACE):
+        spriteImage2.pause = not spriteImage2.pause
+
+    # arrow keys to change state of s3 sprite
+    if input.isKeyDown(pygame.K_UP):
+        spriteImage3.setState('walk_up')
+    elif input.isKeyDown(pygame.K_DOWN):
+        spriteImage3.setState('walk_down')
+    elif input.isKeyDown(pygame.K_LEFT):
+        spriteImage3.setState('walk_left')
+    elif input.isKeyDown(pygame.K_RIGHT):
+        spriteImage3.setState('walk_right')
+    # idle state is the default
+    else:
+        spriteImage3.setState('idle')
+
+    #
+    # update
+    #
+
+    input.update()
+    spriteImage1.update()
+    spriteImage2.update()
+    spriteImage3.update()
+
+    #
+    # draw
+    #
+
+    # clear screen
+    screen.fill('cornflowerblue')
+    
+    # draw split texture
+    for col in range(len(splitTextures)):
+        for row in range(len(splitTextures[0])):
+            pygame.draw.rect(screen, 'gray10', (col * 100, row * 100, 96, 96), False)
+            screen.blit(splitTextures[row][col], (col * 100, row * 100, 96, 96))
+
+    # draw sprites and accompanying text
+    pygamepal.drawText(screen, 'Sprite 1 (single texture)', 420, 40)
+    spriteImage1.draw(screen, 500, 70)
+    pygamepal.drawText(screen, 'Sprite 2 (space to pause/play)', 420, 140)
+    spriteImage2.draw(screen, 500, 170)
+    pygamepal.drawText(screen, 'Sprite 3 (arrow keys to change)', 420, 240)
+    spriteImage3.draw(screen, 500, 270)
+
+    # draw to screen
+    pygame.display.flip()
+
+# quit Pygame
+pygame.quit()
```

### Comparing `pygamepal-0.2.0/examples/transitionExample.py` & `pygamepal-0.3.0/examples/transitionExample.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-#
-# pygamepal, by Rik Cross
-#  -- homepage: github.com/rik-cross/pygamepal
-#  -- MIT licenced, free to use, modify and distribute
-#  -- run 'pip install pygamepal' to use
-#
-# Image credit - Cup Nooble
-#  --  cupnooble.itch.io/sprout-lands-asset-pack
-#
-
-# import modules
-import pygame
-import pygamepal
-import os
-
-# initialise Pygame
-pygame.init()
-
-# setup screen to required size
-screen = pygame.display.set_mode((680, 460))
-pygame.display.set_caption('Transition Example')
-clock = pygame.time.Clock() 
-
-# load a texture
-texture = pygame.image.load(os.path.join('images','character_spritesheet.png'))
-
-# first surface
-surface1 = pygame.Surface((680, 460))
-surface1.fill('mediumpurple')
-surface1.blit(texture, (400, 100))
-
-# second surface
-surface2 = pygame.Surface((680, 460))
-surface2.fill('goldenrod')
-surface2.blit(texture, (100, 100))
-
-# transition
-transition = pygamepal.TransitionWipeRight(surface1, 
-                                           surface2, 
-                                           duration=200, 
-                                           easingFunction=pygamepal.bounceEaseOut)
-
-# game loop
-running = True
-while running:
-
-    # clear screen to Cornflower Blue
-    screen.fill('cornflowerblue')
-
-    # advance clock at 60 FPS
-    clock.tick(60)
-
-    # respond to quit event
-    for event in pygame.event.get():
-        if event.type == pygame.QUIT:
-            running = False
-
-    #
-    # update
-    #
-
-    # update the transition if it hasn't finished
-    if transition.finished is False:
-        transition.update()
-
-    #
-    # draw
-    #
-
-    # draw the transition if it isn't finished...
-    if transition.finished is False:
-        transition.draw(screen)
-    # ...otherwise draw the second surface
-    else:
-        screen.blit(surface2, (0, 0))
-
-    # draw to the screen
-    pygame.display.flip()
-
-#quit Pygame on exit
-pygame.quit()
+#
+# PygamePal, by Rik Cross
+#  -- homepage: github.com/rik-cross/pygamepal
+#  -- MIT licenced, free to use, modify and distribute
+#  -- run 'pip install pygamepal' to use
+#
+# Image credit - Cup Nooble
+#  --  cupnooble.itch.io/sprout-lands-asset-pack
+#
+
+# import modules
+import pygame
+import pygamepal
+import os
+
+# initialise Pygame
+pygame.init()
+
+# setup screen to required size
+screen = pygame.display.set_mode((680, 460))
+pygame.display.set_caption('Transition Example')
+clock = pygame.time.Clock() 
+
+# load a texture
+texture = pygame.image.load(os.path.join('images','character_spritesheet.png'))
+
+# first surface
+surface1 = pygame.Surface((680, 460))
+surface1.fill('mediumpurple')
+surface1.blit(texture, (400, 100))
+
+# second surface
+surface2 = pygame.Surface((680, 460))
+surface2.fill('goldenrod')
+surface2.blit(texture, (100, 100))
+
+# transition
+transition = pygamepal.TransitionWipeRight(surface1, 
+                                           surface2, 
+                                           duration=200, 
+                                           easingFunction=pygamepal.bounceEaseOut)
+
+# game loop
+running = True
+while running:
+
+    # advance clock at 60 FPS
+    clock.tick(60)
+
+    # respond to quit event
+    for event in pygame.event.get():
+        if event.type == pygame.QUIT:
+            running = False
+
+    #
+    # update
+    #
+
+    # update the transition if it hasn't finished
+    if transition.finished is False:
+        transition.update()
+
+    #
+    # draw
+    #
+
+    # clear screen to Cornflower Blue
+    screen.fill('cornflowerblue')
+  
+    # draw the transition if it isn't finished...
+    if transition.finished is False:
+        transition.draw(screen)
+    # ...otherwise draw the second surface
+    else:
+        screen.blit(surface2, (0, 0))
+
+    # draw to the screen
+    pygame.display.flip()
+
+#quit Pygame on exit
+pygame.quit()
```

### Comparing `pygamepal-0.2.0/examples/transitionShowcase.py` & `pygamepal-0.3.0/examples/transitionShowcase.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-#
-# pygamepal, by Rik Cross
-#  -- homepage: github.com/rik-cross/pygamepal
-#  -- MIT licenced, free to use, modify and distribute
-#  -- run 'pip install pygamepal' to use
-#
-# instructions:
-#  -- up / down arrow to change transition
-#  -- left / right arrow to change duration
-#  -- w / s to change easing function
-#  -- space key to start / pause
-#  -- click and drag mouse to progress transition
-#
-# Image credit - Cup Nooble
-#  --  cupnooble.itch.io/sprout-lands-asset-pack
-#
-
-import pygame
-import pygamepal
-import os
-
-def resetTransitions():
-    # use global data
-    global transitionList
-    global surface1
-    global surface2
-    global duration
-    global currentEasingFunction
-    # reset each transition
-    for t in transitionList:
-        # set easing function
-        t.easingFunction = currentEasingFunction
-        # set duration
-        t.duration = duration
-        t.reset()
-    # reset surface alpha
-    surface1.set_alpha(255)
-    surface2.set_alpha(255)
-
-# initialise Pygame
-pygame.init()
-
-# setup screen to required size
-screen = pygame.display.set_mode((680, 460))
-pygame.display.set_caption('Transition Showcase')
-clock = pygame.time.Clock() 
-
-# load a texture
-texture = pygame.image.load(os.path.join('images','character_spritesheet.png'))
-
-surface1 = pygame.Surface((680, 460))
-surface1.fill('mediumpurple')
-surface1.blit(texture, (400, 100))
-
-surface2 = pygame.Surface((680, 460))
-surface2.fill('goldenrod')
-surface2.blit(texture, (100, 100))
-
-transitionList = [
-    pygamepal.TransitionFade(surface1, surface2),
-    pygamepal.TransitionFadeToBlack(surface1, surface2),
-    pygamepal.TransitionWipeLeft(surface1, surface2),
-    pygamepal.TransitionWipeRight(surface1, surface2),
-    pygamepal.TransitionWipeUp(surface1, surface2),
-    pygamepal.TransitionWipeDown(surface1, surface2),
-    pygamepal.TransitionMoveLeft(surface1, surface2),
-    pygamepal.TransitionMoveRight(surface1, surface2),
-    pygamepal.TransitionMoveUp(surface1, surface2),
-    pygamepal.TransitionMoveDown(surface1, surface2)
-]
-transitionIndex = 0
-currentTransition = transitionList[transitionIndex]
-
-easingList = [
-    pygamepal.linear,
-    pygamepal.bounceEaseOut
-]
-easingIndex = 0
-currentEasingFunction = easingList[easingIndex]
-
-duration = 100
-
-play = False
-circlePos = (100, 410)
-mouseDown = False
-
-input = pygamepal.Input()
-
-# game loop
-running = True
-while running:
-
-    # clear screen to Cornflower Blue
-    screen.fill('cornflowerblue')
-
-    # advance clock at 60 FPS
-    clock.tick(60)
-
-    # respond to quit event
-    for event in pygame.event.get():
-
-        if event.type == pygame.QUIT:
-            running = False
-
-    # check mouseDown to control scrubber
-    if event.type == pygame.MOUSEBUTTONDOWN:
-        mouseDown = True
-    if event.type == pygame.MOUSEBUTTONUP:
-        mouseDown = False
-
-    # space to play / pause
-    if input.isKeyPressed(pygame.K_SPACE):
-        play = not play
-
-    # up / down arrow to change transition
-    if input.isKeyPressed(pygame.K_UP):
-        transitionIndex = max(0, min(len(transitionList) - 1, transitionIndex - 1))
-        currentTransition = transitionList[transitionIndex]
-        resetTransitions()
-    if input.isKeyPressed(pygame.K_DOWN):
-        transitionIndex = max(0, min(len(transitionList) - 1, transitionIndex + 1))
-        currentTransition = transitionList[transitionIndex]
-        resetTransitions()
-
-    # left / right arrow to change duration
-    if input.isKeyDown(pygame.K_LEFT):
-        duration = max(10, min(1000 - 1, duration - 1))
-        resetTransitions()
-    if input.isKeyDown(pygame.K_RIGHT):
-        duration = max(10, min(1000 - 1, duration + 1))
-        resetTransitions()
-
-    # w / s to change easing function
-    if input.isKeyPressed(pygame.K_w):
-        easingIndex = max(0, min(len(easingList) - 1, easingIndex - 1))
-        currentEasingFunction = easingList[easingIndex]
-        resetTransitions()
-    if input.isKeyPressed(pygame.K_s):
-        easingIndex = max(0, min(len(easingList) - 1, easingIndex + 1))
-        currentEasingFunction = easingList[easingIndex]
-        resetTransitions()
-
-    input.update()
-
-    currentTransition = transitionList[transitionIndex]
-
-    # scrubber should reflect the current transition percentage
-    if not mouseDown:
-        if play:
-            currentTransition.update()
-            xPos = 100 + (480 / 100 * currentTransition.currentPercentage)
-            circlePos = (xPos, 410)
-    # scrubber is controlled by mouse position
-    else:
-        xPos = max(100, min(580, pygame.mouse.get_pos()[0]))
-        circlePos = (xPos, 410)
-        calculatedPercentage = (xPos - 100) / (480) * 100
-        transitionList[transitionIndex].currentPercentage = calculatedPercentage
-    
-    currentTransition.draw(screen)
-    
-    pygamepal.drawText(screen, str(currentTransition), 20, 20)
-    pygamepal.drawText(screen, 'Duration: ' + str(currentTransition.duration), 20, 40)
-    pygamepal.drawText(screen, 'Easing function: ' + str(currentTransition.easingFunction), 20, 60)
-    pygamepal.drawText(screen, '% complete: ' + str(round(currentTransition.currentPercentage, 2)), 20, 80)
-    pygamepal.drawText(screen, 'Playing: ' + str(play), 20, 100)
-
-    # draw scrubber
-    pygame.draw.line(screen, 'white', (100, 410), (580, 410), width=4)
-    pygame.draw.circle(screen, 'white', circlePos, 10)
-
-    # draw to the screen
-    pygame.display.flip()
-
-# quit Pygame on exit
-pygame.quit()
+#
+# PygamePal, by Rik Cross
+#  -- homepage: github.com/rik-cross/pygamepal
+#  -- MIT licenced, free to use, modify and distribute
+#  -- run 'pip install pygamepal' to use
+#
+# Instructions:
+#  -- up / down arrow to change transition
+#  -- left / right arrow to change duration
+#  -- w / s to change easing function
+#  -- space key to start / pause
+#  -- click and drag mouse to progress transition
+#
+# Image credit - Cup Nooble
+#  --  cupnooble.itch.io/sprout-lands-asset-pack
+#
+
+import pygame
+import pygamepal
+import os
+
+def resetTransitions():
+    # use global data
+    global transitionList
+    global surface1
+    global surface2
+    global duration
+    global currentEasingFunction
+    # reset each transition
+    for t in transitionList:
+        # set easing function
+        t.easingFunction = currentEasingFunction
+        # set duration
+        t.duration = duration
+        t.reset()
+    # reset surface alpha
+    surface1.set_alpha(255)
+    surface2.set_alpha(255)
+
+# initialise Pygame
+pygame.init()
+
+# setup screen to required size
+screen = pygame.display.set_mode((680, 460))
+pygame.display.set_caption('Transition Showcase')
+clock = pygame.time.Clock() 
+
+# load a texture
+texture = pygame.image.load(os.path.join('images','character_spritesheet.png'))
+
+surface1 = pygame.Surface((680, 460))
+surface1.fill('mediumpurple')
+surface1.blit(texture, (400, 100))
+
+surface2 = pygame.Surface((680, 460))
+surface2.fill('goldenrod')
+surface2.blit(texture, (100, 100))
+
+transitionList = [
+    pygamepal.TransitionFade(surface1, surface2),
+    pygamepal.TransitionFadeToBlack(surface1, surface2),
+    pygamepal.TransitionWipeLeft(surface1, surface2),
+    pygamepal.TransitionWipeRight(surface1, surface2),
+    pygamepal.TransitionWipeUp(surface1, surface2),
+    pygamepal.TransitionWipeDown(surface1, surface2),
+    pygamepal.TransitionMoveLeft(surface1, surface2),
+    pygamepal.TransitionMoveRight(surface1, surface2),
+    pygamepal.TransitionMoveUp(surface1, surface2),
+    pygamepal.TransitionMoveDown(surface1, surface2)
+]
+transitionIndex = 0
+currentTransition = transitionList[transitionIndex]
+
+easingList = [
+    pygamepal.linear,
+    pygamepal.bounceEaseOut
+]
+easingIndex = 0
+currentEasingFunction = easingList[easingIndex]
+
+duration = 100
+
+play = False
+circlePos = (100, 410)
+mouseDown = False
+
+input = pygamepal.Input()
+
+# game loop
+running = True
+while running:
+
+    # advance clock at 60 FPS
+    clock.tick(60)
+
+    # respond to quit event
+    for event in pygame.event.get():
+
+        if event.type == pygame.QUIT:
+            running = False
+
+    # check mouseDown to control scrubber
+    if event.type == pygame.MOUSEBUTTONDOWN:
+        mouseDown = True
+    if event.type == pygame.MOUSEBUTTONUP:
+        mouseDown = False
+
+    # space to play / pause
+    if input.isKeyPressed(pygame.K_SPACE):
+        play = not play
+
+    # up / down arrow to change transition
+    if input.isKeyPressed(pygame.K_UP):
+        transitionIndex = max(0, min(len(transitionList) - 1, transitionIndex - 1))
+        currentTransition = transitionList[transitionIndex]
+        resetTransitions()
+    if input.isKeyPressed(pygame.K_DOWN):
+        transitionIndex = max(0, min(len(transitionList) - 1, transitionIndex + 1))
+        currentTransition = transitionList[transitionIndex]
+        resetTransitions()
+
+    # left / right arrow to change duration
+    if input.isKeyDown(pygame.K_LEFT):
+        duration = max(10, min(1000 - 1, duration - 1))
+        resetTransitions()
+    if input.isKeyDown(pygame.K_RIGHT):
+        duration = max(10, min(1000 - 1, duration + 1))
+        resetTransitions()
+
+    # w / s to change easing function
+    if input.isKeyPressed(pygame.K_w):
+        easingIndex = max(0, min(len(easingList) - 1, easingIndex - 1))
+        currentEasingFunction = easingList[easingIndex]
+        resetTransitions()
+    if input.isKeyPressed(pygame.K_s):
+        easingIndex = max(0, min(len(easingList) - 1, easingIndex + 1))
+        currentEasingFunction = easingList[easingIndex]
+        resetTransitions()
+
+    input.update()
+
+    currentTransition = transitionList[transitionIndex]
+
+    # scrubber should reflect the current transition percentage
+    if not mouseDown:
+        if play:
+            currentTransition.update()
+            xPos = 100 + (480 / 100 * currentTransition.currentPercentage)
+            circlePos = (xPos, 410)
+    # scrubber is controlled by mouse position
+    else:
+        xPos = max(100, min(580, pygame.mouse.get_pos()[0]))
+        circlePos = (xPos, 410)
+        calculatedPercentage = (xPos - 100) / (480) * 100
+        transitionList[transitionIndex].currentPercentage = calculatedPercentage
+
+    # clear screen to Cornflower Blue
+    screen.fill('cornflowerblue')
+    
+    currentTransition.draw(screen)
+    
+    pygamepal.drawText(screen, str(currentTransition), 20, 20)
+    pygamepal.drawText(screen, 'Duration: ' + str(currentTransition.duration), 20, 40)
+    pygamepal.drawText(screen, 'Easing function: ' + str(currentTransition.easingFunction), 20, 60)
+    pygamepal.drawText(screen, '% complete: ' + str(round(currentTransition.currentPercentage, 2)), 20, 80)
+    pygamepal.drawText(screen, 'Playing: ' + str(play), 20, 100)
+
+    # draw scrubber
+    pygame.draw.line(screen, 'white', (100, 410), (580, 410), width=4)
+    pygame.draw.circle(screen, 'white', circlePos, 10)
+
+    # draw to the screen
+    pygame.display.flip()
+
+# quit Pygame on exit
+pygame.quit()
```

### Comparing `pygamepal-0.2.0/examples/images/character.png` & `pygamepal-0.3.0/examples/images/character.png`

 * *Files identical despite different names*

### Comparing `pygamepal-0.2.0/examples/images/character_spritesheet.png` & `pygamepal-0.3.0/examples/images/character_spritesheet.png`

 * *Files identical despite different names*

### Comparing `pygamepal-0.2.0/examples/images/chest.png` & `pygamepal-0.3.0/examples/images/chest.png`

 * *Files identical despite different names*

### Comparing `pygamepal-0.2.0/src/pygamepal/transition.py` & `pygamepal-0.3.0/src/pygamepal/transition.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-import pygame
-
-def linear(x):
-    return x
-
-def bounceEaseOut(x):
-    x = x/100
-    if x < 4 / 11:
-        return (121 * x * x / 16) * 100
-    elif x < 8 / 11:
-        return ((363 / 40.0 * x * x) - (99 / 10.0 * x) + 17 / 5.0) * 100
-    elif x < 9 / 10:
-        return ((4356 / 361.0 * x * x) - (35442 / 1805.0 * x) + 16061 / 1805.0) * 100
-    return ((54 / 5.0 * x * x) - (513 / 25.0 * x) + 268 / 25.0) * 100
-
-class Transition:
-
-    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
-
-        self.fromSurface = fromSurface
-        self.toSurface = toSurface
-        self.duration = duration
-        self.drawMethod = drawMethod
-
-        self.easingFunction = easingFunction
-        self.easeValue = 0
-
-        self.currentPercentage = 0
-        self.finished = False
-
-        # allows adjusting for different durations
-        self.durationCoefficient = 100 / self.duration
-
-    def update(self, deltaTime=1):
-        perc = self.currentPercentage + (deltaTime * self.durationCoefficient)
-        self.currentPercentage = min(perc, 100)
-        self.easeValue = self.easingFunction(self.currentPercentage)
-        if self.currentPercentage == 100:
-            self.finished = True
-
-    def draw(self, surface):
-        if self.drawMethod is not None:
-            self.drawMethod
-
-    def reset(self):
-        self.currentPercentage = 0
-        self.easeValue = 0
-        self.durationCoefficient = 100 / self.duration
-
-class TransitionFade(Transition):
-
-    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=linear):
-        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
-
-    def draw(self, surface):
-        self.easeValue = self.easingFunction(self.currentPercentage)
-        if self.fromSurface is not None:
-            self.fromSurface.set_alpha((100 - self.easeValue) * 2.55)
-            surface.blit(self.fromSurface, (0, 0))
-        if self.toSurface is not None:
-            self.toSurface.set_alpha(self.easeValue * 2.55)
-            surface.blit(self.toSurface, (0, 0))
-
-    def __repr__(self):
-        return 'Transition: Fade between'
-
-class TransitionFadeToBlack(Transition):
-
-    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
-        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
-        self.blacksurface = pygame.Surface((self.fromSurface.get_width(), self.fromSurface.get_height()), pygame.SRCALPHA, 32)
-        self.blacksurface.fill('black')
-
-    def draw(self, surface):
-        self.easeValue = self.easingFunction(self.currentPercentage)
-        if self.fromSurface is not None and self.easeValue < 50:
-            surface.blit(self.fromSurface, (0, 0))
-        if self.toSurface is not None and self.easeValue > 50:
-            surface.blit(self.toSurface, (0, 0))
-        distanceFromMidPoint = abs(50 - self.easeValue)
-        percentageToAlpha = 255 - (distanceFromMidPoint * 2.55 * 2)
-        self.blacksurface.set_alpha(percentageToAlpha)
-        surface.blit(self.blacksurface, (0, 0))
-
-    def __repr__(self):
-        return 'Transition: Fade to black'
-
-class TransitionWipeLeft(Transition):
-
-    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
-        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
-
-    def draw(self, surface):
-        self.easeValue = self.easingFunction(self.currentPercentage)
-        if self.fromSurface is not None:
-            surface.blit(self.fromSurface, (0, 0))
-        if self.toSurface is not None:
-            self.toSurface.set_alpha(255)
-            r = (surface.get_width()) - (surface.get_width() / 100 * self.easeValue)
-            surface.blit(self.toSurface, (r, 0))
-
-    def __repr__(self):
-        return 'Transition: Wipe left'
-
-class TransitionWipeRight(Transition):
-
-    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
-        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
-
-    def draw(self, surface):
-        self.easeValue = self.easingFunction(self.currentPercentage)
-        if self.fromSurface is not None:
-            surface.blit(self.fromSurface, (0, 0))
-        if self.toSurface is not None:
-            self.toSurface.set_alpha(255)
-            r = ((surface.get_width() * -1)) + (surface.get_width() / 100 * self.easeValue)
-            surface.blit(self.toSurface, (r, 0))
-
-    def __repr__(self):
-        return 'Transition: Wipe right'
-
-class TransitionWipeUp(Transition):
-
-    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
-        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
-
-    def draw(self, surface):
-        self.easeValue = self.easingFunction(self.currentPercentage)
-        if self.fromSurface is not None:
-            surface.blit(self.fromSurface, (0, 0))
-        if self.toSurface is not None:
-            self.toSurface.set_alpha(255)
-            r = (surface.get_height()) - (surface.get_height() / 100 * self.easeValue)
-            surface.blit(self.toSurface, (0, r))
-
-    def __repr__(self):
-        return 'Transition: Wipe up'
-
-class TransitionWipeDown(Transition):
-
-    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
-        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
-
-    def draw(self, surface):
-        self.easeValue = self.easingFunction(self.currentPercentage)
-        if self.fromSurface is not None:
-            surface.blit(self.fromSurface, (0, 0))
-        if self.toSurface is not None:
-            self.toSurface.set_alpha(255)
-            r = ((surface.get_height() * -1)) + (surface.get_height() / 100 * self.easeValue)
-            surface.blit(self.toSurface, (0, r))
-
-    def __repr__(self):
-        return 'Transition: Wipe down'
-
-class TransitionMoveLeft(Transition):
-
-    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
-        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
-
-    def draw(self, surface):
-        self.easeValue = self.easingFunction(self.currentPercentage)
-        if self.fromSurface is not None:
-            self.fromSurface.set_alpha(255)
-            r = 0 - (surface.get_width() / 100 * self.easeValue)
-            surface.blit(self.fromSurface, (r, 0))
-        if self.toSurface is not None:
-            self.toSurface.set_alpha(255)
-            r = (surface.get_width()) - (surface.get_width() / 100 * self.easeValue)
-            surface.blit(self.toSurface, (r, 0))
-
-    def __repr__(self):
-        return 'Transition: Move left'
-
-class TransitionMoveRight(Transition):
-
-    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
-        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
-
-    def draw(self, surface):
-        self.easeValue = self.easingFunction(self.currentPercentage)
-        if self.fromSurface is not None:
-            self.fromSurface.set_alpha(255)
-            r = (surface.get_width() / 100 * self.easeValue)
-            surface.blit(self.fromSurface, (r, 0))
-        if self.toSurface is not None:
-            self.toSurface.set_alpha(255)
-            r = ((surface.get_width() * -1)) + (surface.get_width() / 100 * self.easeValue)
-            surface.blit(self.toSurface, (r, 0))
-
-    def __repr__(self):
-        return 'Transition: Move right'
-
-class TransitionMoveUp(Transition):
-
-    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
-        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
-
-    def draw(self, surface):
-        self.easeValue = self.easingFunction(self.currentPercentage)
-        if self.fromSurface is not None:
-            self.fromSurface.set_alpha(255)
-            r = 0 - (surface.get_height() / 100 * self.easeValue)
-            surface.blit(self.fromSurface, (0, r))
-        if self.toSurface is not None:
-            self.toSurface.set_alpha(255)
-            r = (surface.get_height()) - (surface.get_height() / 100 * self.easeValue)
-            surface.blit(self.toSurface, (0, r))
-
-    def __repr__(self):
-        return 'Transition: Move up'
-
-class TransitionMoveDown(Transition):
-
-    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
-        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
-
-    def draw(self, surface):
-        self.easeValue = self.easingFunction(self.currentPercentage)
-        if self.fromSurface is not None:
-            self.fromSurface.set_alpha(255)
-            r = (surface.get_height() / 100 * self.easeValue)
-            surface.blit(self.fromSurface, (0, r))
-        if self.toSurface is not None:
-            self.toSurface.set_alpha(255)
-            r = ((surface.get_height() * -1)) + (surface.get_height() / 100 * self.easeValue)
-            surface.blit(self.toSurface, (0, r))
-
-    def __repr__(self):
+import pygame
+
+def linear(x):
+    return x
+
+def bounceEaseOut(x):
+    x = x/100
+    if x < 4 / 11:
+        return (121 * x * x / 16) * 100
+    elif x < 8 / 11:
+        return ((363 / 40.0 * x * x) - (99 / 10.0 * x) + 17 / 5.0) * 100
+    elif x < 9 / 10:
+        return ((4356 / 361.0 * x * x) - (35442 / 1805.0 * x) + 16061 / 1805.0) * 100
+    return ((54 / 5.0 * x * x) - (513 / 25.0 * x) + 268 / 25.0) * 100
+
+class Transition:
+
+    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
+
+        self.fromSurface = fromSurface
+        self.toSurface = toSurface
+        self.duration = duration
+        self.drawMethod = drawMethod
+
+        self.easingFunction = easingFunction
+        self.easeValue = 0
+
+        self.currentPercentage = 0
+        self.finished = False
+
+        # allows adjusting for different durations
+        self.durationCoefficient = 100 / self.duration
+
+    def update(self, deltaTime=1):
+        perc = self.currentPercentage + (deltaTime * self.durationCoefficient)
+        self.currentPercentage = min(perc, 100)
+        self.easeValue = self.easingFunction(self.currentPercentage)
+        if self.currentPercentage == 100:
+            self.finished = True
+
+    def draw(self, surface):
+        if self.drawMethod is not None:
+            self.drawMethod
+
+    def reset(self):
+        self.currentPercentage = 0
+        self.easeValue = 0
+        self.durationCoefficient = 100 / self.duration
+
+class TransitionFade(Transition):
+
+    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=linear):
+        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
+
+    def draw(self, surface):
+        self.easeValue = self.easingFunction(self.currentPercentage)
+        if self.fromSurface is not None:
+            self.fromSurface.set_alpha((100 - self.easeValue) * 2.55)
+            surface.blit(self.fromSurface, (0, 0))
+        if self.toSurface is not None:
+            self.toSurface.set_alpha(self.easeValue * 2.55)
+            surface.blit(self.toSurface, (0, 0))
+
+    def __repr__(self):
+        return 'Transition: Fade between'
+
+class TransitionFadeToBlack(Transition):
+
+    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
+        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
+        self.blacksurface = pygame.Surface((self.fromSurface.get_width(), self.fromSurface.get_height()), pygame.SRCALPHA, 32)
+        self.blacksurface.fill('black')
+
+    def draw(self, surface):
+        self.easeValue = self.easingFunction(self.currentPercentage)
+        if self.fromSurface is not None and self.easeValue < 50:
+            surface.blit(self.fromSurface, (0, 0))
+        if self.toSurface is not None and self.easeValue > 50:
+            surface.blit(self.toSurface, (0, 0))
+        distanceFromMidPoint = abs(50 - self.easeValue)
+        percentageToAlpha = 255 - (distanceFromMidPoint * 2.55 * 2)
+        self.blacksurface.set_alpha(percentageToAlpha)
+        surface.blit(self.blacksurface, (0, 0))
+
+    def __repr__(self):
+        return 'Transition: Fade to black'
+
+class TransitionWipeLeft(Transition):
+
+    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
+        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
+
+    def draw(self, surface):
+        self.easeValue = self.easingFunction(self.currentPercentage)
+        if self.fromSurface is not None:
+            surface.blit(self.fromSurface, (0, 0))
+        if self.toSurface is not None:
+            self.toSurface.set_alpha(255)
+            r = (surface.get_width()) - (surface.get_width() / 100 * self.easeValue)
+            surface.blit(self.toSurface, (r, 0))
+
+    def __repr__(self):
+        return 'Transition: Wipe left'
+
+class TransitionWipeRight(Transition):
+
+    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
+        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
+
+    def draw(self, surface):
+        self.easeValue = self.easingFunction(self.currentPercentage)
+        if self.fromSurface is not None:
+            surface.blit(self.fromSurface, (0, 0))
+        if self.toSurface is not None:
+            self.toSurface.set_alpha(255)
+            r = ((surface.get_width() * -1)) + (surface.get_width() / 100 * self.easeValue)
+            surface.blit(self.toSurface, (r, 0))
+
+    def __repr__(self):
+        return 'Transition: Wipe right'
+
+class TransitionWipeUp(Transition):
+
+    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
+        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
+
+    def draw(self, surface):
+        self.easeValue = self.easingFunction(self.currentPercentage)
+        if self.fromSurface is not None:
+            surface.blit(self.fromSurface, (0, 0))
+        if self.toSurface is not None:
+            self.toSurface.set_alpha(255)
+            r = (surface.get_height()) - (surface.get_height() / 100 * self.easeValue)
+            surface.blit(self.toSurface, (0, r))
+
+    def __repr__(self):
+        return 'Transition: Wipe up'
+
+class TransitionWipeDown(Transition):
+
+    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
+        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
+
+    def draw(self, surface):
+        self.easeValue = self.easingFunction(self.currentPercentage)
+        if self.fromSurface is not None:
+            surface.blit(self.fromSurface, (0, 0))
+        if self.toSurface is not None:
+            self.toSurface.set_alpha(255)
+            r = ((surface.get_height() * -1)) + (surface.get_height() / 100 * self.easeValue)
+            surface.blit(self.toSurface, (0, r))
+
+    def __repr__(self):
+        return 'Transition: Wipe down'
+
+class TransitionMoveLeft(Transition):
+
+    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
+        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
+
+    def draw(self, surface):
+        self.easeValue = self.easingFunction(self.currentPercentage)
+        if self.fromSurface is not None:
+            self.fromSurface.set_alpha(255)
+            r = 0 - (surface.get_width() / 100 * self.easeValue)
+            surface.blit(self.fromSurface, (r, 0))
+        if self.toSurface is not None:
+            self.toSurface.set_alpha(255)
+            r = (surface.get_width()) - (surface.get_width() / 100 * self.easeValue)
+            surface.blit(self.toSurface, (r, 0))
+
+    def __repr__(self):
+        return 'Transition: Move left'
+
+class TransitionMoveRight(Transition):
+
+    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
+        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
+
+    def draw(self, surface):
+        self.easeValue = self.easingFunction(self.currentPercentage)
+        if self.fromSurface is not None:
+            self.fromSurface.set_alpha(255)
+            r = (surface.get_width() / 100 * self.easeValue)
+            surface.blit(self.fromSurface, (r, 0))
+        if self.toSurface is not None:
+            self.toSurface.set_alpha(255)
+            r = ((surface.get_width() * -1)) + (surface.get_width() / 100 * self.easeValue)
+            surface.blit(self.toSurface, (r, 0))
+
+    def __repr__(self):
+        return 'Transition: Move right'
+
+class TransitionMoveUp(Transition):
+
+    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
+        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
+
+    def draw(self, surface):
+        self.easeValue = self.easingFunction(self.currentPercentage)
+        if self.fromSurface is not None:
+            self.fromSurface.set_alpha(255)
+            r = 0 - (surface.get_height() / 100 * self.easeValue)
+            surface.blit(self.fromSurface, (0, r))
+        if self.toSurface is not None:
+            self.toSurface.set_alpha(255)
+            r = (surface.get_height()) - (surface.get_height() / 100 * self.easeValue)
+            surface.blit(self.toSurface, (0, r))
+
+    def __repr__(self):
+        return 'Transition: Move up'
+
+class TransitionMoveDown(Transition):
+
+    def __init__(self, fromSurface=None, toSurface=None, duration=100, drawMethod=None, easingFunction=None):
+        super().__init__(fromSurface, toSurface, duration, drawMethod, easingFunction)
+
+    def draw(self, surface):
+        self.easeValue = self.easingFunction(self.currentPercentage)
+        if self.fromSurface is not None:
+            self.fromSurface.set_alpha(255)
+            r = (surface.get_height() / 100 * self.easeValue)
+            surface.blit(self.fromSurface, (0, r))
+        if self.toSurface is not None:
+            self.toSurface.set_alpha(255)
+            r = ((surface.get_height() * -1)) + (surface.get_height() / 100 * self.easeValue)
+            surface.blit(self.toSurface, (0, r))
+
+    def __repr__(self):
         return 'Transition: Move down'
```

### Comparing `pygamepal-0.2.0/LICENSE` & `pygamepal-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Rik Cross
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Rik Cross
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

