# Comparing `tmp/hidiffusion-0.1.2.tar.gz` & `tmp/hidiffusion-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidiffusion-0.1.2.tar", last modified: Tue Apr 16 06:51:36 2024, max compression
+gzip compressed data, was "hidiffusion-0.1.4.tar", last modified: Tue Apr 16 08:23:53 2024, max compression
```

## Comparing `hidiffusion-0.1.2.tar` & `hidiffusion-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-16 06:51:36.435990 hidiffusion-0.1.2/
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)    14917 2024-04-16 06:51:36.435990 hidiffusion-0.1.2/PKG-INFO
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)    14624 2024-04-16 06:49:20.000000 hidiffusion-0.1.2/README.md
-drwxr-xr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-16 06:51:36.411989 hidiffusion-0.1.2/hidiffusion/
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)      118 2024-04-16 06:49:20.000000 hidiffusion-0.1.2/hidiffusion/__init__.py
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)   103957 2024-04-16 06:49:20.000000 hidiffusion-0.1.2/hidiffusion/hidiffusion.py
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)      872 2024-04-16 06:49:20.000000 hidiffusion-0.1.2/hidiffusion/utils.py
-drwxr-xr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-16 06:51:36.431990 hidiffusion-0.1.2/hidiffusion.egg-info/
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)    14917 2024-04-16 06:51:35.000000 hidiffusion-0.1.2/hidiffusion.egg-info/PKG-INFO
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)      230 2024-04-16 06:51:35.000000 hidiffusion-0.1.2/hidiffusion.egg-info/SOURCES.txt
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)        1 2024-04-16 06:51:35.000000 hidiffusion-0.1.2/hidiffusion.egg-info/dependency_links.txt
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)       12 2024-04-16 06:51:35.000000 hidiffusion-0.1.2/hidiffusion.egg-info/top_level.txt
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)       38 2024-04-16 06:51:36.435990 hidiffusion-0.1.2/setup.cfg
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)      462 2024-04-16 06:50:02.000000 hidiffusion-0.1.2/setup.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       35 2024-04-16 08:22:52.000000 hidiffusion-0.1.4/MANIFEST.in
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)    14898 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/PKG-INFO
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    14605 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/README.md
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/hidiffusion/
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      118 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/hidiffusion/__init__.py
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   103957 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/hidiffusion/hidiffusion.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/hidiffusion/sd_module_key/
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    30444 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/hidiffusion/sd_module_key/sd15_module_key.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   100878 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/hidiffusion/sd_module_key/sdxl_module_key.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      872 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/hidiffusion/utils.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/hidiffusion.egg-info/
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)    14898 2024-04-16 08:23:53.000000 hidiffusion-0.1.4/hidiffusion.egg-info/PKG-INFO
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      334 2024-04-16 08:23:53.000000 hidiffusion-0.1.4/hidiffusion.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)        1 2024-04-16 08:23:53.000000 hidiffusion-0.1.4/hidiffusion.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       12 2024-04-16 08:23:53.000000 hidiffusion-0.1.4/hidiffusion.egg-info/top_level.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       38 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/setup.cfg
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      493 2024-04-16 08:22:44.000000 hidiffusion-0.1.4/setup.py
```

### Comparing `hidiffusion-0.1.2/PKG-INFO` & `hidiffusion-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidiffusion
-Version: 0.1.2
+Version: 0.1.4
 Summary: HiDiffusion: A training-free method to increase the resolution and speed of diffusion models.
 Home-page: 
 Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 Description-Content-Type: text/markdown
 
 <!-- # 💡 HiDiffusion -->
 
@@ -56,40 +56,40 @@
 ## 💣 Supported Tasks
 
 - ✅ Text-to-image
 - ✅ ControlNet
 - ✅ Inpainting
 
 
-## 🔎 Main requirements
+## 🔎 Main Requirements
 This repository is tested on
 * Python==3.8
 * torch==1.13.1
 * diffusers==0.27.0
 * transformers==4.27.4
 * accelerate==0.18.0
 * xformers==0.0.16rc425
 
 ## 🔑 Install HiDiffusion
-After installing the packages in the main requirements, install HiDiffusion:
+After installing the packages in the [main requirements](#-main-requirements), install HiDiffusion:
 ```shell
 pip3 install hidiffusion
 ```
 ### Installing from source
 Alternatively, you can install from github source. Clone the repository and install:
 ```bash
 git clone https://github.com/ShenZhang-Shin/HiDiffusion.git
 cd HiDiffusion
 python3 setup.py install
 ```
 
 
 ## 🚀 Usage
 
-Generating outputs with HiDiffusion is super easy based on 🤗 [diffusers](https://github.com/huggingface/diffusers/tree/main).
+Generating outputs with HiDiffusion is super easy based on 🤗 [diffusers](https://github.com/huggingface/diffusers/tree/main). **You just need to add a single line of code**.
 
 ## Text-to-image generation
 
 ### Stable Diffusion XL
 
 ```python
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
@@ -322,20 +322,19 @@
 
 
 ## Integration into downstream models
 HiDiffusion supports models based on [supported models](#-supported-models), such as [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion), [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-aesthetic), etc.
 
 ### Ghibli-Diffusion
 ```python
-from diffusers import StableDiffusionPipeline, DDIMScheduler
+from diffusers import StableDiffusionPipeline
 import torch
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
 
 model_id = "nitrosocke/Ghibli-Diffusion"
-scheduler = DDIMScheduler.from_pretrained(model_id, subfolder="scheduler")
 pipe = StableDiffusionPipeline.from_pretrained(model_id, torch_dtype=torch.float16)
 pipe = pipe.to("cuda")
 
 # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe)
 
 prompt = "ghibli style magical princess with golden hair"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.2 Summary: HiDiffusion: A
+Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.4 Summary: HiDiffusion: A
 training-free method to increase the resolution and speed of diffusion models.
 Home-page: Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang,
 Jiajun Liang Description-Content-Type: text/markdown ###
   ð¡ HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
                           Pretrained Diffusion Models
    Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 
@@ -27,27 +27,28 @@
 stabilityai/sdxl-turbo) - â [Stable Diffusion v2](https://huggingface.co/
 stabilityai/stable-diffusion-2-1) - â [Stable Diffusion v1](https://
 huggingface.co/runwayml/stable-diffusion-v1-5) **Note**: HiDiffusion also
 supports the downstream diffusion models based on these repositories, such as
 [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion),
 [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-
 aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet -
-â Inpainting ## ð Main requirements This repository is tested on *
+â Inpainting ## ð Main Requirements This repository is tested on *
 Python==3.8 * torch==1.13.1 * diffusers==0.27.0 * transformers==4.27.4 *
 accelerate==0.18.0 * xformers==0.0.16rc425 ## ð Install HiDiffusion After
-installing the packages in the main requirements, install HiDiffusion: ```shell
-pip3 install hidiffusion ``` ### Installing from source Alternatively, you can
-install from github source. Clone the repository and install: ```bash git clone
-https://github.com/ShenZhang-Shin/HiDiffusion.git cd HiDiffusion python3
-setup.py install ``` ## ð Usage Generating outputs with HiDiffusion is super
-easy based on ð¤ [diffusers](https://github.com/huggingface/diffusers/tree/
-main). ## Text-to-image generation ### Stable Diffusion XL ```python from
-hidiffusion import apply_hidiffusion, remove_hidiffusion from diffusers import
-StableDiffusionXLPipeline, DDIMScheduler import torch pretrain_model =
-"stabilityai/stable-diffusion-xl-base-1.0" scheduler =
+installing the packages in the [main requirements](#-main-requirements),
+install HiDiffusion: ```shell pip3 install hidiffusion ``` ### Installing from
+source Alternatively, you can install from github source. Clone the repository
+and install: ```bash git clone https://github.com/ShenZhang-Shin/
+HiDiffusion.git cd HiDiffusion python3 setup.py install ``` ## ð Usage
+Generating outputs with HiDiffusion is super easy based on ð¤ [diffusers]
+(https://github.com/huggingface/diffusers/tree/main). **You just need to add a
+single line of code**. ## Text-to-image generation ### Stable Diffusion XL
+```python from hidiffusion import apply_hidiffusion, remove_hidiffusion from
+diffusers import StableDiffusionXLPipeline, DDIMScheduler import torch
+pretrain_model = "stabilityai/stable-diffusion-xl-base-1.0" scheduler =
 DDIMScheduler.from_pretrained(pretrain_model, subfolder="scheduler") pipe =
 StableDiffusionXLPipeline.from_pretrained(pretrain_model, scheduler =
 scheduler, torch_dtype=torch.float16, variant="fp16").to("cuda") # # Optional.
 enable_xformers_memory_efficient_attention can save memory usage and increase
 inference speed. enable_model_cpu_offload and enable_vae_tiling can save memory
 usage. # pipe.enable_xformers_memory_efficient_attention() #
 pipe.enable_model_cpu_offload() # pipe.enable_vae_tiling() # Apply hidiffusion
@@ -161,25 +162,24 @@
 negative_prompt, eta=1.0).images[0] image.save('steampunk_explorer.jpg') ```
 Output:
                         [assets/inpainting_result.jpg]
 ## Integration into downstream models HiDiffusion supports models based on
 [supported models](#-supported-models), such as [Ghibli-Diffusion](https://
 huggingface.co/nitrosocke/Ghibli-Diffusion), [Playground](https://
 huggingface.co/playgroundai/playground-v2-1024px-aesthetic), etc. ### Ghibli-
-Diffusion ```python from diffusers import StableDiffusionPipeline,
-DDIMScheduler import torch from hidiffusion import apply_hidiffusion,
-remove_hidiffusion model_id = "nitrosocke/Ghibli-Diffusion" scheduler =
-DDIMScheduler.from_pretrained(model_id, subfolder="scheduler") pipe =
-StableDiffusionPipeline.from_pretrained(model_id, torch_dtype=torch.float16)
-pipe = pipe.to("cuda") # Apply hidiffusion with a single line of code.
-apply_hidiffusion(pipe) prompt = "ghibli style magical princess with golden
-hair" negative_prompt="blurry, ugly, duplicate, poorly drawn face, deformed,
-mosaic, artifacts, bad limbs" image = pipe(prompt, height=1024, width=1024,
-eta=1.0, negative_prompt=negative_prompt).images[0] image.save("./
-magical_princess.jpg") ``` Output:
+Diffusion ```python from diffusers import StableDiffusionPipeline import torch
+from hidiffusion import apply_hidiffusion, remove_hidiffusion model_id =
+"nitrosocke/Ghibli-Diffusion" pipe = StableDiffusionPipeline.from_pretrained
+(model_id, torch_dtype=torch.float16) pipe = pipe.to("cuda") # Apply
+hidiffusion with a single line of code. apply_hidiffusion(pipe) prompt =
+"ghibli style magical princess with golden hair" negative_prompt="blurry, ugly,
+duplicate, poorly drawn face, deformed, mosaic, artifacts, bad limbs" image =
+pipe(prompt, height=1024, width=1024, eta=1.0,
+negative_prompt=negative_prompt).images[0] image.save("./magical_princess.jpg")
+``` Output:
                          [assets/ghibli_diffusion.jpg]
 ### Playground ```python from diffusers import DiffusionPipeline import torch
 from hidiffusion import apply_hidiffusion, remove_hidiffusion pipe =
 DiffusionPipeline.from_pretrained( "playgroundai/playground-v2-1024px-
 aesthetic", torch_dtype=torch.float16, use_safetensors=True,
 add_watermarker=False, variant="fp16" ) pipe.to("cuda")
 pipe.enable_xformers_memory_efficient_attention() # Apply hidiffusion with a
```

### Comparing `hidiffusion-0.1.2/README.md` & `hidiffusion-0.1.4/hidiffusion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: hidiffusion
+Version: 0.1.4
+Summary: HiDiffusion: A training-free method to increase the resolution and speed of diffusion models.
+Home-page: 
+Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
+Description-Content-Type: text/markdown
+
 <!-- # 💡 HiDiffusion -->
 
 ### <div align="center">💡 HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in Pretrained Diffusion Models</div> 
 
 <div align="center">Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang</div> 
 
 <br>
@@ -48,40 +56,40 @@
 ## 💣 Supported Tasks
 
 - ✅ Text-to-image
 - ✅ ControlNet
 - ✅ Inpainting
 
 
-## 🔎 Main requirements
+## 🔎 Main Requirements
 This repository is tested on
 * Python==3.8
 * torch==1.13.1
 * diffusers==0.27.0
 * transformers==4.27.4
 * accelerate==0.18.0
 * xformers==0.0.16rc425
 
 ## 🔑 Install HiDiffusion
-After installing the packages in the main requirements, install HiDiffusion:
+After installing the packages in the [main requirements](#-main-requirements), install HiDiffusion:
 ```shell
 pip3 install hidiffusion
 ```
 ### Installing from source
 Alternatively, you can install from github source. Clone the repository and install:
 ```bash
 git clone https://github.com/ShenZhang-Shin/HiDiffusion.git
 cd HiDiffusion
 python3 setup.py install
 ```
 
 
 ## 🚀 Usage
 
-Generating outputs with HiDiffusion is super easy based on 🤗 [diffusers](https://github.com/huggingface/diffusers/tree/main).
+Generating outputs with HiDiffusion is super easy based on 🤗 [diffusers](https://github.com/huggingface/diffusers/tree/main). **You just need to add a single line of code**.
 
 ## Text-to-image generation
 
 ### Stable Diffusion XL
 
 ```python
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
@@ -314,20 +322,19 @@
 
 
 ## Integration into downstream models
 HiDiffusion supports models based on [supported models](#-supported-models), such as [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion), [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-aesthetic), etc.
 
 ### Ghibli-Diffusion
 ```python
-from diffusers import StableDiffusionPipeline, DDIMScheduler
+from diffusers import StableDiffusionPipeline
 import torch
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
 
 model_id = "nitrosocke/Ghibli-Diffusion"
-scheduler = DDIMScheduler.from_pretrained(model_id, subfolder="scheduler")
 pipe = StableDiffusionPipeline.from_pretrained(model_id, torch_dtype=torch.float16)
 pipe = pipe.to("cuda")
 
 # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe)
 
 prompt = "ghibli style magical princess with golden hair"
```

#### html2text {}

```diff
@@ -1,8 +1,11 @@
-###
+Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.4 Summary: HiDiffusion: A
+training-free method to increase the resolution and speed of diffusion models.
+Home-page: Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang,
+Jiajun Liang Description-Content-Type: text/markdown ###
   ð¡ HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
                           Pretrained Diffusion Models
    Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 
                         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
 _v_1_?_l_a_b_e_l_=_P_r_o_j_e_c_t_%_2_0_P_a_g_e_&_m_e_s_s_a_g_e_=_G_i_t_h_u_b_&_c_o_l_o_r_=_b_l_u_e_&_l_o_g_o_=_g_i_t_h_u_b_-_p_a_g_e_s_]  _[_h_t_t_p_s_:_/_/
               _i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/_v_1_?_l_a_b_e_l_=_P_a_p_e_r_&_m_e_s_s_a_g_e_=_A_r_x_i_v_:
@@ -24,27 +27,28 @@
 stabilityai/sdxl-turbo) - â [Stable Diffusion v2](https://huggingface.co/
 stabilityai/stable-diffusion-2-1) - â [Stable Diffusion v1](https://
 huggingface.co/runwayml/stable-diffusion-v1-5) **Note**: HiDiffusion also
 supports the downstream diffusion models based on these repositories, such as
 [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion),
 [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-
 aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet -
-â Inpainting ## ð Main requirements This repository is tested on *
+â Inpainting ## ð Main Requirements This repository is tested on *
 Python==3.8 * torch==1.13.1 * diffusers==0.27.0 * transformers==4.27.4 *
 accelerate==0.18.0 * xformers==0.0.16rc425 ## ð Install HiDiffusion After
-installing the packages in the main requirements, install HiDiffusion: ```shell
-pip3 install hidiffusion ``` ### Installing from source Alternatively, you can
-install from github source. Clone the repository and install: ```bash git clone
-https://github.com/ShenZhang-Shin/HiDiffusion.git cd HiDiffusion python3
-setup.py install ``` ## ð Usage Generating outputs with HiDiffusion is super
-easy based on ð¤ [diffusers](https://github.com/huggingface/diffusers/tree/
-main). ## Text-to-image generation ### Stable Diffusion XL ```python from
-hidiffusion import apply_hidiffusion, remove_hidiffusion from diffusers import
-StableDiffusionXLPipeline, DDIMScheduler import torch pretrain_model =
-"stabilityai/stable-diffusion-xl-base-1.0" scheduler =
+installing the packages in the [main requirements](#-main-requirements),
+install HiDiffusion: ```shell pip3 install hidiffusion ``` ### Installing from
+source Alternatively, you can install from github source. Clone the repository
+and install: ```bash git clone https://github.com/ShenZhang-Shin/
+HiDiffusion.git cd HiDiffusion python3 setup.py install ``` ## ð Usage
+Generating outputs with HiDiffusion is super easy based on ð¤ [diffusers]
+(https://github.com/huggingface/diffusers/tree/main). **You just need to add a
+single line of code**. ## Text-to-image generation ### Stable Diffusion XL
+```python from hidiffusion import apply_hidiffusion, remove_hidiffusion from
+diffusers import StableDiffusionXLPipeline, DDIMScheduler import torch
+pretrain_model = "stabilityai/stable-diffusion-xl-base-1.0" scheduler =
 DDIMScheduler.from_pretrained(pretrain_model, subfolder="scheduler") pipe =
 StableDiffusionXLPipeline.from_pretrained(pretrain_model, scheduler =
 scheduler, torch_dtype=torch.float16, variant="fp16").to("cuda") # # Optional.
 enable_xformers_memory_efficient_attention can save memory usage and increase
 inference speed. enable_model_cpu_offload and enable_vae_tiling can save memory
 usage. # pipe.enable_xformers_memory_efficient_attention() #
 pipe.enable_model_cpu_offload() # pipe.enable_vae_tiling() # Apply hidiffusion
@@ -158,25 +162,24 @@
 negative_prompt, eta=1.0).images[0] image.save('steampunk_explorer.jpg') ```
 Output:
                         [assets/inpainting_result.jpg]
 ## Integration into downstream models HiDiffusion supports models based on
 [supported models](#-supported-models), such as [Ghibli-Diffusion](https://
 huggingface.co/nitrosocke/Ghibli-Diffusion), [Playground](https://
 huggingface.co/playgroundai/playground-v2-1024px-aesthetic), etc. ### Ghibli-
-Diffusion ```python from diffusers import StableDiffusionPipeline,
-DDIMScheduler import torch from hidiffusion import apply_hidiffusion,
-remove_hidiffusion model_id = "nitrosocke/Ghibli-Diffusion" scheduler =
-DDIMScheduler.from_pretrained(model_id, subfolder="scheduler") pipe =
-StableDiffusionPipeline.from_pretrained(model_id, torch_dtype=torch.float16)
-pipe = pipe.to("cuda") # Apply hidiffusion with a single line of code.
-apply_hidiffusion(pipe) prompt = "ghibli style magical princess with golden
-hair" negative_prompt="blurry, ugly, duplicate, poorly drawn face, deformed,
-mosaic, artifacts, bad limbs" image = pipe(prompt, height=1024, width=1024,
-eta=1.0, negative_prompt=negative_prompt).images[0] image.save("./
-magical_princess.jpg") ``` Output:
+Diffusion ```python from diffusers import StableDiffusionPipeline import torch
+from hidiffusion import apply_hidiffusion, remove_hidiffusion model_id =
+"nitrosocke/Ghibli-Diffusion" pipe = StableDiffusionPipeline.from_pretrained
+(model_id, torch_dtype=torch.float16) pipe = pipe.to("cuda") # Apply
+hidiffusion with a single line of code. apply_hidiffusion(pipe) prompt =
+"ghibli style magical princess with golden hair" negative_prompt="blurry, ugly,
+duplicate, poorly drawn face, deformed, mosaic, artifacts, bad limbs" image =
+pipe(prompt, height=1024, width=1024, eta=1.0,
+negative_prompt=negative_prompt).images[0] image.save("./magical_princess.jpg")
+``` Output:
                          [assets/ghibli_diffusion.jpg]
 ### Playground ```python from diffusers import DiffusionPipeline import torch
 from hidiffusion import apply_hidiffusion, remove_hidiffusion pipe =
 DiffusionPipeline.from_pretrained( "playgroundai/playground-v2-1024px-
 aesthetic", torch_dtype=torch.float16, use_safetensors=True,
 add_watermarker=False, variant="fp16" ) pipe.to("cuda")
 pipe.enable_xformers_memory_efficient_attention() # Apply hidiffusion with a
```

### Comparing `hidiffusion-0.1.2/hidiffusion/hidiffusion.py` & `hidiffusion-0.1.4/hidiffusion/hidiffusion.py`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.2/hidiffusion/utils.py` & `hidiffusion-0.1.4/hidiffusion/utils.py`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.2/hidiffusion.egg-info/PKG-INFO` & `hidiffusion-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: hidiffusion
-Version: 0.1.2
-Summary: HiDiffusion: A training-free method to increase the resolution and speed of diffusion models.
-Home-page: 
-Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
-Description-Content-Type: text/markdown
-
 <!-- # 💡 HiDiffusion -->
 
 ### <div align="center">💡 HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in Pretrained Diffusion Models</div> 
 
 <div align="center">Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang</div> 
 
 <br>
@@ -56,40 +48,40 @@
 ## 💣 Supported Tasks
 
 - ✅ Text-to-image
 - ✅ ControlNet
 - ✅ Inpainting
 
 
-## 🔎 Main requirements
+## 🔎 Main Requirements
 This repository is tested on
 * Python==3.8
 * torch==1.13.1
 * diffusers==0.27.0
 * transformers==4.27.4
 * accelerate==0.18.0
 * xformers==0.0.16rc425
 
 ## 🔑 Install HiDiffusion
-After installing the packages in the main requirements, install HiDiffusion:
+After installing the packages in the [main requirements](#-main-requirements), install HiDiffusion:
 ```shell
 pip3 install hidiffusion
 ```
 ### Installing from source
 Alternatively, you can install from github source. Clone the repository and install:
 ```bash
 git clone https://github.com/ShenZhang-Shin/HiDiffusion.git
 cd HiDiffusion
 python3 setup.py install
 ```
 
 
 ## 🚀 Usage
 
-Generating outputs with HiDiffusion is super easy based on 🤗 [diffusers](https://github.com/huggingface/diffusers/tree/main).
+Generating outputs with HiDiffusion is super easy based on 🤗 [diffusers](https://github.com/huggingface/diffusers/tree/main). **You just need to add a single line of code**.
 
 ## Text-to-image generation
 
 ### Stable Diffusion XL
 
 ```python
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
@@ -322,20 +314,19 @@
 
 
 ## Integration into downstream models
 HiDiffusion supports models based on [supported models](#-supported-models), such as [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion), [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-aesthetic), etc.
 
 ### Ghibli-Diffusion
 ```python
-from diffusers import StableDiffusionPipeline, DDIMScheduler
+from diffusers import StableDiffusionPipeline
 import torch
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
 
 model_id = "nitrosocke/Ghibli-Diffusion"
-scheduler = DDIMScheduler.from_pretrained(model_id, subfolder="scheduler")
 pipe = StableDiffusionPipeline.from_pretrained(model_id, torch_dtype=torch.float16)
 pipe = pipe.to("cuda")
 
 # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe)
 
 prompt = "ghibli style magical princess with golden hair"
```

#### html2text {}

```diff
@@ -1,11 +1,8 @@
-Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.2 Summary: HiDiffusion: A
-training-free method to increase the resolution and speed of diffusion models.
-Home-page: Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang,
-Jiajun Liang Description-Content-Type: text/markdown ###
+###
   ð¡ HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
                           Pretrained Diffusion Models
    Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 
                         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
 _v_1_?_l_a_b_e_l_=_P_r_o_j_e_c_t_%_2_0_P_a_g_e_&_m_e_s_s_a_g_e_=_G_i_t_h_u_b_&_c_o_l_o_r_=_b_l_u_e_&_l_o_g_o_=_g_i_t_h_u_b_-_p_a_g_e_s_]  _[_h_t_t_p_s_:_/_/
               _i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/_v_1_?_l_a_b_e_l_=_P_a_p_e_r_&_m_e_s_s_a_g_e_=_A_r_x_i_v_:
@@ -27,27 +24,28 @@
 stabilityai/sdxl-turbo) - â [Stable Diffusion v2](https://huggingface.co/
 stabilityai/stable-diffusion-2-1) - â [Stable Diffusion v1](https://
 huggingface.co/runwayml/stable-diffusion-v1-5) **Note**: HiDiffusion also
 supports the downstream diffusion models based on these repositories, such as
 [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion),
 [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-
 aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet -
-â Inpainting ## ð Main requirements This repository is tested on *
+â Inpainting ## ð Main Requirements This repository is tested on *
 Python==3.8 * torch==1.13.1 * diffusers==0.27.0 * transformers==4.27.4 *
 accelerate==0.18.0 * xformers==0.0.16rc425 ## ð Install HiDiffusion After
-installing the packages in the main requirements, install HiDiffusion: ```shell
-pip3 install hidiffusion ``` ### Installing from source Alternatively, you can
-install from github source. Clone the repository and install: ```bash git clone
-https://github.com/ShenZhang-Shin/HiDiffusion.git cd HiDiffusion python3
-setup.py install ``` ## ð Usage Generating outputs with HiDiffusion is super
-easy based on ð¤ [diffusers](https://github.com/huggingface/diffusers/tree/
-main). ## Text-to-image generation ### Stable Diffusion XL ```python from
-hidiffusion import apply_hidiffusion, remove_hidiffusion from diffusers import
-StableDiffusionXLPipeline, DDIMScheduler import torch pretrain_model =
-"stabilityai/stable-diffusion-xl-base-1.0" scheduler =
+installing the packages in the [main requirements](#-main-requirements),
+install HiDiffusion: ```shell pip3 install hidiffusion ``` ### Installing from
+source Alternatively, you can install from github source. Clone the repository
+and install: ```bash git clone https://github.com/ShenZhang-Shin/
+HiDiffusion.git cd HiDiffusion python3 setup.py install ``` ## ð Usage
+Generating outputs with HiDiffusion is super easy based on ð¤ [diffusers]
+(https://github.com/huggingface/diffusers/tree/main). **You just need to add a
+single line of code**. ## Text-to-image generation ### Stable Diffusion XL
+```python from hidiffusion import apply_hidiffusion, remove_hidiffusion from
+diffusers import StableDiffusionXLPipeline, DDIMScheduler import torch
+pretrain_model = "stabilityai/stable-diffusion-xl-base-1.0" scheduler =
 DDIMScheduler.from_pretrained(pretrain_model, subfolder="scheduler") pipe =
 StableDiffusionXLPipeline.from_pretrained(pretrain_model, scheduler =
 scheduler, torch_dtype=torch.float16, variant="fp16").to("cuda") # # Optional.
 enable_xformers_memory_efficient_attention can save memory usage and increase
 inference speed. enable_model_cpu_offload and enable_vae_tiling can save memory
 usage. # pipe.enable_xformers_memory_efficient_attention() #
 pipe.enable_model_cpu_offload() # pipe.enable_vae_tiling() # Apply hidiffusion
@@ -161,25 +159,24 @@
 negative_prompt, eta=1.0).images[0] image.save('steampunk_explorer.jpg') ```
 Output:
                         [assets/inpainting_result.jpg]
 ## Integration into downstream models HiDiffusion supports models based on
 [supported models](#-supported-models), such as [Ghibli-Diffusion](https://
 huggingface.co/nitrosocke/Ghibli-Diffusion), [Playground](https://
 huggingface.co/playgroundai/playground-v2-1024px-aesthetic), etc. ### Ghibli-
-Diffusion ```python from diffusers import StableDiffusionPipeline,
-DDIMScheduler import torch from hidiffusion import apply_hidiffusion,
-remove_hidiffusion model_id = "nitrosocke/Ghibli-Diffusion" scheduler =
-DDIMScheduler.from_pretrained(model_id, subfolder="scheduler") pipe =
-StableDiffusionPipeline.from_pretrained(model_id, torch_dtype=torch.float16)
-pipe = pipe.to("cuda") # Apply hidiffusion with a single line of code.
-apply_hidiffusion(pipe) prompt = "ghibli style magical princess with golden
-hair" negative_prompt="blurry, ugly, duplicate, poorly drawn face, deformed,
-mosaic, artifacts, bad limbs" image = pipe(prompt, height=1024, width=1024,
-eta=1.0, negative_prompt=negative_prompt).images[0] image.save("./
-magical_princess.jpg") ``` Output:
+Diffusion ```python from diffusers import StableDiffusionPipeline import torch
+from hidiffusion import apply_hidiffusion, remove_hidiffusion model_id =
+"nitrosocke/Ghibli-Diffusion" pipe = StableDiffusionPipeline.from_pretrained
+(model_id, torch_dtype=torch.float16) pipe = pipe.to("cuda") # Apply
+hidiffusion with a single line of code. apply_hidiffusion(pipe) prompt =
+"ghibli style magical princess with golden hair" negative_prompt="blurry, ugly,
+duplicate, poorly drawn face, deformed, mosaic, artifacts, bad limbs" image =
+pipe(prompt, height=1024, width=1024, eta=1.0,
+negative_prompt=negative_prompt).images[0] image.save("./magical_princess.jpg")
+``` Output:
                          [assets/ghibli_diffusion.jpg]
 ### Playground ```python from diffusers import DiffusionPipeline import torch
 from hidiffusion import apply_hidiffusion, remove_hidiffusion pipe =
 DiffusionPipeline.from_pretrained( "playgroundai/playground-v2-1024px-
 aesthetic", torch_dtype=torch.float16, use_safetensors=True,
 add_watermarker=False, variant="fp16" ) pipe.to("cuda")
 pipe.enable_xformers_memory_efficient_attention() # Apply hidiffusion with a
```

