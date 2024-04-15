# Comparing `tmp/thepipe_api-0.1.7.tar.gz` & `tmp/thepipe_api-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.1.7.tar", last modified: Mon Apr 15 22:52:06 2024, max compression
+gzip compressed data, was "thepipe_api-0.1.8.tar", last modified: Mon Apr 15 23:07:30 2024, max compression
```

## Comparing `thepipe_api-0.1.7.tar` & `thepipe_api-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 22:52:06.262720 thepipe_api-0.1.7/
--rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     9416 2024-04-15 22:52:06.261721 thepipe_api-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     8688 2024-04-14 00:39:19.000000 thepipe_api-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 22:52:06.262720 thepipe_api-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-15 22:51:37.000000 thepipe_api-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:52:06.239718 thepipe_api-0.1.7/tests/
--rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0     9523 2024-04-13 23:06:00.000000 thepipe_api-0.1.7/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:52:06.243719 thepipe_api-0.1.7/thepipe_api/
--rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.1.7/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.1.7/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2767 2024-04-15 06:49:44.000000 thepipe_api-0.1.7/thepipe_api/core.py
--rw-rw-rw-   0        0        0    19810 2024-04-15 22:43:34.000000 thepipe_api-0.1.7/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3504 2024-04-13 20:43:49.000000 thepipe_api-0.1.7/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:52:06.259719 thepipe_api-0.1.7/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0     9416 2024-04-15 22:52:05.000000 thepipe_api-0.1.7/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-15 22:52:06.000000 thepipe_api-0.1.7/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 22:52:05.000000 thepipe_api-0.1.7/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-15 22:52:06.000000 thepipe_api-0.1.7/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2024-04-15 22:52:06.000000 thepipe_api-0.1.7/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-15 22:52:06.000000 thepipe_api-0.1.7/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 23:07:30.469329 thepipe_api-0.1.8/
+-rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     9671 2024-04-15 23:07:30.468328 thepipe_api-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8943 2024-04-15 22:58:42.000000 thepipe_api-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 23:07:30.469329 thepipe_api-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-15 23:07:13.000000 thepipe_api-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 23:07:30.447328 thepipe_api-0.1.8/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.8/tests/__init__.py
+-rw-rw-rw-   0        0        0     9523 2024-04-13 23:06:00.000000 thepipe_api-0.1.8/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-15 23:07:30.452327 thepipe_api-0.1.8/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.1.8/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.1.8/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2789 2024-04-15 23:00:33.000000 thepipe_api-0.1.8/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    19810 2024-04-15 22:43:34.000000 thepipe_api-0.1.8/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3606 2024-04-15 23:06:13.000000 thepipe_api-0.1.8/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-15 23:07:30.467328 thepipe_api-0.1.8/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0     9671 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-15 23:07:30.000000 thepipe_api-0.1.8/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.1.7/LICENSE` & `thepipe_api-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.7/PKG-INFO` & `thepipe_api-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.7
+Version: 0.1.8
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,17 @@
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can be called from Python (`thepipe.extract("https://example.com")`) or from the command line (`thepipe path/to/example.pdf`).
+
+![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
 ## Getting Started  🚀
 
 First, install The Pipe. 
 ```
 pip install thepipe_api
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.7 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.8 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
@@ -15,42 +15,46 @@
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
 docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
 Pipe is a multimodal-first tool for feeding files and web pages into vision-
 language models such as GPT-4V. It is best for LLM and RAG applications that
 require a deep understanding of tricky data sources. The Pipe is available as a
-hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. ##
-Getting Started ð First, install The Pipe. ``` pip install thepipe_api ```
-Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key
-yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally
-instead? See the local installation section. Now you can extract comprehensive
-text and visuals from any file: ```python from thepipe_api import thepipe
-chunks = thepipe.extract("example.pdf") ``` Or any website: ```python chunks =
-thepipe.extract("https://example.com") ``` Then feed it into GPT-4-Vision:
-```python response = client.chat.completions.create( model="gpt-4-vision-
-preview", messages = chunks, ) ``` The Pipe's output is a list of sensible
-"chunks", and thus can be used either for storage in a vector database or for
-direct use as a prompt. Extra features such as data table extraction, bar chart
-extraction, custom web authentications and more are available in the [API
-documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/
-litellm) can be used to easily integrate The Pipe with any LLM provider. ##
-Features ð - Extracts text and visuals from any file or web page ð -
-Outputs RAG-ready chunks, optimized for multimodal LLMs ð¼ï¸ + ð¬ - Can
-interpret complex PDFs, web apps, markdown, etc ð§  - Auto-compress prompts
-exceeding your chosen token limit ð¦ - Works with missing file extensions,
-in-memory data streams ð¾ - Works with codebases, URL, git repos, and more
-ð - Multi-threaded â¡ï¸ ## How it works ð ï¸ The pipe is accessible
-from the command line or from [Python](https://www.python.org/downloads/). The
-input source is either a file path, a URL, or a directory (or zip file) path.
-The pipe will extract information from the source and process it for downstream
-use with [language models](https://en.wikipedia.org/wiki/Large_language_model),
-[vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or
-[vision-language models](https://arxiv.org/abs/2304.00685). The output from the
-pipe is a sensible text-based (or multimodal) representation of the extracted
+hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can
+be called from Python (`thepipe.extract("https://example.com")`) or from the
+command line (`thepipe path/to/example.pdf`). ![Demo](https://
+ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/
+demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First, install
+The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
+environment variable is set. Don't have an API key yet? [Get one here](https://
+thepi.pe). Looking to operate it yourself locally instead? See the local
+installation section. Now you can extract comprehensive text and visuals from
+any file: ```python from thepipe_api import thepipe chunks = thepipe.extract
+("example.pdf") ``` Or any website: ```python chunks = thepipe.extract("https:/
+/example.com") ``` Then feed it into GPT-4-Vision: ```python response =
+client.chat.completions.create( model="gpt-4-vision-preview", messages =
+chunks, ) ``` The Pipe's output is a list of sensible "chunks", and thus can be
+used either for storage in a vector database or for direct use as a prompt.
+Extra features such as data table extraction, bar chart extraction, custom web
+authentications and more are available in the [API documentation](https://
+thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to
+easily integrate The Pipe with any LLM provider. ## Features ð - Extracts
+text and visuals from any file or web page ð - Outputs RAG-ready chunks,
+optimized for multimodal LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web
+apps, markdown, etc ð§  - Auto-compress prompts exceeding your chosen token
+limit ð¦ - Works with missing file extensions, in-memory data streams ð¾ -
+Works with codebases, URL, git repos, and more ð - Multi-threaded â¡ï¸ ##
+How it works ð ï¸ The pipe is accessible from the command line or from
+[Python](https://www.python.org/downloads/). The input source is either a file
+path, a URL, or a directory (or zip file) path. The pipe will extract
+information from the source and process it for downstream use with [language
+models](https://en.wikipedia.org/wiki/Large_language_model), [vision
+transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-
+language models](https://arxiv.org/abs/2304.00685). The output from the pipe is
+a sensible text-based (or multimodal) representation of the extracted
 information, carefully crafted to fit within context windows for any models
 from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://
 openai.com/gpt-4). It uses a variety of heuristics for optimal performance with
 vision-language models, including AI filetype detection with [filetype
 detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-
 and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/
 docs), efficient [token compression](https://arxiv.org/abs/2403.12968),
```

### Comparing `thepipe_api-0.1.7/README.md` & `thepipe_api-0.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,17 @@
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can be called from Python (`thepipe.extract("https://example.com")`) or from the command line (`thepipe path/to/example.pdf`).
+
+![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
 ## Getting Started  🚀
 
 First, install The Pipe. 
 ```
 pip install thepipe_api
 ```
```

#### html2text {}

```diff
@@ -6,42 +6,46 @@
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
 docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
 Pipe is a multimodal-first tool for feeding files and web pages into vision-
 language models such as GPT-4V. It is best for LLM and RAG applications that
 require a deep understanding of tricky data sources. The Pipe is available as a
-hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. ##
-Getting Started ð First, install The Pipe. ``` pip install thepipe_api ```
-Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key
-yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally
-instead? See the local installation section. Now you can extract comprehensive
-text and visuals from any file: ```python from thepipe_api import thepipe
-chunks = thepipe.extract("example.pdf") ``` Or any website: ```python chunks =
-thepipe.extract("https://example.com") ``` Then feed it into GPT-4-Vision:
-```python response = client.chat.completions.create( model="gpt-4-vision-
-preview", messages = chunks, ) ``` The Pipe's output is a list of sensible
-"chunks", and thus can be used either for storage in a vector database or for
-direct use as a prompt. Extra features such as data table extraction, bar chart
-extraction, custom web authentications and more are available in the [API
-documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/
-litellm) can be used to easily integrate The Pipe with any LLM provider. ##
-Features ð - Extracts text and visuals from any file or web page ð -
-Outputs RAG-ready chunks, optimized for multimodal LLMs ð¼ï¸ + ð¬ - Can
-interpret complex PDFs, web apps, markdown, etc ð§  - Auto-compress prompts
-exceeding your chosen token limit ð¦ - Works with missing file extensions,
-in-memory data streams ð¾ - Works with codebases, URL, git repos, and more
-ð - Multi-threaded â¡ï¸ ## How it works ð ï¸ The pipe is accessible
-from the command line or from [Python](https://www.python.org/downloads/). The
-input source is either a file path, a URL, or a directory (or zip file) path.
-The pipe will extract information from the source and process it for downstream
-use with [language models](https://en.wikipedia.org/wiki/Large_language_model),
-[vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or
-[vision-language models](https://arxiv.org/abs/2304.00685). The output from the
-pipe is a sensible text-based (or multimodal) representation of the extracted
+hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can
+be called from Python (`thepipe.extract("https://example.com")`) or from the
+command line (`thepipe path/to/example.pdf`). ![Demo](https://
+ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/
+demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First, install
+The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
+environment variable is set. Don't have an API key yet? [Get one here](https://
+thepi.pe). Looking to operate it yourself locally instead? See the local
+installation section. Now you can extract comprehensive text and visuals from
+any file: ```python from thepipe_api import thepipe chunks = thepipe.extract
+("example.pdf") ``` Or any website: ```python chunks = thepipe.extract("https:/
+/example.com") ``` Then feed it into GPT-4-Vision: ```python response =
+client.chat.completions.create( model="gpt-4-vision-preview", messages =
+chunks, ) ``` The Pipe's output is a list of sensible "chunks", and thus can be
+used either for storage in a vector database or for direct use as a prompt.
+Extra features such as data table extraction, bar chart extraction, custom web
+authentications and more are available in the [API documentation](https://
+thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to
+easily integrate The Pipe with any LLM provider. ## Features ð - Extracts
+text and visuals from any file or web page ð - Outputs RAG-ready chunks,
+optimized for multimodal LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web
+apps, markdown, etc ð§  - Auto-compress prompts exceeding your chosen token
+limit ð¦ - Works with missing file extensions, in-memory data streams ð¾ -
+Works with codebases, URL, git repos, and more ð - Multi-threaded â¡ï¸ ##
+How it works ð ï¸ The pipe is accessible from the command line or from
+[Python](https://www.python.org/downloads/). The input source is either a file
+path, a URL, or a directory (or zip file) path. The pipe will extract
+information from the source and process it for downstream use with [language
+models](https://en.wikipedia.org/wiki/Large_language_model), [vision
+transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-
+language models](https://arxiv.org/abs/2304.00685). The output from the pipe is
+a sensible text-based (or multimodal) representation of the extracted
 information, carefully crafted to fit within context windows for any models
 from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://
 openai.com/gpt-4). It uses a variety of heuristics for optimal performance with
 vision-language models, including AI filetype detection with [filetype
 detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-
 and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/
 docs), efficient [token compression](https://arxiv.org/abs/2403.12968),
```

### Comparing `thepipe_api-0.1.7/setup.py` & `thepipe_api-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.1.7',
+    version='0.1.8',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.1.7/tests/test_thepipe.py` & `thepipe_api-0.1.8/tests/test_thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.7/thepipe_api/compressor.py` & `thepipe_api-0.1.8/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.7/thepipe_api/core.py` & `thepipe_api-0.1.8/thepipe_api/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     elif status == 'info':
         message = Fore.YELLOW + f"{text}..."
     elif status == 'error':
         message = Fore.RED + f"{text} ❌"
     print(Style.RESET_ALL + message + Style.RESET_ALL)
 
 def count_tokens(chunks: List[Chunk]) -> int:
-    return sum([(len(chunk.path)+len(chunk.text))/4 for chunk in chunks if chunk.text is not None])
+    return sum([((len(chunk.path) if chunk.path else 0) + (len(chunk.text) if chunk.text else 0))/4 for chunk in chunks])
 
 def image_to_base64(image: Image.Image) -> str:
     buffered = BytesIO()
     if image.mode == 'RGBA':
         image = image.convert('RGB')
     image.save(buffered, format="JPEG")
     return base64.b64encode(buffered.getvalue()).decode()
```

### Comparing `thepipe_api-0.1.7/thepipe_api/extractor.py` & `thepipe_api-0.1.8/thepipe_api/extractor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.7/thepipe_api/thepipe.py` & `thepipe_api-0.1.8/thepipe_api/thepipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     n_images = 0
     for i, chunk in enumerate(chunks):
         if chunk is None:
             continue
         if chunk.text is not None:
             text += f"""{chunk.path}:\n```\n{chunk.text}\n```\n\n"""
         if chunk.image is not None:
-            clean_path = chunk.path.replace('/', '_').replace('\\', '_')
-            clean_path = re.sub(r"[^a-zA-Z0-9 _]", "", clean_path)
+            if chunk.path is None:
+                clean_path = f"image"
+            else:
+                clean_path = chunk.path.replace('/', '_').replace('\\', '_')
+                clean_path = re.sub(r"[^a-zA-Z0-9 _]", "", clean_path)
             chunk.image.convert('RGB').save(f'outputs/{clean_path}_{i}.jpg')
             n_images += 1
     # Save the text
     with open('outputs/prompt.txt', 'w', encoding='utf-8') as file:
         file.write(text)
     if verbose:
         print_status(f"Output {len(text)/4} tokens and {n_images} images to 'outputs'", status='success')
```

### Comparing `thepipe_api-0.1.7/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.1.8/thepipe_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.7
+Version: 0.1.8
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,17 @@
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can be called from Python (`thepipe.extract("https://example.com")`) or from the command line (`thepipe path/to/example.pdf`).
+
+![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
 ## Getting Started  🚀
 
 First, install The Pipe. 
 ```
 pip install thepipe_api
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.7 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.8 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
@@ -15,42 +15,46 @@
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
 docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
 Pipe is a multimodal-first tool for feeding files and web pages into vision-
 language models such as GPT-4V. It is best for LLM and RAG applications that
 require a deep understanding of tricky data sources. The Pipe is available as a
-hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. ##
-Getting Started ð First, install The Pipe. ``` pip install thepipe_api ```
-Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key
-yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally
-instead? See the local installation section. Now you can extract comprehensive
-text and visuals from any file: ```python from thepipe_api import thepipe
-chunks = thepipe.extract("example.pdf") ``` Or any website: ```python chunks =
-thepipe.extract("https://example.com") ``` Then feed it into GPT-4-Vision:
-```python response = client.chat.completions.create( model="gpt-4-vision-
-preview", messages = chunks, ) ``` The Pipe's output is a list of sensible
-"chunks", and thus can be used either for storage in a vector database or for
-direct use as a prompt. Extra features such as data table extraction, bar chart
-extraction, custom web authentications and more are available in the [API
-documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/
-litellm) can be used to easily integrate The Pipe with any LLM provider. ##
-Features ð - Extracts text and visuals from any file or web page ð -
-Outputs RAG-ready chunks, optimized for multimodal LLMs ð¼ï¸ + ð¬ - Can
-interpret complex PDFs, web apps, markdown, etc ð§  - Auto-compress prompts
-exceeding your chosen token limit ð¦ - Works with missing file extensions,
-in-memory data streams ð¾ - Works with codebases, URL, git repos, and more
-ð - Multi-threaded â¡ï¸ ## How it works ð ï¸ The pipe is accessible
-from the command line or from [Python](https://www.python.org/downloads/). The
-input source is either a file path, a URL, or a directory (or zip file) path.
-The pipe will extract information from the source and process it for downstream
-use with [language models](https://en.wikipedia.org/wiki/Large_language_model),
-[vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or
-[vision-language models](https://arxiv.org/abs/2304.00685). The output from the
-pipe is a sensible text-based (or multimodal) representation of the extracted
+hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. It can
+be called from Python (`thepipe.extract("https://example.com")`) or from the
+command line (`thepipe path/to/example.pdf`). ![Demo](https://
+ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/
+demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First, install
+The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
+environment variable is set. Don't have an API key yet? [Get one here](https://
+thepi.pe). Looking to operate it yourself locally instead? See the local
+installation section. Now you can extract comprehensive text and visuals from
+any file: ```python from thepipe_api import thepipe chunks = thepipe.extract
+("example.pdf") ``` Or any website: ```python chunks = thepipe.extract("https:/
+/example.com") ``` Then feed it into GPT-4-Vision: ```python response =
+client.chat.completions.create( model="gpt-4-vision-preview", messages =
+chunks, ) ``` The Pipe's output is a list of sensible "chunks", and thus can be
+used either for storage in a vector database or for direct use as a prompt.
+Extra features such as data table extraction, bar chart extraction, custom web
+authentications and more are available in the [API documentation](https://
+thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to
+easily integrate The Pipe with any LLM provider. ## Features ð - Extracts
+text and visuals from any file or web page ð - Outputs RAG-ready chunks,
+optimized for multimodal LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web
+apps, markdown, etc ð§  - Auto-compress prompts exceeding your chosen token
+limit ð¦ - Works with missing file extensions, in-memory data streams ð¾ -
+Works with codebases, URL, git repos, and more ð - Multi-threaded â¡ï¸ ##
+How it works ð ï¸ The pipe is accessible from the command line or from
+[Python](https://www.python.org/downloads/). The input source is either a file
+path, a URL, or a directory (or zip file) path. The pipe will extract
+information from the source and process it for downstream use with [language
+models](https://en.wikipedia.org/wiki/Large_language_model), [vision
+transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-
+language models](https://arxiv.org/abs/2304.00685). The output from the pipe is
+a sensible text-based (or multimodal) representation of the extracted
 information, carefully crafted to fit within context windows for any models
 from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://
 openai.com/gpt-4). It uses a variety of heuristics for optimal performance with
 vision-language models, including AI filetype detection with [filetype
 detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-
 and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/
 docs), efficient [token compression](https://arxiv.org/abs/2403.12968),
```

