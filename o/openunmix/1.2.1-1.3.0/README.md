# Comparing `tmp/openunmix-1.2.1.tar.gz` & `tmp/openunmix-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openunmix-1.2.1.tar", last modified: Fri Jul 23 08:39:35 2021, max compression
+gzip compressed data, was "openunmix-1.3.0.tar", last modified: Tue Apr 16 11:03:42 2024, max compression
```

## Comparing `openunmix-1.2.1.tar` & `openunmix-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 faro       (501) staff       (20)        0 2021-07-23 08:39:35.000000 openunmix-1.2.1/
--rw-r--r--   0 faro       (501) staff       (20)     1103 2021-05-26 09:47:00.000000 openunmix-1.2.1/LICENSE
--rw-r--r--   0 faro       (501) staff       (20)    18682 2021-07-23 08:39:35.000000 openunmix-1.2.1/PKG-INFO
--rw-r--r--   0 faro       (501) staff       (20)    15571 2021-07-23 08:38:56.000000 openunmix-1.2.1/README.md
-drwxr-xr-x   0 faro       (501) staff       (20)        0 2021-07-23 08:39:35.000000 openunmix-1.2.1/openunmix/
--rw-r--r--   0 faro       (501) staff       (20)    12622 2021-07-05 12:14:08.000000 openunmix-1.2.1/openunmix/__init__.py
--rw-r--r--   0 faro       (501) staff       (20)     6398 2021-07-23 08:38:56.000000 openunmix-1.2.1/openunmix/cli.py
--rw-r--r--   0 faro       (501) staff       (20)    35261 2021-07-15 13:07:29.000000 openunmix-1.2.1/openunmix/data.py
--rw-r--r--   0 faro       (501) staff       (20)     5567 2021-07-23 08:38:56.000000 openunmix-1.2.1/openunmix/evaluate.py
--rw-r--r--   0 faro       (501) staff       (20)    20255 2021-07-15 13:07:29.000000 openunmix-1.2.1/openunmix/filtering.py
--rw-r--r--   0 faro       (501) staff       (20)    12186 2021-07-01 20:30:54.000000 openunmix-1.2.1/openunmix/model.py
--rw-r--r--   0 faro       (501) staff       (20)     2985 2021-07-23 08:38:56.000000 openunmix-1.2.1/openunmix/predict.py
--rw-r--r--   0 faro       (501) staff       (20)     6542 2021-07-23 07:55:18.000000 openunmix-1.2.1/openunmix/transforms.py
--rw-r--r--   0 faro       (501) staff       (20)    10498 2021-06-08 14:23:06.000000 openunmix-1.2.1/openunmix/utils.py
-drwxr-xr-x   0 faro       (501) staff       (20)        0 2021-07-23 08:39:35.000000 openunmix-1.2.1/openunmix.egg-info/
--rw-r--r--   0 faro       (501) staff       (20)    18682 2021-07-23 08:39:34.000000 openunmix-1.2.1/openunmix.egg-info/PKG-INFO
--rw-r--r--   0 faro       (501) staff       (20)      665 2021-07-23 08:39:34.000000 openunmix-1.2.1/openunmix.egg-info/SOURCES.txt
--rw-r--r--   0 faro       (501) staff       (20)        1 2021-07-23 08:39:34.000000 openunmix-1.2.1/openunmix.egg-info/dependency_links.txt
--rw-r--r--   0 faro       (501) staff       (20)       48 2021-07-23 08:39:34.000000 openunmix-1.2.1/openunmix.egg-info/entry_points.txt
--rw-r--r--   0 faro       (501) staff       (20)      225 2021-07-23 08:39:34.000000 openunmix-1.2.1/openunmix.egg-info/requires.txt
--rw-r--r--   0 faro       (501) staff       (20)       16 2021-07-23 08:39:34.000000 openunmix-1.2.1/openunmix.egg-info/top_level.txt
--rw-r--r--   0 faro       (501) staff       (20)      176 2021-05-26 09:47:00.000000 openunmix-1.2.1/pyproject.toml
--rw-r--r--   0 faro       (501) staff       (20)       38 2021-07-23 08:39:35.000000 openunmix-1.2.1/setup.cfg
--rw-r--r--   0 faro       (501) staff       (20)     1480 2021-07-23 08:39:09.000000 openunmix-1.2.1/setup.py
-drwxr-xr-x   0 faro       (501) staff       (20)        0 2021-07-23 08:39:35.000000 openunmix-1.2.1/tests/
--rw-r--r--   0 faro       (501) staff       (20)        0 2021-05-26 09:47:00.000000 openunmix-1.2.1/tests/__init__.py
--rw-r--r--   0 faro       (501) staff       (20)      850 2021-05-26 09:47:00.000000 openunmix-1.2.1/tests/create_vectors.py
--rw-r--r--   0 faro       (501) staff       (20)      726 2021-05-26 09:47:00.000000 openunmix-1.2.1/tests/test_augmentations.py
--rw-r--r--   0 faro       (501) staff       (20)     1589 2021-05-26 09:47:00.000000 openunmix-1.2.1/tests/test_datasets.py
--rw-r--r--   0 faro       (501) staff       (20)      886 2021-05-26 09:47:00.000000 openunmix-1.2.1/tests/test_io.py
--rw-r--r--   0 faro       (501) staff       (20)     2471 2021-05-26 09:47:00.000000 openunmix-1.2.1/tests/test_jit.py
--rw-r--r--   0 faro       (501) staff       (20)     1455 2021-07-15 12:40:46.000000 openunmix-1.2.1/tests/test_model.py
--rw-r--r--   0 faro       (501) staff       (20)     2622 2021-07-23 07:55:18.000000 openunmix-1.2.1/tests/test_regression.py
--rw-r--r--   0 faro       (501) staff       (20)     1198 2021-05-26 09:47:00.000000 openunmix-1.2.1/tests/test_transforms.py
--rw-r--r--   0 faro       (501) staff       (20)      349 2021-05-26 09:47:00.000000 openunmix-1.2.1/tests/test_utils.py
--rw-r--r--   0 faro       (501) staff       (20)     1654 2021-07-15 13:07:29.000000 openunmix-1.2.1/tests/test_wiener.py
+drwxr-xr-x   0 faro       (501) staff       (20)        0 2024-04-16 11:03:42.136144 openunmix-1.3.0/
+-rw-r--r--   0 faro       (501) staff       (20)     1103 2021-05-26 09:47:00.000000 openunmix-1.3.0/LICENSE
+-rw-r--r--   0 faro       (501) staff       (20)    17388 2024-04-16 11:03:42.135029 openunmix-1.3.0/PKG-INFO
+-rw-r--r--   0 faro       (501) staff       (20)    15571 2024-04-16 11:03:29.000000 openunmix-1.3.0/README.md
+drwxr-xr-x   0 faro       (501) staff       (20)        0 2024-04-16 11:03:42.126465 openunmix-1.3.0/openunmix/
+-rw-r--r--   0 faro       (501) staff       (20)    13750 2024-04-16 11:03:29.000000 openunmix-1.3.0/openunmix/__init__.py
+-rw-r--r--   0 faro       (501) staff       (20)     6381 2024-04-16 11:03:29.000000 openunmix-1.3.0/openunmix/cli.py
+-rw-r--r--   0 faro       (501) staff       (20)    35093 2024-04-16 11:03:29.000000 openunmix-1.3.0/openunmix/data.py
+-rw-r--r--   0 faro       (501) staff       (20)     5545 2024-04-16 11:03:29.000000 openunmix-1.3.0/openunmix/evaluate.py
+-rw-r--r--   0 faro       (501) staff       (20)    20195 2024-04-16 11:03:29.000000 openunmix-1.3.0/openunmix/filtering.py
+-rw-r--r--   0 faro       (501) staff       (20)    12312 2024-04-16 11:03:29.000000 openunmix-1.3.0/openunmix/model.py
+-rw-r--r--   0 faro       (501) staff       (20)     2985 2021-12-04 10:23:54.000000 openunmix-1.3.0/openunmix/predict.py
+-rw-r--r--   0 faro       (501) staff       (20)     6630 2021-12-04 11:13:35.000000 openunmix-1.3.0/openunmix/transforms.py
+-rw-r--r--   0 faro       (501) staff       (20)    10516 2024-04-16 11:03:29.000000 openunmix-1.3.0/openunmix/utils.py
+drwxr-xr-x   0 faro       (501) staff       (20)        0 2024-04-16 11:03:42.133127 openunmix-1.3.0/openunmix.egg-info/
+-rw-r--r--   0 faro       (501) staff       (20)    17388 2024-04-16 11:03:42.000000 openunmix-1.3.0/openunmix.egg-info/PKG-INFO
+-rw-r--r--   0 faro       (501) staff       (20)      656 2024-04-16 11:03:42.000000 openunmix-1.3.0/openunmix.egg-info/SOURCES.txt
+-rw-r--r--   0 faro       (501) staff       (20)        1 2024-04-16 11:03:42.000000 openunmix-1.3.0/openunmix.egg-info/dependency_links.txt
+-rw-r--r--   0 faro       (501) staff       (20)       47 2024-04-16 11:03:42.000000 openunmix-1.3.0/openunmix.egg-info/entry_points.txt
+-rw-r--r--   0 faro       (501) staff       (20)      233 2024-04-16 11:03:42.000000 openunmix-1.3.0/openunmix.egg-info/requires.txt
+-rw-r--r--   0 faro       (501) staff       (20)       10 2024-04-16 11:03:42.000000 openunmix-1.3.0/openunmix.egg-info/top_level.txt
+-rw-r--r--   0 faro       (501) staff       (20)     1997 2024-04-16 11:03:29.000000 openunmix-1.3.0/pyproject.toml
+-rw-r--r--   0 faro       (501) staff       (20)       38 2024-04-16 11:03:42.136269 openunmix-1.3.0/setup.cfg
+drwxr-xr-x   0 faro       (501) staff       (20)        0 2024-04-16 11:03:42.132717 openunmix-1.3.0/tests/
+-rw-r--r--   0 faro       (501) staff       (20)        0 2021-05-26 09:47:00.000000 openunmix-1.3.0/tests/__init__.py
+-rw-r--r--   0 faro       (501) staff       (20)      850 2021-12-04 10:23:54.000000 openunmix-1.3.0/tests/create_vectors.py
+-rw-r--r--   0 faro       (501) staff       (20)      712 2024-04-16 11:03:29.000000 openunmix-1.3.0/tests/test_augmentations.py
+-rw-r--r--   0 faro       (501) staff       (20)     1589 2021-12-04 10:23:54.000000 openunmix-1.3.0/tests/test_datasets.py
+-rw-r--r--   0 faro       (501) staff       (20)      886 2021-12-04 10:23:54.000000 openunmix-1.3.0/tests/test_io.py
+-rw-r--r--   0 faro       (501) staff       (20)     1143 2024-04-16 11:03:29.000000 openunmix-1.3.0/tests/test_jit.py
+-rw-r--r--   0 faro       (501) staff       (20)     1434 2024-04-16 11:03:29.000000 openunmix-1.3.0/tests/test_model.py
+-rw-r--r--   0 faro       (501) staff       (20)     2597 2024-04-16 11:03:29.000000 openunmix-1.3.0/tests/test_regression.py
+-rw-r--r--   0 faro       (501) staff       (20)     1170 2024-04-16 11:03:29.000000 openunmix-1.3.0/tests/test_transforms.py
+-rw-r--r--   0 faro       (501) staff       (20)      349 2021-12-04 10:23:54.000000 openunmix-1.3.0/tests/test_utils.py
+-rw-r--r--   0 faro       (501) staff       (20)     1654 2021-12-04 10:23:54.000000 openunmix-1.3.0/tests/test_wiener.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `openunmix-1.2.1/LICENSE` & `openunmix-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openunmix-1.2.1/PKG-INFO` & `openunmix-1.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,314 +1,335 @@
 Metadata-Version: 2.1
 Name: openunmix
-Version: 1.2.1
+Version: 1.3.0
 Summary: PyTorch-based music source separation toolkit
-Home-page: https://github.com/sigsep/open-unmix-pytorch
-Author: Fabian-Robert Stöter
-Author-email: fabian-robert.stoter@inria.fr
+Author-email: Fabian-Robert Stöter <mail@faroit.com>, Antoine Liutkus <antoine.liutkus@inria.fr>
 License: MIT
-Description: #  _Open-Unmix_ for PyTorch
-        
-        [![status](https://joss.theoj.org/papers/571753bc54c5d6dd36382c3d801de41d/status.svg)](https://joss.theoj.org/papers/571753bc54c5d6dd36382c3d801de41d) 
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1mijF0zGWxN-KaxTnd0q6hayAlrID5fEQ)
-        [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/open-unmix-a-reference-implementation-for/music-source-separation-on-musdb18)](https://paperswithcode.com/sota/music-source-separation-on-musdb18?p=open-unmix-a-reference-implementation-for)
-        
-        [![Build Status](https://github.com/sigsep/open-unmix-pytorch/workflows/CI/badge.svg)](https://github.com/sigsep/open-unmix-pytorch/actions?query=workflow%3ACI+branch%3Amaster+event%3Apush)
-        [![Latest Version](https://img.shields.io/pypi/v/openunmix.svg)](https://pypi.python.org/pypi/openunmix)
-        [![Supported Python versions](https://img.shields.io/pypi/pyversions/openunmix.svg)](https://pypi.python.org/pypi/openunmix)
-        
-        This repository contains the PyTorch (1.8+) implementation of __Open-Unmix__, a deep neural network reference implementation for music source separation, applicable for researchers, audio engineers and artists. __Open-Unmix__ provides ready-to-use models that allow users to separate pop music into four stems: __vocals__, __drums__, __bass__ and the remaining __other__ instruments. The models were pre-trained on the freely available [MUSDB18](https://sigsep.github.io/datasets/musdb.html) dataset. See details at [apply pre-trained model](#getting-started).
-        
-        ## ⭐️ News 
-        
-        - 03/07/2021: We added `umxl`, a model that was trained on extra data which significantly improves the performance, especially generalization.
-        - 14/02/2021: We released the new version of open-unmix as a python package. This comes with: a fully differentiable version of [norbert](https://github.com/sigsep/norbert), improved audio loading pipeline and large number of bug fixes. See [release notes](https://github.com/sigsep/open-unmix-pytorch/releases/) for further info.
-        
-        - 06/05/2020: We added a pre-trained speech enhancement model `umxse` provided by Sony.
-        
-        - 13/03/2020: Open-unmix was awarded 2nd place in the [PyTorch Global Summer Hackathon 2020](https://devpost.com/software/open-unmix).
-        
-        __Related Projects:__ open-unmix-pytorch | [open-unmix-nnabla](https://github.com/sigsep/open-unmix-nnabla) | [musdb](https://github.com/sigsep/sigsep-mus-db) | [museval](https://github.com/sigsep/sigsep-mus-eval) | [norbert](https://github.com/sigsep/norbert)
-        
-        ## 🧠 The Model (for one source)
-        
-        ![](https://docs.google.com/drawings/d/e/2PACX-1vTPoQiPwmdfET4pZhue1RvG7oEUJz7eUeQvCu6vzYeKRwHl6by4RRTnphImSKM0k5KXw9rZ1iIFnpGW/pub?w=959&h=308)
-        
-        To perform separation into multiple sources, _Open-unmix_ comprises multiple models that are trained for each particular target. While this makes the training less comfortable, it allows great flexibility to customize the training data for each target source.
-        
-        Each _Open-Unmix_ source model is based on a three-layer bidirectional deep LSTM. The model learns to predict the magnitude spectrogram of a target source, like _vocals_, from the magnitude spectrogram of a mixture input. Internally, the prediction is obtained by applying a mask on the input. The model is optimized in the magnitude domain using mean squared error.
-        
-        ### Input Stage
-        
-        __Open-Unmix__ operates in the time-frequency domain to perform its prediction. The input of the model is either:
-        
-        * __`models.Separator`:__ A time domain signal tensor of shape `(nb_samples, nb_channels, nb_timesteps)`, where `nb_samples` are the samples in a batch, `nb_channels` is 1 or 2 for mono or stereo audio, respectively, and `nb_timesteps` is the number of audio samples in the recording. In this case, the model computes STFTs with either `torch` or `asteroid_filteranks` on the fly.
-        
-        * __`models.OpenUnmix`:__ The core open-unmix takes **magnitude spectrograms** directly (e.g. when pre-computed and loaded from disk). In that case, the input is of shape `(nb_frames, nb_samples, nb_channels, nb_bins)`, where `nb_frames` and `nb_bins` are the time and frequency-dimensions of a Short-Time-Fourier-Transform.
-        
-        The input spectrogram is _standardized_ using the global mean and standard deviation for every frequency bin across all frames. Furthermore, we apply batch normalization in multiple stages of the model to make the training more robust against gain variation.
-        
-        ### Dimensionality reduction
-        
-        The LSTM is not operating on the original input spectrogram resolution. Instead, in the first step after the normalization, the network learns to compresses the frequency and channel axis of the model to reduce redundancy and make the model converge faster.
-        
-        ### Bidirectional-LSTM
-        
-        The core of __open-unmix__ is a three layer bidirectional [LSTM network](https://dl.acm.org/citation.cfm?id=1246450). Due to its recurrent nature, the model can be trained and evaluated on arbitrary length of audio signals. Since the model takes information from past and future simultaneously, the model cannot be used in an online/real-time manner.
-        An uni-directional model can easily be trained as described [here](docs/training.md).
-        
-        ### Output Stage
-        
-        After applying the LSTM, the signal is decoded back to its original input dimensionality. In the last steps the output is multiplied with the input magnitude spectrogram, so that the models is asked to learn a mask.
-        
-        ## 🤹‍♀️ Putting source models together: the `Separator`
-        
-        `models.Separator` puts together _Open-unmix_ spectrogram model for each desired target, and combines their output through a multichannel generalized Wiener filter, before application of inverse STFTs using `torchaudio`.
-        The filtering is differentiable (but parameter-free) version of [norbert](https://github.com/sigsep/norbert). The separator is currently currently only used during inference.
-        
-        ## 🏁 Getting started
-        
-        ### Installation
-        
-        `openunmix` can be installed from pypi using:
-        
-        ```
-        pip install openunmix
-        ```
-        
-        Note, that the pypi version of openunmix uses [torchaudio] to load and save audio files. To increase the number of supported input and output file formats (such as STEMS export), please additionally install [stempeg](https://github.com/faroit/stempeg).
-        
-        Training is not part of the open-unmix package, please follow [docs/train.md] for more information.
-        
-        #### Using Docker
-        
-        We also provide a docker container. Performing separation of a local track in `~/Music/track1.wav` can be performed in a single line:
-        
-        ```
-        docker run -v ~/Music/:/data -it faroit/open-unmix-pytorch "/data/track1.wav" --outdir /data/track1
-        ```
-        
-        ### Pre-trained models
-        
-        We provide three core pre-trained music separation models. All three models are end-to-end models that take waveform inputs and output the separated waveforms.
-        
-        * __`umxl` (default)__  trained on private stems dataset of compressed stems. __Note, that the weights are only licensed for non-commercial use (CC BY-NC-SA 4.0).__
-        
-          [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5069601.svg)](https://doi.org/10.5281/zenodo.5069601)
-        
-        * __`umxhq`__  trained on [MUSDB18-HQ](https://sigsep.github.io/datasets/musdb.html#uncompressed-wav) which comprises the same tracks as in MUSDB18 but un-compressed which yield in a full bandwidth of 22050 Hz.
-        
-          [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3370489.svg)](https://doi.org/10.5281/zenodo.3370489)
-        
-        * __`umx`__ is trained on the regular [MUSDB18](https://sigsep.github.io/datasets/musdb.html#compressed-stems) which is bandwidth limited to 16 kHz do to AAC compression. This model should be used for comparison with other (older) methods for evaluation in [SiSEC18](sisec18.unmix.app).
-        
-          [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3370486.svg)](https://doi.org/10.5281/zenodo.3370486)
-        
-        Furthermore, we provide a model for speech enhancement trained by [Sony Corporation](link)
-        
-        * __`umxse`__ speech enhancement model is trained on the 28-speaker version of the [Voicebank+DEMAND corpus](https://datashare.is.ed.ac.uk/handle/10283/1942?show=full).
-        
-          [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3786908.svg)](https://doi.org/10.5281/zenodo.3786908)
-        
-        All four models are also available as spectrogram (core) models, which take magnitude spectrogram inputs and ouput separated spectrograms.
-        These models can be loaded using `umxl_spec`, `umxhq_spec`, `umx_spec` and `umxse_spec`.
-        
-        To separate audio files (`wav`, `flac`, `ogg` - but not `mp3`) files just run:
-        
-        ```bash
-        umx input_file.wav
-        ```
-        
-        A more detailed list of the parameters used for the separation is given in the [inference.md](/docs/inference.md) document.
-        
-        We provide a [jupyter notebook on google colab](https://colab.research.google.com/drive/1mijF0zGWxN-KaxTnd0q6hayAlrID5fEQ) to experiment with open-unmix and to separate files online without any installation setup.
-        
-        ### Using pre-trained models from within python
-        
-        We implementes several ways to load pre-trained models and use them from within your python projects:
-        #### When the package is installed
-        
-        Loading a pre-trained models is as simple as loading
-        
-        ```python
-        separator = openunmix.umxl(...)
-        ```
-        #### torch.hub
-        
-        We also provide a torch.hub compatible modules that can be loaded. Note that this does _not_ even require to install the open-unmix packagen and should generally work when the pytorch version is the same.
-        
-        ```python
-        separator = torch.hub.load('sigsep/open-unmix-pytorch', 'umxl, device=device)
-        ```
-        
-        Where, `umxl` specifies the pre-trained model. 
-        #### Performing separation
-        
-        With a created separator object, one can perform separation of some `audio` (torch.Tensor of shape `(channels, length)`, provided as at a sampling rate `separator.sample_rate`) through:
-        
-        ```python
-        estimates = separator(audio, ...)
-        # returns estimates as tensor
-        ```
-        
-        Note that this requires the audio to be in the right shape and sampling rate. For convenience we provide a pre-processing in `openunmix.utils.preprocess(..`)` that takes numpy audio and converts it to be used for open-unmix.
-        
-        #### One-liner
-        
-        To perform model loading, preprocessing and separation in one step, just use:
-        
-        ```python
-        from openunmix import separate
-        estimates = separate.predict(audio, ...)
-        ```
-        
-        ### Load user-trained models
-        
-        When a path instead of a model-name is provided to `--model`, pre-trained `Separator` will be loaded from disk.
-        E.g. The following files are assumed to present when loading `--model mymodel --targets vocals`
-        
-        * `mymodel/separator.json`
-        * `mymodel/vocals.pth`
-        * `mymodel/vocals.json`
-        
-        
-        Note that the separator usually joins multiple models for each target and performs separation using all models. E.g. if the separator contains `vocals` and `drums` models, two output files are generated, unless the `--residual` option is selected, in which case an additional source will be produced, containing an estimate of all that is not the targets in the mixtures.
-        
-        ### Evaluation using `museval`
-        
-        To perform evaluation in comparison to other SISEC systems, you would need to install the `museval` package using
-        
-        ```
-        pip install museval
-        ```
-        
-        and then run the evaluation using
-        
-        `python -m openunmix.evaluate --outdir /path/to/musdb/estimates --evaldir /path/to/museval/results`
-        
-        ### Results compared to SiSEC 2018 (SDR/Vocals)
-        
-        Open-Unmix yields state-of-the-art results compared to participants from [SiSEC 2018](https://sisec18.unmix.app/#/methods). The performance of `UMXHQ` and `UMX` is almost identical since it was evaluated on compressed STEMS.
-        
-        ![boxplot_updated](https://user-images.githubusercontent.com/72940/63944652-3f624c80-ca72-11e9-8d33-bed701679fe6.png)
-        
-        Note that
-        
-        1. [`STL1`, `TAK2`, `TAK3`, `TAU1`, `UHL3`, `UMXHQ`] were omitted as they were _not_ trained on only _MUSDB18_.
-        2. [`HEL1`, `TAK1`, `UHL1`, `UHL2`] are not open-source.
-        
-        #### Scores (Median of frames, Median of tracks)
-        
-        |target|SDR  | SDR |  SDR |
-        |------|-----|-----|-----|
-        |`model`|UMX  |UMXHQ|UMXL |
-        |vocals|6.32 | 6.25|__7.21__ |
-        |bass  |5.23 | 5.07|__6.02__ |
-        |drums |5.73 | 6.04|__7.15__ |
-        |other |4.02 | 4.28|__4.89__ |
-        
-        ## Training
-        
-        Details on the training is provided in a separate document [here](docs/training.md).
-        
-        ## Extensions
-        
-        Details on how _open-unmix_ can be extended or improved for future research on music separation is described in a separate document [here](docs/extensions.md).
-        
-        
-        ## Design Choices
-        
-        we favored simplicity over performance to promote clearness of the code. The rationale is to have __open-unmix__ serve as a __baseline__ for future research while performance still meets current state-of-the-art (See [Evaluation](#Evaluation)). The results are comparable/better to those of `UHL1`/`UHL2` which obtained the best performance over all systems trained on MUSDB18 in the [SiSEC 2018 Evaluation campaign](https://sisec18.unmix.app).
-        We designed the code to allow researchers to reproduce existing results, quickly develop new architectures and add own user data for training and testing. We favored framework specifics implementations instead of having a monolithic repository with common code for all frameworks.
-        
-        ## How to contribute
-        
-        _open-unmix_ is a community focused project, we therefore encourage the community to submit bug-fixes and requests for technical support through [github issues](https://github.com/sigsep/open-unmix-pytorch/issues/new/choose). For more details of how to contribute, please follow our [`CONTRIBUTING.md`](CONTRIBUTING.md). For help and support, please use the gitter chat or the google groups forums. 
-        
-        ### Authors
-        
-        [Fabian-Robert Stöter](https://www.faroit.com/), [Antoine Liutkus](https://github.com/aliutkus), Inria and LIRMM, Montpellier, France
-        
-        ## References
-        
-        <details><summary>If you use open-unmix for your research – Cite Open-Unmix</summary>
-        
-        ```latex
-        @article{stoter19,  
-          author={F.-R. St\\"oter and S. Uhlich and A. Liutkus and Y. Mitsufuji},  
-          title={Open-Unmix - A Reference Implementation for Music Source Separation},  
-          journal={Journal of Open Source Software},  
-          year=2019,
-          doi = {10.21105/joss.01667},
-          url = {https://doi.org/10.21105/joss.01667}
-        }
-        ```
-        
-        </p>
-        </details>
-        
-        <details><summary>If you use the MUSDB dataset for your research - Cite the MUSDB18 Dataset</summary>
-        <p>
-        
-        ```latex
-        @misc{MUSDB18,
-          author       = {Rafii, Zafar and
-                          Liutkus, Antoine and
-                          Fabian-Robert St{\"o}ter and
-                          Mimilakis, Stylianos Ioannis and
-                          Bittner, Rachel},
-          title        = {The {MUSDB18} corpus for music separation},
-          month        = dec,
-          year         = 2017,
-          doi          = {10.5281/zenodo.1117372},
-          url          = {https://doi.org/10.5281/zenodo.1117372}
-        }
-        ```
-        
-        </p>
-        </details>
-        
-        
-        <details><summary>If compare your results with SiSEC 2018 Participants - Cite the SiSEC 2018 LVA/ICA Paper</summary>
-        <p>
-        
-        ```latex
-        @inproceedings{SiSEC18,
-          author="St{\"o}ter, Fabian-Robert and Liutkus, Antoine and Ito, Nobutaka",
-          title="The 2018 Signal Separation Evaluation Campaign",
-          booktitle="Latent Variable Analysis and Signal Separation:
-          14th International Conference, LVA/ICA 2018, Surrey, UK",
-          year="2018",
-          pages="293--305"
-        }
-        ```
-        
-        </p>
-        </details>
-        
-        ⚠️ Please note that the official acronym for _open-unmix_ is **UMX**.
-        
-        ### License
-        
-        MIT
-        
-        ### Acknowledgements
-        
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/sigsep/website/master/content/open-unmix/logo_INRIA.svg?sanitize=true" width="200" title="inria">
-          <img src="https://raw.githubusercontent.com/sigsep/website/master/content/open-unmix/anr.jpg" width="100" alt="anr">
-        </p>
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Project-URL: Homepage, https://github.com/sigsep/open-unmix-pytorch
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: torchaudio>=0.9.0
+Requires-Dist: torch>=1.9.0
+Requires-Dist: tqdm
 Provides-Extra: asteroid
-Provides-Extra: tests
+Requires-Dist: asteroid-filterbanks>=0.3.2; extra == "asteroid"
 Provides-Extra: stempeg
+Requires-Dist: stempeg; extra == "stempeg"
 Provides-Extra: evaluation
+Requires-Dist: musdb>=0.4.0; extra == "evaluation"
+Requires-Dist: museval>=0.4.0; extra == "evaluation"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: musdb>=0.4.0; extra == "tests"
+Requires-Dist: museval>=0.4.0; extra == "tests"
+Requires-Dist: stempeg; extra == "tests"
+Requires-Dist: asteroid-filterbanks>=0.3.2; extra == "tests"
+Requires-Dist: onnx; extra == "tests"
+Requires-Dist: tqdm; extra == "tests"
+
+#  _Open-Unmix_ for PyTorch
+
+[![status](https://joss.theoj.org/papers/571753bc54c5d6dd36382c3d801de41d/status.svg)](https://joss.theoj.org/papers/571753bc54c5d6dd36382c3d801de41d) 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1mijF0zGWxN-KaxTnd0q6hayAlrID5fEQ)
+[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/open-unmix-a-reference-implementation-for/music-source-separation-on-musdb18)](https://paperswithcode.com/sota/music-source-separation-on-musdb18?p=open-unmix-a-reference-implementation-for)
+
+[![Build Status](https://github.com/sigsep/open-unmix-pytorch/workflows/CI/badge.svg)](https://github.com/sigsep/open-unmix-pytorch/actions?query=workflow%3ACI+branch%3Amaster+event%3Apush)
+[![Latest Version](https://img.shields.io/pypi/v/openunmix.svg)](https://pypi.python.org/pypi/openunmix)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/openunmix.svg)](https://pypi.python.org/pypi/openunmix)
+
+This repository contains the PyTorch (1.8+) implementation of __Open-Unmix__, a deep neural network reference implementation for music source separation, applicable for researchers, audio engineers and artists. __Open-Unmix__ provides ready-to-use models that allow users to separate pop music into four stems: __vocals__, __drums__, __bass__ and the remaining __other__ instruments. The models were pre-trained on the freely available [MUSDB18](https://sigsep.github.io/datasets/musdb.html) dataset. See details at [apply pre-trained model](#getting-started).
+
+## ⭐️ News 
+
+- 03/07/2021: We added `umxl`, a model that was trained on extra data which significantly improves the performance, especially generalization.
+- 14/02/2021: We released the new version of open-unmix as a python package. This comes with: a fully differentiable version of [norbert](https://github.com/sigsep/norbert), improved audio loading pipeline and large number of bug fixes. See [release notes](https://github.com/sigsep/open-unmix-pytorch/releases/) for further info.
+
+- 06/05/2020: We added a pre-trained speech enhancement model `umxse` provided by Sony.
+
+- 13/03/2020: Open-unmix was awarded 2nd place in the [PyTorch Global Summer Hackathon 2020](https://devpost.com/software/open-unmix).
+
+__Related Projects:__ open-unmix-pytorch | [open-unmix-nnabla](https://github.com/sigsep/open-unmix-nnabla) | [musdb](https://github.com/sigsep/sigsep-mus-db) | [museval](https://github.com/sigsep/sigsep-mus-eval) | [norbert](https://github.com/sigsep/norbert)
+
+## 🧠 The Model (for one source)
+
+![](https://docs.google.com/drawings/d/e/2PACX-1vTPoQiPwmdfET4pZhue1RvG7oEUJz7eUeQvCu6vzYeKRwHl6by4RRTnphImSKM0k5KXw9rZ1iIFnpGW/pub?w=959&h=308)
+
+To perform separation into multiple sources, _Open-unmix_ comprises multiple models that are trained for each particular target. While this makes the training less comfortable, it allows great flexibility to customize the training data for each target source.
+
+Each _Open-Unmix_ source model is based on a three-layer bidirectional deep LSTM. The model learns to predict the magnitude spectrogram of a target source, like _vocals_, from the magnitude spectrogram of a mixture input. Internally, the prediction is obtained by applying a mask on the input. The model is optimized in the magnitude domain using mean squared error.
+
+### Input Stage
+
+__Open-Unmix__ operates in the time-frequency domain to perform its prediction. The input of the model is either:
+
+* __`models.Separator`:__ A time domain signal tensor of shape `(nb_samples, nb_channels, nb_timesteps)`, where `nb_samples` are the samples in a batch, `nb_channels` is 1 or 2 for mono or stereo audio, respectively, and `nb_timesteps` is the number of audio samples in the recording. In this case, the model computes STFTs with either `torch` or `asteroid_filteranks` on the fly.
+
+* __`models.OpenUnmix`:__ The core open-unmix takes **magnitude spectrograms** directly (e.g. when pre-computed and loaded from disk). In that case, the input is of shape `(nb_frames, nb_samples, nb_channels, nb_bins)`, where `nb_frames` and `nb_bins` are the time and frequency-dimensions of a Short-Time-Fourier-Transform.
+
+The input spectrogram is _standardized_ using the global mean and standard deviation for every frequency bin across all frames. Furthermore, we apply batch normalization in multiple stages of the model to make the training more robust against gain variation.
+
+### Dimensionality reduction
+
+The LSTM is not operating on the original input spectrogram resolution. Instead, in the first step after the normalization, the network learns to compresses the frequency and channel axis of the model to reduce redundancy and make the model converge faster.
+
+### Bidirectional-LSTM
+
+The core of __open-unmix__ is a three layer bidirectional [LSTM network](https://dl.acm.org/citation.cfm?id=1246450). Due to its recurrent nature, the model can be trained and evaluated on arbitrary length of audio signals. Since the model takes information from past and future simultaneously, the model cannot be used in an online/real-time manner.
+An uni-directional model can easily be trained as described [here](docs/training.md).
+
+### Output Stage
+
+After applying the LSTM, the signal is decoded back to its original input dimensionality. In the last steps the output is multiplied with the input magnitude spectrogram, so that the models is asked to learn a mask.
+
+## 🤹‍♀️ Putting source models together: the `Separator`
+
+`models.Separator` puts together _Open-unmix_ spectrogram model for each desired target, and combines their output through a multichannel generalized Wiener filter, before application of inverse STFTs using `torchaudio`.
+The filtering is differentiable (but parameter-free) version of [norbert](https://github.com/sigsep/norbert). The separator is currently currently only used during inference.
+
+## 🏁 Getting started
+
+### Installation
+
+`openunmix` can be installed from pypi using:
+
+```
+pip install openunmix
+```
+
+Note, that the pypi version of openunmix uses [torchaudio] to load and save audio files. To increase the number of supported input and output file formats (such as STEMS export), please additionally install [stempeg](https://github.com/faroit/stempeg).
+
+Training is not part of the open-unmix package, please follow [docs/train.md] for more information.
+
+#### Using Docker
+
+We also provide a docker container. Performing separation of a local track in `~/Music/track1.wav` can be performed in a single line:
+
+```
+docker run -v ~/Music/:/data -it faroit/open-unmix-pytorch "/data/track1.wav" --outdir /data/track1
+```
+
+### Pre-trained models
+
+We provide three core pre-trained music separation models. All three models are end-to-end models that take waveform inputs and output the separated waveforms.
+
+* __`umxl` (default)__  trained on private stems dataset of compressed stems. __Note, that the weights are only licensed for non-commercial use (CC BY-NC-SA 4.0).__
+
+  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5069601.svg)](https://doi.org/10.5281/zenodo.5069601)
+
+* __`umxhq`__  trained on [MUSDB18-HQ](https://sigsep.github.io/datasets/musdb.html#uncompressed-wav) which comprises the same tracks as in MUSDB18 but un-compressed which yield in a full bandwidth of 22050 Hz.
+
+  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3370489.svg)](https://doi.org/10.5281/zenodo.3370489)
+
+* __`umx`__ is trained on the regular [MUSDB18](https://sigsep.github.io/datasets/musdb.html#compressed-stems) which is bandwidth limited to 16 kHz do to AAC compression. This model should be used for comparison with other (older) methods for evaluation in [SiSEC18](sisec18.unmix.app).
+
+  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3370486.svg)](https://doi.org/10.5281/zenodo.3370486)
+
+Furthermore, we provide a model for speech enhancement trained by [Sony Corporation](link)
+
+* __`umxse`__ speech enhancement model is trained on the 28-speaker version of the [Voicebank+DEMAND corpus](https://datashare.is.ed.ac.uk/handle/10283/1942?show=full).
+
+  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3786908.svg)](https://doi.org/10.5281/zenodo.3786908)
+
+All four models are also available as spectrogram (core) models, which take magnitude spectrogram inputs and ouput separated spectrograms.
+These models can be loaded using `umxl_spec`, `umxhq_spec`, `umx_spec` and `umxse_spec`.
+
+To separate audio files (`wav`, `flac`, `ogg` - but not `mp3`) files just run:
+
+```bash
+umx input_file.wav
+```
+
+A more detailed list of the parameters used for the separation is given in the [inference.md](/docs/inference.md) document.
+
+We provide a [jupyter notebook on google colab](https://colab.research.google.com/drive/1mijF0zGWxN-KaxTnd0q6hayAlrID5fEQ) to experiment with open-unmix and to separate files online without any installation setup.
+
+### Using pre-trained models from within python
+
+We implementes several ways to load pre-trained models and use them from within your python projects:
+#### When the package is installed
+
+Loading a pre-trained models is as simple as loading
+
+```python
+separator = openunmix.umxl(...)
+```
+#### torch.hub
+
+We also provide a torch.hub compatible modules that can be loaded. Note that this does _not_ even require to install the open-unmix packagen and should generally work when the pytorch version is the same.
+
+```python
+separator = torch.hub.load('sigsep/open-unmix-pytorch', 'umxl, device=device)
+```
+
+Where, `umxl` specifies the pre-trained model. 
+#### Performing separation
+
+With a created separator object, one can perform separation of some `audio` (torch.Tensor of shape `(channels, length)`, provided as at a sampling rate `separator.sample_rate`) through:
+
+```python
+estimates = separator(audio, ...)
+# returns estimates as tensor
+```
+
+Note that this requires the audio to be in the right shape and sampling rate. For convenience we provide a pre-processing in `openunmix.utils.preprocess(..`)` that takes numpy audio and converts it to be used for open-unmix.
+
+#### One-liner
+
+To perform model loading, preprocessing and separation in one step, just use:
+
+```python
+from openunmix.predict import separate
+estimates = separate(audio, ...)
+```
+
+### Load user-trained models
+
+When a path instead of a model-name is provided to `--model`, pre-trained `Separator` will be loaded from disk.
+E.g. The following files are assumed to present when loading `--model mymodel --targets vocals`
+
+* `mymodel/separator.json`
+* `mymodel/vocals.pth`
+* `mymodel/vocals.json`
+
+
+Note that the separator usually joins multiple models for each target and performs separation using all models. E.g. if the separator contains `vocals` and `drums` models, two output files are generated, unless the `--residual` option is selected, in which case an additional source will be produced, containing an estimate of all that is not the targets in the mixtures.
+
+### Evaluation using `museval`
+
+To perform evaluation in comparison to other SISEC systems, you would need to install the `museval` package using
+
+```
+pip install museval
+```
+
+and then run the evaluation using
+
+`python -m openunmix.evaluate --outdir /path/to/musdb/estimates --evaldir /path/to/museval/results`
+
+### Results compared to SiSEC 2018 (SDR/Vocals)
+
+Open-Unmix yields state-of-the-art results compared to participants from [SiSEC 2018](https://sisec18.unmix.app/#/methods). The performance of `UMXHQ` and `UMX` is almost identical since it was evaluated on compressed STEMS.
+
+![boxplot_updated](https://user-images.githubusercontent.com/72940/63944652-3f624c80-ca72-11e9-8d33-bed701679fe6.png)
+
+Note that
+
+1. [`STL1`, `TAK2`, `TAK3`, `TAU1`, `UHL3`, `UMXHQ`] were omitted as they were _not_ trained on only _MUSDB18_.
+2. [`HEL1`, `TAK1`, `UHL1`, `UHL2`] are not open-source.
+
+#### Scores (Median of frames, Median of tracks)
+
+|target|SDR  | SDR |  SDR |
+|------|-----|-----|-----|
+|`model`|UMX  |UMXHQ|UMXL |
+|vocals|6.32 | 6.25|__7.21__ |
+|bass  |5.23 | 5.07|__6.02__ |
+|drums |5.73 | 6.04|__7.15__ |
+|other |4.02 | 4.28|__4.89__ |
+
+## Training
+
+Details on the training is provided in a separate document [here](docs/training.md).
+
+## Extensions
+
+Details on how _open-unmix_ can be extended or improved for future research on music separation is described in a separate document [here](docs/extensions.md).
+
+
+## Design Choices
+
+we favored simplicity over performance to promote clearness of the code. The rationale is to have __open-unmix__ serve as a __baseline__ for future research while performance still meets current state-of-the-art (See [Evaluation](#Evaluation)). The results are comparable/better to those of `UHL1`/`UHL2` which obtained the best performance over all systems trained on MUSDB18 in the [SiSEC 2018 Evaluation campaign](https://sisec18.unmix.app).
+We designed the code to allow researchers to reproduce existing results, quickly develop new architectures and add own user data for training and testing. We favored framework specifics implementations instead of having a monolithic repository with common code for all frameworks.
+
+## How to contribute
+
+_open-unmix_ is a community focused project, we therefore encourage the community to submit bug-fixes and requests for technical support through [github issues](https://github.com/sigsep/open-unmix-pytorch/issues/new/choose). For more details of how to contribute, please follow our [`CONTRIBUTING.md`](CONTRIBUTING.md). For help and support, please use the gitter chat or the google groups forums. 
+
+### Authors
+
+[Fabian-Robert Stöter](https://www.faroit.com/), [Antoine Liutkus](https://github.com/aliutkus), Inria and LIRMM, Montpellier, France
+
+## References
+
+<details><summary>If you use open-unmix for your research – Cite Open-Unmix</summary>
+
+```latex
+@article{stoter19,  
+  author={F.-R. St\\"oter and S. Uhlich and A. Liutkus and Y. Mitsufuji},  
+  title={Open-Unmix - A Reference Implementation for Music Source Separation},  
+  journal={Journal of Open Source Software},  
+  year=2019,
+  doi = {10.21105/joss.01667},
+  url = {https://doi.org/10.21105/joss.01667}
+}
+```
+
+</p>
+</details>
+
+<details><summary>If you use the MUSDB dataset for your research - Cite the MUSDB18 Dataset</summary>
+<p>
+
+```latex
+@misc{MUSDB18,
+  author       = {Rafii, Zafar and
+                  Liutkus, Antoine and
+                  Fabian-Robert St{\"o}ter and
+                  Mimilakis, Stylianos Ioannis and
+                  Bittner, Rachel},
+  title        = {The {MUSDB18} corpus for music separation},
+  month        = dec,
+  year         = 2017,
+  doi          = {10.5281/zenodo.1117372},
+  url          = {https://doi.org/10.5281/zenodo.1117372}
+}
+```
+
+</p>
+</details>
+
+
+<details><summary>If compare your results with SiSEC 2018 Participants - Cite the SiSEC 2018 LVA/ICA Paper</summary>
+<p>
+
+```latex
+@inproceedings{SiSEC18,
+  author="St{\"o}ter, Fabian-Robert and Liutkus, Antoine and Ito, Nobutaka",
+  title="The 2018 Signal Separation Evaluation Campaign",
+  booktitle="Latent Variable Analysis and Signal Separation:
+  14th International Conference, LVA/ICA 2018, Surrey, UK",
+  year="2018",
+  pages="293--305"
+}
+```
+
+</p>
+</details>
+
+⚠️ Please note that the official acronym for _open-unmix_ is **UMX**.
+
+### License
+
+MIT
+
+### Acknowledgements
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/sigsep/website/master/content/open-unmix/logo_INRIA.svg?sanitize=true" width="200" title="inria">
+  <img src="https://raw.githubusercontent.com/sigsep/website/master/content/open-unmix/anr.jpg" width="100" alt="anr">
+</p>
```

### Comparing `openunmix-1.2.1/README.md` & `openunmix-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -145,16 +145,16 @@
 Note that this requires the audio to be in the right shape and sampling rate. For convenience we provide a pre-processing in `openunmix.utils.preprocess(..`)` that takes numpy audio and converts it to be used for open-unmix.
 
 #### One-liner
 
 To perform model loading, preprocessing and separation in one step, just use:
 
 ```python
-from openunmix import separate
-estimates = separate.predict(audio, ...)
+from openunmix.predict import separate
+estimates = separate(audio, ...)
 ```
 
 ### Load user-trained models
 
 When a path instead of a model-name is provided to `--model`, pre-trained `Separator` will be loaded from disk.
 E.g. The following files are assumed to present when loading `--model mymodel --targets vocals`
```

### Comparing `openunmix-1.2.1/openunmix/__init__.py` & `openunmix-1.3.0/openunmix/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,50 @@
 """
 ![sigsep logo](https://sigsep.github.io/hero.png)
 Open-Unmix is a deep neural network reference implementation for music source separation, applicable for researchers, audio engineers and artists. Open-Unmix provides ready-to-use models that allow users to separate pop music into four stems: vocals, drums, bass and the remaining other instruments. The models were pre-trained on the MUSDB18 dataset. See details at apply pre-trained model.
 
 This is the python package API documentation. 
 Please checkout [the open-unmix website](https://sigsep.github.io/open-unmix) for more information.
 """
+
 from openunmix import utils
 import torch.hub
 
 
 def umxse_spec(targets=None, device="cpu", pretrained=True):
     target_urls = {
-        "speech": "https://zenodo.org/api/files/765b45a3-c70d-48a6-936b-09a7989c349a/speech_f5e0d9f9.pth",
-        "noise": "https://zenodo.org/api/files/765b45a3-c70d-48a6-936b-09a7989c349a/noise_04a6fc2d.pth",
+        "speech": "https://zenodo.org/records/3786908/files/speech_f5e0d9f9.pth",
+        "noise": "https://zenodo.org/records/3786908/files/noise_04a6fc2d.pth",
     }
 
     from .model import OpenUnmix
 
     if targets is None:
         targets = ["speech", "noise"]
 
     # determine the maximum bin count for a 16khz bandwidth model
     max_bin = utils.bandwidth_to_max_bin(rate=16000.0, n_fft=1024, bandwidth=16000)
 
     # load open unmix models speech enhancement models
     target_models = {}
     for target in targets:
-        target_unmix = OpenUnmix(
-            nb_bins=1024 // 2 + 1, nb_channels=1, hidden_size=256, max_bin=max_bin
-        )
+        target_unmix = OpenUnmix(nb_bins=1024 // 2 + 1, nb_channels=1, hidden_size=256, max_bin=max_bin)
 
         # enable centering of stft to minimize reconstruction error
         if pretrained:
-            state_dict = torch.hub.load_state_dict_from_url(
-                target_urls[target], map_location=device
-            )
+            state_dict = torch.hub.load_state_dict_from_url(target_urls[target], map_location=device)
             target_unmix.load_state_dict(state_dict, strict=False)
             target_unmix.eval()
 
         target_unmix.to(device)
         target_models[target] = target_unmix
     return target_models
 
 
-def umxse(
-    targets=None,
-    residual=False,
-    niter=1,
-    device="cpu",
-    pretrained=True,
-    filterbank="torch",
-):
+def umxse(targets=None, residual=False, niter=1, device="cpu", pretrained=True, filterbank="torch", wiener_win_len=300):
     """
     Open Unmix Speech Enhancemennt 1-channel BiLSTM Model
     trained on the 28-speaker version of Voicebank+Demand
     (Sampling rate: 16kHz)
 
     Args:
         targets (str): select the targets for the source to be separated.
@@ -62,14 +52,20 @@
                 If you don't pick them all, you probably want to
                 activate the `residual=True` option.
                 Defaults to all available targets per model.
         pretrained (bool): If True, returns a model pre-trained on MUSDB18-HQ
         residual (bool): if True, a "garbage" target is created
         niter (int): the number of post-processingiterations, defaults to 0
         device (str): selects device to be used for inference
+        wiener_win_len (int or None): The size of the excerpts
+            (number of frames) on which to apply filtering
+            independently. This means assuming time varying stereo models and
+            localization of sources.
+            None means not batching but using the whole signal. It comes at the
+            price of a much larger memory usage.
         filterbank (str): filterbank implementation method.
             Supported are `['torch', 'asteroid']`. `torch` is about 30% faster
             compared to `asteroid` on large FFT sizes such as 4096. However,
             asteroids stft can be exported to onnx, which makes is practical
             for deployment.
 
     Reference:
@@ -85,63 +81,61 @@
         target_models=target_models,
         niter=niter,
         residual=residual,
         n_fft=1024,
         n_hop=512,
         nb_channels=1,
         sample_rate=16000.0,
+        wiener_win_len=wiener_win_len,
         filterbank=filterbank,
     ).to(device)
 
     return separator
 
 
 def umxhq_spec(targets=None, device="cpu", pretrained=True):
     from .model import OpenUnmix
 
     # set urls for weights
     target_urls = {
-        "bass": "https://zenodo.org/api/files/1c8f83c5-33a5-4f59-b109-721fdd234875/bass-8d85a5bd.pth",
-        "drums": "https://zenodo.org/api/files/1c8f83c5-33a5-4f59-b109-721fdd234875/drums-9619578f.pth",
-        "other": "https://zenodo.org/api/files/1c8f83c5-33a5-4f59-b109-721fdd234875/other-b52fbbf7.pth",
-        "vocals": "https://zenodo.org/api/files/1c8f83c5-33a5-4f59-b109-721fdd234875/vocals-b62c91ce.pth",
+        "bass": "https://zenodo.org/records/3370489/files/bass-8d85a5bd.pth",
+        "drums": "https://zenodo.org/records/3370489/files/drums-9619578f.pth",
+        "other": "https://zenodo.org/records/3370489/files/other-b52fbbf7.pth",
+        "vocals": "https://zenodo.org/records/3370489/files/vocals-b62c91ce.pth",
     }
 
     if targets is None:
         targets = ["vocals", "drums", "bass", "other"]
 
     # determine the maximum bin count for a 16khz bandwidth model
     max_bin = utils.bandwidth_to_max_bin(rate=44100.0, n_fft=4096, bandwidth=16000)
 
     target_models = {}
     for target in targets:
         # load open unmix model
-        target_unmix = OpenUnmix(
-            nb_bins=4096 // 2 + 1, nb_channels=2, hidden_size=512, max_bin=max_bin
-        )
+        target_unmix = OpenUnmix(nb_bins=4096 // 2 + 1, nb_channels=2, hidden_size=512, max_bin=max_bin)
 
         # enable centering of stft to minimize reconstruction error
         if pretrained:
-            state_dict = torch.hub.load_state_dict_from_url(
-                target_urls[target], map_location=device
-            )
+            state_dict = torch.hub.load_state_dict_from_url(target_urls[target], map_location=device)
             target_unmix.load_state_dict(state_dict, strict=False)
             target_unmix.eval()
 
         target_unmix.to(device)
         target_models[target] = target_unmix
     return target_models
 
 
 def umxhq(
     targets=None,
     residual=False,
     niter=1,
     device="cpu",
     pretrained=True,
+    wiener_win_len=300,
     filterbank="torch",
 ):
     """
     Open Unmix 2-channel/stereo BiLSTM Model trained on MUSDB18-HQ
 
     Args:
         targets (str): select the targets for the source to be separated.
@@ -149,14 +143,20 @@
                 If you don't pick them all, you probably want to
                 activate the `residual=True` option.
                 Defaults to all available targets per model.
         pretrained (bool): If True, returns a model pre-trained on MUSDB18-HQ
         residual (bool): if True, a "garbage" target is created
         niter (int): the number of post-processingiterations, defaults to 0
         device (str): selects device to be used for inference
+        wiener_win_len (int or None): The size of the excerpts
+            (number of frames) on which to apply filtering
+            independently. This means assuming time varying stereo models and
+            localization of sources.
+            None means not batching but using the whole signal. It comes at the
+            price of a much larger memory usage.
         filterbank (str): filterbank implementation method.
             Supported are `['torch', 'asteroid']`. `torch` is about 30% faster
             compared to `asteroid` on large FFT sizes such as 4096. However,
             asteroids stft can be exported to onnx, which makes is practical
             for deployment.
     """
 
@@ -168,63 +168,61 @@
         target_models=target_models,
         niter=niter,
         residual=residual,
         n_fft=4096,
         n_hop=1024,
         nb_channels=2,
         sample_rate=44100.0,
+        wiener_win_len=wiener_win_len,
         filterbank=filterbank,
     ).to(device)
 
     return separator
 
 
 def umx_spec(targets=None, device="cpu", pretrained=True):
     from .model import OpenUnmix
 
     # set urls for weights
     target_urls = {
-        "bass": "https://zenodo.org/api/files/d6105b95-8c52-430c-84ce-bd14b803faaf/bass-646024d3.pth",
-        "drums": "https://zenodo.org/api/files/d6105b95-8c52-430c-84ce-bd14b803faaf/drums-5a48008b.pth",
-        "other": "https://zenodo.org/api/files/d6105b95-8c52-430c-84ce-bd14b803faaf/other-f8e132cc.pth",
-        "vocals": "https://zenodo.org/api/files/d6105b95-8c52-430c-84ce-bd14b803faaf/vocals-c8df74a5.pth",
+        "bass": "https://zenodo.org/records/3370486/files/bass-646024d3.pth",
+        "drums": "https://zenodo.org/records/3370486/files/drums-5a48008b.pth",
+        "other": "https://zenodo.org/records/3370486/files/other-f8e132cc.pth",
+        "vocals": "https://zenodo.org/records/3370486/files/vocals-c8df74a5.pth",
     }
 
     if targets is None:
         targets = ["vocals", "drums", "bass", "other"]
 
     # determine the maximum bin count for a 16khz bandwidth model
     max_bin = utils.bandwidth_to_max_bin(rate=44100.0, n_fft=4096, bandwidth=16000)
 
     target_models = {}
     for target in targets:
         # load open unmix model
-        target_unmix = OpenUnmix(
-            nb_bins=4096 // 2 + 1, nb_channels=2, hidden_size=512, max_bin=max_bin
-        )
+        target_unmix = OpenUnmix(nb_bins=4096 // 2 + 1, nb_channels=2, hidden_size=512, max_bin=max_bin)
 
         # enable centering of stft to minimize reconstruction error
         if pretrained:
-            state_dict = torch.hub.load_state_dict_from_url(
-                target_urls[target], map_location=device
-            )
+            state_dict = torch.hub.load_state_dict_from_url(target_urls[target], map_location=device)
             target_unmix.load_state_dict(state_dict, strict=False)
             target_unmix.eval()
 
         target_unmix.to(device)
         target_models[target] = target_unmix
     return target_models
 
 
 def umx(
     targets=None,
     residual=False,
     niter=1,
     device="cpu",
     pretrained=True,
+    wiener_win_len=300,
     filterbank="torch",
 ):
     """
     Open Unmix 2-channel/stereo BiLSTM Model trained on MUSDB18
 
     Args:
         targets (str): select the targets for the source to be separated.
@@ -232,14 +230,20 @@
                 If you don't pick them all, you probably want to
                 activate the `residual=True` option.
                 Defaults to all available targets per model.
         pretrained (bool): If True, returns a model pre-trained on MUSDB18-HQ
         residual (bool): if True, a "garbage" target is created
         niter (int): the number of post-processingiterations, defaults to 0
         device (str): selects device to be used for inference
+        wiener_win_len (int or None): The size of the excerpts
+            (number of frames) on which to apply filtering
+            independently. This means assuming time varying stereo models and
+            localization of sources.
+            None means not batching but using the whole signal. It comes at the
+            price of a much larger memory usage.
         filterbank (str): filterbank implementation method.
             Supported are `['torch', 'asteroid']`. `torch` is about 30% faster
             compared to `asteroid` on large FFT sizes such as 4096. However,
             asteroids stft can be exported to onnx, which makes is practical
             for deployment.
 
     """
@@ -251,63 +255,61 @@
         target_models=target_models,
         niter=niter,
         residual=residual,
         n_fft=4096,
         n_hop=1024,
         nb_channels=2,
         sample_rate=44100.0,
+        wiener_win_len=wiener_win_len,
         filterbank=filterbank,
     ).to(device)
 
     return separator
 
 
 def umxl_spec(targets=None, device="cpu", pretrained=True):
     from .model import OpenUnmix
 
     # set urls for weights
     target_urls = {
-        "bass": "https://zenodo.org/api/files/f8209c3e-ba60-48cf-8e79-71ae65beca61/bass-2ca1ce51.pth",
-        "drums": "https://zenodo.org/api/files/f8209c3e-ba60-48cf-8e79-71ae65beca61/drums-69e0ebd4.pth",
-        "other": "https://zenodo.org/api/files/f8209c3e-ba60-48cf-8e79-71ae65beca61/other-c8c5b3e6.pth",
-        "vocals": "https://zenodo.org/api/files/f8209c3e-ba60-48cf-8e79-71ae65beca61/vocals-bccbd9aa.pth",
+        "bass": "https://zenodo.org/records/5069601/files/bass-2ca1ce51.pth",
+        "drums": "https://zenodo.org/records/5069601/files/drums-69e0ebd4.pth",
+        "other": "https://zenodo.org/records/5069601/files/other-c8c5b3e6.pth",
+        "vocals": "https://zenodo.org/records/5069601/files/vocals-bccbd9aa.pth",
     }
 
     if targets is None:
         targets = ["vocals", "drums", "bass", "other"]
 
     # determine the maximum bin count for a 16khz bandwidth model
     max_bin = utils.bandwidth_to_max_bin(rate=44100.0, n_fft=4096, bandwidth=16000)
 
     target_models = {}
     for target in targets:
         # load open unmix model
-        target_unmix = OpenUnmix(
-            nb_bins=4096 // 2 + 1, nb_channels=2, hidden_size=1024, max_bin=max_bin
-        )
+        target_unmix = OpenUnmix(nb_bins=4096 // 2 + 1, nb_channels=2, hidden_size=1024, max_bin=max_bin)
 
         # enable centering of stft to minimize reconstruction error
         if pretrained:
-            state_dict = torch.hub.load_state_dict_from_url(
-                target_urls[target], map_location=device
-            )
+            state_dict = torch.hub.load_state_dict_from_url(target_urls[target], map_location=device)
             target_unmix.load_state_dict(state_dict, strict=False)
             target_unmix.eval()
 
         target_unmix.to(device)
         target_models[target] = target_unmix
     return target_models
 
 
 def umxl(
     targets=None,
     residual=False,
     niter=1,
     device="cpu",
     pretrained=True,
+    wiener_win_len=300,
     filterbank="torch",
 ):
     """
     Open Unmix Extra (UMX-L), 2-channel/stereo BLSTM Model trained on a private dataset
     of ~400h of multi-track audio.
 
 
@@ -317,14 +319,20 @@
                 If you don't pick them all, you probably want to
                 activate the `residual=True` option.
                 Defaults to all available targets per model.
         pretrained (bool): If True, returns a model pre-trained on MUSDB18-HQ
         residual (bool): if True, a "garbage" target is created
         niter (int): the number of post-processingiterations, defaults to 0
         device (str): selects device to be used for inference
+        wiener_win_len (int or None): The size of the excerpts
+            (number of frames) on which to apply filtering
+            independently. This means assuming time varying stereo models and
+            localization of sources.
+            None means not batching but using the whole signal. It comes at the
+            price of a much larger memory usage.
         filterbank (str): filterbank implementation method.
             Supported are `['torch', 'asteroid']`. `torch` is about 30% faster
             compared to `asteroid` on large FFT sizes such as 4096. However,
             asteroids stft can be exported to onnx, which makes is practical
             for deployment.
 
     """
@@ -336,11 +344,12 @@
         target_models=target_models,
         niter=niter,
         residual=residual,
         n_fft=4096,
         n_hop=1024,
         nb_channels=2,
         sample_rate=44100.0,
+        wiener_win_len=wiener_win_len,
         filterbank=filterbank,
     ).to(device)
 
     return separator
```

### Comparing `openunmix-1.2.1/openunmix/cli.py` & `openunmix-1.3.0/openunmix/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,15 @@
 
     parser.add_argument(
         "--duration",
         type=float,
         help="Audio chunk duration in seconds, negative values load full track",
     )
 
-    parser.add_argument(
-        "--no-cuda", action="store_true", default=False, help="disables CUDA inference"
-    )
+    parser.add_argument("--no-cuda", action="store_true", default=False, help="disables CUDA inference")
 
     parser.add_argument(
         "--audio-backend",
         type=str,
         help="Sets audio backend. Default to torchaudio's default backend: See https://pytorch.org/audio/stable/backend.html"
         "(`sox_io`, `sox`, `soundfile` or `stempeg`)",
     )
@@ -82,16 +80,15 @@
         help="Number of frames on which to apply filtering independently",
     )
 
     parser.add_argument(
         "--residual",
         type=str,
         default=None,
-        help="if provided, build a source with given name"
-        "for the mix minus all estimated targets",
+        help="if provided, build a source with given name " "for the mix minus all estimated targets",
     )
 
     parser.add_argument(
         "--aggregate",
         type=str,
         default=None,
         help="if provided, must be a string containing a valid expression for "
@@ -102,17 +99,17 @@
     )
 
     parser.add_argument(
         "--filterbank",
         type=str,
         default="torch",
         help="filterbank implementation method. "
-        "Supported: `['torch', 'asteroid']`. `torch` is ~30% faster"
-        "compared to `asteroid` on large FFT sizes such as 4096. However"
-        "asteroids stft can be exported to onnx, which makes is practical"
+        "Supported: `['torch', 'asteroid']`. `torch` is ~30%% faster "
+        "compared to `asteroid` on large FFT sizes such as 4096. However "
+        "asteroids stft can be exported to onnx, which makes is practical "
         "for deployment.",
     )
     parser.add_argument(
         "--verbose",
         action="store_true",
         default=False,
         help="Enable log messages",
```

### Comparing `openunmix-1.2.1/openunmix/data.py` & `openunmix-1.3.0/openunmix/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,17 +165,15 @@
         dataset_kwargs = {
             "root": Path(args.root),
             "seq_duration": args.seq_dur,
             "input_file": args.input_file,
             "output_file": args.output_file,
         }
         args.target = Path(args.output_file).stem
-        train_dataset = AlignedDataset(
-            split="train", random_chunks=True, **dataset_kwargs
-        )  # type: UnmixDataset
+        train_dataset = AlignedDataset(split="train", random_chunks=True, **dataset_kwargs)  # type: UnmixDataset
         valid_dataset = AlignedDataset(split="valid", **dataset_kwargs)  # type: UnmixDataset
 
     elif args.dataset == "sourcefolder":
         parser.add_argument("--interferer-dirs", type=str, nargs="+")
         parser.add_argument("--target-dir", type=str)
         parser.add_argument("--ext", type=str, default=".wav")
         parser.add_argument("--nb-train-samples", type=int, default=1000)
@@ -236,17 +234,15 @@
             split="train",
             source_augmentations=source_augmentations,
             random_track_mix=args.random_track_mix,
             random_chunks=True,
             seq_duration=args.seq_dur,
             **dataset_kwargs,
         )
-        valid_dataset = FixedSourcesTrackFolderDataset(
-            split="valid", seq_duration=None, **dataset_kwargs
-        )
+        valid_dataset = FixedSourcesTrackFolderDataset(split="valid", seq_duration=None, **dataset_kwargs)
 
     elif args.dataset == "trackfolder_var":
         parser.add_argument("--ext", type=str, default=".wav")
         parser.add_argument("--target-file", type=str)
         parser.add_argument("--source-augmentations", type=str, nargs="+")
         parser.add_argument(
             "--random-interferer-mix",
@@ -267,41 +263,35 @@
         dataset_kwargs = {
             "root": Path(args.root),
             "target_file": args.target_file,
             "ext": args.ext,
             "silence_missing_targets": args.silence_missing,
         }
 
-        source_augmentations = Compose(
-            [globals()["_augment_" + aug] for aug in args.source_augmentations]
-        )
+        source_augmentations = Compose([globals()["_augment_" + aug] for aug in args.source_augmentations])
 
         train_dataset = VariableSourcesTrackFolderDataset(
             split="train",
             source_augmentations=source_augmentations,
             random_interferer_mix=args.random_interferer_mix,
             random_chunks=True,
             seq_duration=args.seq_dur,
             **dataset_kwargs,
         )
-        valid_dataset = VariableSourcesTrackFolderDataset(
-            split="valid", seq_duration=None, **dataset_kwargs
-        )
+        valid_dataset = VariableSourcesTrackFolderDataset(split="valid", seq_duration=None, **dataset_kwargs)
 
     else:
         parser.add_argument(
             "--is-wav",
             action="store_true",
             default=False,
             help="loads wav instead of STEMS",
         )
         parser.add_argument("--samples-per-track", type=int, default=64)
-        parser.add_argument(
-            "--source-augmentations", type=str, default=["gain", "channelswap"], nargs="+"
-        )
+        parser.add_argument("--source-augmentations", type=str, default=["gain", "channelswap"], nargs="+")
 
         args = parser.parse_args()
         dataset_kwargs = {
             "root": args.root,
             "is_wav": args.is_wav,
             "subsets": "train",
             "target": args.target,
@@ -316,17 +306,15 @@
             samples_per_track=args.samples_per_track,
             seq_duration=args.seq_dur,
             source_augmentations=source_augmentations,
             random_track_mix=True,
             **dataset_kwargs,
         )
 
-        valid_dataset = MUSDBDataset(
-            split="valid", samples_per_track=1, seq_duration=None, **dataset_kwargs
-        )
+        valid_dataset = MUSDBDataset(split="valid", samples_per_track=1, seq_duration=None, **dataset_kwargs)
 
     return train_dataset, valid_dataset, args
 
 
 class AlignedDataset(UnmixDataset):
     def __init__(
         self,
@@ -582,17 +570,15 @@
             start = random.uniform(0, min_duration - self.seq_duration)
         else:
             start = 0
 
         # assemble the mixture of target and interferers
         audio_sources = []
         # load target
-        target_audio, _ = load_audio(
-            track_path / self.target_file, start=start, dur=self.seq_duration
-        )
+        target_audio, _ = load_audio(track_path / self.target_file, start=start, dur=self.seq_duration)
         target_audio = self.source_augmentations(target_audio)
         audio_sources.append(target_audio)
         # load interferers
         for source in self.interferer_files:
             # optionally select a random track for each source
             if self.random_track_mix:
                 random_idx = random.choice(range(len(self.tracks)))
@@ -913,17 +899,15 @@
             "trackfolder_fix",
         ],
         help="Name of the dataset.",
     )
 
     parser.add_argument("--root", type=str, help="root path of dataset")
 
-    parser.add_argument(
-        "--save", action="store_true", help=("write out a fixed dataset of samples")
-    )
+    parser.add_argument("--save", action="store_true", help=("write out a fixed dataset of samples"))
 
     parser.add_argument("--target", type=str, default="vocals")
     parser.add_argument("--seed", type=int, default=42)
     parser.add_argument(
         "--audio-backend",
         type=str,
         default="soundfile",
```

### Comparing `openunmix-1.2.1/openunmix/evaluate.py` & `openunmix-1.3.0/openunmix/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,17 +86,15 @@
 
     parser.add_argument("--root", type=str, help="Path to MUSDB18")
 
     parser.add_argument("--subset", type=str, default="test", help="MUSDB subset (`train`/`test`)")
 
     parser.add_argument("--cores", type=int, default=1)
 
-    parser.add_argument(
-        "--no-cuda", action="store_true", default=False, help="disables CUDA inference"
-    )
+    parser.add_argument("--no-cuda", action="store_true", default=False, help="disables CUDA inference")
 
     parser.add_argument(
         "--is-wav",
         action="store_true",
         default=False,
         help="flags wav version of the dataset",
     )
@@ -115,16 +113,15 @@
         help="Number of frames on which to apply filtering independently",
     )
 
     parser.add_argument(
         "--residual",
         type=str,
         default=None,
-        help="if provided, build a source with given name"
-        "for the mix minus all estimated targets",
+        help="if provided, build a source with given name" "for the mix minus all estimated targets",
     )
 
     parser.add_argument(
         "--aggregate",
         type=str,
         default=None,
         help="if provided, must be a string containing a valid expression for "
```

### Comparing `openunmix-1.2.1/openunmix/filtering.py` & `openunmix-1.3.0/openunmix/filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,18 +256,15 @@
         dim=2,
     )
     regularization = torch.sqrt(torch.as_tensor(eps)) * (
         regularization[None, None, ...].expand((-1, nb_bins, -1, -1, -1))
     )
 
     # allocate the spatial covariance matrices
-    R = [
-        torch.zeros((nb_bins, nb_channels, nb_channels, 2), dtype=x.dtype, device=x.device)
-        for j in range(nb_sources)
-    ]
+    R = [torch.zeros((nb_bins, nb_channels, nb_channels, 2), dtype=x.dtype, device=x.device) for j in range(nb_sources)]
     weight: torch.Tensor = torch.zeros((nb_bins,), dtype=x.dtype, device=x.device)
 
     v: torch.Tensor = torch.zeros((nb_frames, nb_bins, nb_sources), dtype=x.dtype, device=x.device)
     for it in range(iterations):
         # constructing the mixture covariance matrix. Doing it with a loop
         # to avoid storing anytime in RAM the whole 6D tensor
 
@@ -430,27 +427,24 @@
         :func:`wiener`.
     """
     if softmask:
         # if we use softmask, we compute the ratio mask for all targets and
         # multiply by the mix stft
         y = (
             mix_stft[..., None]
-            * (
-                targets_spectrograms
-                / (eps + torch.sum(targets_spectrograms, dim=-1, keepdim=True).to(mix_stft.dtype))
-            )[..., None, :]
+            * (targets_spectrograms / (eps + torch.sum(targets_spectrograms, dim=-1, keepdim=True).to(mix_stft.dtype)))[
+                ..., None, :
+            ]
         )
     else:
         # otherwise, we just multiply the targets spectrograms with mix phase
         # we tacitly assume that we have magnitude estimates.
         angle = atan2(mix_stft[..., 1], mix_stft[..., 0])[..., None]
         nb_sources = targets_spectrograms.shape[-1]
-        y = torch.zeros(
-            mix_stft.shape + (nb_sources,), dtype=mix_stft.dtype, device=mix_stft.device
-        )
+        y = torch.zeros(mix_stft.shape + (nb_sources,), dtype=mix_stft.dtype, device=mix_stft.device)
         y[..., 0, :] = targets_spectrograms * torch.cos(angle)
         y[..., 1, :] = targets_spectrograms * torch.sin(angle)
 
     if residual:
         # if required, adding an additional target as the mix minus
         # available targets
         y = torch.cat([y, mix_stft[..., None] - y.sum(dim=-1, keepdim=True)], dim=-1)
```

### Comparing `openunmix-1.2.1/openunmix/model.py` & `openunmix-1.3.0/openunmix/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Optional
+from typing import Optional, Mapping
 
+import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn import LSTM, BatchNorm1d, Linear, Parameter
 from .filtering import wiener
 from .transforms import make_filterbanks, ComplexNorm
@@ -26,22 +27,22 @@
         max_bin (int or None): Internal frequency bin threshold to
             reduce high frequency content. Defaults to `None` which results
             in `nb_bins`
     """
 
     def __init__(
         self,
-        nb_bins=4096,
-        nb_channels=2,
-        hidden_size=512,
-        nb_layers=3,
-        unidirectional=False,
-        input_mean=None,
-        input_scale=None,
-        max_bin=None,
+        nb_bins: int = 4096,
+        nb_channels: int = 2,
+        hidden_size: int = 512,
+        nb_layers: int = 3,
+        unidirectional: bool = False,
+        input_mean: Optional[np.ndarray] = None,
+        input_scale: Optional[np.ndarray] = None,
+        max_bin: Optional[int] = None,
     ):
         super(OpenUnmix, self).__init__()
 
         self.nb_output_bins = nb_bins
         if max_bin:
             self.nb_bins = max_bin
         else:
@@ -191,15 +192,15 @@
             compared to `asteroid` on large FFT sizes such as 4096. However,
             asteroids stft can be exported to onnx, which makes is practical
             for deployment.
     """
 
     def __init__(
         self,
-        target_models: dict,
+        target_models: Mapping[str, nn.Module],
         niter: int = 0,
         softmask: bool = False,
         residual: bool = False,
         sample_rate: float = 44100.0,
         n_fft: int = 4096,
         n_hop: int = 1024,
         nb_channels: int = 2,
@@ -284,17 +285,15 @@
             raise Exception(
                 "Cannot use EM if only one target is estimated."
                 "Provide two targets or create an additional "
                 "one with `--residual`"
             )
 
         nb_frames = spectrograms.shape[1]
-        targets_stft = torch.zeros(
-            mix_stft.shape + (nb_sources,), dtype=audio.dtype, device=mix_stft.device
-        )
+        targets_stft = torch.zeros(mix_stft.shape + (nb_sources,), dtype=audio.dtype, device=mix_stft.device)
         for sample in range(nb_samples):
             pos = 0
             if self.wiener_win_len:
                 wiener_win_len = self.wiener_win_len
             else:
                 wiener_win_len = nb_frames
             while pos < nb_frames:
```

### Comparing `openunmix-1.2.1/openunmix/predict.py` & `openunmix-1.3.0/openunmix/predict.py`

 * *Files identical despite different names*

### Comparing `openunmix-1.2.1/openunmix/transforms.py` & `openunmix-1.3.0/openunmix/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,20 +65,27 @@
             zero padded. Centering is required for a perfect
             reconstruction of the signal. However, during training
             of spectrogram models, it can safely turned off.
             Defaults to `true`
         window (nn.Parameter, optional): window function
     """
 
-    def __init__(self, n_fft=4096, n_hop=1024, center=False, window=None):
+    def __init__(
+        self,
+        n_fft: int = 4096,
+        n_hop: int = 1024,
+        center: bool = False,
+        window: Optional[nn.Parameter] = None,
+    ):
         super(TorchSTFT, self).__init__()
-        if window is not None:
+        if window is None:
             self.window = nn.Parameter(torch.hann_window(n_fft), requires_grad=False)
         else:
             self.window = window
+
         self.n_fft = n_fft
         self.n_hop = n_hop
         self.center = center
 
     def forward(self, x: Tensor) -> Tensor:
         """STFT forward path
         Args:
@@ -145,15 +152,15 @@
         super(TorchISTFT, self).__init__()
 
         self.n_fft = n_fft
         self.n_hop = n_hop
         self.center = center
         self.sample_rate = sample_rate
 
-        if window is not None:
+        if window is None:
             self.window = nn.Parameter(torch.hann_window(n_fft), requires_grad=False)
         else:
             self.window = window
 
     def forward(self, X: Tensor, length: Optional[int] = None) -> Tensor:
         shape = X.size()
         X = X.reshape(-1, shape[-3], shape[-2], shape[-1])
```

### Comparing `openunmix-1.2.1/openunmix/utils.py` & `openunmix-1.3.0/openunmix/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             raise ValueError("mode " + mode + " is unknown!")
         if mode == "min":
             self.is_better = lambda a, best: a < best - min_delta
         if mode == "max":
             self.is_better = lambda a, best: a > best + min_delta
 
 
-def load_target_models(targets, model_str_or_path="umxhq", device="cpu", pretrained=True):
+def load_target_models(targets, model_str_or_path="umxl", device="cpu", pretrained=True):
     """Core model loader
 
     target model path can be either <target>.pth, or <target>-sha256.pth
     (as used on torchub)
 
     The loader either loads the models from a known model string
     as registered in the __init__.py or loads from custom configs.
@@ -158,15 +158,15 @@
                 models[target].load_state_dict(state, strict=False)
 
             models[target].to(device)
         return models
 
 
 def load_separator(
-    model_str_or_path: str = "umxhq",
+    model_str_or_path: str = "umxl",
     targets: Optional[list] = None,
     niter: int = 1,
     residual: bool = False,
     wiener_win_len: Optional[int] = 300,
     device: Union[str, torch.device] = "cpu",
     pretrained: bool = True,
     filterbank: str = "torch",
@@ -174,15 +174,15 @@
     """Separator loader
 
     Args:
         model_str_or_path (str): Model name or path to model _parent_ directory
             E.g. The following files are assumed to present when
             loading `model_str_or_path='mymodel', targets=['vocals']`
             'mymodel/separator.json', mymodel/vocals.pth', 'mymodel/vocals.json'.
-            Defaults to `umxhq`.
+            Defaults to `umxl`.
         targets (list of str or None): list of target names. When loading a
             pre-trained model, all `targets` can be None as all targets
             will be loaded
         niter (int): Number of EM steps for refining initial estimates
             in a post-processing stage. `--niter 0` skips this step altogether
             (and thus makes separation significantly faster) More iterations
             can get better interference reduction at the price of artifacts.
@@ -208,17 +208,15 @@
     model_path = Path(model_str_or_path).expanduser()
 
     # when path exists, we assume its a custom model saved locally
     if model_path.exists():
         if targets is None:
             raise UserWarning("For custom models, please specify the targets")
 
-        target_models = load_target_models(
-            targets=targets, model_str_or_path=model_path, pretrained=pretrained
-        )
+        target_models = load_target_models(targets=targets, model_str_or_path=model_path, pretrained=pretrained)
 
         with open(Path(model_path, "separator.json"), "r") as stream:
             enc_conf = json.load(stream)
 
         separator = model.Separator(
             target_models=target_models,
             niter=niter,
@@ -236,14 +234,15 @@
         hub_loader = getattr(openunmix, model_str_or_path)
         separator = hub_loader(
             targets=targets,
             device=device,
             pretrained=True,
             niter=niter,
             residual=residual,
+            wiener_win_len=wiener_win_len,
             filterbank=filterbank,
         )
 
     return separator
 
 
 def preprocess(
```

### Comparing `openunmix-1.2.1/openunmix.egg-info/PKG-INFO` & `openunmix-1.3.0/openunmix.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,314 +1,335 @@
 Metadata-Version: 2.1
 Name: openunmix
-Version: 1.2.1
+Version: 1.3.0
 Summary: PyTorch-based music source separation toolkit
-Home-page: https://github.com/sigsep/open-unmix-pytorch
-Author: Fabian-Robert Stöter
-Author-email: fabian-robert.stoter@inria.fr
+Author-email: Fabian-Robert Stöter <mail@faroit.com>, Antoine Liutkus <antoine.liutkus@inria.fr>
 License: MIT
-Description: #  _Open-Unmix_ for PyTorch
-        
-        [![status](https://joss.theoj.org/papers/571753bc54c5d6dd36382c3d801de41d/status.svg)](https://joss.theoj.org/papers/571753bc54c5d6dd36382c3d801de41d) 
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1mijF0zGWxN-KaxTnd0q6hayAlrID5fEQ)
-        [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/open-unmix-a-reference-implementation-for/music-source-separation-on-musdb18)](https://paperswithcode.com/sota/music-source-separation-on-musdb18?p=open-unmix-a-reference-implementation-for)
-        
-        [![Build Status](https://github.com/sigsep/open-unmix-pytorch/workflows/CI/badge.svg)](https://github.com/sigsep/open-unmix-pytorch/actions?query=workflow%3ACI+branch%3Amaster+event%3Apush)
-        [![Latest Version](https://img.shields.io/pypi/v/openunmix.svg)](https://pypi.python.org/pypi/openunmix)
-        [![Supported Python versions](https://img.shields.io/pypi/pyversions/openunmix.svg)](https://pypi.python.org/pypi/openunmix)
-        
-        This repository contains the PyTorch (1.8+) implementation of __Open-Unmix__, a deep neural network reference implementation for music source separation, applicable for researchers, audio engineers and artists. __Open-Unmix__ provides ready-to-use models that allow users to separate pop music into four stems: __vocals__, __drums__, __bass__ and the remaining __other__ instruments. The models were pre-trained on the freely available [MUSDB18](https://sigsep.github.io/datasets/musdb.html) dataset. See details at [apply pre-trained model](#getting-started).
-        
-        ## ⭐️ News 
-        
-        - 03/07/2021: We added `umxl`, a model that was trained on extra data which significantly improves the performance, especially generalization.
-        - 14/02/2021: We released the new version of open-unmix as a python package. This comes with: a fully differentiable version of [norbert](https://github.com/sigsep/norbert), improved audio loading pipeline and large number of bug fixes. See [release notes](https://github.com/sigsep/open-unmix-pytorch/releases/) for further info.
-        
-        - 06/05/2020: We added a pre-trained speech enhancement model `umxse` provided by Sony.
-        
-        - 13/03/2020: Open-unmix was awarded 2nd place in the [PyTorch Global Summer Hackathon 2020](https://devpost.com/software/open-unmix).
-        
-        __Related Projects:__ open-unmix-pytorch | [open-unmix-nnabla](https://github.com/sigsep/open-unmix-nnabla) | [musdb](https://github.com/sigsep/sigsep-mus-db) | [museval](https://github.com/sigsep/sigsep-mus-eval) | [norbert](https://github.com/sigsep/norbert)
-        
-        ## 🧠 The Model (for one source)
-        
-        ![](https://docs.google.com/drawings/d/e/2PACX-1vTPoQiPwmdfET4pZhue1RvG7oEUJz7eUeQvCu6vzYeKRwHl6by4RRTnphImSKM0k5KXw9rZ1iIFnpGW/pub?w=959&h=308)
-        
-        To perform separation into multiple sources, _Open-unmix_ comprises multiple models that are trained for each particular target. While this makes the training less comfortable, it allows great flexibility to customize the training data for each target source.
-        
-        Each _Open-Unmix_ source model is based on a three-layer bidirectional deep LSTM. The model learns to predict the magnitude spectrogram of a target source, like _vocals_, from the magnitude spectrogram of a mixture input. Internally, the prediction is obtained by applying a mask on the input. The model is optimized in the magnitude domain using mean squared error.
-        
-        ### Input Stage
-        
-        __Open-Unmix__ operates in the time-frequency domain to perform its prediction. The input of the model is either:
-        
-        * __`models.Separator`:__ A time domain signal tensor of shape `(nb_samples, nb_channels, nb_timesteps)`, where `nb_samples` are the samples in a batch, `nb_channels` is 1 or 2 for mono or stereo audio, respectively, and `nb_timesteps` is the number of audio samples in the recording. In this case, the model computes STFTs with either `torch` or `asteroid_filteranks` on the fly.
-        
-        * __`models.OpenUnmix`:__ The core open-unmix takes **magnitude spectrograms** directly (e.g. when pre-computed and loaded from disk). In that case, the input is of shape `(nb_frames, nb_samples, nb_channels, nb_bins)`, where `nb_frames` and `nb_bins` are the time and frequency-dimensions of a Short-Time-Fourier-Transform.
-        
-        The input spectrogram is _standardized_ using the global mean and standard deviation for every frequency bin across all frames. Furthermore, we apply batch normalization in multiple stages of the model to make the training more robust against gain variation.
-        
-        ### Dimensionality reduction
-        
-        The LSTM is not operating on the original input spectrogram resolution. Instead, in the first step after the normalization, the network learns to compresses the frequency and channel axis of the model to reduce redundancy and make the model converge faster.
-        
-        ### Bidirectional-LSTM
-        
-        The core of __open-unmix__ is a three layer bidirectional [LSTM network](https://dl.acm.org/citation.cfm?id=1246450). Due to its recurrent nature, the model can be trained and evaluated on arbitrary length of audio signals. Since the model takes information from past and future simultaneously, the model cannot be used in an online/real-time manner.
-        An uni-directional model can easily be trained as described [here](docs/training.md).
-        
-        ### Output Stage
-        
-        After applying the LSTM, the signal is decoded back to its original input dimensionality. In the last steps the output is multiplied with the input magnitude spectrogram, so that the models is asked to learn a mask.
-        
-        ## 🤹‍♀️ Putting source models together: the `Separator`
-        
-        `models.Separator` puts together _Open-unmix_ spectrogram model for each desired target, and combines their output through a multichannel generalized Wiener filter, before application of inverse STFTs using `torchaudio`.
-        The filtering is differentiable (but parameter-free) version of [norbert](https://github.com/sigsep/norbert). The separator is currently currently only used during inference.
-        
-        ## 🏁 Getting started
-        
-        ### Installation
-        
-        `openunmix` can be installed from pypi using:
-        
-        ```
-        pip install openunmix
-        ```
-        
-        Note, that the pypi version of openunmix uses [torchaudio] to load and save audio files. To increase the number of supported input and output file formats (such as STEMS export), please additionally install [stempeg](https://github.com/faroit/stempeg).
-        
-        Training is not part of the open-unmix package, please follow [docs/train.md] for more information.
-        
-        #### Using Docker
-        
-        We also provide a docker container. Performing separation of a local track in `~/Music/track1.wav` can be performed in a single line:
-        
-        ```
-        docker run -v ~/Music/:/data -it faroit/open-unmix-pytorch "/data/track1.wav" --outdir /data/track1
-        ```
-        
-        ### Pre-trained models
-        
-        We provide three core pre-trained music separation models. All three models are end-to-end models that take waveform inputs and output the separated waveforms.
-        
-        * __`umxl` (default)__  trained on private stems dataset of compressed stems. __Note, that the weights are only licensed for non-commercial use (CC BY-NC-SA 4.0).__
-        
-          [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5069601.svg)](https://doi.org/10.5281/zenodo.5069601)
-        
-        * __`umxhq`__  trained on [MUSDB18-HQ](https://sigsep.github.io/datasets/musdb.html#uncompressed-wav) which comprises the same tracks as in MUSDB18 but un-compressed which yield in a full bandwidth of 22050 Hz.
-        
-          [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3370489.svg)](https://doi.org/10.5281/zenodo.3370489)
-        
-        * __`umx`__ is trained on the regular [MUSDB18](https://sigsep.github.io/datasets/musdb.html#compressed-stems) which is bandwidth limited to 16 kHz do to AAC compression. This model should be used for comparison with other (older) methods for evaluation in [SiSEC18](sisec18.unmix.app).
-        
-          [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3370486.svg)](https://doi.org/10.5281/zenodo.3370486)
-        
-        Furthermore, we provide a model for speech enhancement trained by [Sony Corporation](link)
-        
-        * __`umxse`__ speech enhancement model is trained on the 28-speaker version of the [Voicebank+DEMAND corpus](https://datashare.is.ed.ac.uk/handle/10283/1942?show=full).
-        
-          [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3786908.svg)](https://doi.org/10.5281/zenodo.3786908)
-        
-        All four models are also available as spectrogram (core) models, which take magnitude spectrogram inputs and ouput separated spectrograms.
-        These models can be loaded using `umxl_spec`, `umxhq_spec`, `umx_spec` and `umxse_spec`.
-        
-        To separate audio files (`wav`, `flac`, `ogg` - but not `mp3`) files just run:
-        
-        ```bash
-        umx input_file.wav
-        ```
-        
-        A more detailed list of the parameters used for the separation is given in the [inference.md](/docs/inference.md) document.
-        
-        We provide a [jupyter notebook on google colab](https://colab.research.google.com/drive/1mijF0zGWxN-KaxTnd0q6hayAlrID5fEQ) to experiment with open-unmix and to separate files online without any installation setup.
-        
-        ### Using pre-trained models from within python
-        
-        We implementes several ways to load pre-trained models and use them from within your python projects:
-        #### When the package is installed
-        
-        Loading a pre-trained models is as simple as loading
-        
-        ```python
-        separator = openunmix.umxl(...)
-        ```
-        #### torch.hub
-        
-        We also provide a torch.hub compatible modules that can be loaded. Note that this does _not_ even require to install the open-unmix packagen and should generally work when the pytorch version is the same.
-        
-        ```python
-        separator = torch.hub.load('sigsep/open-unmix-pytorch', 'umxl, device=device)
-        ```
-        
-        Where, `umxl` specifies the pre-trained model. 
-        #### Performing separation
-        
-        With a created separator object, one can perform separation of some `audio` (torch.Tensor of shape `(channels, length)`, provided as at a sampling rate `separator.sample_rate`) through:
-        
-        ```python
-        estimates = separator(audio, ...)
-        # returns estimates as tensor
-        ```
-        
-        Note that this requires the audio to be in the right shape and sampling rate. For convenience we provide a pre-processing in `openunmix.utils.preprocess(..`)` that takes numpy audio and converts it to be used for open-unmix.
-        
-        #### One-liner
-        
-        To perform model loading, preprocessing and separation in one step, just use:
-        
-        ```python
-        from openunmix import separate
-        estimates = separate.predict(audio, ...)
-        ```
-        
-        ### Load user-trained models
-        
-        When a path instead of a model-name is provided to `--model`, pre-trained `Separator` will be loaded from disk.
-        E.g. The following files are assumed to present when loading `--model mymodel --targets vocals`
-        
-        * `mymodel/separator.json`
-        * `mymodel/vocals.pth`
-        * `mymodel/vocals.json`
-        
-        
-        Note that the separator usually joins multiple models for each target and performs separation using all models. E.g. if the separator contains `vocals` and `drums` models, two output files are generated, unless the `--residual` option is selected, in which case an additional source will be produced, containing an estimate of all that is not the targets in the mixtures.
-        
-        ### Evaluation using `museval`
-        
-        To perform evaluation in comparison to other SISEC systems, you would need to install the `museval` package using
-        
-        ```
-        pip install museval
-        ```
-        
-        and then run the evaluation using
-        
-        `python -m openunmix.evaluate --outdir /path/to/musdb/estimates --evaldir /path/to/museval/results`
-        
-        ### Results compared to SiSEC 2018 (SDR/Vocals)
-        
-        Open-Unmix yields state-of-the-art results compared to participants from [SiSEC 2018](https://sisec18.unmix.app/#/methods). The performance of `UMXHQ` and `UMX` is almost identical since it was evaluated on compressed STEMS.
-        
-        ![boxplot_updated](https://user-images.githubusercontent.com/72940/63944652-3f624c80-ca72-11e9-8d33-bed701679fe6.png)
-        
-        Note that
-        
-        1. [`STL1`, `TAK2`, `TAK3`, `TAU1`, `UHL3`, `UMXHQ`] were omitted as they were _not_ trained on only _MUSDB18_.
-        2. [`HEL1`, `TAK1`, `UHL1`, `UHL2`] are not open-source.
-        
-        #### Scores (Median of frames, Median of tracks)
-        
-        |target|SDR  | SDR |  SDR |
-        |------|-----|-----|-----|
-        |`model`|UMX  |UMXHQ|UMXL |
-        |vocals|6.32 | 6.25|__7.21__ |
-        |bass  |5.23 | 5.07|__6.02__ |
-        |drums |5.73 | 6.04|__7.15__ |
-        |other |4.02 | 4.28|__4.89__ |
-        
-        ## Training
-        
-        Details on the training is provided in a separate document [here](docs/training.md).
-        
-        ## Extensions
-        
-        Details on how _open-unmix_ can be extended or improved for future research on music separation is described in a separate document [here](docs/extensions.md).
-        
-        
-        ## Design Choices
-        
-        we favored simplicity over performance to promote clearness of the code. The rationale is to have __open-unmix__ serve as a __baseline__ for future research while performance still meets current state-of-the-art (See [Evaluation](#Evaluation)). The results are comparable/better to those of `UHL1`/`UHL2` which obtained the best performance over all systems trained on MUSDB18 in the [SiSEC 2018 Evaluation campaign](https://sisec18.unmix.app).
-        We designed the code to allow researchers to reproduce existing results, quickly develop new architectures and add own user data for training and testing. We favored framework specifics implementations instead of having a monolithic repository with common code for all frameworks.
-        
-        ## How to contribute
-        
-        _open-unmix_ is a community focused project, we therefore encourage the community to submit bug-fixes and requests for technical support through [github issues](https://github.com/sigsep/open-unmix-pytorch/issues/new/choose). For more details of how to contribute, please follow our [`CONTRIBUTING.md`](CONTRIBUTING.md). For help and support, please use the gitter chat or the google groups forums. 
-        
-        ### Authors
-        
-        [Fabian-Robert Stöter](https://www.faroit.com/), [Antoine Liutkus](https://github.com/aliutkus), Inria and LIRMM, Montpellier, France
-        
-        ## References
-        
-        <details><summary>If you use open-unmix for your research – Cite Open-Unmix</summary>
-        
-        ```latex
-        @article{stoter19,  
-          author={F.-R. St\\"oter and S. Uhlich and A. Liutkus and Y. Mitsufuji},  
-          title={Open-Unmix - A Reference Implementation for Music Source Separation},  
-          journal={Journal of Open Source Software},  
-          year=2019,
-          doi = {10.21105/joss.01667},
-          url = {https://doi.org/10.21105/joss.01667}
-        }
-        ```
-        
-        </p>
-        </details>
-        
-        <details><summary>If you use the MUSDB dataset for your research - Cite the MUSDB18 Dataset</summary>
-        <p>
-        
-        ```latex
-        @misc{MUSDB18,
-          author       = {Rafii, Zafar and
-                          Liutkus, Antoine and
-                          Fabian-Robert St{\"o}ter and
-                          Mimilakis, Stylianos Ioannis and
-                          Bittner, Rachel},
-          title        = {The {MUSDB18} corpus for music separation},
-          month        = dec,
-          year         = 2017,
-          doi          = {10.5281/zenodo.1117372},
-          url          = {https://doi.org/10.5281/zenodo.1117372}
-        }
-        ```
-        
-        </p>
-        </details>
-        
-        
-        <details><summary>If compare your results with SiSEC 2018 Participants - Cite the SiSEC 2018 LVA/ICA Paper</summary>
-        <p>
-        
-        ```latex
-        @inproceedings{SiSEC18,
-          author="St{\"o}ter, Fabian-Robert and Liutkus, Antoine and Ito, Nobutaka",
-          title="The 2018 Signal Separation Evaluation Campaign",
-          booktitle="Latent Variable Analysis and Signal Separation:
-          14th International Conference, LVA/ICA 2018, Surrey, UK",
-          year="2018",
-          pages="293--305"
-        }
-        ```
-        
-        </p>
-        </details>
-        
-        ⚠️ Please note that the official acronym for _open-unmix_ is **UMX**.
-        
-        ### License
-        
-        MIT
-        
-        ### Acknowledgements
-        
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/sigsep/website/master/content/open-unmix/logo_INRIA.svg?sanitize=true" width="200" title="inria">
-          <img src="https://raw.githubusercontent.com/sigsep/website/master/content/open-unmix/anr.jpg" width="100" alt="anr">
-        </p>
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Project-URL: Homepage, https://github.com/sigsep/open-unmix-pytorch
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: torchaudio>=0.9.0
+Requires-Dist: torch>=1.9.0
+Requires-Dist: tqdm
 Provides-Extra: asteroid
-Provides-Extra: tests
+Requires-Dist: asteroid-filterbanks>=0.3.2; extra == "asteroid"
 Provides-Extra: stempeg
+Requires-Dist: stempeg; extra == "stempeg"
 Provides-Extra: evaluation
+Requires-Dist: musdb>=0.4.0; extra == "evaluation"
+Requires-Dist: museval>=0.4.0; extra == "evaluation"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: musdb>=0.4.0; extra == "tests"
+Requires-Dist: museval>=0.4.0; extra == "tests"
+Requires-Dist: stempeg; extra == "tests"
+Requires-Dist: asteroid-filterbanks>=0.3.2; extra == "tests"
+Requires-Dist: onnx; extra == "tests"
+Requires-Dist: tqdm; extra == "tests"
+
+#  _Open-Unmix_ for PyTorch
+
+[![status](https://joss.theoj.org/papers/571753bc54c5d6dd36382c3d801de41d/status.svg)](https://joss.theoj.org/papers/571753bc54c5d6dd36382c3d801de41d) 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1mijF0zGWxN-KaxTnd0q6hayAlrID5fEQ)
+[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/open-unmix-a-reference-implementation-for/music-source-separation-on-musdb18)](https://paperswithcode.com/sota/music-source-separation-on-musdb18?p=open-unmix-a-reference-implementation-for)
+
+[![Build Status](https://github.com/sigsep/open-unmix-pytorch/workflows/CI/badge.svg)](https://github.com/sigsep/open-unmix-pytorch/actions?query=workflow%3ACI+branch%3Amaster+event%3Apush)
+[![Latest Version](https://img.shields.io/pypi/v/openunmix.svg)](https://pypi.python.org/pypi/openunmix)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/openunmix.svg)](https://pypi.python.org/pypi/openunmix)
+
+This repository contains the PyTorch (1.8+) implementation of __Open-Unmix__, a deep neural network reference implementation for music source separation, applicable for researchers, audio engineers and artists. __Open-Unmix__ provides ready-to-use models that allow users to separate pop music into four stems: __vocals__, __drums__, __bass__ and the remaining __other__ instruments. The models were pre-trained on the freely available [MUSDB18](https://sigsep.github.io/datasets/musdb.html) dataset. See details at [apply pre-trained model](#getting-started).
+
+## ⭐️ News 
+
+- 03/07/2021: We added `umxl`, a model that was trained on extra data which significantly improves the performance, especially generalization.
+- 14/02/2021: We released the new version of open-unmix as a python package. This comes with: a fully differentiable version of [norbert](https://github.com/sigsep/norbert), improved audio loading pipeline and large number of bug fixes. See [release notes](https://github.com/sigsep/open-unmix-pytorch/releases/) for further info.
+
+- 06/05/2020: We added a pre-trained speech enhancement model `umxse` provided by Sony.
+
+- 13/03/2020: Open-unmix was awarded 2nd place in the [PyTorch Global Summer Hackathon 2020](https://devpost.com/software/open-unmix).
+
+__Related Projects:__ open-unmix-pytorch | [open-unmix-nnabla](https://github.com/sigsep/open-unmix-nnabla) | [musdb](https://github.com/sigsep/sigsep-mus-db) | [museval](https://github.com/sigsep/sigsep-mus-eval) | [norbert](https://github.com/sigsep/norbert)
+
+## 🧠 The Model (for one source)
+
+![](https://docs.google.com/drawings/d/e/2PACX-1vTPoQiPwmdfET4pZhue1RvG7oEUJz7eUeQvCu6vzYeKRwHl6by4RRTnphImSKM0k5KXw9rZ1iIFnpGW/pub?w=959&h=308)
+
+To perform separation into multiple sources, _Open-unmix_ comprises multiple models that are trained for each particular target. While this makes the training less comfortable, it allows great flexibility to customize the training data for each target source.
+
+Each _Open-Unmix_ source model is based on a three-layer bidirectional deep LSTM. The model learns to predict the magnitude spectrogram of a target source, like _vocals_, from the magnitude spectrogram of a mixture input. Internally, the prediction is obtained by applying a mask on the input. The model is optimized in the magnitude domain using mean squared error.
+
+### Input Stage
+
+__Open-Unmix__ operates in the time-frequency domain to perform its prediction. The input of the model is either:
+
+* __`models.Separator`:__ A time domain signal tensor of shape `(nb_samples, nb_channels, nb_timesteps)`, where `nb_samples` are the samples in a batch, `nb_channels` is 1 or 2 for mono or stereo audio, respectively, and `nb_timesteps` is the number of audio samples in the recording. In this case, the model computes STFTs with either `torch` or `asteroid_filteranks` on the fly.
+
+* __`models.OpenUnmix`:__ The core open-unmix takes **magnitude spectrograms** directly (e.g. when pre-computed and loaded from disk). In that case, the input is of shape `(nb_frames, nb_samples, nb_channels, nb_bins)`, where `nb_frames` and `nb_bins` are the time and frequency-dimensions of a Short-Time-Fourier-Transform.
+
+The input spectrogram is _standardized_ using the global mean and standard deviation for every frequency bin across all frames. Furthermore, we apply batch normalization in multiple stages of the model to make the training more robust against gain variation.
+
+### Dimensionality reduction
+
+The LSTM is not operating on the original input spectrogram resolution. Instead, in the first step after the normalization, the network learns to compresses the frequency and channel axis of the model to reduce redundancy and make the model converge faster.
+
+### Bidirectional-LSTM
+
+The core of __open-unmix__ is a three layer bidirectional [LSTM network](https://dl.acm.org/citation.cfm?id=1246450). Due to its recurrent nature, the model can be trained and evaluated on arbitrary length of audio signals. Since the model takes information from past and future simultaneously, the model cannot be used in an online/real-time manner.
+An uni-directional model can easily be trained as described [here](docs/training.md).
+
+### Output Stage
+
+After applying the LSTM, the signal is decoded back to its original input dimensionality. In the last steps the output is multiplied with the input magnitude spectrogram, so that the models is asked to learn a mask.
+
+## 🤹‍♀️ Putting source models together: the `Separator`
+
+`models.Separator` puts together _Open-unmix_ spectrogram model for each desired target, and combines their output through a multichannel generalized Wiener filter, before application of inverse STFTs using `torchaudio`.
+The filtering is differentiable (but parameter-free) version of [norbert](https://github.com/sigsep/norbert). The separator is currently currently only used during inference.
+
+## 🏁 Getting started
+
+### Installation
+
+`openunmix` can be installed from pypi using:
+
+```
+pip install openunmix
+```
+
+Note, that the pypi version of openunmix uses [torchaudio] to load and save audio files. To increase the number of supported input and output file formats (such as STEMS export), please additionally install [stempeg](https://github.com/faroit/stempeg).
+
+Training is not part of the open-unmix package, please follow [docs/train.md] for more information.
+
+#### Using Docker
+
+We also provide a docker container. Performing separation of a local track in `~/Music/track1.wav` can be performed in a single line:
+
+```
+docker run -v ~/Music/:/data -it faroit/open-unmix-pytorch "/data/track1.wav" --outdir /data/track1
+```
+
+### Pre-trained models
+
+We provide three core pre-trained music separation models. All three models are end-to-end models that take waveform inputs and output the separated waveforms.
+
+* __`umxl` (default)__  trained on private stems dataset of compressed stems. __Note, that the weights are only licensed for non-commercial use (CC BY-NC-SA 4.0).__
+
+  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5069601.svg)](https://doi.org/10.5281/zenodo.5069601)
+
+* __`umxhq`__  trained on [MUSDB18-HQ](https://sigsep.github.io/datasets/musdb.html#uncompressed-wav) which comprises the same tracks as in MUSDB18 but un-compressed which yield in a full bandwidth of 22050 Hz.
+
+  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3370489.svg)](https://doi.org/10.5281/zenodo.3370489)
+
+* __`umx`__ is trained on the regular [MUSDB18](https://sigsep.github.io/datasets/musdb.html#compressed-stems) which is bandwidth limited to 16 kHz do to AAC compression. This model should be used for comparison with other (older) methods for evaluation in [SiSEC18](sisec18.unmix.app).
+
+  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3370486.svg)](https://doi.org/10.5281/zenodo.3370486)
+
+Furthermore, we provide a model for speech enhancement trained by [Sony Corporation](link)
+
+* __`umxse`__ speech enhancement model is trained on the 28-speaker version of the [Voicebank+DEMAND corpus](https://datashare.is.ed.ac.uk/handle/10283/1942?show=full).
+
+  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3786908.svg)](https://doi.org/10.5281/zenodo.3786908)
+
+All four models are also available as spectrogram (core) models, which take magnitude spectrogram inputs and ouput separated spectrograms.
+These models can be loaded using `umxl_spec`, `umxhq_spec`, `umx_spec` and `umxse_spec`.
+
+To separate audio files (`wav`, `flac`, `ogg` - but not `mp3`) files just run:
+
+```bash
+umx input_file.wav
+```
+
+A more detailed list of the parameters used for the separation is given in the [inference.md](/docs/inference.md) document.
+
+We provide a [jupyter notebook on google colab](https://colab.research.google.com/drive/1mijF0zGWxN-KaxTnd0q6hayAlrID5fEQ) to experiment with open-unmix and to separate files online without any installation setup.
+
+### Using pre-trained models from within python
+
+We implementes several ways to load pre-trained models and use them from within your python projects:
+#### When the package is installed
+
+Loading a pre-trained models is as simple as loading
+
+```python
+separator = openunmix.umxl(...)
+```
+#### torch.hub
+
+We also provide a torch.hub compatible modules that can be loaded. Note that this does _not_ even require to install the open-unmix packagen and should generally work when the pytorch version is the same.
+
+```python
+separator = torch.hub.load('sigsep/open-unmix-pytorch', 'umxl, device=device)
+```
+
+Where, `umxl` specifies the pre-trained model. 
+#### Performing separation
+
+With a created separator object, one can perform separation of some `audio` (torch.Tensor of shape `(channels, length)`, provided as at a sampling rate `separator.sample_rate`) through:
+
+```python
+estimates = separator(audio, ...)
+# returns estimates as tensor
+```
+
+Note that this requires the audio to be in the right shape and sampling rate. For convenience we provide a pre-processing in `openunmix.utils.preprocess(..`)` that takes numpy audio and converts it to be used for open-unmix.
+
+#### One-liner
+
+To perform model loading, preprocessing and separation in one step, just use:
+
+```python
+from openunmix.predict import separate
+estimates = separate(audio, ...)
+```
+
+### Load user-trained models
+
+When a path instead of a model-name is provided to `--model`, pre-trained `Separator` will be loaded from disk.
+E.g. The following files are assumed to present when loading `--model mymodel --targets vocals`
+
+* `mymodel/separator.json`
+* `mymodel/vocals.pth`
+* `mymodel/vocals.json`
+
+
+Note that the separator usually joins multiple models for each target and performs separation using all models. E.g. if the separator contains `vocals` and `drums` models, two output files are generated, unless the `--residual` option is selected, in which case an additional source will be produced, containing an estimate of all that is not the targets in the mixtures.
+
+### Evaluation using `museval`
+
+To perform evaluation in comparison to other SISEC systems, you would need to install the `museval` package using
+
+```
+pip install museval
+```
+
+and then run the evaluation using
+
+`python -m openunmix.evaluate --outdir /path/to/musdb/estimates --evaldir /path/to/museval/results`
+
+### Results compared to SiSEC 2018 (SDR/Vocals)
+
+Open-Unmix yields state-of-the-art results compared to participants from [SiSEC 2018](https://sisec18.unmix.app/#/methods). The performance of `UMXHQ` and `UMX` is almost identical since it was evaluated on compressed STEMS.
+
+![boxplot_updated](https://user-images.githubusercontent.com/72940/63944652-3f624c80-ca72-11e9-8d33-bed701679fe6.png)
+
+Note that
+
+1. [`STL1`, `TAK2`, `TAK3`, `TAU1`, `UHL3`, `UMXHQ`] were omitted as they were _not_ trained on only _MUSDB18_.
+2. [`HEL1`, `TAK1`, `UHL1`, `UHL2`] are not open-source.
+
+#### Scores (Median of frames, Median of tracks)
+
+|target|SDR  | SDR |  SDR |
+|------|-----|-----|-----|
+|`model`|UMX  |UMXHQ|UMXL |
+|vocals|6.32 | 6.25|__7.21__ |
+|bass  |5.23 | 5.07|__6.02__ |
+|drums |5.73 | 6.04|__7.15__ |
+|other |4.02 | 4.28|__4.89__ |
+
+## Training
+
+Details on the training is provided in a separate document [here](docs/training.md).
+
+## Extensions
+
+Details on how _open-unmix_ can be extended or improved for future research on music separation is described in a separate document [here](docs/extensions.md).
+
+
+## Design Choices
+
+we favored simplicity over performance to promote clearness of the code. The rationale is to have __open-unmix__ serve as a __baseline__ for future research while performance still meets current state-of-the-art (See [Evaluation](#Evaluation)). The results are comparable/better to those of `UHL1`/`UHL2` which obtained the best performance over all systems trained on MUSDB18 in the [SiSEC 2018 Evaluation campaign](https://sisec18.unmix.app).
+We designed the code to allow researchers to reproduce existing results, quickly develop new architectures and add own user data for training and testing. We favored framework specifics implementations instead of having a monolithic repository with common code for all frameworks.
+
+## How to contribute
+
+_open-unmix_ is a community focused project, we therefore encourage the community to submit bug-fixes and requests for technical support through [github issues](https://github.com/sigsep/open-unmix-pytorch/issues/new/choose). For more details of how to contribute, please follow our [`CONTRIBUTING.md`](CONTRIBUTING.md). For help and support, please use the gitter chat or the google groups forums. 
+
+### Authors
+
+[Fabian-Robert Stöter](https://www.faroit.com/), [Antoine Liutkus](https://github.com/aliutkus), Inria and LIRMM, Montpellier, France
+
+## References
+
+<details><summary>If you use open-unmix for your research – Cite Open-Unmix</summary>
+
+```latex
+@article{stoter19,  
+  author={F.-R. St\\"oter and S. Uhlich and A. Liutkus and Y. Mitsufuji},  
+  title={Open-Unmix - A Reference Implementation for Music Source Separation},  
+  journal={Journal of Open Source Software},  
+  year=2019,
+  doi = {10.21105/joss.01667},
+  url = {https://doi.org/10.21105/joss.01667}
+}
+```
+
+</p>
+</details>
+
+<details><summary>If you use the MUSDB dataset for your research - Cite the MUSDB18 Dataset</summary>
+<p>
+
+```latex
+@misc{MUSDB18,
+  author       = {Rafii, Zafar and
+                  Liutkus, Antoine and
+                  Fabian-Robert St{\"o}ter and
+                  Mimilakis, Stylianos Ioannis and
+                  Bittner, Rachel},
+  title        = {The {MUSDB18} corpus for music separation},
+  month        = dec,
+  year         = 2017,
+  doi          = {10.5281/zenodo.1117372},
+  url          = {https://doi.org/10.5281/zenodo.1117372}
+}
+```
+
+</p>
+</details>
+
+
+<details><summary>If compare your results with SiSEC 2018 Participants - Cite the SiSEC 2018 LVA/ICA Paper</summary>
+<p>
+
+```latex
+@inproceedings{SiSEC18,
+  author="St{\"o}ter, Fabian-Robert and Liutkus, Antoine and Ito, Nobutaka",
+  title="The 2018 Signal Separation Evaluation Campaign",
+  booktitle="Latent Variable Analysis and Signal Separation:
+  14th International Conference, LVA/ICA 2018, Surrey, UK",
+  year="2018",
+  pages="293--305"
+}
+```
+
+</p>
+</details>
+
+⚠️ Please note that the official acronym for _open-unmix_ is **UMX**.
+
+### License
+
+MIT
+
+### Acknowledgements
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/sigsep/website/master/content/open-unmix/logo_INRIA.svg?sanitize=true" width="200" title="inria">
+  <img src="https://raw.githubusercontent.com/sigsep/website/master/content/open-unmix/anr.jpg" width="100" alt="anr">
+</p>
```

### Comparing `openunmix-1.2.1/openunmix.egg-info/SOURCES.txt` & `openunmix-1.3.0/openunmix.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 openunmix/__init__.py
 openunmix/cli.py
 openunmix/data.py
 openunmix/evaluate.py
 openunmix/filtering.py
 openunmix/model.py
 openunmix/predict.py
```

### Comparing `openunmix-1.2.1/tests/create_vectors.py` & `openunmix-1.3.0/tests/create_vectors.py`

 * *Files identical despite different names*

### Comparing `openunmix-1.2.1/tests/test_augmentations.py` & `openunmix-1.3.0/tests/test_augmentations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pytest
 import torch
 
 from openunmix import data
 
 
-@pytest.fixture(params=[4096, 4096 * 10])
+@pytest.fixture(params=[4096])
 def nb_timesteps(request):
     return int(request.param)
 
 
-@pytest.fixture(params=[1, 2, 3])
+@pytest.fixture(params=[1, 2])
 def nb_channels(request):
     return request.param
 
 
 @pytest.fixture
 def audio(request, nb_channels, nb_timesteps):
     return torch.rand((nb_channels, nb_timesteps))
```

### Comparing `openunmix-1.2.1/tests/test_datasets.py` & `openunmix-1.3.0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `openunmix-1.2.1/tests/test_io.py` & `openunmix-1.3.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `openunmix-1.2.1/tests/test_model.py` & `openunmix-1.3.0/tests/test_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 from openunmix import model
 from openunmix import umxse
 from openunmix import umxhq
 from openunmix import umx
 from openunmix import umxl
 
 
-@pytest.fixture(params=[10, 100])
+@pytest.fixture(params=[100])
 def nb_frames(request):
     return int(request.param)
 
 
-@pytest.fixture(params=[1, 2, 3])
+@pytest.fixture(params=[1, 2])
 def nb_channels(request):
     return request.param
 
 
-@pytest.fixture(params=[1, 5])
+@pytest.fixture(params=[2])
 def nb_samples(request):
     return request.param
 
 
-@pytest.fixture(params=[111, 1024])
+@pytest.fixture(params=[1024])
 def nb_bins(request):
     return request.param
 
 
 @pytest.fixture
 def spectrogram(request, nb_samples, nb_channels, nb_bins, nb_frames):
     return torch.rand((nb_samples, nb_channels, nb_bins, nb_frames))
 
 
-@pytest.fixture(params=[True, False])
+@pytest.fixture(params=[False])
 def unidirectional(request):
     return request.param
 
 
 @pytest.fixture(params=[32])
 def hidden_size(request):
     return request.param
```

### Comparing `openunmix-1.2.1/tests/test_regression.py` & `openunmix-1.3.0/tests/test_regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,17 +78,15 @@
 
     Loads pre-computed transform and compare to current spectrogram
     e.g. this makes sure that the training is reproducible if parameters
     such as STFT centering would be subject to change.
     """
     track = [track for track in mus.tracks if track.name == test_track][0]
 
-    stft, _ = transforms.make_filterbanks(
-        n_fft=4096, n_hop=1024, sample_rate=track.rate, method=method
-    )
+    stft, _ = transforms.make_filterbanks(n_fft=4096, n_hop=1024, sample_rate=track.rate, method=method)
     encoder = torch.nn.Sequential(stft, model.ComplexNorm(mono=False))
     audio = torch.as_tensor(track.audio, dtype=torch.float32, device="cpu")
     audio = utils.preprocess(audio, track.rate, track.rate)
     ref = torch.load(spec_path)
     dut = encoder(audio).permute(3, 0, 1, 2)
 
-    assert torch.allclose(ref, dut, atol=1e-4, rtol=1e-3)
+    assert torch.allclose(ref, dut, atol=1e-1)
```

### Comparing `openunmix-1.2.1/tests/test_transforms.py` & `openunmix-1.3.0/tests/test_transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import pytest
 import numpy as np
 import torch
 from openunmix import transforms
 
 
-@pytest.fixture(params=[4096, 44100])
+@pytest.fixture(params=[4096])
 def nb_timesteps(request):
     return int(request.param)
 
 
-@pytest.fixture(params=[1, 2])
+@pytest.fixture(params=[2])
 def nb_channels(request):
     return request.param
 
 
-@pytest.fixture(params=[1, 2])
+@pytest.fixture(params=[2])
 def nb_samples(request):
     return request.param
 
 
-@pytest.fixture(params=[1024, 2048, 4096])
+@pytest.fixture(params=[2048])
 def nfft(request):
     return int(request.param)
 
 
-@pytest.fixture(params=[2, 4])
+@pytest.fixture(params=[2])
 def hop(request, nfft):
     return nfft // request.param
 
 
 @pytest.fixture(params=["torch", "asteroid"])
 def method(request):
     return request.param
```

### Comparing `openunmix-1.2.1/tests/test_wiener.py` & `openunmix-1.3.0/tests/test_wiener.py`

 * *Files identical despite different names*

