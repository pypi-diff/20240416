# Comparing `tmp/thepipe_api-0.1.9.tar.gz` & `tmp/thepipe_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.1.9.tar", last modified: Mon Apr 15 23:17:18 2024, max compression
+gzip compressed data, was "thepipe_api-0.2.0.tar", last modified: Tue Apr 16 00:12:54 2024, max compression
```

## Comparing `thepipe_api-0.1.9.tar` & `thepipe_api-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 23:17:18.091697 thepipe_api-0.1.9/
--rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     9671 2024-04-15 23:17:18.090696 thepipe_api-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     8943 2024-04-15 22:58:42.000000 thepipe_api-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 23:17:18.091697 thepipe_api-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-15 23:16:36.000000 thepipe_api-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 23:17:18.068698 thepipe_api-0.1.9/tests/
--rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.9/tests/__init__.py
--rw-rw-rw-   0        0        0     9523 2024-04-13 23:06:00.000000 thepipe_api-0.1.9/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-15 23:17:18.073696 thepipe_api-0.1.9/thepipe_api/
--rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.1.9/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.1.9/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2789 2024-04-15 23:00:33.000000 thepipe_api-0.1.9/thepipe_api/core.py
--rw-rw-rw-   0        0        0    19810 2024-04-15 22:43:34.000000 thepipe_api-0.1.9/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3689 2024-04-15 23:15:24.000000 thepipe_api-0.1.9/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-15 23:17:18.089697 thepipe_api-0.1.9/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0     9671 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-15 23:17:17.000000 thepipe_api-0.1.9/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 00:12:54.856780 thepipe_api-0.2.0/
+-rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     9672 2024-04-16 00:12:54.854779 thepipe_api-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8944 2024-04-16 00:09:20.000000 thepipe_api-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 00:12:54.856780 thepipe_api-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-16 00:10:02.000000 thepipe_api-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 00:12:54.826780 thepipe_api-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     9523 2024-04-13 23:06:00.000000 thepipe_api-0.2.0/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-16 00:12:54.831779 thepipe_api-0.2.0/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.2.0/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.2.0/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2789 2024-04-15 23:00:33.000000 thepipe_api-0.2.0/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    19781 2024-04-16 00:09:41.000000 thepipe_api-0.2.0/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3628 2024-04-16 00:06:35.000000 thepipe_api-0.2.0/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-16 00:12:54.853779 thepipe_api-0.2.0/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0     9672 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.1.9/LICENSE` & `thepipe_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.9/PKG-INFO` & `thepipe_api-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.9
+Version: 0.2.0
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can be called from Python (`thepipe.extract("https://example.com")`) or from the command line (`thepipe path/to/example.pdf`).
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
 
 ![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
 ## Getting Started  🚀
 
 First, install The Pipe. 
 ```
@@ -59,14 +59,19 @@
 response = client.chat.completions.create(
     model="gpt-4-vision-preview",
     messages = chunks,
 )
 ```
 The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
 
+You can also use The Pipe from the command line. Here's how to recursively extract from a directory:
+```
+thepipe path/to/folder
+```
+
 ## Features 🌟
 
 - Extracts text and visuals from any file or web page 📚
 - Outputs RAG-ready chunks, optimized for multimodal LLMs 🖼️ + 💬
 - Can interpret complex PDFs, web apps, markdown, etc 🧠
 - Auto-compress prompts exceeding your chosen token limit 📦
 - Works with missing file extensions, in-memory data streams 💾
@@ -86,15 +91,15 @@
 | Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
 | PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
 | Image                                 | `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
 | Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
-| Website                               | URLs (inputs containing `http`, `https`, `www`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
+| Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
 ## Local Installation 🛠️
 
 To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.9 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.0 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
@@ -15,93 +15,93 @@
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
 docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
 Pipe is a multimodal-first tool for feeding files and web pages into vision-
 language models such as GPT-4V. It is best for LLM and RAG applications that
 require a deep understanding of tricky data sources. The Pipe is available as a
-hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can
-be called from Python (`thepipe.extract("https://example.com")`) or from the
-command line (`thepipe path/to/example.pdf`). ![Demo](https://
-ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/
-demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First, install
-The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
+hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
+[Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
+assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First,
+install The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
 environment variable is set. Don't have an API key yet? [Get one here](https://
 thepi.pe). Looking to operate it yourself locally instead? See the local
 installation section. Now you can extract comprehensive text and visuals from
 any file: ```python from thepipe_api import thepipe chunks = thepipe.extract
 ("example.pdf") ``` Or any website: ```python chunks = thepipe.extract("https:/
 /example.com") ``` Then feed it into GPT-4-Vision: ```python response =
 client.chat.completions.create( model="gpt-4-vision-preview", messages =
 chunks, ) ``` The Pipe's output is a list of sensible "chunks", and thus can be
 used either for storage in a vector database or for direct use as a prompt.
 Extra features such as data table extraction, bar chart extraction, custom web
 authentications and more are available in the [API documentation](https://
 thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to
-easily integrate The Pipe with any LLM provider. ## Features ð - Extracts
-text and visuals from any file or web page ð - Outputs RAG-ready chunks,
-optimized for multimodal LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web
-apps, markdown, etc ð§  - Auto-compress prompts exceeding your chosen token
-limit ð¦ - Works with missing file extensions, in-memory data streams ð¾ -
-Works with codebases, URL, git repos, and more ð - Multi-threaded â¡ï¸ ##
-How it works ð ï¸ The pipe is accessible from the command line or from
-[Python](https://www.python.org/downloads/). The input source is either a file
-path, a URL, or a directory (or zip file) path. The pipe will extract
-information from the source and process it for downstream use with [language
-models](https://en.wikipedia.org/wiki/Large_language_model), [vision
-transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-
-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is
-a sensible text-based (or multimodal) representation of the extracted
-information, carefully crafted to fit within context windows for any models
-from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://
-openai.com/gpt-4). It uses a variety of heuristics for optimal performance with
-vision-language models, including AI filetype detection with [filetype
-detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-
-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/
-docs), efficient [token compression](https://arxiv.org/abs/2403.12968),
-automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking]
-(https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/
-abs/2307.03172) effects, and more, all pre-built to work out-of-the-box. ##
-Supported File Types ð | Source Type | Input types | Token Compression
-ðï¸ | Image Extraction ðï¸ | Notes ð | |----------------------------
------------|------------------------------------------|-------------------|----
---------------|---------------------------------------------------------| |
-Directory | Any `/path/to/directory` | âï¸ | âï¸ | Extracts from all
-files in directory, supports match and ignore patterns | | Code | `.py`,
-`.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | âï¸ (varies) | â | Combines
-all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not
-| | Plaintext | `.txt`, `.md`, `.rtf`, etc | âï¸ | â | Regular text files
-| | PDF | `.pdf` | âï¸ | âï¸ | Extracts text and images of each page; can
-use AI for extraction of table data and images within pages | | Image | `.jpg`,
-`.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | â | âï¸ |
-Extracts images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx`
-| âï¸ | â | Extracts data from spreadsheets; converts to text
-representation. For very large datasets, will only extract column names and
-types | | Jupyter Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown,
-and images from Jupyter notebooks | | Microsoft Word Document | `.docx` |
-âï¸ | âï¸ | Extracts text and images from Word documents | | Microsoft
-PowerPoint Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images
-from PowerPoint presentations | | Website | URLs (inputs containing `http`,
-`https`, `www`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along
-with image (or images if scrollable); text-only extraction available | | GitHub
-Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
-repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
-âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
-## Local Installation ð ï¸ To use The Pipe locally, you will need
-[playwright](https://github.com/microsoft/playwright), [ctags](https://
-github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract),
-and the local python requirements, which differ from the more lightweight API
-requirements. You will also need to use the local version of the requirements
-file: ```bash git clone https://github.com/emcf/thepipe pip install -
-r requirements_local.txt ``` Tip for windows users: you may need to install the
-python-libmagic binaries with `pip install python-magic-bin`. Now you can use
-The Pipe: ```bash from thepipe_api import thepipe chunks = thepipe.extract
-("example.pdf", local=True) ``` Arguments are: - `source` (required): can be a
-file path, a URL, or a directory path. - `local` (optional): Use the local
-version of The Pipe instead of the hosted API. - `match` (optional): Regex
-pattern to match files in the directory. - `ignore` (optional): Regex pattern
-to ignore files in the directory. - `limit` (optional): The token limit for the
-output prompt, defaults to 100K. Prompts exceeding the limit will be
-compressed. - `ai_extraction` (optional): Extract tables, figures, and math
-from PDFs using our extractor. Incurs extra costs. - `text_only` (optional): Do
-not extract images from documents or websites. Additionally, image files will
-be represented with OCR instead of as images.
+easily integrate The Pipe with any LLM provider. You can also use The Pipe from
+the command line. Here's how to recursively extract from a directory: ```
+thepipe path/to/folder ``` ## Features ð - Extracts text and visuals from
+any file or web page ð - Outputs RAG-ready chunks, optimized for multimodal
+LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web apps, markdown, etc ð§ 
+- Auto-compress prompts exceeding your chosen token limit ð¦ - Works with
+missing file extensions, in-memory data streams ð¾ - Works with codebases,
+URL, git repos, and more ð - Multi-threaded â¡ï¸ ## How it works ð ï¸
+The pipe is accessible from the command line or from [Python](https://
+www.python.org/downloads/). The input source is either a file path, a URL, or a
+directory (or zip file) path. The pipe will extract information from the source
+and process it for downstream use with [language models](https://
+en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://
+en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://
+arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based
+(or multimodal) representation of the extracted information, carefully crafted
+to fit within context windows for any models from [gemma-7b](https://
+huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a
+variety of heuristics for optimal performance with vision-language models,
+including AI filetype detection with [filetype detection](https://
+opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
+type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token
+compression](https://arxiv.org/abs/2403.12968), automatic [image encoding]
+(https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/
+2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects,
+and more, all pre-built to work out-of-the-box. ## Supported File Types ð |
+Source Type | Input types | Token Compression ðï¸ | Image Extraction
+ðï¸ | Notes ð | |---------------------------------------|---------------
+---------------------------|-------------------|------------------|------------
+---------------------------------------------| | Directory | Any `/path/to/
+directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
+match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
+`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
+`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
+`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
+âï¸ | âï¸ | Extracts text and images of each page; can use AI for
+extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
+`.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | â | âï¸ | Extracts
+images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸
+| â | Extracts data from spreadsheets; converts to text representation. For
+very large datasets, will only extract column names and types | | Jupyter
+Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown, and images from
+Jupyter notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ |
+Extracts text and images from Word documents | | Microsoft PowerPoint
+Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images from
+PowerPoint presentations | | Website | URLs (inputs containing `http`, `https`,
+`ftp`) | âï¸ | âï¸ | Extracts text from web page along with image (or
+images if scrollable); text-only extraction available | | GitHub Repository |
+GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub repositories;
+supports branch specification | | ZIP File | `.zip` | âï¸ | âï¸ |
+Extracts contents of ZIP files; supports nested directory extraction | ## Local
+Installation ð ï¸ To use The Pipe locally, you will need [playwright](https:
+//github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/
+), [pytesseract](https://github.com/h/pytesseract), and the local python
+requirements, which differ from the more lightweight API requirements. You will
+also need to use the local version of the requirements file: ```bash git clone
+https://github.com/emcf/thepipe pip install -r requirements_local.txt ``` Tip
+for windows users: you may need to install the python-libmagic binaries with
+`pip install python-magic-bin`. Now you can use The Pipe: ```bash from
+thepipe_api import thepipe chunks = thepipe.extract("example.pdf", local=True)
+``` Arguments are: - `source` (required): can be a file path, a URL, or a
+directory path. - `local` (optional): Use the local version of The Pipe instead
+of the hosted API. - `match` (optional): Regex pattern to match files in the
+directory. - `ignore` (optional): Regex pattern to ignore files in the
+directory. - `limit` (optional): The token limit for the output prompt,
+defaults to 100K. Prompts exceeding the limit will be compressed. -
+`ai_extraction` (optional): Extract tables, figures, and math from PDFs using
+our extractor. Incurs extra costs. - `text_only` (optional): Do not extract
+images from documents or websites. Additionally, image files will be
+represented with OCR instead of as images.
```

### Comparing `thepipe_api-0.1.9/README.md` & `thepipe_api-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can be called from Python (`thepipe.extract("https://example.com")`) or from the command line (`thepipe path/to/example.pdf`).
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
 
 ![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
 ## Getting Started  🚀
 
 First, install The Pipe. 
 ```
@@ -35,14 +35,19 @@
 response = client.chat.completions.create(
     model="gpt-4-vision-preview",
     messages = chunks,
 )
 ```
 The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
 
+You can also use The Pipe from the command line. Here's how to recursively extract from a directory:
+```
+thepipe path/to/folder
+```
+
 ## Features 🌟
 
 - Extracts text and visuals from any file or web page 📚
 - Outputs RAG-ready chunks, optimized for multimodal LLMs 🖼️ + 💬
 - Can interpret complex PDFs, web apps, markdown, etc 🧠
 - Auto-compress prompts exceeding your chosen token limit 📦
 - Works with missing file extensions, in-memory data streams 💾
@@ -62,15 +67,15 @@
 | Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
 | PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
 | Image                                 | `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
 | Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
-| Website                               | URLs (inputs containing `http`, `https`, `www`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
+| Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
 ## Local Installation 🛠️
 
 To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
```

#### html2text {}

```diff
@@ -6,93 +6,93 @@
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
 docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
 Pipe is a multimodal-first tool for feeding files and web pages into vision-
 language models such as GPT-4V. It is best for LLM and RAG applications that
 require a deep understanding of tricky data sources. The Pipe is available as a
-hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can
-be called from Python (`thepipe.extract("https://example.com")`) or from the
-command line (`thepipe path/to/example.pdf`). ![Demo](https://
-ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/
-demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First, install
-The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
+hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
+[Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
+assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First,
+install The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
 environment variable is set. Don't have an API key yet? [Get one here](https://
 thepi.pe). Looking to operate it yourself locally instead? See the local
 installation section. Now you can extract comprehensive text and visuals from
 any file: ```python from thepipe_api import thepipe chunks = thepipe.extract
 ("example.pdf") ``` Or any website: ```python chunks = thepipe.extract("https:/
 /example.com") ``` Then feed it into GPT-4-Vision: ```python response =
 client.chat.completions.create( model="gpt-4-vision-preview", messages =
 chunks, ) ``` The Pipe's output is a list of sensible "chunks", and thus can be
 used either for storage in a vector database or for direct use as a prompt.
 Extra features such as data table extraction, bar chart extraction, custom web
 authentications and more are available in the [API documentation](https://
 thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to
-easily integrate The Pipe with any LLM provider. ## Features ð - Extracts
-text and visuals from any file or web page ð - Outputs RAG-ready chunks,
-optimized for multimodal LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web
-apps, markdown, etc ð§  - Auto-compress prompts exceeding your chosen token
-limit ð¦ - Works with missing file extensions, in-memory data streams ð¾ -
-Works with codebases, URL, git repos, and more ð - Multi-threaded â¡ï¸ ##
-How it works ð ï¸ The pipe is accessible from the command line or from
-[Python](https://www.python.org/downloads/). The input source is either a file
-path, a URL, or a directory (or zip file) path. The pipe will extract
-information from the source and process it for downstream use with [language
-models](https://en.wikipedia.org/wiki/Large_language_model), [vision
-transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-
-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is
-a sensible text-based (or multimodal) representation of the extracted
-information, carefully crafted to fit within context windows for any models
-from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://
-openai.com/gpt-4). It uses a variety of heuristics for optimal performance with
-vision-language models, including AI filetype detection with [filetype
-detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-
-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/
-docs), efficient [token compression](https://arxiv.org/abs/2403.12968),
-automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking]
-(https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/
-abs/2307.03172) effects, and more, all pre-built to work out-of-the-box. ##
-Supported File Types ð | Source Type | Input types | Token Compression
-ðï¸ | Image Extraction ðï¸ | Notes ð | |----------------------------
------------|------------------------------------------|-------------------|----
---------------|---------------------------------------------------------| |
-Directory | Any `/path/to/directory` | âï¸ | âï¸ | Extracts from all
-files in directory, supports match and ignore patterns | | Code | `.py`,
-`.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | âï¸ (varies) | â | Combines
-all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not
-| | Plaintext | `.txt`, `.md`, `.rtf`, etc | âï¸ | â | Regular text files
-| | PDF | `.pdf` | âï¸ | âï¸ | Extracts text and images of each page; can
-use AI for extraction of table data and images within pages | | Image | `.jpg`,
-`.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | â | âï¸ |
-Extracts images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx`
-| âï¸ | â | Extracts data from spreadsheets; converts to text
-representation. For very large datasets, will only extract column names and
-types | | Jupyter Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown,
-and images from Jupyter notebooks | | Microsoft Word Document | `.docx` |
-âï¸ | âï¸ | Extracts text and images from Word documents | | Microsoft
-PowerPoint Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images
-from PowerPoint presentations | | Website | URLs (inputs containing `http`,
-`https`, `www`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along
-with image (or images if scrollable); text-only extraction available | | GitHub
-Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
-repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
-âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
-## Local Installation ð ï¸ To use The Pipe locally, you will need
-[playwright](https://github.com/microsoft/playwright), [ctags](https://
-github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract),
-and the local python requirements, which differ from the more lightweight API
-requirements. You will also need to use the local version of the requirements
-file: ```bash git clone https://github.com/emcf/thepipe pip install -
-r requirements_local.txt ``` Tip for windows users: you may need to install the
-python-libmagic binaries with `pip install python-magic-bin`. Now you can use
-The Pipe: ```bash from thepipe_api import thepipe chunks = thepipe.extract
-("example.pdf", local=True) ``` Arguments are: - `source` (required): can be a
-file path, a URL, or a directory path. - `local` (optional): Use the local
-version of The Pipe instead of the hosted API. - `match` (optional): Regex
-pattern to match files in the directory. - `ignore` (optional): Regex pattern
-to ignore files in the directory. - `limit` (optional): The token limit for the
-output prompt, defaults to 100K. Prompts exceeding the limit will be
-compressed. - `ai_extraction` (optional): Extract tables, figures, and math
-from PDFs using our extractor. Incurs extra costs. - `text_only` (optional): Do
-not extract images from documents or websites. Additionally, image files will
-be represented with OCR instead of as images.
+easily integrate The Pipe with any LLM provider. You can also use The Pipe from
+the command line. Here's how to recursively extract from a directory: ```
+thepipe path/to/folder ``` ## Features ð - Extracts text and visuals from
+any file or web page ð - Outputs RAG-ready chunks, optimized for multimodal
+LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web apps, markdown, etc ð§ 
+- Auto-compress prompts exceeding your chosen token limit ð¦ - Works with
+missing file extensions, in-memory data streams ð¾ - Works with codebases,
+URL, git repos, and more ð - Multi-threaded â¡ï¸ ## How it works ð ï¸
+The pipe is accessible from the command line or from [Python](https://
+www.python.org/downloads/). The input source is either a file path, a URL, or a
+directory (or zip file) path. The pipe will extract information from the source
+and process it for downstream use with [language models](https://
+en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://
+en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://
+arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based
+(or multimodal) representation of the extracted information, carefully crafted
+to fit within context windows for any models from [gemma-7b](https://
+huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a
+variety of heuristics for optimal performance with vision-language models,
+including AI filetype detection with [filetype detection](https://
+opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
+type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token
+compression](https://arxiv.org/abs/2403.12968), automatic [image encoding]
+(https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/
+2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects,
+and more, all pre-built to work out-of-the-box. ## Supported File Types ð |
+Source Type | Input types | Token Compression ðï¸ | Image Extraction
+ðï¸ | Notes ð | |---------------------------------------|---------------
+---------------------------|-------------------|------------------|------------
+---------------------------------------------| | Directory | Any `/path/to/
+directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
+match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
+`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
+`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
+`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
+âï¸ | âï¸ | Extracts text and images of each page; can use AI for
+extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
+`.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | â | âï¸ | Extracts
+images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸
+| â | Extracts data from spreadsheets; converts to text representation. For
+very large datasets, will only extract column names and types | | Jupyter
+Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown, and images from
+Jupyter notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ |
+Extracts text and images from Word documents | | Microsoft PowerPoint
+Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images from
+PowerPoint presentations | | Website | URLs (inputs containing `http`, `https`,
+`ftp`) | âï¸ | âï¸ | Extracts text from web page along with image (or
+images if scrollable); text-only extraction available | | GitHub Repository |
+GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub repositories;
+supports branch specification | | ZIP File | `.zip` | âï¸ | âï¸ |
+Extracts contents of ZIP files; supports nested directory extraction | ## Local
+Installation ð ï¸ To use The Pipe locally, you will need [playwright](https:
+//github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/
+), [pytesseract](https://github.com/h/pytesseract), and the local python
+requirements, which differ from the more lightweight API requirements. You will
+also need to use the local version of the requirements file: ```bash git clone
+https://github.com/emcf/thepipe pip install -r requirements_local.txt ``` Tip
+for windows users: you may need to install the python-libmagic binaries with
+`pip install python-magic-bin`. Now you can use The Pipe: ```bash from
+thepipe_api import thepipe chunks = thepipe.extract("example.pdf", local=True)
+``` Arguments are: - `source` (required): can be a file path, a URL, or a
+directory path. - `local` (optional): Use the local version of The Pipe instead
+of the hosted API. - `match` (optional): Regex pattern to match files in the
+directory. - `ignore` (optional): Regex pattern to ignore files in the
+directory. - `limit` (optional): The token limit for the output prompt,
+defaults to 100K. Prompts exceeding the limit will be compressed. -
+`ai_extraction` (optional): Extract tables, figures, and math from PDFs using
+our extractor. Incurs extra costs. - `text_only` (optional): Do not extract
+images from documents or websites. Additionally, image files will be
+represented with OCR instead of as images.
```

### Comparing `thepipe_api-0.1.9/setup.py` & `thepipe_api-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.1.9',
+    version='0.2.0',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.1.9/tests/test_thepipe.py` & `thepipe_api-0.2.0/tests/test_thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.9/thepipe_api/compressor.py` & `thepipe_api-0.2.0/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.9/thepipe_api/core.py` & `thepipe_api-0.2.0/thepipe_api/core.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.9/thepipe_api/extractor.py` & `thepipe_api-0.2.0/thepipe_api/extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     except Exception as e:
         if verbose: print_status(f"Failed to extract from {file_path}: {e}", status='error')
         return [Chunk(path=file_path)]
 
 def detect_type(source: str) -> Optional[SourceTypes]:
     if source.startswith("https://github.com"):
         return SourceTypes.GITHUB
-    elif source.startswith("http") or source.startswith("www.") or source.startswith("ftp."):
+    elif source.startswith("http") or source.startswith("ftp."):
         return SourceTypes.URL
     elif source.endswith(".zip"):
         return SourceTypes.ZIP
     elif os.path.isdir(source) or source == '.' or source == './':
         return SourceTypes.DIR
     # try splitting the source into a filename and extension
     _, extension = os.path.splitext(source)
```

### Comparing `thepipe_api-0.1.9/thepipe_api/thepipe.py` & `thepipe_api-0.2.0/thepipe_api/thepipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,12 @@
     args = parser.parse_args()
     verbose = not args.quiet
     args.verbose = verbose
     return args
 
 def main() -> None:
     args = parse_arguments()
-    chunks = extract(source=args.source, match=args.match, ignore=args.ignore, limit=args.limit, verbose=args.verbose, ai_extraction=args.ai_extraction, text_only=args.text_only, local=args.local)
-    if not args.local:
-        chunks = core.create_chunks_from_messages(chunks)
+    chunks = extractor.extract_from_source(source=args.source, match=args.match, ignore=args.ignore, limit=args.limit, verbose=args.verbose, ai_extraction=args.ai_extraction, text_only=args.text_only, local=args.local)
     save_outputs(chunks=chunks, verbose=args.verbose, text_only=args.text_only)
 
 if __name__ == '__main__':
     main()
```

### Comparing `thepipe_api-0.1.9/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.2.0/thepipe_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.9
+Version: 0.2.0
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can be called from Python (`thepipe.extract("https://example.com")`) or from the command line (`thepipe path/to/example.pdf`).
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
 
 ![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
 ## Getting Started  🚀
 
 First, install The Pipe. 
 ```
@@ -59,14 +59,19 @@
 response = client.chat.completions.create(
     model="gpt-4-vision-preview",
     messages = chunks,
 )
 ```
 The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
 
+You can also use The Pipe from the command line. Here's how to recursively extract from a directory:
+```
+thepipe path/to/folder
+```
+
 ## Features 🌟
 
 - Extracts text and visuals from any file or web page 📚
 - Outputs RAG-ready chunks, optimized for multimodal LLMs 🖼️ + 💬
 - Can interpret complex PDFs, web apps, markdown, etc 🧠
 - Auto-compress prompts exceeding your chosen token limit 📦
 - Works with missing file extensions, in-memory data streams 💾
@@ -86,15 +91,15 @@
 | Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
 | PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
 | Image                                 | `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
 | Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
-| Website                               | URLs (inputs containing `http`, `https`, `www`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
+| Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
 ## Local Installation 🛠️
 
 To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.9 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.0 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
@@ -15,93 +15,93 @@
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
 docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
 Pipe is a multimodal-first tool for feeding files and web pages into vision-
 language models such as GPT-4V. It is best for LLM and RAG applications that
 require a deep understanding of tricky data sources. The Pipe is available as a
-hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can
-be called from Python (`thepipe.extract("https://example.com")`) or from the
-command line (`thepipe path/to/example.pdf`). ![Demo](https://
-ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/
-demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First, install
-The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
+hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
+[Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
+assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First,
+install The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
 environment variable is set. Don't have an API key yet? [Get one here](https://
 thepi.pe). Looking to operate it yourself locally instead? See the local
 installation section. Now you can extract comprehensive text and visuals from
 any file: ```python from thepipe_api import thepipe chunks = thepipe.extract
 ("example.pdf") ``` Or any website: ```python chunks = thepipe.extract("https:/
 /example.com") ``` Then feed it into GPT-4-Vision: ```python response =
 client.chat.completions.create( model="gpt-4-vision-preview", messages =
 chunks, ) ``` The Pipe's output is a list of sensible "chunks", and thus can be
 used either for storage in a vector database or for direct use as a prompt.
 Extra features such as data table extraction, bar chart extraction, custom web
 authentications and more are available in the [API documentation](https://
 thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to
-easily integrate The Pipe with any LLM provider. ## Features ð - Extracts
-text and visuals from any file or web page ð - Outputs RAG-ready chunks,
-optimized for multimodal LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web
-apps, markdown, etc ð§  - Auto-compress prompts exceeding your chosen token
-limit ð¦ - Works with missing file extensions, in-memory data streams ð¾ -
-Works with codebases, URL, git repos, and more ð - Multi-threaded â¡ï¸ ##
-How it works ð ï¸ The pipe is accessible from the command line or from
-[Python](https://www.python.org/downloads/). The input source is either a file
-path, a URL, or a directory (or zip file) path. The pipe will extract
-information from the source and process it for downstream use with [language
-models](https://en.wikipedia.org/wiki/Large_language_model), [vision
-transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-
-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is
-a sensible text-based (or multimodal) representation of the extracted
-information, carefully crafted to fit within context windows for any models
-from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://
-openai.com/gpt-4). It uses a variety of heuristics for optimal performance with
-vision-language models, including AI filetype detection with [filetype
-detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-
-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/
-docs), efficient [token compression](https://arxiv.org/abs/2403.12968),
-automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking]
-(https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/
-abs/2307.03172) effects, and more, all pre-built to work out-of-the-box. ##
-Supported File Types ð | Source Type | Input types | Token Compression
-ðï¸ | Image Extraction ðï¸ | Notes ð | |----------------------------
------------|------------------------------------------|-------------------|----
---------------|---------------------------------------------------------| |
-Directory | Any `/path/to/directory` | âï¸ | âï¸ | Extracts from all
-files in directory, supports match and ignore patterns | | Code | `.py`,
-`.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | âï¸ (varies) | â | Combines
-all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not
-| | Plaintext | `.txt`, `.md`, `.rtf`, etc | âï¸ | â | Regular text files
-| | PDF | `.pdf` | âï¸ | âï¸ | Extracts text and images of each page; can
-use AI for extraction of table data and images within pages | | Image | `.jpg`,
-`.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | â | âï¸ |
-Extracts images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx`
-| âï¸ | â | Extracts data from spreadsheets; converts to text
-representation. For very large datasets, will only extract column names and
-types | | Jupyter Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown,
-and images from Jupyter notebooks | | Microsoft Word Document | `.docx` |
-âï¸ | âï¸ | Extracts text and images from Word documents | | Microsoft
-PowerPoint Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images
-from PowerPoint presentations | | Website | URLs (inputs containing `http`,
-`https`, `www`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along
-with image (or images if scrollable); text-only extraction available | | GitHub
-Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
-repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
-âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
-## Local Installation ð ï¸ To use The Pipe locally, you will need
-[playwright](https://github.com/microsoft/playwright), [ctags](https://
-github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract),
-and the local python requirements, which differ from the more lightweight API
-requirements. You will also need to use the local version of the requirements
-file: ```bash git clone https://github.com/emcf/thepipe pip install -
-r requirements_local.txt ``` Tip for windows users: you may need to install the
-python-libmagic binaries with `pip install python-magic-bin`. Now you can use
-The Pipe: ```bash from thepipe_api import thepipe chunks = thepipe.extract
-("example.pdf", local=True) ``` Arguments are: - `source` (required): can be a
-file path, a URL, or a directory path. - `local` (optional): Use the local
-version of The Pipe instead of the hosted API. - `match` (optional): Regex
-pattern to match files in the directory. - `ignore` (optional): Regex pattern
-to ignore files in the directory. - `limit` (optional): The token limit for the
-output prompt, defaults to 100K. Prompts exceeding the limit will be
-compressed. - `ai_extraction` (optional): Extract tables, figures, and math
-from PDFs using our extractor. Incurs extra costs. - `text_only` (optional): Do
-not extract images from documents or websites. Additionally, image files will
-be represented with OCR instead of as images.
+easily integrate The Pipe with any LLM provider. You can also use The Pipe from
+the command line. Here's how to recursively extract from a directory: ```
+thepipe path/to/folder ``` ## Features ð - Extracts text and visuals from
+any file or web page ð - Outputs RAG-ready chunks, optimized for multimodal
+LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web apps, markdown, etc ð§ 
+- Auto-compress prompts exceeding your chosen token limit ð¦ - Works with
+missing file extensions, in-memory data streams ð¾ - Works with codebases,
+URL, git repos, and more ð - Multi-threaded â¡ï¸ ## How it works ð ï¸
+The pipe is accessible from the command line or from [Python](https://
+www.python.org/downloads/). The input source is either a file path, a URL, or a
+directory (or zip file) path. The pipe will extract information from the source
+and process it for downstream use with [language models](https://
+en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://
+en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://
+arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based
+(or multimodal) representation of the extracted information, carefully crafted
+to fit within context windows for any models from [gemma-7b](https://
+huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a
+variety of heuristics for optimal performance with vision-language models,
+including AI filetype detection with [filetype detection](https://
+opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
+type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token
+compression](https://arxiv.org/abs/2403.12968), automatic [image encoding]
+(https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/
+2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects,
+and more, all pre-built to work out-of-the-box. ## Supported File Types ð |
+Source Type | Input types | Token Compression ðï¸ | Image Extraction
+ðï¸ | Notes ð | |---------------------------------------|---------------
+---------------------------|-------------------|------------------|------------
+---------------------------------------------| | Directory | Any `/path/to/
+directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
+match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
+`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
+`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
+`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
+âï¸ | âï¸ | Extracts text and images of each page; can use AI for
+extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
+`.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | â | âï¸ | Extracts
+images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸
+| â | Extracts data from spreadsheets; converts to text representation. For
+very large datasets, will only extract column names and types | | Jupyter
+Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown, and images from
+Jupyter notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ |
+Extracts text and images from Word documents | | Microsoft PowerPoint
+Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images from
+PowerPoint presentations | | Website | URLs (inputs containing `http`, `https`,
+`ftp`) | âï¸ | âï¸ | Extracts text from web page along with image (or
+images if scrollable); text-only extraction available | | GitHub Repository |
+GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub repositories;
+supports branch specification | | ZIP File | `.zip` | âï¸ | âï¸ |
+Extracts contents of ZIP files; supports nested directory extraction | ## Local
+Installation ð ï¸ To use The Pipe locally, you will need [playwright](https:
+//github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/
+), [pytesseract](https://github.com/h/pytesseract), and the local python
+requirements, which differ from the more lightweight API requirements. You will
+also need to use the local version of the requirements file: ```bash git clone
+https://github.com/emcf/thepipe pip install -r requirements_local.txt ``` Tip
+for windows users: you may need to install the python-libmagic binaries with
+`pip install python-magic-bin`. Now you can use The Pipe: ```bash from
+thepipe_api import thepipe chunks = thepipe.extract("example.pdf", local=True)
+``` Arguments are: - `source` (required): can be a file path, a URL, or a
+directory path. - `local` (optional): Use the local version of The Pipe instead
+of the hosted API. - `match` (optional): Regex pattern to match files in the
+directory. - `ignore` (optional): Regex pattern to ignore files in the
+directory. - `limit` (optional): The token limit for the output prompt,
+defaults to 100K. Prompts exceeding the limit will be compressed. -
+`ai_extraction` (optional): Extract tables, figures, and math from PDFs using
+our extractor. Incurs extra costs. - `text_only` (optional): Do not extract
+images from documents or websites. Additionally, image files will be
+represented with OCR instead of as images.
```

