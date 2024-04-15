# Comparing `tmp/decor8ai-0.20.tar.gz` & `tmp/decor8ai-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decor8ai-0.20.tar", max compression
+gzip compressed data, was "decor8ai-0.21.tar", max compression
```

## Comparing `decor8ai-0.20.tar` & `decor8ai-0.21.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11045 2024-03-13 21:08:08.996416 decor8ai-0.20/README.md
--rw-r--r--   0        0        0        0 2023-10-24 05:55:12.275635 decor8ai-0.20/decor8ai/__init__.py
--rw-r--r--   0        0        0     4951 2024-03-13 20:56:15.674918 decor8ai-0.20/decor8ai/client.py
--rw-r--r--   0        0        0      534 2024-03-13 21:25:14.235257 decor8ai-0.20/pyproject.toml
--rw-r--r--   0        0        0    11725 1970-01-01 00:00:00.000000 decor8ai-0.20/PKG-INFO
+-rw-r--r--   0        0        0    11102 2024-04-15 18:41:58.478588 decor8ai-0.21/README.md
+-rw-r--r--   0        0        0        0 2023-10-24 05:55:12.275635 decor8ai-0.21/decor8ai/__init__.py
+-rw-r--r--   0        0        0     6445 2024-04-15 17:37:52.313129 decor8ai-0.21/decor8ai/client.py
+-rw-r--r--   0        0        0      534 2024-04-15 23:21:07.668205 decor8ai-0.21/pyproject.toml
+-rw-r--r--   0        0        0    11782 1970-01-01 00:00:00.000000 decor8ai-0.21/PKG-INFO
```

### Comparing `decor8ai-0.20/README.md` & `decor8ai-0.21/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,30 +53,30 @@
 ```bash
 export DECOR8AI_API_KEY='<YOUR_API_KEY>'
 ```
 
 ## <a id="design-with-photo"> Generating Interior Design with a Photo of the room
 
 ```python
-from decor8ai.client import generate_designs
+from decor8ai.client import generate_designs_for_room
 
 # Mandatory Parameters
-input_image = 'path/to/your/image.png'  #local-file-path or URL or bytes
+input_image_url = 'https://prod-files.decor8.ai/test-images/sdk_test_image.png'  #local-file-path or URL or bytes
 room_type = 'livingroom' # See below for all supported room types
 design_style = 'frenchcountry' # See below for all supported design Styles
 num_images = 1 # Up to 4 images can be generated at a time
 
 # Optional Parameters
 num_captions = None # Choose 1 or 2 for number of image captions to generate
 keep_original_dimensions = False # Optional. True or False. Generated designs retain original image's dimensions (and aspect ratio)
 color_scheme = 'COLOR_SCHEME_5' # Optional
-speciality_decor = 'SPECIALITY_DECOR_5'; # Optional
-
+speciality_decor = 'SPECIALITY_DECOR_5' # Optional
+mask_info = None #Optional. Use mask_info string returned by first invocation of generate_designs_for_room api. Helpful in speeding up api response time.
 
-response_json = generate_designs(input_image=input_image, room_type=room_type, design_style=design_style, num_images=num_images, num_captions=1, keep_original_dimensions=True, color_scheme=color_scheme, speciality_decor=speciality_decor)
+response_json = generate_designs_for_room(input_image_url=input_image_url, mask_info=mask_info, room_type=room_type, design_style=design_style, num_images=num_images, keep_original_dimensions=True, color_scheme=color_scheme, speciality_decor=speciality_decor)
 
 ```
 
 ```
 The response is a JSON object containing the generated designs and other information.
 
 Sample response for successful design generation
@@ -86,21 +86,17 @@
     "message": "Successfully generated designs.",
     "info":
     {
         "images":
         [
             {
                 "uuid": "81133196-4477-4cdd-834a-89f5482bb9d0",
-                "data": "<base64-encoded_data>",
+                "url": "http://<generated-image-path>",
                 "width": 768,
-                "height": 512,
-                "captions":
-                [
-                    "Unveiling the art of rustic elegance in this French Country haven, where warmth and sophistication meet effortlessly."
-                ]
+                "height": 512
             }
         ]
     }
 }
 
 Sample response when unsuccessful. "error" will be non-empty value.
 {
@@ -129,18 +125,18 @@
 ## <a id="prime-the-walls">Priming the walls
 
 If your room contains unfinished walls, unpainted walls or walls which need touch-up, use this API to get walls with basic white colored, smooth textured walls or as it's called 'primed walls'. 
 
 You can use the returned image as input to generate_designs API for filling it with furniture. 
 
 ```Python
-from decor8ai.client import prime_the_room_walls
+from decor8ai.client import prime_walls_for_room
 
-input_image = 'path/to/your/image.png'  #local-file-path or URL or bytes
-response_json = prime_the_room_walls(input_image=input_image)
+input_image_url = 'http://example.com/path/to/your/image.png'  #local-file-path or URL or bytes
+response_json = prime_walls_for_room(input_image_url=input_image_url)
 
 ```
 ## <a id="upscale-the-image">Upscale the image
 AI generated designs may have a smaller resolution for some use-cases. Use this API to get upto 4x the original resolution of the image. Original images of upto maximum 1024px width or height or both are supported. 
 
 ```Python
 from decor8ai.client import upscale_image
```

### Comparing `decor8ai-0.20/decor8ai/client.py` & `decor8ai-0.21/decor8ai/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,50 +6,66 @@
 dev_server_url = 'http://localhost:8000'
 prod_server_url = 'https://prod-app.decor8.ai:8000'
 url = prod_server_url
 token = os.environ.get('DECOR8AI_API_KEY')
 
 
 def prime_the_room_walls(input_image):
-        
-        def is_url(path):
-            try:
-                result = urlparse(path)
-                return all([result.scheme, result.netloc])
-            except ValueError:
-                return False
-        
-        if not token:
-            raise Exception("DECOR8AI_API_KEY environment variable is not set.")
-        
-        headers = {
-            'Authorization': f'Bearer {token}'
-        }
-        
-        # Handling various input types for the image
-        if isinstance(input_image, bytes):
-            input_image_content = input_image
-        elif is_url(input_image):
-            response = requests.get(input_image)
-            input_image_content = response.content
-        else:  # Assuming it's a file path
-            with open(input_image, 'rb') as img_file:
-                input_image_content = img_file.read()
-        
-        files = {
-            'input_image': ('input_image.jpg', input_image_content)
-        }
-        
-        response = requests.post(url + '/prime_the_room_walls', headers=headers, files=files)
-        response_json = json.loads(response.text)
-        
-        return response_json
+    def is_url(path):
+        try:
+            result = urlparse(path)
+            return all([result.scheme, result.netloc])
+        except ValueError:
+            return False
+    
+    if not token:
+        raise Exception("DECOR8AI_API_KEY environment variable is not set.")
+    
+    headers = {
+        'Authorization': f'Bearer {token}'
+    }
+    
+    # Handling various input types for the image
+    if isinstance(input_image, bytes):
+        input_image_content = input_image
+    elif is_url(input_image):
+        response = requests.get(input_image)
+        input_image_content = response.content
+    else:  # Assuming it's a file path
+        with open(input_image, 'rb') as img_file:
+            input_image_content = img_file.read()
+    
+    files = {
+        'input_image': ('input_image.jpg', input_image_content)
+    }
+    
+    response = requests.post(url + '/prime_the_room_walls', headers=headers, files=files)
+    response_json = json.loads(response.text)
+    
+    return response_json
 
-def generate_designs(input_image, room_type, design_style, num_captions = None, num_images=1, keep_original_dimensions=False, color_scheme=None, speciality_decor=None):
+def prime_walls_for_room(input_image_url):
+            
+    if not token:
+        raise Exception("DECOR8AI_API_KEY environment variable is not set.")
     
+    headers = {
+        'Authorization': f'Bearer {token}'
+    }
+
+    data = {
+        'input_image_url': input_image_url
+    }
+    
+    response = requests.post(url + '/prime_walls_for_room', headers=headers, data=data)
+    response_json = json.loads(response.text)
+    
+    return response_json
+
+def generate_designs(input_image, room_type, design_style, num_captions = None, num_images=1, keep_original_dimensions=False, color_scheme=None, speciality_decor=None):
     def is_url(path):
         try:
             result = urlparse(path)
             return all([result.scheme, result.netloc])
         except ValueError:
             return False
     
@@ -91,14 +107,51 @@
         
     response = requests.post(url + '/generate_designs', headers=headers, files=files, data=data)
     
     response_json = json.loads(response.text)
     
     return response_json
 
+def generate_designs_for_room(input_image_url,room_type, design_style,  mask_info = None, num_images=1, keep_original_dimensions=False, color_scheme=None, speciality_decor=None):
+    
+    def is_url(path):
+        try:
+            result = urlparse(path)
+            return all([result.scheme, result.netloc])
+        except ValueError:
+            return False
+    
+    if not token:
+        raise Exception("DECOR8AI_API_KEY environment variable is not set.")
+    
+    headers = {
+        'Authorization': f'Bearer {token}'
+    }
+    data = {
+        'input_image_url': input_image_url,
+        'room_type': room_type,
+        'design_style': design_style,
+        'num_images': num_images
+    }
+    if keep_original_dimensions:
+        data['keep_original_dimensions'] = keep_original_dimensions
+    if color_scheme:
+        data['color_scheme'] = color_scheme
+    if speciality_decor:
+        data['speciality_decor'] = speciality_decor
+
+    if mask_info:
+        data['mask_info'] = mask_info
+        
+    response = requests.post(url + '/generate_designs_for_room', headers=headers, data=data)
+    
+    response_json = json.loads(response.text)
+    
+    return response_json
+
 def generate_image_captions(design_style, room_type, num_captions):
     
     if not token:
         raise Exception("DECOR8AI_API_KEY environment variable is not set.")
     
     headers = {
         'Authorization': f'Bearer {token}'
```

### Comparing `decor8ai-0.20/pyproject.toml` & `decor8ai-0.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decor8ai"
-version = "0.20"
+version = "0.21"
 description = "Decor8 AI is an AI Interior Design Tool. With Decor8 AI Python SDK, you can automate interior design generation tasks for room photos."
 authors = ["Akhilesh Joshi <akhilesh@immex.tech>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.decor8.ai"
 repository = "https://github.com/immex-tech/decor8ai-sdk"
```

### Comparing `decor8ai-0.20/PKG-INFO` & `decor8ai-0.21/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decor8ai
-Version: 0.20
+Version: 0.21
 Summary: Decor8 AI is an AI Interior Design Tool. With Decor8 AI Python SDK, you can automate interior design generation tasks for room photos.
 Home-page: https://www.decor8.ai
 License: MIT
 Author: Akhilesh Joshi
 Author-email: akhilesh@immex.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -70,30 +70,30 @@
 ```bash
 export DECOR8AI_API_KEY='<YOUR_API_KEY>'
 ```
 
 ## <a id="design-with-photo"> Generating Interior Design with a Photo of the room
 
 ```python
-from decor8ai.client import generate_designs
+from decor8ai.client import generate_designs_for_room
 
 # Mandatory Parameters
-input_image = 'path/to/your/image.png'  #local-file-path or URL or bytes
+input_image_url = 'https://prod-files.decor8.ai/test-images/sdk_test_image.png'  #local-file-path or URL or bytes
 room_type = 'livingroom' # See below for all supported room types
 design_style = 'frenchcountry' # See below for all supported design Styles
 num_images = 1 # Up to 4 images can be generated at a time
 
 # Optional Parameters
 num_captions = None # Choose 1 or 2 for number of image captions to generate
 keep_original_dimensions = False # Optional. True or False. Generated designs retain original image's dimensions (and aspect ratio)
 color_scheme = 'COLOR_SCHEME_5' # Optional
-speciality_decor = 'SPECIALITY_DECOR_5'; # Optional
-
+speciality_decor = 'SPECIALITY_DECOR_5' # Optional
+mask_info = None #Optional. Use mask_info string returned by first invocation of generate_designs_for_room api. Helpful in speeding up api response time.
 
-response_json = generate_designs(input_image=input_image, room_type=room_type, design_style=design_style, num_images=num_images, num_captions=1, keep_original_dimensions=True, color_scheme=color_scheme, speciality_decor=speciality_decor)
+response_json = generate_designs_for_room(input_image_url=input_image_url, mask_info=mask_info, room_type=room_type, design_style=design_style, num_images=num_images, keep_original_dimensions=True, color_scheme=color_scheme, speciality_decor=speciality_decor)
 
 ```
 
 ```
 The response is a JSON object containing the generated designs and other information.
 
 Sample response for successful design generation
@@ -103,21 +103,17 @@
     "message": "Successfully generated designs.",
     "info":
     {
         "images":
         [
             {
                 "uuid": "81133196-4477-4cdd-834a-89f5482bb9d0",
-                "data": "<base64-encoded_data>",
+                "url": "http://<generated-image-path>",
                 "width": 768,
-                "height": 512,
-                "captions":
-                [
-                    "Unveiling the art of rustic elegance in this French Country haven, where warmth and sophistication meet effortlessly."
-                ]
+                "height": 512
             }
         ]
     }
 }
 
 Sample response when unsuccessful. "error" will be non-empty value.
 {
@@ -146,18 +142,18 @@
 ## <a id="prime-the-walls">Priming the walls
 
 If your room contains unfinished walls, unpainted walls or walls which need touch-up, use this API to get walls with basic white colored, smooth textured walls or as it's called 'primed walls'. 
 
 You can use the returned image as input to generate_designs API for filling it with furniture. 
 
 ```Python
-from decor8ai.client import prime_the_room_walls
+from decor8ai.client import prime_walls_for_room
 
-input_image = 'path/to/your/image.png'  #local-file-path or URL or bytes
-response_json = prime_the_room_walls(input_image=input_image)
+input_image_url = 'http://example.com/path/to/your/image.png'  #local-file-path or URL or bytes
+response_json = prime_walls_for_room(input_image_url=input_image_url)
 
 ```
 ## <a id="upscale-the-image">Upscale the image
 AI generated designs may have a smaller resolution for some use-cases. Use this API to get upto 4x the original resolution of the image. Original images of upto maximum 1024px width or height or both are supported. 
 
 ```Python
 from decor8ai.client import upscale_image
```

