# Comparing `tmp/nostr-dvm-0.3.2.tar.gz` & `tmp/nostr_dvm-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr-dvm-0.3.2.tar", last modified: Tue Apr  9 13:41:35 2024, max compression
+gzip compressed data, was "nostr_dvm-0.3.3.tar", last modified: Tue Apr 16 12:36:19 2024, max compression
```

## Comparing `nostr-dvm-0.3.2.tar` & `nostr_dvm-0.3.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.945900 nostr-dvm-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-09 13:41:35.945900 nostr-dvm-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.929900 nostr-dvm-0.3.2/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.929900 nostr-dvm-0.3.2/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.929900 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.929900 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36516 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39387 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.933899 nostr-dvm-0.3.2/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    22893 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.941900 nostr-dvm-0.3.2/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.941900 nostr-dvm-0.3.2/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.941900 nostr-dvm-0.3.2/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.945900 nostr-dvm-0.3.2/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-09 13:41:35.000000 nostr-dvm-0.3.2/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-09 13:41:35.000000 nostr-dvm-0.3.2/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:41:35.000000 nostr-dvm-0.3.2/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-09 13:41:35.000000 nostr-dvm-0.3.2/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 13:41:35.000000 nostr-dvm-0.3.2/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:41:35.945900 nostr-dvm-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:41:35.945900 nostr-dvm-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-09 13:41:31.000000 nostr-dvm-0.3.2/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.722750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.722750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.722750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.722750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39831 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39377 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.722750 nostr_dvm-0.3.3/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.726750 nostr_dvm-0.3.3/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12646 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-16 12:36:19.000000 nostr_dvm-0.3.3/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-16 12:36:19.000000 nostr_dvm-0.3.3/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:36:19.000000 nostr_dvm-0.3.3/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-16 12:36:19.000000 nostr_dvm-0.3.3/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 12:36:19.000000 nostr_dvm-0.3.3/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/tests/test_events.py
```

### Comparing `nostr-dvm-0.3.2/LICENSE` & `nostr_dvm-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/PKG-INFO` & `nostr_dvm-0.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.2
+Version: 0.3.3
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
-Requires-Dist: nostr-sdk==0.10.0
+Requires-Dist: nostr-sdk==0.11.0
 Requires-Dist: bech32
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: emoji==2.8.0
 Requires-Dist: eva-decord==0.6.1
 Requires-Dist: ffmpegio==0.8.5
 Requires-Dist: lnurl
```

### Comparing `nostr-dvm-0.3.2/README.md` & `nostr_dvm-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/bot.py` & `nostr_dvm-0.3.3/nostr_dvm/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import signal
 import time
 from datetime import timedelta
 
 from nostr_sdk import (Keys, Client, Timestamp, Filter, nip04_decrypt, HandleNotification, EventBuilder, PublicKey,
                        Options, Tag, Event, nip04_encrypt, NostrSigner, EventId, Nip19Event, Kind, KindEnum,
-                       UnsignedEvent, nip59_extract_rumor)
+                       UnsignedEvent, UnwrappedGift)
 
 from nostr_dvm.utils.admin_utils import admin_make_database_updates
 from nostr_dvm.utils.database_utils import get_or_add_user, update_user_balance, create_sql_table, update_sql_table
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.nip89_utils import nip89_fetch_events_pubkey, NIP89Config
 from nostr_dvm.utils.nostr_utils import send_event
 from nostr_dvm.utils.output_utils import PostProcessFunctionType, post_process_list_to_users, \
@@ -49,171 +49,218 @@
 
         for relay in self.dvm_config.RELAY_LIST:
             self.client.add_relay(relay)
         self.client.connect()
 
         zap_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_ZAP]).since(Timestamp.now())
         dm_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_DM]).since(Timestamp.now())
+        nip59_filter = Filter().pubkey(pk).kind(Kind.from_enum(KindEnum.GIFT_WRAP())).since(
+            Timestamp.from_secs(Timestamp.now().as_secs() - 60 * 60 * 24 * 7))
         kinds = [EventDefinitions.KIND_NIP90_GENERIC, EventDefinitions.KIND_FEEDBACK]
         for dvm in self.dvm_config.SUPPORTED_DVMS:
             if dvm.KIND not in kinds:
                 kinds.append(Kind(dvm.KIND.as_u64() + 1000))
         dvm_filter = (Filter().kinds(kinds).since(Timestamp.now()))
 
-        self.client.subscribe([zap_filter, dm_filter, dvm_filter], None)
+        self.client.subscribe([zap_filter, dm_filter, nip59_filter, dvm_filter], None)
 
         create_sql_table(self.dvm_config.DB)
         admin_make_database_updates(adminconfig=self.admin_config, dvmconfig=self.dvm_config, client=self.client)
+
         # add_sql_table_column(dvm_config.DB)
 
         class NotificationHandler(HandleNotification):
             client = self.client
             dvm_config = self.dvm_config
             keys = self.keys
 
             def handle(self, relay_url, subscription_id, nostr_event):
                 if (EventDefinitions.KIND_NIP90_EXTRACT_TEXT.as_u64() + 1000 <= nostr_event.kind().as_u64()
                         <= EventDefinitions.KIND_NIP90_GENERIC.as_u64() + 1000):
                     handle_nip90_response_event(nostr_event)
-                elif nostr_event.kind().as_u64() == EventDefinitions.KIND_FEEDBACK.as_u64():
+                elif nostr_event.kind() == EventDefinitions.KIND_FEEDBACK:
                     handle_nip90_feedback(nostr_event)
 
-                elif nostr_event.kind().as_u64() == EventDefinitions.KIND_ZAP.as_u64():
+                elif nostr_event.kind() == EventDefinitions.KIND_ZAP:
                     handle_zap(nostr_event)
 
-                elif nostr_event.kind().match_enum(KindEnum.ENCRYPTED_DIRECT_MESSAGE()):
+                elif nostr_event.kind() == EventDefinitions.KIND_DM:
                     try:
-                        handle_dm(nostr_event)
+                        handle_dm(nostr_event, False)
                     except Exception as e:
                         print(f"Error during content NIP04 decryption: {e}")
                 elif nostr_event.kind().match_enum(KindEnum.GIFT_WRAP()):
-                    print("Decrypting NIP59 event")
                     try:
-                        rumor: UnsignedEvent = nip59_extract_rumor(self.keys, nostr_event)
-                        if rumor.kind().match_enum(KindEnum.SEALED_DIRECT()):
-                            msg = rumor.content()
-                            print(f"Received new msg [sealed]: {msg}")
-                            self.client.send_sealed_msg(rumor.author(), "Nip44 is not supported yet, but coming soon", None)
-                        else:
-                            print(f"{rumor.as_json()}")
+                      handle_dm(nostr_event, True)
                     except Exception as e:
                         print(f"Error during content NIP59 decryption: {e}")
 
             def handle_msg(self, relay_url, msg):
                 return
 
-        def handle_dm(nostr_event):
+        def handle_dm(nostr_event, giftwrap):
             sender = nostr_event.author().to_hex()
             if sender == self.keys.public_key().to_hex():
                 return
-
+            decrypted_text = ""
             try:
-                decrypted_text = nip04_decrypt(self.keys.secret_key(), nostr_event.author(), nostr_event.content())
-                user = get_or_add_user(db=self.dvm_config.DB, npub=sender, client=self.client, config=self.dvm_config)
-                print("[" + self.NAME + "] Message from " + user.name + ": " + decrypted_text)
-
-                # if user selects an index from the overview list...
-                if decrypted_text[0].isdigit():
-                    split = decrypted_text.split(' ')
-                    index = int(split[0]) - 1
-                    # if user sends index info, e.g. 1 info, we fetch the nip89 information and reply with it.
-                    if len(split) > 1 and split[1].lower() == "info":
-                        answer_nip89(nostr_event, index)
-                    # otherwise we probably have to do some work, so build an event from input and send it to the DVM
-                    else:
-                        task = self.dvm_config.SUPPORTED_DVMS[index].TASK
-                        print("[" + self.NAME + "] Request from " + str(user.name) + " (" + str(user.nip05) +
-                              ", Balance: " + str(user.balance) + " Sats) Task: " + str(task))
-
-                        if user.isblacklisted:
-                            # If users are blacklisted for some reason, tell them.
-                            answer_blacklisted(nostr_event)
+                sealed = " "
+                if giftwrap:
+                    try:
+                        # Extract rumor
+                        unwrapped_gift = UnwrappedGift.from_gift_wrap(self.keys, nostr_event)
+                        sender = unwrapped_gift.sender().to_hex()
+                        rumor: UnsignedEvent = unwrapped_gift.rumor()
+
+                        # Check timestamp of rumor
+                        if rumor.created_at().as_secs() >= Timestamp.now().as_secs():
+                            if rumor.kind().match_enum(KindEnum.SEALED_DIRECT()):
+                                decrypted_text = rumor.content()
+                                print(f"Received new msg [sealed]: {decrypted_text}")
+                                sealed = " [sealed] "
+                                # client.send_sealed_msg(sender, f"Echo: {msg}", None)
+                            else:
+                                print(f"{rumor.as_json()}")
+                    except Exception as e:
+                        print(f"Error during content NIP59 decryption: {e}")
 
+                else:
+                    try:
+                        decrypted_text = nip04_decrypt(self.keys.secret_key(), nostr_event.author(),
+                                                       nostr_event.content())
+                    except Exception as e:
+                        print(f"Error during content NIP04 decryption: {e}")
+
+                if decrypted_text != "":
+                    user = get_or_add_user(db=self.dvm_config.DB, npub=sender, client=self.client,
+                                           config=self.dvm_config)
+
+                    print("[" + self.NAME + "]" + sealed + "Message from " + user.name + ": " + decrypted_text)
+
+                    # if user selects an index from the overview list...
+                    if decrypted_text != "" and decrypted_text[0].isdigit():
+
+                        split = decrypted_text.split(' ')
+                        index = int(split[0]) - 1
+                        # if user sends index info, e.g. 1 info, we fetch the nip89 information and reply with it.
+                        if len(split) > 1 and split[1].lower() == "info":
+                            answer_nip89(nostr_event, index)
+                        # otherwise we probably have to do some work, so build an event from input and send it to the DVM
                         else:
-                            # Parse inputs to params
-                            tags = build_params(decrypted_text, nostr_event, index)
-                            p_tag = Tag.parse(['p', self.dvm_config.SUPPORTED_DVMS[index].PUBLIC_KEY])
-
-                            if self.dvm_config.SUPPORTED_DVMS[index].SUPPORTS_ENCRYPTION:
-                                tags_str = []
-                                for tag in tags:
-                                    tags_str.append(tag.as_vec())
-                                params_as_str = json.dumps(tags_str)
-                                print(params_as_str)
-                                #  and encrypt them
-                                encrypted_params = nip04_encrypt(self.keys.secret_key(),
-                                                                 PublicKey.from_hex(
-                                                                     self.dvm_config.SUPPORTED_DVMS[index].PUBLIC_KEY),
-                                                                 params_as_str)
-                                #  add encrypted and p tag on the outside
-                                encrypted_tag = Tag.parse(['encrypted'])
-                                #  add the encrypted params to the content
-                                nip90request = (EventBuilder(self.dvm_config.SUPPORTED_DVMS[index].KIND,
-                                                             encrypted_params, [p_tag, encrypted_tag]).
-                                                to_event(self.keys))
-                            else:
-                                tags.append(p_tag)
+                            task = self.dvm_config.SUPPORTED_DVMS[index].TASK
+                            print("[" + self.NAME + "] Request from " + str(user.name) + " (" + str(user.nip05) +
+                                  ", Balance: " + str(user.balance) + " Sats) Task: " + str(task))
+
+                            if user.isblacklisted:
+                                # If users are blacklisted for some reason, tell them.
+                                answer_blacklisted(nostr_event, giftwrap, sender)
 
-                                nip90request = (EventBuilder(self.dvm_config.SUPPORTED_DVMS[index].KIND,
-                                                             "", tags).
-                                                to_event(self.keys))
+                            else:
+                                # Parse inputs to params
+                                tags = build_params(decrypted_text, nostr_event, index)
+                                p_tag = Tag.parse(['p', self.dvm_config.SUPPORTED_DVMS[index].PUBLIC_KEY])
+
+                                if self.dvm_config.SUPPORTED_DVMS[index].SUPPORTS_ENCRYPTION:
+                                    tags_str = []
+                                    for tag in tags:
+                                        tags_str.append(tag.as_vec())
+                                    params_as_str = json.dumps(tags_str)
+                                    print(params_as_str)
+                                    #  and encrypt them
+                                    encrypted_params = nip04_encrypt(self.keys.secret_key(),
+                                                                     PublicKey.from_hex(
+                                                                         self.dvm_config.SUPPORTED_DVMS[
+                                                                             index].PUBLIC_KEY),
+                                                                     params_as_str)
+                                    #  add encrypted and p tag on the outside
+                                    encrypted_tag = Tag.parse(['encrypted'])
+                                    #  add the encrypted params to the content
+                                    nip90request = (EventBuilder(self.dvm_config.SUPPORTED_DVMS[index].KIND,
+                                                                 encrypted_params, [p_tag, encrypted_tag]).
+                                                    to_event(self.keys))
+                                else:
+                                    tags.append(p_tag)
 
-                            # remember in the job_list that we have made an event, if anybody asks for payment,
-                            # we know we actually sent the request
-                            entry = {"npub": user.npub, "event_id": nip90request.id().to_hex(),
-                                     "dvm_key": self.dvm_config.SUPPORTED_DVMS[index].PUBLIC_KEY, "is_paid": False}
-                            self.job_list.append(entry)
+                                    nip90request = (EventBuilder(self.dvm_config.SUPPORTED_DVMS[index].KIND,
+                                                                 "", tags).
+                                                    to_event(self.keys))
+
+                                # remember in the job_list that we have made an event, if anybody asks for payment,
+                                # we know we actually sent the request
+                                entry = {"npub": user.npub, "event_id": nip90request.id().to_hex(),
+                                         "dvm_key": self.dvm_config.SUPPORTED_DVMS[index].PUBLIC_KEY, "is_paid": False, "giftwrap": giftwrap}
+                                self.job_list.append(entry)
+
+                                # send the event to the DVM
+                                send_event(nip90request, client=self.client, dvm_config=self.dvm_config)
+                                # print(nip90request.as_json())
 
-                            # send the event to the DVM
-                            send_event(nip90request, client=self.client, dvm_config=self.dvm_config)
-                            # print(nip90request.as_json())
 
 
+                    elif decrypted_text.lower().startswith("balance"):
+                        time.sleep(3.0)
+                        message = "Your current balance is " + str(user.balance) + ("Sats. Zap me to add to your "
+                                                                                    "balance. I will use your "
+                                                                                    "balance interact with the DVMs "
+                                                                                    "for you.\n I support both "
+                                                                                    "public and private Zaps, "
+                                                                                    "as well as "
+                                                                                    "Zapplepay.\nAlternativly you "
+                                                                                    "can add a #cashu token with "
+                                                                                    "\"-cashu cashuASomeToken\" to "
+                                                                                    "your command.\n Make sure the "
+                                                                                    "token is worth the requested "
+                                                                                    "amount mint fees (at least 3 "
+                                                                                    "sat).\n Not all DVMs might "
+                                                                                    "accept Cashu tokens.")
+                        if giftwrap:
+                            self.client.send_sealed_msg(PublicKey.parse(sender), message, None)
+                        else:
+                            evt = EventBuilder.encrypted_direct_msg(self.keys, PublicKey.parse(sender),
+                                                                    message,None).to_event(self.keys)
+                            send_event(evt, client=self.client, dvm_config=dvm_config)
+                    elif decrypted_text.startswith("cashuA"):
+                        print("Received Cashu token:" + decrypted_text)
+                        cashu_redeemed, cashu_message, total_amount, fees = redeem_cashu(decrypted_text,
+                                                                                         self.dvm_config,
+                                                                                         self.client)
+                        print(cashu_message)
+                        if cashu_message == "success":
+                            update_user_balance(self.dvm_config.DB, sender, total_amount, client=self.client,
+                                                config=self.dvm_config)
+                        else:
+                            time.sleep(2.0)
+                            message = "Error: " + cashu_message + ". Token has not been redeemed."
 
-                elif decrypted_text.lower().startswith("balance"):
-                    time.sleep(3.0)
-                    evt = EventBuilder.encrypted_direct_msg(self.keys, nostr_event.author(),
-                                                                "Your current balance is " + str(
-                                                                    user.balance) + " Sats. Zap me to add to your balance. I will use your balance interact with the DVMs for you.\n"
-                                                                                    "I support both public and private Zaps, as well as Zapplepay.\n"
-                                                                                    "Alternativly you can add a #cashu token with \"-cashu cashuASomeToken\" to your command.\n Make sure the token is worth the requested amount + "
-                                                                                    "mint fees (at least 3 sat).\n Not all DVMs might accept Cashu tokens."
-                                                                , None).to_event(self.keys)
-                    send_event(evt, client=self.client, dvm_config=dvm_config)
+                            if giftwrap:
+                                self.client.send_sealed_msg(PublicKey.parse(sender), message, None)
+                            else:
+                                evt = EventBuilder.encrypted_direct_msg(self.keys, PublicKey.from_hex(sender), message,
+                                                                        None).to_event(self.keys)
+                                send_event(evt, client=self.client, dvm_config=self.dvm_config)
+                    elif decrypted_text.lower().startswith("what's the second best"):
+                        time.sleep(3.0)
+                        message = "No, there is no second best.\n\nhttps://cdn.nostr.build/p/mYLv.mp4"
+                        if giftwrap:
+                            self.client.send_sealed_msg(PublicKey.parse(sender), message, None)
+                        else:
+                            evt = EventBuilder.encrypted_direct_msg(self.keys, PublicKey.parse(sender),
+                                                                    message,
+                                                                    nostr_event.id()).to_event(self.keys)
+                            send_event(evt, client=self.client, dvm_config=self.dvm_config)
 
-                elif decrypted_text.startswith("cashuA"):
-                    print("Received Cashu token:" + decrypted_text)
-                    cashu_redeemed, cashu_message, total_amount, fees = redeem_cashu(decrypted_text, self.dvm_config,
-                                                                                     self.client)
-                    print(cashu_message)
-                    if cashu_message == "success":
-                        update_user_balance(self.dvm_config.DB, sender, total_amount, client=self.client,
-                                            config=self.dvm_config)
                     else:
-                        time.sleep(2.0)
-                        message = "Error: " + cashu_message + ". Token has not been redeemed."
-                        evt = EventBuilder.encrypted_direct_msg(self.keys, PublicKey.from_hex(sender), message,
-                                                                    None).to_event(self.keys)
-                        send_event(evt, client=self.client, dvm_config=self.dvm_config)
-                elif decrypted_text.lower().startswith("what's the second best"):
-                    time.sleep(3.0)
-                    evt = EventBuilder.encrypted_direct_msg(self.keys, nostr_event.author(),
-                                                                "No, there is no second best.\n\nhttps://cdn.nostr.build/p/mYLv.mp4",
-                                                                nostr_event.id()).to_event(self.keys)
-                    send_event(evt, client=self.client, dvm_config=self.dvm_config)
-
-                else:
-                    # Build an overview of known DVMs and send it to the user
-                    answer_overview(nostr_event)
+                        # Build an overview of known DVMs and send it to the user
+                        answer_overview(nostr_event, giftwrap, sender)
 
             except Exception as e:
                 print("Error in bot " + str(e))
 
         def handle_nip90_feedback(nostr_event):
-            #print(nostr_event.as_json())
+            # print(nostr_event.as_json())
             try:
                 is_encrypted = False
                 status = ""
                 etag = ""
                 ptag = ""
                 content = nostr_event.content()
                 for tag in nostr_event.tags():
@@ -255,22 +302,26 @@
 
                 if status == "success" or status == "error" or status == "processing" or status == "partial" and content != "":
                     entry = next((x for x in self.job_list if x['event_id'] == etag), None)
                     if entry is not None and entry['dvm_key'] == nostr_event.author().to_hex():
                         user = get_or_add_user(db=self.dvm_config.DB, npub=entry['npub'],
                                                client=self.client, config=self.dvm_config)
                         time.sleep(2.0)
-                        reply_event = EventBuilder.encrypted_direct_msg(self.keys,
+                        if entry["giftwrap"]:
+                            self.client.send_sealed_msg(PublicKey.parse(entry["npub"]), content, None)
+                        else:
+                            reply_event = EventBuilder.encrypted_direct_msg(self.keys,
                                                                             PublicKey.from_hex(entry['npub']),
                                                                             content,
                                                                             None).to_event(self.keys)
+
+                            send_event(reply_event, client=self.client, dvm_config=dvm_config)
                         print(status + ": " + content)
                         print(
                             "[" + self.NAME + "] Received reaction from " + nostr_event.author().to_hex() + " message to orignal sender " + user.name)
-                        send_event(reply_event, client=self.client, dvm_config=dvm_config)
 
                 elif status == "payment-required" or status == "partial":
                     for tag in nostr_event.tags():
                         if tag.as_vec()[0] == "amount":
                             amount_msats = int(tag.as_vec()[1])
                             amount = int(amount_msats / 1000)
                             entry = next((x for x in self.job_list if x['event_id'] == etag), None)
@@ -281,36 +332,38 @@
                                                        client=self.client, config=self.dvm_config)
                                 if user.balance >= amount:
                                     balance = max(user.balance - amount, 0)
                                     update_sql_table(db=self.dvm_config.DB, npub=user.npub, balance=balance,
                                                      iswhitelisted=user.iswhitelisted, isblacklisted=user.isblacklisted,
                                                      nip05=user.nip05, lud16=user.lud16, name=user.name,
                                                      lastactive=Timestamp.now().as_secs(), subscribed=user.subscribed)
-                                    evt = EventBuilder.encrypted_direct_msg(self.keys,
-                                                                                PublicKey.from_hex(entry["npub"]),
-                                                                                "Paid " + str(
-                                                                                    amount) + " Sats from balance to DVM. New balance is " +
-                                                                                str(balance)
-                                                                                + " Sats.\n",
-                                                                                None).to_event(self.keys)
 
+                                    message = "Paid " + str(amount) + " Sats from balance to DVM. New balance is " + str(balance) + " Sats.\n"
+                                    if entry["giftwrap"]:
+                                        self.client.send_sealed_msg(PublicKey.parse(entry["npub"]), message, None)
+                                    else:
+                                        evt = EventBuilder.encrypted_direct_msg(self.keys,
+                                                                                PublicKey.parse(entry["npub"]),
+                                                                                message,
+                                                                                None).to_event(self.keys)
+                                        send_event(evt, client=self.client, dvm_config=dvm_config)
                                     print(
                                         "[" + self.NAME + "] Replying " + user.name + " with \"scheduled\" confirmation")
-                                    send_event(evt, client=self.client, dvm_config=dvm_config)
+
                                 else:
                                     print("Bot payment-required")
                                     time.sleep(2.0)
                                     evt = EventBuilder.encrypted_direct_msg(self.keys,
-                                                                                PublicKey.from_hex(entry["npub"]),
-                                                                                "Current balance: " + str(
-                                                                                    user.balance) + " Sats. Balance of " + str(
-                                                                                    amount) + " Sats required. Please zap me with at least " +
-                                                                                str(int(amount - user.balance))
-                                                                                + " Sats, then try again.",
-                                                                                None).to_event(self.keys)
+                                                                            PublicKey.parse(entry["npub"]),
+                                                                            "Current balance: " + str(
+                                                                                user.balance) + " Sats. Balance of " + str(
+                                                                                amount) + " Sats required. Please zap me with at least " +
+                                                                            str(int(amount - user.balance))
+                                                                            + " Sats, then try again.",
+                                                                            None).to_event(self.keys)
                                     send_event(evt, client=self.client, dvm_config=dvm_config)
                                     return
 
                                 if len(tag.as_vec()) > 2:
                                     bolt11 = tag.as_vec()[2]
                                 # else we create a zap
                                 else:
@@ -372,19 +425,22 @@
                             if dvm.dvm_config.EXTERNAL_POST_PROCESS_TYPE == PostProcessFunctionType.LIST_TO_EVENTS:
                                 content = post_process_list_to_events(content)
                             elif dvm.dvm_config.EXTERNAL_POST_PROCESS_TYPE == PostProcessFunctionType.LIST_TO_USERS:
                                 content = post_process_list_to_users(content)
 
                     print("[" + self.NAME + "] Received results, message to orignal sender " + user.name)
                     time.sleep(1.0)
-                    reply_event = EventBuilder.encrypted_direct_msg(self.keys,
-                                                                        PublicKey.from_hex(user.npub),
+                    if entry["giftwrap"]:
+                        self.client.send_sealed_msg(PublicKey.parse(user.npub), content, None)
+                    else:
+                        reply_event = EventBuilder.encrypted_direct_msg(self.keys,
+                                                                        PublicKey.parse(user.npub),
                                                                         content,
                                                                         None).to_event(self.keys)
-                    send_event(reply_event, client=self.client, dvm_config=dvm_config)
+                        send_event(reply_event, client=self.client, dvm_config=dvm_config)
 
             except Exception as e:
                 print(e)
 
         def handle_zap(zap_event):
             print("[" + self.NAME + "] Zap received")
             try:
@@ -427,56 +483,60 @@
                         user.name))
                     update_user_balance(self.dvm_config.DB, sender, invoice_amount, client=self.client,
                                         config=self.dvm_config)
 
             except Exception as e:
                 print("[" + self.NAME + "] Error during content decryption:" + str(e))
 
-        def answer_overview(nostr_event):
+        def answer_overview(nostr_event, giftwrap, sender):
             message = "DVMs that I support:\n\n"
             index = 1
             for p in self.dvm_config.SUPPORTED_DVMS:
                 if p.PER_UNIT_COST != 0 and p.PER_UNIT_COST is not None:
                     message += (str(index) + " " + p.NAME + " " + p.TASK + "\n\t" + str(p.FIX_COST) +
                                 " Sats + " + str(p.PER_UNIT_COST) + " Sats per Second\n\n")
                 else:
                     message += (str(index) + " " + p.NAME + " " + p.TASK + "\n\t" + str(p.FIX_COST) +
                                 " Sats\n\n")
                 index += 1
 
             time.sleep(3.0)
-            evt = EventBuilder.encrypted_direct_msg(self.keys, nostr_event.author(),
-                                                        message + "\nSelect an Index and provide an input ("
-                                                                  "e.g. \"2 A purple ostrich\")\nType \"index info\" to learn "
-                                                                  "more about each DVM. (e.g. \"2 info\")\n\n"
-                                                                  "Type \"balance\" to see your current balance",
+
+            text =  message + "\nSelect an Index and provide an input (e.g. \"2 A purple ostrich\")\nType \"index info\" to learn more about each DVM. (e.g. \"2 info\")\n\n Type \"balance\" to see your current balance"
+            if giftwrap:
+                self.client.send_sealed_msg(PublicKey.parse(sender), text, None)
+            else:
+                evt = EventBuilder.encrypted_direct_msg(self.keys, PublicKey.parse(sender),
+                                                        text,
                                                         nostr_event.id()).to_event(self.keys)
 
-            send_event(evt, client=self.client, dvm_config=dvm_config)
+                send_event(evt, client=self.client, dvm_config=dvm_config)
 
-        def answer_blacklisted(nostr_event):
-            # For some reason an admin might blacklist npubs, e.g. for abusing the service
-            evt = EventBuilder.encrypted_direct_msg(self.keys, nostr_event.author(),
-                                                        "Your are currently blocked from all "
-                                                        "services.", None).to_event(self.keys)
-            send_event(evt, client=self.client, dvm_config=dvm_config)
+        def answer_blacklisted(nostr_event, giftwrap, sender):
+            message = "Your are currently blocked from this service."
+            if giftwrap:
+                self.client.send_sealed_msg(PublicKey.parse(sender), message, None)
+            else:
+                 # For some reason an admin might blacklist npubs, e.g. for abusing the service
+                evt = EventBuilder.encrypted_direct_msg(self.keys, nostr_event.author(),
+                                                        message, None).to_event(self.keys)
+                send_event(evt, client=self.client, dvm_config=dvm_config)
 
-        def answer_nip89(nostr_event, index):
+        def answer_nip89(nostr_event, index, giftwrap, sender):
             info = print_dvm_info(self.client, index)
+            if info is None:
+                info =  "No NIP89 Info found for " + self.dvm_config.SUPPORTED_DVMS[index].NAME
             time.sleep(2.0)
-            if info is not None:
-                evt = EventBuilder.encrypted_direct_msg(self.keys, nostr_event.author(),
-                                                            info, None).to_event(self.keys)
-            else:
-                evt = EventBuilder.encrypted_direct_msg(self.keys, nostr_event.author(),
-                                                            "No NIP89 Info found for " +
-                                                            self.dvm_config.SUPPORTED_DVMS[index].NAME,
-                                                            None).to_event(self.keys)
 
-            send_event(evt, client=self.client, dvm_config=dvm_config)
+            if giftwrap:
+                self.client.send_sealed_msg(PublicKey.parse(sender), info, None)
+            else:
+                    evt = EventBuilder.encrypted_direct_msg(self.keys, nostr_event.author(),
+                                                            info, None).to_event(self.keys)
+                    send_event(evt, client=self.client, dvm_config=dvm_config)
 
         def build_params(decrypted_text, nostr_event, index):
             tags = []
             splitzero = decrypted_text.split(' -')
             split = splitzero[0].split(' ')
             # If only a command without parameters is sent, we assume no input is required, and that means the dvm might take in the user as input (e.g. for content discovery)
             if len(split) == 1:
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/dvm.py` & `nostr_dvm-0.3.3/nostr_dvm/dvm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 import subprocess
 from datetime import timedelta
 from sys import platform
 
 from nostr_sdk import PublicKey, Keys, Client, Tag, Event, EventBuilder, Filter, HandleNotification, Timestamp, \
-    init_logger, LogLevel, Options, nip04_encrypt, NostrSigner, Kind, SubscribeAutoCloseOptions
+    init_logger, LogLevel, Options, nip04_encrypt, NostrSigner, Kind
 
 import time
 
 from nostr_dvm.utils.definitions import EventDefinitions, RequiredJobToWatch, JobToWatch
 from nostr_dvm.utils.dvmconfig import DVMConfig
 from nostr_dvm.utils.admin_utils import admin_make_database_updates, AdminConfig
 from nostr_dvm.utils.backend_utils import get_amount_per_task, check_task_is_supported, get_task
@@ -160,15 +160,15 @@
                             user_has_active_subscription = True
                             update_user_subscription(user.npub,
                                                      int(subscription_status["validUntil"]),
                                                      self.client, self.dvm_config)
                         else:
                             print("No active subscription found")
                             send_job_status_reaction(nip90_event, "subscription-required", True, amount, self.client,
-                                                     "No active subscription found..",
+                                                     "No active subscription found. Manage your subscription at: " + self.dvm_config.SUBSCRIPTION_MANAGEMENT,
                                                      self.dvm_config)
 
                 for dvm in self.dvm_config.SUPPORTED_DVMS:
                     if dvm.TASK == task and dvm.FIX_COST == 0 and dvm.PER_UNIT_COST == 0 and dvm_config.NIP88 is None:
                         task_is_free = True
 
                 cashu_redeemed = False
@@ -268,15 +268,15 @@
                 invoice_amount, zapped_event, sender, message, anon = parse_zap_event_tags(zap_event,
                                                                                            self.keys,
                                                                                            self.dvm_config.NIP89.NAME,
                                                                                            self.client, self.dvm_config)
                 user = get_or_add_user(db=self.dvm_config.DB, npub=sender, client=self.client, config=self.dvm_config)
 
                 if zapped_event is not None:
-                    if zapped_event.kind().as_u64() == EventDefinitions.KIND_FEEDBACK.as_u64():
+                    if zapped_event.kind() == EventDefinitions.KIND_FEEDBACK:
 
                         amount = 0
                         job_event = None
                         p_tag_str = ""
                         status = ""
                         for tag in zapped_event.tags():
                             if tag.as_vec()[0] == 'amount':
@@ -291,15 +291,15 @@
                                     return
                             elif tag.as_vec()[0] == 'status':
                                 status = tag.as_vec()[1]
                                 print(status)
 
                             # if a reaction by us got zapped
                         print(status)
-                        if job_event.kind().as_u64() == EventDefinitions.KIND_NIP88_SUBSCRIBE_EVENT.as_u64():
+                        if job_event.kind() == EventDefinitions.KIND_NIP88_SUBSCRIBE_EVENT:
                             send_job_status_reaction(job_event, "subscription-success", client=self.client,
                                                      dvm_config=self.dvm_config, user=user)
 
 
 
                         else:
                             task_supported, task = check_task_is_supported(job_event, client=self.client,
@@ -330,15 +330,15 @@
                                         do_work(job_event, invoice_amount)
 
                                 else:
                                     send_job_status_reaction(job_event, "payment-rejected",
                                                              False, invoice_amount, client=self.client,
                                                              dvm_config=self.dvm_config)
                                     print("[" + self.dvm_config.NIP89.NAME + "] Invoice was not paid sufficiently")
-                    elif zapped_event.kind().as_u64() == EventDefinitions.KIND_NIP88_SUBSCRIBE_EVENT.as_u64():
+                    elif zapped_event.kind() == EventDefinitions.KIND_NIP88_SUBSCRIBE_EVENT:
                         print("new subscription, doing nothing")
 
                     elif zapped_event.kind() in EventDefinitions.ANY_RESULT:
                         print("[" + self.dvm_config.NIP89.NAME + "] "
                                                                  "Someone zapped the result of an exisiting Task. Nice")
                     elif not anon:
                         print("[" + self.dvm_config.NIP89.NAME + "] Note Zap received for DVM balance: " +
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.3.3/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/subscription.py` & `nostr_dvm-0.3.3/nostr_dvm/subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,33 +52,39 @@
             self.client.add_relay(relay)
         self.client.connect()
 
         zap_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_ZAP]).since(Timestamp.now())
         cancel_subscription_filter = Filter().kinds([EventDefinitions.KIND_NIP88_STOP_SUBSCRIPTION_EVENT]).since(
             Timestamp.now())
         authors = []
-        if admin_config is not None:
+        if admin_config is not None and len(admin_config.USERNPUBS) > 0:
+            #we might want to limit which services can connect to the subscription handler
             for key in admin_config.USERNPUBS:
                 authors.append(PublicKey.parse(key))
-        dvm_filter = Filter().authors(authors).pubkey(pk).kinds([EventDefinitions.KIND_NIP90_DVM_SUBSCRIPTION]).since(
-            Timestamp.now())
+            dvm_filter = Filter().authors(authors).pubkey(pk).kinds([EventDefinitions.KIND_NIP90_DVM_SUBSCRIPTION]).since(
+                Timestamp.now())
+        else:
+            # or we don't
+            dvm_filter = Filter().pubkey(pk).kinds(
+                [EventDefinitions.KIND_NIP90_DVM_SUBSCRIPTION]).since(
+                Timestamp.now())
 
         self.client.subscribe([zap_filter, dvm_filter, cancel_subscription_filter], None)
 
         create_subscription_sql_table(dvm_config.DB)
 
         class NotificationHandler(HandleNotification):
             client = self.client
             dvm_config = self.dvm_config
             keys = self.keys
 
             def handle(self, relay_url, subscription_id, nostr_event: Event):
-                if nostr_event.kind().as_u64() == EventDefinitions.KIND_NIP90_DVM_SUBSCRIPTION.as_u64():
+                if nostr_event.kind() == EventDefinitions.KIND_NIP90_DVM_SUBSCRIPTION:
                     handle_nwc_request(nostr_event)
-                elif nostr_event.kind().as_u64() == EventDefinitions.KIND_NIP88_STOP_SUBSCRIPTION_EVENT.as_u64():
+                elif nostr_event.kind() == EventDefinitions.KIND_NIP88_STOP_SUBSCRIPTION_EVENT:
                     handle_cancel(nostr_event)
 
             def handle_msg(self, relay_url, msg):
                 return
 
         def handle_cancel(nostr_event):
             print(nostr_event.as_json())
@@ -156,14 +162,15 @@
                 print(zap)
                 overallsplit += int(zap[3])
 
             print(overallsplit)
             zapped_amount = 0
             for zap in zaps:
                 if zap[1] == "":
+                    #If the client did decide to not add itself to the zap split, or if a slot is left we add the subscription service in the empty space
                     zap[1] = Keys.parse(self.dvm_config.PRIVATE_KEY).public_key().to_hex()
 
                 name, nip05, lud16 = fetch_user_metadata(zap[1], self.client)
                 splitted_amount = math.floor(
                     (int(zap[3]) / overallsplit) * int(overall_amount) / 1000)
                 # invoice = create_bolt11_lud16(lud16, splitted_amount)
                 # TODO add details about DVM in message
@@ -329,15 +336,15 @@
                                                           Timestamp.now().as_secs(), tier)
                             print("updated subscription entry after payment")
 
                             send_status_success(nostr_event, "noogle.lol")
 
                             keys = Keys.parse(dvm_config.PRIVATE_KEY)
                             message = ("Subscribed to DVM " + tier + ". Renewing on: " + str(
-                                Timestamp.from_secs(end).to_human_datetime().replace("Z", " ").replace("T", " ")))
+                                Timestamp.from_secs(end).to_human_datetime().replace("Z", " ").replace("T", " ") + " GMT"))
                             evt = EventBuilder.encrypted_direct_msg(keys, PublicKey.parse(subscriber), message,
                                                                     None).to_event(keys)
                             send_event(evt, client=self.client, dvm_config=dvm_config)
 
 
 
                 except Exception as e:
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
         filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(lasthour)
         events = cli.database().query([filter1])
         ns.finallist = {}
         for event in events:
             if event.created_at().as_secs() > timestamp_hour_ago:
                 ns.finallist[event.id().to_hex()] = 0
-                filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(lasthour)
+                filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REPOST, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(lasthour)
                 reactions = cli.database().query([filt])
                 ns.finallist[event.id().to_hex()] = len(reactions)
 
         result_list = []
         finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
         for entry in finallist_sorted:
             #print(EventId.parse(entry[0]).to_bech32() + "/" + EventId.parse(entry[0]).to_hex() + ": " + str(entry[1]))
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             events = cli.database().query([filter1])
 
             ns.finallist = {}
             for event in events:
                 if event.created_at().as_secs() > timestamp_hour_ago:
                     ns.finallist[event.id().to_hex()] = 0
                     filt = Filter().kinds(
-                        [definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REACTION,
+                        [definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_REPOST,
                          definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(lasthour)
                     reactions = cli.database().query([filt])
                     ns.finallist[event.id().to_hex()] = len(reactions)
 
 
             finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
             for entry in finallist_sorted:
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/imageupscale.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,35 +55,40 @@
                 input_type = tag.as_vec()[2]
                 if input_type == "url":
                     url = tag.as_vec()[1]
 
             elif tag.as_vec()[0] == 'param':
                 print("Param: " + tag.as_vec()[1] + ": " + tag.as_vec()[2])
                 if tag.as_vec()[1] == "upscale":
-                    out_scale = tag.as_vec()[2]
+                    out_scale = int(tag.as_vec()[2])
 
         io_input_image = {
             "id": "input_image",
             "type": "input",
-            "src": "url:Image",
+            "src": "url:image",
             "uri": url
         }
 
         io_output = {
             "id": "output_image",
             "type": "output",
             "src": "request:image"
         }
 
         request_form['data'] = json.dumps([io_input_image, io_output])
 
-        options = {
-            "outscale": out_scale,
+        options = {"model": "RealESRGAN_x4plus",
+                   "outscale": out_scale,
+                   "denoise_strength": 0.5,
+                   "tile": 0,
+                   "tile_pad": 10,
+                   "pre_pad": 0,
+                   "compute_type": "fp32",
+                   "face_enhance": False}
 
-        }
         request_form['options'] = json.dumps(options)
 
         return request_form
 
     def process(self, request_form):
         try:
             # Call the process route of NOVA-Server with our request form.
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/search_users.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,28 +50,28 @@
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
                 if input_type == "text":
                     prompt += tag.as_vec()[1] + "\n"
                 elif input_type == "event":
                     collect_events.append(tag.as_vec()[1])
-                    #evt = get_event_by_id(tag.as_vec()[1], client=client, config=dvm_config)
-                    #prompt += evt.content() + "\n"
+                    # evt = get_event_by_id(tag.as_vec()[1], client=client, config=dvm_config)
+                    # prompt += evt.content() + "\n"
                 elif input_type == "job":
                     evt = get_referenced_event_by_id(event_id=tag.as_vec()[1], client=client,
                                                      kinds=[EventDefinitions.KIND_NIP90_RESULT_EXTRACT_TEXT,
                                                             EventDefinitions.KIND_NIP90_RESULT_SUMMARIZE_TEXT,
                                                             EventDefinitions.KIND_NIP90_RESULT_TRANSLATE_TEXT,
                                                             EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY],
                                                      dvm_config=dvm_config)
                     if evt is None:
                         print("Event not found")
                         raise Exception
-                    
-                    if evt.kind().as_u64() == EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY:
+
+                    if evt.kind() == EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY:
                         result_list = json.loads(evt.content())
                         prompt = ""
                         for tag in result_list:
                             e_tag = Tag.parse(tag)
                             evt = get_event_by_id(e_tag.as_vec()[1], client=client, config=dvm_config)
                             prompt += evt.content() + "\n"
 
@@ -79,17 +79,19 @@
                         prompt = evt.content()
 
         evts = get_events_by_ids(collect_events, client=client, config=dvm_config)
         if evts is not None:
             for evt in evts:
                 prompt += evt.content() + "\n"
 
+        clean_prompt = re.sub(r'^https?:\/\/.*[\r\n]*', '', prompt, flags=re.MULTILINE)
         options = {
-            "prompt": prompt,
+            "prompt": clean_prompt[:4000],
         }
+
         request_form['options'] = json.dumps(options)
 
         return request_form
 
     def process(self, request_form):
         from hugchat import hugchat
         from hugchat.login import Login
@@ -98,31 +100,27 @@
         try:
             cookies = sign.loadCookiesFromDir(
                 cookie_path_dir)  # This will detect if the JSON file exists, return cookies if it does and raise an Exception if it's not.
         except:
             cookies = sign.login()
             sign.saveCookiesToDir(cookie_path_dir)
 
-
         options = DVMTaskInterface.set_options(request_form)
 
         try:
             chatbot = hugchat.ChatBot(cookies=cookies.get_dict())  # or cookie_path="usercookies/<email>.json"
-            text = re.sub(r'^https?:\/\/.*[\r\n]*', '', str(options["prompt"]), flags=re.MULTILINE)
-
-            query_result = chatbot.query("Summarize the following notes: " + text[:3500])
+            query_result = chatbot.query("Summarize the following notes: " + str(options["prompt"]))
             print(query_result["text"])  # or query_result.text or query_result["text"]
             return str(query_result["text"]).lstrip()
 
         except Exception as e:
             print("Error in Module: " + str(e))
             raise Exception(e)
 
 
-
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
@@ -136,12 +134,12 @@
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
     return TextSummarizationHuggingChat(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                     admin_config=admin_config)
+                                        admin_config=admin_config)
 
 
 if __name__ == '__main__':
     process_venv(TextSummarizationHuggingChat)
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import re
 from nostr_sdk import Tag, Kind
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
-from nostr_dvm.utils.definitions  import EventDefinitions
+from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.nostr_utils import get_referenced_event_by_id, get_events_by_ids, get_event_by_id
 
 """
 This File contains a Module to generate Text, based on a prompt using the Unleashed.chat API.
@@ -64,15 +64,15 @@
                                                             EventDefinitions.KIND_NIP90_RESULT_TRANSLATE_TEXT,
                                                             EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY],
                                                      dvm_config=dvm_config)
                     if evt is None:
                         print("Event not found")
                         raise Exception
 
-                    if evt.kind().as_u64() == EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY:
+                    if evt.kind() == EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY:
                         result_list = json.loads(evt.content())
                         prompt = ""
                         for tag in result_list:
                             e_tag = Tag.parse(tag)
                             evt = get_event_by_id(e_tag.as_vec()[1], client=client, config=dvm_config)
                             prompt += evt.content() + "\n"
 
@@ -80,17 +80,17 @@
                         prompt = evt.content()
 
         evts = get_events_by_ids(collect_events, client=client, config=dvm_config)
         if evts is not None:
             for evt in evts:
                 prompt += evt.content() + "\n"
 
-        prompt = re.sub(r'http\S+', '', prompt)
+        clean_prompt = re.sub(r'^https?:\/\/.*[\r\n]*', '', prompt, flags=re.MULTILINE)
         options = {
-            "prompt": prompt,
+            "prompt": clean_prompt[:4000],
             "nostr": nostr_mode,
         }
         request_form['options'] = json.dumps(options)
 
         return request_form
 
     def process(self, request_form):
@@ -104,22 +104,21 @@
                 base_url='https://unleashed.chat/api/v1',
             )
 
             print('Models:\n')
 
             for model in client.models.list():
                 print('- ' + model.id)
-            text = re.sub(r'^https?:\/\/.*[\r\n]*', '', str(options["prompt"]), flags=re.MULTILINE)
 
-            content = "Summarize the following notes: " + text[:3500]
+            content = "Summarize the following notes: " + str(options["prompt"])
             normal_stream = client.chat.completions.create(
                 messages=[
                     {
                         'role': 'user',
-                        'content':content,
+                        'content': content,
                     }
                 ],
                 model='dolphin-2.2.1-mistral-7b',
                 stream=True,
                 extra_body={
                     'nostr_mode': options["nostr"],
                 },
@@ -144,15 +143,14 @@
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
     dvm_config.SEND_FEEDBACK_EVENTS = True
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
-
     nip89info = {
         "name": name,
         "image": "https://unleashed.chat/_app/immutable/assets/hero.pehsu4x_.jpeg",
         "about": "I summarize Text with https://unleashed.chat",
         "encryptionSupported": True,
         "cashuAccepted": True,
         "nip90Params": {}
@@ -160,13 +158,13 @@
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
     admin_config2 = AdminConfig()
     admin_config2.REBROADCAST_NIP89 = False
 
-    return SummarizationUnleashedChat(name=name, dvm_config=dvm_config, nip89config=nip89config, admin_config=admin_config2)
+    return SummarizationUnleashedChat(name=name, dvm_config=dvm_config, nip89config=nip89config,
+                                      admin_config=admin_config2)
 
 
 if __name__ == '__main__':
     process_venv(SummarizationUnleashedChat)
-
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/tasks/videogeneration_svd.py` & `nostr_dvm-0.3.3/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/backend_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.mediasource_utils import check_source_type, media_source
 from nostr_dvm.utils.nostr_utils import get_event_by_id, get_referenced_event_by_id
 
 
 def get_task(event, client, dvm_config):
     try:
-        if event.kind().as_u64() == EventDefinitions.KIND_NIP90_GENERIC.as_u64():  # use this for events that have no id yet, inclufr j tag
+        if event.kind() == EventDefinitions.KIND_NIP90_GENERIC:  # use this for events that have no id yet, inclufr j tag
             for tag in event.tags():
                 if tag.as_vec()[0] == 'j':
                     return tag.as_vec()[1]
             else:
                 return "unknown job: " + event.as_json()
         elif event.kind() == EventDefinitions.KIND_DM:  # dm
             for tag in event.tags():
                 if tag.as_vec()[0] == 'j':
                     return tag.as_vec()[1]
             else:
                 return "unknown job: " + event.as_json()
 
         # This looks a bit more complicated, but we do several tasks for text-extraction in the future
-        elif event.kind().as_u64() == EventDefinitions.KIND_NIP90_EXTRACT_TEXT.as_u64():
+        elif event.kind() == EventDefinitions.KIND_NIP90_EXTRACT_TEXT:
             for tag in event.tags():
                 if tag.as_vec()[0] == "i":
                     if tag.as_vec()[2] == "url":
                         file_type = check_url_is_readable(tag.as_vec()[1])
                         print(file_type)
                         if file_type == "pdf":
                             return "pdf-to-text"
@@ -53,15 +53,15 @@
                                             return "speech-to-text"
                                         else:
                                             return "unknown job"
                             else:
                                 return "unknown type"
                     else:
                         return "unknown job"
-        elif event.kind().as_u64() == EventDefinitions.KIND_NIP90_GENERATE_IMAGE.as_u64():
+        elif event.kind() == EventDefinitions.KIND_NIP90_GENERATE_IMAGE:
             has_image_tag = False
             has_text_tag = False
             for tag in event.tags():
                 if tag.as_vec()[0] == "i":
                     if tag.as_vec()[2] == "url":
                         file_type = check_url_is_readable(tag.as_vec()[1])
                         if file_type == "image":
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/database_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         for row in rows:
             print(row)
         con.close()
     except Error as e:
         print(e)
 
 
-def update_user_balance(db, npub, additional_sats, client, config):
+def update_user_balance(db, npub, additional_sats, client, config, giftwrap=False):
     user = get_from_sql_table(db, npub)
     if user is None:
         name, nip05, lud16 = fetch_user_metadata(npub, client)
         add_to_sql_table(db, npub, (int(additional_sats) + config.NEW_USER_BALANCE), False, False,
                          nip05, lud16, name, Timestamp.now().as_secs(), 0)
         print("Adding User: " + npub + " (" + npub + ")")
     else:
@@ -188,17 +188,22 @@
         if config is not None:
             keys = Keys.parse(config.PRIVATE_KEY)
             # time.sleep(1.0)
 
             message = ("Added " + str(additional_sats) + " Sats to balance. New balance is " + str(
                 new_balance) + " Sats.")
 
-            evt = EventBuilder.encrypted_direct_msg(keys, PublicKey.from_hex(npub), message,
-                                                    None).to_event(keys)
-            send_event(evt, client=client, dvm_config=config)
+            if giftwrap:
+                client.send_sealed_msg(PublicKey.parse(npub), message, None)
+            else:
+
+
+                evt = EventBuilder.encrypted_direct_msg(keys, PublicKey.parse(npub), message,
+                                                        None).to_event(keys)
+                send_event(evt, client=client, dvm_config=config)
 
 
 def update_user_subscription(npub, subscribed_until, client, dvm_config):
     user = get_from_sql_table(dvm_config.DB, npub)
     if user is None:
         name, nip05, lud16 = fetch_user_metadata(npub, client)
         add_to_sql_table(dvm_config.DB, npub, dvm_config.NEW_USER_BALANCE, False, False,
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from nostr_sdk import Event, Kind
 
 
 class EventDefinitions:
     KIND_NOTE = Kind(1)
     KIND_DM = Kind(4)
+    KIND_REPOST = Kind(6)
     KIND_REACTION = Kind(7)
     KIND_ZAP = Kind(9735)
     KIND_ANNOUNCEMENT = Kind(31990)
     KIND_NIP94_METADATA = Kind(1063)
     KIND_FEEDBACK = Kind(7000)
     KIND_NIP90_EXTRACT_TEXT = Kind(5000)
     KIND_NIP90_RESULT_EXTRACT_TEXT = Kind(6000)
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/dvmconfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     LNBITS_URL = 'https://lnbits.com'
     LN_ADDRESS = ''
     SCRIPT = ''
     IDENTIFIER = ''
     USE_OWN_VENV = True  # Make an own venv for each dvm's process function.Disable if you want to install packages into main venv. Only recommended if you dont want to run dvms with different dependency versions
     DB: str
     NEW_USER_BALANCE: int = 0  # Free credits for new users
+    SUBSCRIPTION_MANAGEMENT = 'https://noogle.lol/discovery'
     NIP88: NIP88Config
     NIP89: NIP89Config
     SEND_FEEDBACK_EVENTS = True
     SHOW_RESULT_BEFORE_PAYMENT: bool = False  # if this is true show results even when not paid right after autoprocess
     SCHEDULE_UPDATES_SECONDS = 0
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/nip89_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.3.3/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.3.3/nostr_dvm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.2
+Version: 0.3.3
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
-Requires-Dist: nostr-sdk==0.10.0
+Requires-Dist: nostr-sdk==0.11.0
 Requires-Dist: bech32
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: emoji==2.8.0
 Requires-Dist: eva-decord==0.6.1
 Requires-Dist: ffmpegio==0.8.5
 Requires-Dist: lnurl
```

### Comparing `nostr-dvm-0.3.2/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.3.3/nostr_dvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/setup.py` & `nostr_dvm-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.2'
+VERSION = '0.3.3'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. '
                     'This is an early stage release. Interfaces might change/brick')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
     author="Believethehype",
     author_email="believethehypeonnostr@proton.me",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(include=['nostr_dvm', 'nostr_dvm.*']),
 
-    install_requires=["nostr-sdk==0.10.0",
+    install_requires=["nostr-sdk==0.11.0",
                       "bech32",
                       "pycryptodome==3.20.0",
                       "python-dotenv==1.0.0",
                       "emoji==2.8.0",
                       "eva-decord==0.6.1",
                       "ffmpegio==0.8.5",
                       "lnurl",
```

### Comparing `nostr-dvm-0.3.2/tests/test_dvm_client.py` & `nostr_dvm-0.3.3/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.3.2/tests/test_events.py` & `nostr_dvm-0.3.3/tests/test_events.py`

 * *Files identical despite different names*

