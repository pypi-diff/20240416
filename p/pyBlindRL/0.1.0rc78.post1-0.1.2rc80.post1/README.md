# Comparing `tmp/pyblindrl-0.1.0rc78.post1.tar.gz` & `tmp/pyblindrl-0.1.2rc80.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblindrl-0.1.0rc78.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyblindrl-0.1.2rc80.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyblindrl-0.1.0rc78.post1.tar` & `pyblindrl-0.1.2rc80.post1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      340 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      418 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      476 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.pypirc
--rw-r--r--   0        0        0      459 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1137 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/LICENSE
--rw-r--r--   0        0        0      458 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/README.md
--rw-r--r--   0        0        0      634 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/Makefile
--rw-r--r--   0        0        0     2320 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/developer.md
--rw-r--r--   0        0        0      461 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/make.bat
--rw-r--r--   0        0        0       57 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/pyproject.md
--rw-r--r--   0        0        0      437 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      406 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/docs/workflows.md
--rw-r--r--   0        0        0     6579 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/src/README.md
--rw-r--r--   0        0        0      406 2024-04-16 14:34:43.480414 pyblindrl-0.1.0rc78.post1/src/pyBlindRL/__init__.py
--rw-r--r--   0        0        0     6952 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/src/pyBlindRL/commands.py
--rw-r--r--   0        0        0      989 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/tests/conftest.py
--rw-r--r--   0        0        0      562 2024-04-16 14:34:29.848406 pyblindrl-0.1.0rc78.post1/tests/test_methods.py
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 pyblindrl-0.1.0rc78.post1/PKG-INFO
+-rw-r--r--   0        0        0      340 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      418 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      476 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1137 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/LICENSE
+-rw-r--r--   0        0        0      458 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/README.md
+-rw-r--r--   0        0        0      634 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/Makefile
+-rw-r--r--   0        0        0     2320 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/developer.md
+-rw-r--r--   0        0        0      461 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/make.bat
+-rw-r--r--   0        0        0       57 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      437 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      406 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6579 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/src/README.md
+-rw-r--r--   0        0        0      406 2024-04-16 18:48:35.477275 pyblindrl-0.1.2rc80.post1/src/pyBlindRL/__init__.py
+-rw-r--r--   0        0        0     7238 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/src/pyBlindRL/commands.py
+-rw-r--r--   0        0        0      989 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/tests/conftest.py
+-rw-r--r--   0        0        0      562 2024-04-16 18:48:23.517230 pyblindrl-0.1.2rc80.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 pyblindrl-0.1.2rc80.post1/PKG-INFO
```

### Comparing `pyblindrl-0.1.0rc78.post1/.devcontainer/devcontainer.json` & `pyblindrl-0.1.2rc80.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/.github/workflows/schedule-update-actions.yml` & `pyblindrl-0.1.2rc80.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/.gitignore` & `pyblindrl-0.1.2rc80.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/.pre-commit-config.yaml` & `pyblindrl-0.1.2rc80.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/.vscode/settings.json` & `pyblindrl-0.1.2rc80.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/LICENSE` & `pyblindrl-0.1.2rc80.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/docs/Makefile` & `pyblindrl-0.1.2rc80.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/docs/conf.py` & `pyblindrl-0.1.2rc80.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/docs/make.bat` & `pyblindrl-0.1.2rc80.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/docs/pylint.md` & `pyblindrl-0.1.2rc80.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/pyproject.toml` & `pyblindrl-0.1.2rc80.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/src/pyBlindRL/commands.py` & `pyblindrl-0.1.2rc80.post1/src/pyBlindRL/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,37 +32,49 @@
 
     gaussian_array -= gaussian_array.min()
     gaussian_array /= gaussian_array.max()
 
     return gaussian_array
 
 
+def emplace_center(img, img2, dtype=np.complex128):
+    """
+    Place given img2 into the center of a new array given dimensions of img
+
+    Parameters:
+        img (3d numpy array): Image to use as a template
+        img2 (3d numpy array): Image to place
+    """
+    out = np.zeros_like(img, dtype=dtype)
+
+    out[
+        int(img.shape[0] / 2 - img2.shape[0] / 2) :,
+        int(img.shape[1] / 2 - img2.shape[1] / 2) :,
+        int(img.shape[2] / 2 - img2.shape[2] / 2) :,
+    ][: img2.shape[0], : img2.shape[1], : img2.shape[2]] += img2
+
+    return out
+
+
 def generate_initial_psf(img):
     """
     Creates a PSF image based on a Gaussian centered on the corners
 
     Parameters:
         img (3d numpy array): Image to use as a template
     """
-    out = np.zeros_like(img, dtype=np.complex128)
-    out += 1
-
     psf_shape = (64, 64, 64)
     psf = gaussian_3d(psf_shape, sigma=(1, 1, 2))
 
-    out[
-        int(img.shape[0] / 2 - psf.shape[0] / 2) :,
-        int(img.shape[1] / 2 - psf.shape[1] / 2) :,
-        int(img.shape[2] / 2 - psf.shape[2] / 2) :,
-    ][: psf.shape[0], : psf.shape[1], : psf.shape[2]] += psf
+    out = emplace_center(img, psf)
+    out += 1
 
     out = roll_psf(out)
 
     return out
-    # return np.fft.fftn(out)
 
 
 def roll_psf(img):
     """
     Roll PSF at center of image to edge of image.
 
     Parameters:
```

### Comparing `pyblindrl-0.1.0rc78.post1/tests/conftest.py` & `pyblindrl-0.1.2rc80.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/tests/test_methods.py` & `pyblindrl-0.1.2rc80.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.1.0rc78.post1/PKG-INFO` & `pyblindrl-0.1.2rc80.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBlindRL
-Version: 0.1.0rc78.post1
+Version: 0.1.2rc80.post1
 Summary: A Python implementation of blind Richardson-Lucy deconvolution
 Author-email: "Logan Walker, PhD" <loganaw@umich.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

