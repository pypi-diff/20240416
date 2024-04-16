# Comparing `tmp/tokenizers-0.9.3.tar.gz` & `tmp/tokenizers-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tokenizers-0.9.3.tar", last modified: Mon Oct 26 20:52:58 2020, max compression
+gzip compressed data, was "dist/tokenizers-0.9.4.tar", last modified: Tue Nov 10 04:37:44 2020, max compression
```

## Comparing `tokenizers-0.9.3.tar` & `tokenizers-0.9.4.tar`

### file list

```diff
@@ -1,153 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.940727 tokenizers-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (116)      770 2020-10-26 20:52:58.000000 tokenizers-0.9.3/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (116)      188 2020-10-26 20:52:48.000000 tokenizers-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7081 2020-10-26 20:52:58.940727 tokenizers-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4803 2020-10-26 20:52:48.000000 tokenizers-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.896727 tokenizers-0.9.3/py_src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.908727 tokenizers-0.9.3/py_src/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (116)     1436 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    28737 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.908727 tokenizers-0.9.3/py_src/tokenizers/decoders/
--rw-r--r--   0 runner    (1001) docker     (116)      178 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2031 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/decoders/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.912727 tokenizers-0.9.3/py_src/tokenizers/implementations/
--rw-r--r--   0 runner    (1001) docker     (116)      310 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12670 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/implementations/base_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (116)     4421 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/implementations/bert_wordpiece.py
--rw-r--r--   0 runner    (1001) docker     (116)     3523 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/implementations/byte_level_bpe.py
--rw-r--r--   0 runner    (1001) docker     (116)     4437 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/implementations/char_level_bpe.py
--rw-r--r--   0 runner    (1001) docker     (116)     2703 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/implementations/sentencepiece_bpe.py
--rw-r--r--   0 runner    (1001) docker     (116)     4087 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/implementations/sentencepiece_unigram.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.912727 tokenizers-0.9.3/py_src/tokenizers/models/
--rw-r--r--   0 runner    (1001) docker     (116)      185 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5577 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/models/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.916727 tokenizers-0.9.3/py_src/tokenizers/normalizers/
--rw-r--r--   0 runner    (1001) docker     (116)      807 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/normalizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3890 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/normalizers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.916727 tokenizers-0.9.3/py_src/tokenizers/pre_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (116)      496 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/pre_tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5172 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/pre_tokenizers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.916727 tokenizers-0.9.3/py_src/tokenizers/processors/
--rw-r--r--   0 runner    (1001) docker     (116)      244 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6533 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/processors/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.916727 tokenizers-0.9.3/py_src/tokenizers/trainers/
--rw-r--r--   0 runner    (1001) docker     (116)      171 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4914 2020-10-26 20:52:48.000000 tokenizers-0.9.3/py_src/tokenizers/trainers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.908727 tokenizers-0.9.3/py_src/tokenizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7081 2020-10-26 20:52:58.000000 tokenizers-0.9.3/py_src/tokenizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4429 2020-10-26 20:52:58.000000 tokenizers-0.9.3/py_src/tokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-26 20:52:58.000000 tokenizers-0.9.3/py_src/tokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-26 20:52:58.000000 tokenizers-0.9.3/py_src/tokenizers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       18 2020-10-26 20:52:58.000000 tokenizers-0.9.3/py_src/tokenizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2020-10-26 20:52:58.000000 tokenizers-0.9.3/py_src/tokenizers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      127 2020-10-26 20:52:48.000000 tokenizers-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-10-26 20:52:48.000000 tokenizers-0.9.3/rust-toolchain
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-26 20:52:58.940727 tokenizers-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2160 2020-10-26 20:52:48.000000 tokenizers-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.920727 tokenizers-0.9.3/src/
--rw-r--r--   0 runner    (1001) docker     (116)     9161 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/decoders.rs
--rw-r--r--   0 runner    (1001) docker     (116)     6138 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/encoding.rs
--rw-r--r--   0 runner    (1001) docker     (116)     1327 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (116)     4947 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (116)    16149 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/models.rs
--rw-r--r--   0 runner    (1001) docker     (116)    17164 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/normalizers.rs
--rw-r--r--   0 runner    (1001) docker     (116)    17081 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/pre_tokenizers.rs
--rw-r--r--   0 runner    (1001) docker     (116)    10502 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/processors.rs
--rw-r--r--   0 runner    (1001) docker     (116)      934 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/token.rs
--rw-r--r--   0 runner    (1001) docker     (116)    28850 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/tokenizer.rs
--rw-r--r--   0 runner    (1001) docker     (116)    10342 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/trainers.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.920727 tokenizers-0.9.3/src/utils/
--rw-r--r--   0 runner    (1001) docker     (116)     1595 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)    13824 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/utils/normalization.rs
--rw-r--r--   0 runner    (1001) docker     (116)     7693 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/utils/pretokenization.rs
--rw-r--r--   0 runner    (1001) docker     (116)      456 2020-10-26 20:52:48.000000 tokenizers-0.9.3/src/utils/regex.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.924727 tokenizers-0.9.3/tokenizers-lib/
--rw-r--r--   0 runner    (1001) docker     (116)     7963 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)     1439 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1598 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     4243 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      589 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/README.tpl
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.924727 tokenizers-0.9.3/tokenizers-lib/benches/
--rw-r--r--   0 runner    (1001) docker     (116)     3827 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/benches/bert_benchmark.rs
--rw-r--r--   0 runner    (1001) docker     (116)     3642 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/benches/bpe_benchmark.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.924727 tokenizers-0.9.3/tokenizers-lib/benches/common/
--rw-r--r--   0 runner    (1001) docker     (116)     2242 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/benches/common/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/rust-toolchain
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.924727 tokenizers-0.9.3/tokenizers-lib/src/
--rw-r--r--   0 runner    (1001) docker     (116)     2996 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/cli.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.924727 tokenizers-0.9.3/tokenizers-lib/src/decoders/
--rw-r--r--   0 runner    (1001) docker     (116)      712 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/decoders/bpe.rs
--rw-r--r--   0 runner    (1001) docker     (116)     1197 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/decoders/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)     1431 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/decoders/wordpiece.rs
--rw-r--r--   0 runner    (1001) docker     (116)     4590 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.924727 tokenizers-0.9.3/tokenizers-lib/src/models/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.928727 tokenizers-0.9.3/tokenizers-lib/src/models/bpe/
--rw-r--r--   0 runner    (1001) docker     (116)     3288 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/bpe/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)    25202 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/bpe/model.rs
--rw-r--r--   0 runner    (1001) docker     (116)     4131 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/bpe/serialization.rs
--rw-r--r--   0 runner    (1001) docker     (116)    22543 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/bpe/trainer.rs
--rw-r--r--   0 runner    (1001) docker     (116)     9979 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/bpe/word.rs
--rw-r--r--   0 runner    (1001) docker     (116)     4860 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.928727 tokenizers-0.9.3/tokenizers-lib/src/models/unigram/
--rw-r--r--   0 runner    (1001) docker     (116)    22753 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/unigram/lattice.rs
--rw-r--r--   0 runner    (1001) docker     (116)      180 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/unigram/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)    20430 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/unigram/model.rs
--rw-r--r--   0 runner    (1001) docker     (116)     2885 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/unigram/serialization.rs
--rw-r--r--   0 runner    (1001) docker     (116)    26220 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/unigram/trainer.rs
--rw-r--r--   0 runner    (1001) docker     (116)     1970 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/unigram/trie.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.932727 tokenizers-0.9.3/tokenizers-lib/src/models/wordlevel/
--rw-r--r--   0 runner    (1001) docker     (116)     5344 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/wordlevel/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)     1603 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/wordlevel/serialization.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.932727 tokenizers-0.9.3/tokenizers-lib/src/models/wordpiece/
--rw-r--r--   0 runner    (1001) docker     (116)     8924 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/wordpiece/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)     2365 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/wordpiece/serialization.rs
--rw-r--r--   0 runner    (1001) docker     (116)     3524 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/models/wordpiece/trainer.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.932727 tokenizers-0.9.3/tokenizers-lib/src/normalizers/
--rw-r--r--   0 runner    (1001) docker     (116)     4289 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/normalizers/bert.rs
--rw-r--r--   0 runner    (1001) docker     (116)     2636 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/normalizers/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)     2451 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/normalizers/precompiled.rs
--rw-r--r--   0 runner    (1001) docker     (116)     3662 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/normalizers/replace.rs
--rw-r--r--   0 runner    (1001) docker     (116)     5215 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/normalizers/strip.rs
--rw-r--r--   0 runner    (1001) docker     (116)     2585 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/normalizers/unicode.rs
--rw-r--r--   0 runner    (1001) docker     (116)     1186 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/normalizers/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.936727 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (116)     2601 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/bert.rs
--rw-r--r--   0 runner    (1001) docker     (116)    15194 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/byte_level.rs
--rw-r--r--   0 runner    (1001) docker     (116)      709 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/delimiter.rs
--rw-r--r--   0 runner    (1001) docker     (116)     3105 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/digits.rs
--rw-r--r--   0 runner    (1001) docker     (116)     3987 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/metaspace.rs
--rw-r--r--   0 runner    (1001) docker     (116)     2791 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)     1366 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/punctuation.rs
--rw-r--r--   0 runner    (1001) docker     (116)     1843 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/sequence.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.936727 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/unicode_scripts/
--rw-r--r--   0 runner    (1001) docker     (116)      102 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/unicode_scripts/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)     4948 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/unicode_scripts/pre_tokenizer.rs
--rw-r--r--   0 runner    (1001) docker     (116)    81858 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/unicode_scripts/scripts.rs
--rw-r--r--   0 runner    (1001) docker     (116)     4284 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/whitespace.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.940727 tokenizers-0.9.3/tokenizers-lib/src/processors/
--rw-r--r--   0 runner    (1001) docker     (116)     5922 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/processors/bert.rs
--rw-r--r--   0 runner    (1001) docker     (116)     3232 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/processors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)     7565 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/processors/roberta.rs
--rw-r--r--   0 runner    (1001) docker     (116)    30271 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/processors/template.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.940727 tokenizers-0.9.3/tokenizers-lib/src/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (116)    25469 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/tokenizer/added_vocabulary.rs
--rw-r--r--   0 runner    (1001) docker     (116)    21401 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/tokenizer/encoding.rs
--rw-r--r--   0 runner    (1001) docker     (116)    35676 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/tokenizer/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)    68317 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/tokenizer/normalizer.rs
--rw-r--r--   0 runner    (1001) docker     (116)     7609 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/tokenizer/pattern.rs
--rw-r--r--   0 runner    (1001) docker     (116)    10128 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/tokenizer/pre_tokenizer.rs
--rw-r--r--   0 runner    (1001) docker     (116)     5827 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/tokenizer/serialization.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.940727 tokenizers-0.9.3/tokenizers-lib/src/utils/
--rw-r--r--   0 runner    (1001) docker     (116)     3200 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/utils/cache.rs
--rw-r--r--   0 runner    (1001) docker     (116)     2809 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/utils/iter.rs
--rw-r--r--   0 runner    (1001) docker     (116)     2603 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)     3732 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/utils/padding.rs
--rw-r--r--   0 runner    (1001) docker     (116)     6148 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/utils/parallelism.rs
--rw-r--r--   0 runner    (1001) docker     (116)     9784 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/src/utils/truncation.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.940727 tokenizers-0.9.3/tokenizers-lib/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     3759 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/tests/added_tokens.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 20:52:58.940727 tokenizers-0.9.3/tokenizers-lib/tests/common/
--rw-r--r--   0 runner    (1001) docker     (116)     1918 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/tests/common/mod.rs
--rw-r--r--   0 runner    (1001) docker     (116)     4893 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/tests/offsets.rs
--rw-r--r--   0 runner    (1001) docker     (116)     7510 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/tests/serialization.rs
--rw-r--r--   0 runner    (1001) docker     (116)     3143 2020-10-26 20:52:48.000000 tokenizers-0.9.3/tokenizers-lib/tests/unigram.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.586253 tokenizers-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (116)      770 2020-11-10 04:37:44.000000 tokenizers-0.9.4/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (116)      188 2020-11-10 04:37:28.000000 tokenizers-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     7081 2020-11-10 04:37:44.586253 tokenizers-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4803 2020-11-10 04:37:28.000000 tokenizers-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.570253 tokenizers-0.9.4/py_src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.574253 tokenizers-0.9.4/py_src/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (116)     2741 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    39480 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.574253 tokenizers-0.9.4/py_src/tokenizers/decoders/
+-rw-r--r--   0 runner    (1001) docker     (116)      178 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2031 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/decoders/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.574253 tokenizers-0.9.4/py_src/tokenizers/implementations/
+-rw-r--r--   0 runner    (1001) docker     (116)      310 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12670 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/implementations/base_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4439 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/implementations/bert_wordpiece.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3523 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/implementations/byte_level_bpe.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4437 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/implementations/char_level_bpe.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2703 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/implementations/sentencepiece_bpe.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4105 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/implementations/sentencepiece_unigram.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.574253 tokenizers-0.9.4/py_src/tokenizers/models/
+-rw-r--r--   0 runner    (1001) docker     (116)      185 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5577 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/models/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.574253 tokenizers-0.9.4/py_src/tokenizers/normalizers/
+-rw-r--r--   0 runner    (1001) docker     (116)      807 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/normalizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3890 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/normalizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.578253 tokenizers-0.9.4/py_src/tokenizers/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (116)      496 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/pre_tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5172 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/pre_tokenizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.578253 tokenizers-0.9.4/py_src/tokenizers/processors/
+-rw-r--r--   0 runner    (1001) docker     (116)      244 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6533 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/processors/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.578253 tokenizers-0.9.4/py_src/tokenizers/trainers/
+-rw-r--r--   0 runner    (1001) docker     (116)      171 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4914 2020-11-10 04:37:28.000000 tokenizers-0.9.4/py_src/tokenizers/trainers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.574253 tokenizers-0.9.4/py_src/tokenizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     7081 2020-11-10 04:37:44.000000 tokenizers-0.9.4/py_src/tokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4467 2020-11-10 04:37:44.000000 tokenizers-0.9.4/py_src/tokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-10 04:37:44.000000 tokenizers-0.9.4/py_src/tokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-10 04:37:44.000000 tokenizers-0.9.4/py_src/tokenizers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       18 2020-11-10 04:37:44.000000 tokenizers-0.9.4/py_src/tokenizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       11 2020-11-10 04:37:44.000000 tokenizers-0.9.4/py_src/tokenizers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      127 2020-11-10 04:37:28.000000 tokenizers-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2020-11-10 04:37:28.000000 tokenizers-0.9.4/rust-toolchain
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-11-10 04:37:44.586253 tokenizers-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2160 2020-11-10 04:37:28.000000 tokenizers-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.578253 tokenizers-0.9.4/src/
+-rw-r--r--   0 runner    (1001) docker     (116)     9161 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/decoders.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    16806 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/encoding.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     1327 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     4947 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    16260 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/models.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    17164 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/normalizers.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    17081 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/pre_tokenizers.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    10502 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/processors.rs
+-rw-r--r--   0 runner    (1001) docker     (116)      934 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/token.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    44075 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/tokenizer.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    10342 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/trainers.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.578253 tokenizers-0.9.4/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)     1595 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    13824 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/utils/normalization.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     7693 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/utils/pretokenization.rs
+-rw-r--r--   0 runner    (1001) docker     (116)      456 2020-11-10 04:37:28.000000 tokenizers-0.9.4/src/utils/regex.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.578253 tokenizers-0.9.4/tokenizers-lib/
+-rw-r--r--   0 runner    (1001) docker     (116)     7963 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1439 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (116)     2085 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)     4085 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      589 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/README.tpl
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.578253 tokenizers-0.9.4/tokenizers-lib/benches/
+-rw-r--r--   0 runner    (1001) docker     (116)     3827 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/benches/bert_benchmark.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     3642 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/benches/bpe_benchmark.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.578253 tokenizers-0.9.4/tokenizers-lib/benches/common/
+-rw-r--r--   0 runner    (1001) docker     (116)     2242 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/benches/common/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/rust-toolchain
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.578253 tokenizers-0.9.4/tokenizers-lib/src/
+-rw-r--r--   0 runner    (1001) docker     (116)     2996 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/cli.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.582253 tokenizers-0.9.4/tokenizers-lib/src/decoders/
+-rw-r--r--   0 runner    (1001) docker     (116)      712 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/decoders/bpe.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     1197 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/decoders/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     1431 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/decoders/wordpiece.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     4432 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.582253 tokenizers-0.9.4/tokenizers-lib/src/models/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.582253 tokenizers-0.9.4/tokenizers-lib/src/models/bpe/
+-rw-r--r--   0 runner    (1001) docker     (116)     3288 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/bpe/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    25202 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/bpe/model.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     4131 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/bpe/serialization.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    22543 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/bpe/trainer.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     9979 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/bpe/word.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     4860 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.582253 tokenizers-0.9.4/tokenizers-lib/src/models/unigram/
+-rw-r--r--   0 runner    (1001) docker     (116)    22753 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/unigram/lattice.rs
+-rw-r--r--   0 runner    (1001) docker     (116)      180 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/unigram/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    20430 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/unigram/model.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     2885 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/unigram/serialization.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    26220 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/unigram/trainer.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     1970 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/unigram/trie.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.582253 tokenizers-0.9.4/tokenizers-lib/src/models/wordlevel/
+-rw-r--r--   0 runner    (1001) docker     (116)     5678 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/wordlevel/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     1638 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/wordlevel/serialization.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.582253 tokenizers-0.9.4/tokenizers-lib/src/models/wordpiece/
+-rw-r--r--   0 runner    (1001) docker     (116)     8924 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/wordpiece/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     2365 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/wordpiece/serialization.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     3524 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/models/wordpiece/trainer.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.582253 tokenizers-0.9.4/tokenizers-lib/src/normalizers/
+-rw-r--r--   0 runner    (1001) docker     (116)     4289 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/normalizers/bert.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     2636 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/normalizers/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     2451 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/normalizers/precompiled.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     3662 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/normalizers/replace.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     5215 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/normalizers/strip.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     2585 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/normalizers/unicode.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     1186 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/normalizers/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.582253 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (116)     2601 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/bert.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    15753 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/byte_level.rs
+-rw-r--r--   0 runner    (1001) docker     (116)      709 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/delimiter.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     3105 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/digits.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     3987 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/metaspace.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     2791 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     1366 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/punctuation.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     1843 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/sequence.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.586253 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/unicode_scripts/
+-rw-r--r--   0 runner    (1001) docker     (116)      102 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/unicode_scripts/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     4948 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/unicode_scripts/pre_tokenizer.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    81858 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/unicode_scripts/scripts.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     4284 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/whitespace.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.586253 tokenizers-0.9.4/tokenizers-lib/src/processors/
+-rw-r--r--   0 runner    (1001) docker     (116)     7112 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/processors/bert.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     3232 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/processors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     8755 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/processors/roberta.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    31331 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/processors/template.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.586253 tokenizers-0.9.4/tokenizers-lib/src/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (116)    25469 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/tokenizer/added_vocabulary.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    26292 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/tokenizer/encoding.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    36018 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/tokenizer/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    68317 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/tokenizer/normalizer.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     7609 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/tokenizer/pattern.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    10128 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/tokenizer/pre_tokenizer.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     5827 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/tokenizer/serialization.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.586253 tokenizers-0.9.4/tokenizers-lib/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)     3200 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/utils/cache.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     2809 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/utils/iter.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     2603 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     3839 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/utils/padding.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     6148 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/utils/parallelism.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     9931 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/src/utils/truncation.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.586253 tokenizers-0.9.4/tokenizers-lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)     3759 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/tests/added_tokens.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 04:37:44.586253 tokenizers-0.9.4/tokenizers-lib/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (116)     1918 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/tests/common/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    16889 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/tests/documentation.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     4905 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/tests/offsets.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     7510 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/tests/serialization.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     3143 2020-11-10 04:37:28.000000 tokenizers-0.9.4/tokenizers-lib/tests/unigram.rs
```

### Comparing `tokenizers-0.9.3/Cargo.toml` & `tokenizers-0.9.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "tokenizers-python"
-version = "0.9.3"
+version = "0.9.4"
 authors = ["Anthony MOI <m.anthony.moi@gmail.com>"]
 edition = "2018"
 
 [lib]
 name = "tokenizers"
 crate-type = ["cdylib"]
```

### Comparing `tokenizers-0.9.3/PKG-INFO` & `tokenizers-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenizers
-Version: 0.9.3
+Version: 0.9.4
 Summary: Fast and Customizable Tokenizers
 Home-page: https://github.com/huggingface/tokenizers
 Author: Anthony MOI
 Author-email: anthony@huggingface.co
 License: Apache License 2.0
 Description: <p align="center">
             <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tokenizers Version: 0.9.3 Summary: Fast and
+Metadata-Version: 2.1 Name: tokenizers Version: 0.9.4 Summary: Fast and
 Customizable Tokenizers Home-page: https://github.com/huggingface/tokenizers
 Author: Anthony MOI Author-email: anthony@huggingface.co License: Apache
 License 2.0 Description:
 
     [https://huggingface.co/landing/assets/tokenizers/tokenizers-logo.png]
                                 _[_B_u_i_l_d_]_[_G_i_t_H_u_b_]
```

### Comparing `tokenizers-0.9.3/README.md` & `tokenizers-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers/__init__.pyi` & `tokenizers-0.9.4/py_src/tokenizers/__init__.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -251,304 +251,448 @@
     """ A Regex """
 
     def __new__(pattern: str) -> Regex:
         """ Instantiate a new Regex with the given pattern """
         pass
 
 class Encoding:
-    """ An Encoding as returned by the Tokenizer """
+    """
+    The :class:`~tokenizers.Encoding` represents the output of a :class:`~tokenizers.Tokenizer`.
+    """
 
     @staticmethod
     def merge(encodings: List[Encoding], growing_offsets: bool = True) -> Encoding:
-        """Merge the list of Encoding into one final Encoding
+        """Merge the list of encodings into one final :class:`~tokenizers.Encoding`
 
         Args:
-            encodings: List[Encoding]:
-                The list of encodings
+            encodings (A :obj:`List` of :class:`~tokenizers.Encoding`):
+                The list of encodings that should be merged in one
 
-            growing_offsets: bool:
+            growing_offsets (:obj:`bool`, defaults to :obj:`True`):
                 Whether the offsets should accumulate while merging
 
         Returns:
-            The resulting Encoding
+            :class:`~tokenizers.Encoding`: The resulting Encoding
+        """
+        pass
+    @property
+    def n_sequences(self) -> int:
+        """The number of sequences represented
+
+        Returns:
+            :obj:`int`: The number of sequences in this :class:`~tokenizers.Encoding`
+        """
+        pass
+    def set_sequence_id(self, sequence_index: int):
+        """Set the given sequence index
+
+        Set the given sequence index for the whole range of tokens contained in this
+        :class:`~tokenizers.Encoding`.
         """
         pass
     @property
     def ids(self) -> List[int]:
-        """ The tokenized ids """
+        """The generated IDs
+
+        The IDs are the main input to a Language Model. They are the token indices,
+        the numerical representations that a LM understands.
+
+        Returns:
+            :obj:`List[int]`: The list of IDs
+        """
         pass
     @property
     def tokens(self) -> List[str]:
-        """ The tokenized strings """
+        """The generated tokens
+
+        They are the string representation of the IDs.
+
+        Returns:
+            :obj:`List[str]`: The list of tokens
+        """
         pass
     @property
     def words(self) -> List[Optional[int]]:
-        """ The tokenized words index """
+        """The generated word indices.
+
+        They represent the index of the word associated to each token.
+        When the input is pre-tokenized, they correspond to the ID of the given input label,
+        otherwise they correspond to the words indices as defined by the
+        :class:`~tokenizers.pre_tokenizers.PreTokenizer` that was used.
+
+        For special tokens and such (any token that was generated from something that was
+        not part of the input), the output is :obj:`None`
+
+        Returns:
+            A :obj:`List` of :obj:`Optional[int]`: A list of optional word index.
+        """
         pass
     @property
+    def sequences(self) -> List[Optional[int]]:
+        """The generated sequence indices.
+
+        They represent the index of the input sequence associated to each token.
+        The sequence id can be None if the token is not related to any input sequence,
+        like for example with special tokens.
+
+        Returns:
+            A :obj:`List` of :obj:`Optional[int]`: A list of optional sequence index.
+        """
+    @property
     def type_ids(self) -> List[int]:
-        """ The type ids """
+        """The generated type IDs
+
+        Generally used for tasks like sequence classification or question answering,
+        these tokens let the LM know which input sequence corresponds to each tokens.
+
+        Returns:
+            :obj:`List[int]`: The list of type ids
+        """
         pass
     @property
     def offsets(self) -> List[Offsets]:
-        """The offsets.
-        These offsets can be used to index any `IndexableString` directly. If you want to
-        index the original `str`, make sure to retrieve the converted offsets using the `.offsets`
-        method on the `original_str`.
+        """The offsets associated to each token
+
+        These offsets let's you slice the input string, and thus retrieve the original
+        part that led to producing the corresponding token.
+
+        Returns:
+            A :obj:`List` of :obj:`Tuple[int, int]`: The list of offsets
         """
         pass
     @property
     def special_tokens_mask(self) -> List[int]:
-        """ The special tokens mask """
+        """The special token mask
+
+        This indicates which tokens are special tokens, and which are not.
+
+        Returns:
+            :obj:`List[int]`: The special tokens mask
+        """
         pass
     @property
     def attention_mask(self) -> List[int]:
-        """ The attention mask """
+        """The attention mask
+
+        This indicates to the LM which tokens should be attended to, and which should not.
+        This is especially important when batching sequences, where we need to applying
+        padding.
+
+        Returns:
+           :obj:`List[int]`: The attention mask
+        """
         pass
     @property
     def overflowing(self) -> Optional[Encoding]:
-        """ The overflowing encoding, after truncation """
-        pass
-    def word_to_tokens(self, word_index: int) -> Optional[Tuple[int, int]]:
+        """A :obj:`List` of overflowing :class:`~tokenizers.Encoding`
+
+        When using truncation, the :class:`~tokenizers.Tokenizer` takes care of splitting
+        the output into as many pieces as required to match the specified maximum length.
+        This field lets you retrieve all the subsequent pieces.
+
+        When you use pairs of sequences, the overflowing pieces will contain enough
+        variations to cover all the possible combinations, while respecting the provided
+        maximum length.
         """
-        Get the encoded tokens corresponding to the word at the given index in the input
-        sequence, with the form [start_token, end_token + 1]
+        pass
+    def word_to_tokens(self, word_index: int, sequence_index: int = 0) -> Optional[Tuple[int, int]]:
+        """Get the encoded tokens corresponding to the word at the given index
+        in one of the input sequences.
 
         Args:
-            word_index: int:
-                The index of the word in the input sequence.
+            word_index (:obj:`int`):
+                The index of a word in one of the input sequences.
+            sequence_index (:obj:`int`, defaults to :obj:`0`):
+                The index of the sequence that contains the target word
 
         Returns:
-            The range of tokens with the form [start_token, end_token + 1]
+            :obj:`Tuple[int, int]`: The range of tokens: :obj:`(first, last + 1)`
         """
         pass
-    def word_to_chars(self, word_index: int) -> Optional[Offsets]:
+    def word_to_chars(self, word_index: int, sequence_index: int = 0) -> Optional[Offsets]:
+        """Get the offsets of the word at the given index in one of the input sequences.
+
+        Args:
+            word_index (:obj:`int`):
+                The index of a word in one of the input sequences.
+            sequence_index (:obj:`int`, defaults to :obj:`0`):
+                The index of the sequence that contains the target word
+
+        Returns:
+            :obj:`Tuple[int, int]`: The range of characters (span) :obj:`(first, last + 1)`
         """
-        Get the offsets of the word at the given index in the input sequence.
+        pass
+    def token_to_sequence(self, token_index: int) -> Optional[int]:
+        """Get the index of the sequence represented by the given token.
+
+        In the general use case, this method returns :obj:`0` for a single sequence or
+        the first sequence of a pair, and :obj:`1` for the second sequence of a pair
 
         Args:
-            word_index: int:
-                The index of the word in the input sequence.
+            token_index (:obj:`int`):
+                The index of a token in the encoded sequence.
 
         Returns:
-            The word offsets
+            :obj:`int`: The sequence id of the given token
         """
         pass
     def token_to_chars(self, token_index: int) -> Optional[Offsets]:
-        """
-        Get the offsets of the token at the given index
+        """Get the offsets of the token at the given index.
+
+        The returned offsets are related to the input sequence that contains the
+        token.  In order to determine in which input sequence it belongs, you
+        must call :meth:`~tokenizers.Encoding.token_to_sequence()`.
 
         Args:
-            token_index: int:
-                The index of the token in the encoded sequence.
+            token_index (:obj:`int`):
+                The index of a token in the encoded sequence.
 
         Returns:
-            The token offsets
+            :obj:`Tuple[int, int]`: The token offsets :obj:`(first, last + 1)`
         """
         pass
     def token_to_word(self, token_index: int) -> Optional[int]:
-        """
-        Get the word that contains the token at the given index
+        """Get the index of the word that contains the token in one of the input sequences.
+
+        The returned word index is related to the input sequence that contains
+        the token.  In order to determine in which input sequence it belongs, you
+        must call :meth:`~tokenizers.Encoding.token_to_sequence()`.
 
         Args:
-            token_index: int:
-                The index of the token in the encoded sequence.
+            token_index (:obj:`int`):
+                The index of a token in the encoded sequence.
 
         Returns:
-            The index of the word in the input sequence.
+            :obj:`int`: The index of the word in the relevant input sequence.
         """
         pass
-    def char_to_token(self, pos: int) -> Optional[int]:
-        """
-        Get the token that contains the char at the given position
+    def char_to_token(self, pos: int, sequence_index: int = 0) -> Optional[int]:
+        """Get the token that contains the char at the given position in the input sequence.
 
         Args:
-            pos: int:
+            char_pos (:obj:`int`):
                 The position of a char in the input string
+            sequence_index (:obj:`int`, defaults to :obj:`0`):
+                The index of the sequence that contains the target char
 
         Returns:
-            The index of the token that contains this char
+            :obj:`int`: The index of the token that contains this char in the encoded sequence
         """
         pass
-    def char_to_word(self, pos: int) -> Optional[int]:
-        """
-        Get the word that contains the given char.
+    def char_to_word(self, pos: int, sequence_index: int = 0) -> Optional[int]:
+        """Get the word that contains the char at the given position in the input sequence.
 
         Args:
-            pos: int:
+            char_pos (:obj:`int`):
                 The position of a char in the input string
+            sequence_index (:obj:`int`, defaults to :obj:`0`):
+                The index of the sequence that contains the target char
 
         Returns:
-            The index of the word that contains this char
+            :obj:`int`: The index of the word that contains this char in the input sequence
         """
         pass
     def pad(
         self,
         length: int,
         pad_id: Optional[int] = 0,
         pad_type_id: Optional[int] = 0,
         pad_token: Optional[str] = "[PAD]",
         direction: Optional[str] = "right",
     ):
-        """Pad the current Encoding at the given length
+        """Pad the :class:`~tokenizers.Encoding` at the given length
 
         Args:
-            length: int:
-                The length at which to pad
+            length (:obj:`int`):
+                The desired length
 
-            direction: (`optional`) str:
-                Can be one of: `right` or `left`
+            direction: (:obj:`str`, defaults to :obj:`right`):
+                The expected padding direction. Can be either :obj:`right` or :obj:`left`
 
-            pad_id: (`optional`) unsigned int:
-                The indice to be used when padding
+            pad_id (:obj:`int`, defaults to :obj:`0`):
+                The ID corresponding to the padding token
 
-            pad_type_id: (`optional`) unsigned int:
-                The type indice to be used when padding
+            pad_type_id (:obj:`int`, defaults to :obj:`0`):
+                The type ID corresponding to the padding token
 
-            pad_token: (`optional`) str:
-                The pad token to be used when padding
+            pad_token (:obj:`str`, defaults to `[PAD]`):
+                The pad token to use
         """
         pass
     def truncate(self, max_length: int, stride: Optional[int] = 0):
-        """Truncate the current Encoding at the given max_length
+        """Truncate the :class:`~tokenizers.Encoding` at the given length
+
+        If this :class:`~tokenizers.Encoding` represents multiple sequences, when truncating
+        this information is lost. It will be considered as representing a single sequence.
 
         Args:
-            max_length: int:
-                The maximum length to be kept
+            max_length (:obj:`int`):
+                The desired length
 
-            stride: (`optional`) unsigned int:
-                The length of the previous first sequence to be included
-                in the overflowing sequence
+            stride (:obj:`int`, defaults to :obj:`0`):
+                The length of previous content to be included in each overflowing piece
         """
         pass
 
 class AddedToken:
-    """AddedToken represents a token to be added to a Tokenizer
+    """AddedToken
+
+    Represents a token that can be be added to a :class:`~tokenizers.Tokenizer`.
+    It can have special options that defines the way it should behave.
 
-    An AddedToken can have special options defining the way it should behave.
+    Args:
+        content (:obj:`str`): The content of the token
+
+        single_word (:obj:`bool`, defaults to :obj:`False`):
+            Defines whether this token should only match single words. If :obj:`True`, this
+            token will never match inside of a word. For example the token ``ing`` would match
+            on ``tokenizing`` if this option is :obj:`False`, but not if it is :obj:`True`.
+            The notion of "`inside of a word`" is defined by the word boundaries pattern in
+            regular expressions (ie. the token should start and end with word boundaries).
+
+        lstrip (:obj:`bool`, defaults to :obj:`False`):
+            Defines whether this token should strip all potential whitespaces on its left side.
+            If :obj:`True`, this token will greedily match any whitespace on its left. For
+            example if we try to match the token ``[MASK]`` with ``lstrip=True``, in the text
+            ``"I saw a [MASK]"``, we would match on ``" [MASK]"``. (Note the space on the left).
+
+        rstrip (:obj:`bool`, defaults to :obj:`False`):
+            Defines whether this token should strip all potential whitespaces on its right
+            side. If :obj:`True`, this token will greedily match any whitespace on its right.
+            It works just like :obj:`lstrip` but on the right.
+
+        normalized (:obj:`bool`, defaults to :obj:`True` with :meth:`~tokenizers.Tokenizer.add_tokens` and :obj:`False` with :meth:`~tokenizers.Tokenizer.add_special_tokens`):
+            Defines whether this token should match against the normalized version of the input
+            text. For example, with the added token ``"yesterday"``, and a normalizer in charge of
+            lowercasing the text, the token could be extract from the input ``"I saw a lion
+            Yesterday"``.
     """
 
     def __new__(
         cls,
         content: str = "",
         single_word: bool = False,
         lstrip: bool = False,
         rstrip: bool = False,
         normalized: bool = True,
     ) -> AddedToken:
         """Instantiate a new AddedToken
 
         Args:
-            content: str:
-                The content of the token
+            content (:obj:`str`): The content of the token
 
-            single_word: bool
-                Whether this token should only match against single words. If True,
-                this token will never match inside of a word. For example the token `ing` would
-                match on `tokenizing` if this option if False, but not if this option is True.
-
-            lstrip: bool
-                Whether this token should strip all potential whitespaces on the left side.
-                If True, this token will greedily match any whitespace on the left. For example,
-                if we try to match the token `[MASK]` with lstrip=True, in the text `I saw a [MASK]`
-                we will match on ` [MASK]`.
-
-            rstrip: bool
-                Whether this token should strip all potential whitespaces on the right side.
-                If True, this token will greedily match any whitespace on the right. It works just
-                like lstrip, but on the right.
-
-            normalized: bool:
-                Whether this token should be match the normalized version of the input text. For
-                example, with the added token `yesterday` and a normalizer in charge of lowercasing
-                the text, the token could be extract from the input `I saw a lion Yesterday`.
+            single_word (:obj:`bool`, defaults to :obj:`False`):
+                Defines whether this token should only match single words. If :obj:`True`, this
+                token will never match inside of a word. For example the token ``ing`` would match
+                on ``tokenizing`` if this option is :obj:`False`, but not if it is :obj:`True`.
+                The notion of "`inside of a word`" is defined by the word boundaries pattern in
+                regular expressions (ie. the token should start and end with word boundaries).
+
+            lstrip (:obj:`bool`, defaults to :obj:`False`):
+                Defines whether this token should strip all potential whitespaces on its left side.
+                If :obj:`True`, this token will greedily match any whitespace on its left. For
+                example if we try to match the token ``[MASK]`` with ``lstrip=True``, in the text
+                ``"I saw a [MASK]"``, we would match on ``" [MASK]"``. (Note the space on the left).
+
+            rstrip (:obj:`bool`, defaults to :obj:`False`):
+                Defines whether this token should strip all potential whitespaces on its right
+                side. If :obj:`True`, this token will greedily match any whitespace on its right.
+                It works just like :obj:`lstrip` but on the right.
+
+            normalized (:obj:`bool`, defaults to :obj:`True` with :meth:`~tokenizers.Tokenizer.add_tokens` and :obj:`False` with :meth:`~tokenizers.Tokenizer.add_special_tokens`):
+                Defines whether this token should match against the normalized version of the input
+                text. For example, with the added token ``"yesterday"``, and a normalizer in charge of
+                lowercasing the text, the token could be extract from the input ``"I saw a lion
+                Yesterday"``.
         """
         pass
 
 class Tokenizer:
     """Tokenizer
 
-    A Tokenizer works as a pipeline, it processes some raw text as input and outputs
-    an `Encoding`.
+    A :obj:`Tokenizer` works as a pipeline. It processes some raw text as input
+    and outputs an :class:`~tokenizers.Encoding`.
 
-    The various steps of the pipeline are:
-        1. The `Normalizer`: in charge of normalizing the text. Common examples of
-           normalization are the unicode normalization standards, such as NFD or NFKC.
-        2. The `PreTokenizer`: in charge of creating initial words splits in the text.
-           The most common way of splitting text is simply on whitespace.
-        3. The `Model`: in charge of doing the actual tokenization. An example of a
-           `Model` would be `BPE` or `WordPiece`.
-        4. The `PostProcessor`: in charge of post-processing the `Encoding` to add anything
-           relevant that, for example, a language model would need, such as special tokens.
+    Args:
+        model (:class:`~tokenizers.models.Model`):
+            The core algorithm that this :obj:`Tokenizer` should be using.
     """
 
     def __new__(cls, model: models.Model) -> Tokenizer:
         """Instantiate a new Tokenizer using the given Model
 
+        A :obj:`Tokenizer` works as a pipeline. It processes some raw text as input
+        and outputs an :class:`~tokenizers.Encoding`.
+
         Args:
-            model: models.Model:
-                The model to be used with this Tokenizer
+            model (:class:`~tokenizers.models.Model`):
+                The core algorithm that this :obj:`Tokenizer` should be using.
 
         Returns:
             Tokenizer
         """
         pass
     @staticmethod
     def from_str(s: str) -> Tokenizer:
-        """Instantiate a new Tokenizer from the given JSON string
+        """Instantiate a new :class:`~tokenizers.Tokenizer` from the given JSON string.
 
         Args:
-            s: str:
-                A JSON string representation of the Tokenizer
+            json (:obj:`str`):
+                A valid JSON string representing a previously serialized
+                :class:`~tokenizers.Tokenizer`
 
         Returns:
-            Tokenizer
+            :class:`~tokenizers.Tokenizer`: The new tokenizer
         """
         pass
     @staticmethod
     def from_file(path: str) -> Tokenizer:
-        """Instantiate a new Tokenizer from the given file
+        """Instantiate a new :class:`~tokenizers.Tokenizer` from the file at the given path.
 
         Args:
-            path: str:
-                Path to a file containing a Tokenizer
+            path (:obj:`str`):
+                A path to a local JSON file representing a previously serialized
+                :class:`~tokenizers.Tokenizer`
 
         Returns:
-            Tokenizer
+            :class:`~tokenizers.Tokenizer`: The new tokenizer
         """
         pass
     @staticmethod
     def from_buffer(buffer: bytes) -> Tokenizer:
-        """Instantiate a new Tokenizer from the given buffer
+        """Instantiate a new :class:`~tokenizers.Tokenizer` from the given buffer.
 
         Args:
-            buffer: bytes:
-                A buffer used to instantiate a new Tokenizer
+            buffer (:obj:`bytes`):
+                A buffer containing a previously serialized :class:`~tokenizers.Tokenizer`
 
         Returns:
-            Tokenizer
+            :class:`~tokenizers.Tokenizer`: The new tokenizer
         """
         pass
     def to_str(self, pretty: bool = False) -> str:
-        """Get a serialized JSON version of the Tokenizer as a str
+        """Gets a serialized string representing this :class:`~tokenizers.Tokenizer`.
 
         Args:
-            pretty: bool:
-                Whether the JSON string should be prettified
+            pretty (:obj:`bool`, defaults to :obj:`False`):
+                Whether the JSON string should be pretty formatted.
 
         Returns:
-            str
+            :obj:`str`: A string representing the serialized Tokenizer
         """
         pass
     def save(self, path: str, pretty: bool = False):
-        """Save the Tokenizer as JSON to the given path
+        """Save the :class:`~tokenizers.Tokenizer` to the file at the given path.
 
         Args:
-            pretty: bool:
-                Whether the JSON string should be prettified
+            path (:obj:`str`):
+                A path to a file in which to save the serialized tokenizer.
+
+            pretty (:obj:`bool`, defaults to :obj:`False`):
+                Whether the JSON file should be pretty formatted.
         """
         pass
     @property
     def model(self) -> Model:
         """ Get the model in use with this Tokenizer """
         pass
     @model.setter
@@ -589,268 +733,305 @@
         """
         Return the number of special tokens that would be added for single/pair sentences.
         :param is_pair: Boolean indicating if the input would be a single sentence or a pair
         :return:
         """
         pass
     def get_vocab(self, with_added_tokens: bool = True) -> Dict[str, int]:
-        """Returns the vocabulary
+        """Get the underlying vocabulary
 
         Args:
-            with_added_tokens: boolean:
-                Whether to include the added tokens in the vocabulary
+            with_added_tokens (:obj:`bool`, defaults to :obj:`True`):
+                Whether to include the added tokens
 
         Returns:
-            The vocabulary
+            :obj:`Dict[str, int]`: The vocabulary
         """
         pass
     def get_vocab_size(self, with_added_tokens: bool = True) -> int:
-        """Returns the size of the vocabulary
+        """Get the size of the underlying vocabulary
 
         Args:
-            with_added_tokens: boolean:
-                Whether to include the added tokens in the vocabulary's size
+            with_added_tokens (:obj:`bool`, defaults to :obj:`True`):
+                Whether to include the added tokens
 
         Returns:
-            The size of the vocabulary
+            :obj:`int`: The size of the vocabulary
         """
         pass
     def enable_truncation(self, max_length: int, stride: Optional[int], strategy: Optional[str]):
-        """Enable the truncation
+        """Enable truncation
 
         Args:
-            max_length: unsigned int:
-                The maximum length at which to truncate
+            max_length (:obj:`int`):
+                The max length at which to truncate
 
-            stride: (`optional`) unsigned int:
-                The length of the previous first sequence to be included
-                in the overflowing sequence
+            stride (:obj:`int`, `optional`):
+                The length of the previous first sequence to be included in the overflowing
+                sequence
 
-            strategy: (`optional) str:
-                Can be one of `longest_first`, `only_first` or `only_second`
+            strategy (:obj:`str`, `optional`, defaults to :obj:`longest_first`):
+                The strategy used to truncation. Can be one of ``longest_first``, ``only_first`` or
+                ``only_second``.
         """
         pass
     def no_truncation(self):
         """ Disable truncation """
         pass
     @property
     def truncation(self) -> Optional[dict]:
-        """Get the current truncation parameters
+        """Get the currently set truncation parameters
+
+        `Cannot set, use` :meth:`~tokenizers.Tokenizer.enable_truncation` `instead`
 
         Returns:
-            None if truncation is disabled, a dict with the current truncation parameters if
-            truncation is enabled
+            (:obj:`dict`, `optional`):
+                A dict with the current truncation parameters if truncation is enabled
         """
         pass
     def enable_padding(
         self,
         direction: Optional[str] = "right",
         pad_to_multiple_of: Optional[int] = None,
         pad_id: Optional[int] = 0,
         pad_type_id: Optional[int] = 0,
         pad_token: Optional[str] = "[PAD]",
         length: Optional[int] = None,
     ):
         """Enable the padding
 
         Args:
-            direction: (`optional`) str:
-                Can be one of: `right` or `left`
+            direction (:obj:`str`, `optional`, defaults to :obj:`right`):
+                The direction in which to pad. Can be either ``right`` or ``left``
 
-            pad_to_multiple_of: (`optional`) unsigned int:
-                If specified, the padding length should always snap to the next multiple of
-                the given value. For example if we were going to pad with a length of 250 but
-                `pad_to_multiple_of=8` then we will pad to 256.
+            pad_to_multiple_of (:obj:`int`, `optional`):
+                If specified, the padding length should always snap to the next multiple of the
+                given value. For example if we were going to pad witha length of 250 but
+                ``pad_to_multiple_of=8`` then we will pad to 256.
 
-            pad_id: (`optional`) unsigned int:
-                The indice to be used when padding
+            pad_id (:obj:`int`, defaults to 0):
+                The id to be used when padding
 
-            pad_type_id: (`optional`) unsigned int:
-                The type indice to be used when padding
+            pad_type_id (:obj:`int`, defaults to 0):
+                The type id to be used when padding
 
-            pad_token: (`optional`) str:
+            pad_token (:obj:`str`, defaults to :obj:`[PAD]`):
                 The pad token to be used when padding
 
-            length: (`optional`) unsigned int:
-                If specified, the length at which to pad. If not specified
-                we pad using the size of the longest sequence in a batch
+            length (:obj:`int`, `optional`):
+                If specified, the length at which to pad. If not specified we pad using the size of
+                the longest sequence in a batch.
         """
         pass
     def no_padding(self):
         """ Disable padding """
         pass
     @property
     def padding(self) -> Optional[dict]:
         """Get the current padding parameters
 
+        `Cannot be set, use` :meth:`~tokenizers.Tokenizer.enable_padding` `instead`
+
         Returns:
-            None if padding is disabled, a dict with the currently set parameters
-            if the padding is enabled.
+            (:obj:`dict`, `optional`):
+                A dict with the current padding parameters if padding is enabled
         """
         pass
     def encode(
         self,
         sequence: InputSequence,
         pair: Optional[InputSequence],
         is_pretokenized: bool = False,
         add_special_tokens: bool = True,
     ) -> Encoding:
-        """Encode the given sequence and pair. This method can process raw text sequences as well
-        as already pre-tokenized sequences.
+        """Encode the given sequence and pair. This method can process raw text sequences
+        as well as already pre-tokenized sequences.
+
+        Example:
+            Here are some examples of the inputs that are accepted::
+
+                encode("A single sequence")`
+                encode("A sequence", "And its pair")`
+                encode([ "A", "pre", "tokenized", "sequence" ], is_pretokenized=True)`
+                encode(
+                    [ "A", "pre", "tokenized", "sequence" ], [ "And", "its", "pair" ],
+                    is_pretokenized=True
+                )
 
         Args:
-            sequence: InputSequence:
-                The sequence we want to encode. This sequence can be either raw text or
-                pre-tokenized, according to the `is_pretokenized` argument:
+            sequence (:obj:`~tokenizers.InputSequence`):
+                The main input sequence we want to encode. This sequence can be either raw
+                text or pre-tokenized, according to the ``is_pretokenized`` argument:
 
-                - If `is_pretokenized=False`: `InputSequence` is expected to be `str`
-                - If `is_pretokenized=True`: `InputSequence` is expected to be
-                    `Union[List[str], Tuple[str]]`
+                - If ``is_pretokenized=False``: :class:`~tokenizers.TextInputSequence`
+                - If ``is_pretokenized=True``: :class:`~tokenizers.PreTokenizedInputSequence`
 
-            is_pretokenized: bool:
+            pair (:obj:`~tokenizers.InputSequence`, `optional`):
+                An optional input sequence. The expected format is the same that for ``sequence``.
+
+            is_pretokenized (:obj:`bool`, defaults to :obj:`False`):
                 Whether the input is already pre-tokenized
 
-            add_special_tokens: bool:
-                Whether to add the special tokens while encoding.
+            add_special_tokens (:obj:`bool`, defaults to :obj:`True`):
+                Whether to add the special tokens
 
         Returns:
-            An Encoding
+            :class:`~tokenizers.Encoding`: The encoded result
         """
         pass
     def encode_batch(
         self,
         inputs: List[EncodeInput],
         is_pretokenized: bool = False,
         add_special_tokens: bool = True,
     ) -> List[Encoding]:
-        """Encode the given inputs. This method accept both raw text sequences as well as already
-        pre-tokenized sequences.
+        """Encode the given batch of inputs. This method accept both raw text sequences
+        as well as already pre-tokenized sequences.
 
-        Args:
-            inputs: List[EncodeInput]:
-                A list of single sequences or pair sequences to encode. Each `EncodeInput` is
-                expected to be of the following form:
-                    `Union[InputSequence, Tuple[InputSequence, InputSequence]]`
+        Example:
+            Here are some examples of the inputs that are accepted::
 
-                Each `InputSequence` can either be raw text or pre-tokenized,
-                according to the `is_pretokenized` argument:
+                encode_batch([
+                    "A single sequence",
+                    ("A tuple with a sequence", "And its pair"),
+                    [ "A", "pre", "tokenized", "sequence" ],
+                    ([ "A", "pre", "tokenized", "sequence" ], "And its pair")
+                ])
 
-                - If `is_pretokenized=False`: `InputSequence` is expected to be `str`
-                - If `is_pretokenized=True`: `InputSequence` is expected to be
-                    `Union[List[str], Tuple[str]]`
+        Args:
+            input (A :obj:`List`/:obj:`Tuple` of :obj:`~tokenizers.EncodeInput`):
+                A list of single sequences or pair sequences to encode. Each sequence
+                can be either raw text or pre-tokenized, according to the ``is_pretokenized``
+                argument:
 
-            is_pretokenized: bool:
-                Whether the input is already pre-tokenized.
+                - If ``is_pretokenized=False``: :class:`~tokenizers.TextEncodeInput`
+                - If ``is_pretokenized=True``: :class:`~tokenizers.PreTokenizedEncodeInput`
+
+            is_pretokenized (:obj:`bool`, defaults to :obj:`False`):
+                Whether the input is already pre-tokenized
 
-            add_special_tokens: bool:
-                Whether to add the special tokens while encoding.
+            add_special_tokens (:obj:`bool`, defaults to :obj:`True`):
+                Whether to add the special tokens
 
         Returns:
-            A list of Encoding
+            A :obj:`List` of :class:`~tokenizers.Encoding`: The encoded batch
+
         """
         pass
     def decode(self, ids: List[int], skip_special_tokens: Optional[bool] = True) -> str:
-        """Decode the given list of ids to a string sequence
+        """Decode the given list of ids back to a string
+
+        This is used to decode anything coming back from a Language Model
 
         Args:
-            ids: List[unsigned int]:
-                A list of ids to be decoded
+            ids (A :obj:`List/Tuple` of :obj:`int`):
+                The list of ids that we want to decode
 
-            skip_special_tokens: (`optional`) boolean:
-                Whether to remove all the special tokens from the output string
+            skip_special_tokens (:obj:`bool`, defaults to :obj:`True`):
+                Whether the special tokens should be removed from the decoded string
 
         Returns:
-            The decoded string
+            :obj:`str`: The decoded string
         """
         pass
     def decode_batch(
         self, sequences: List[List[int]], skip_special_tokens: Optional[bool] = True
     ) -> str:
-        """Decode the list of sequences to a list of string sequences
+        """Decode a batch of ids back to their corresponding string
 
         Args:
-            sequences: List[List[unsigned int]]:
-                A list of sequence of ids to be decoded
+            sequences (:obj:`List` of :obj:`List[int]`):
+                The batch of sequences we want to decode
 
-            skip_special_tokens: (`optional`) boolean:
-                Whether to remove all the special tokens from the output strings
+            skip_special_tokens (:obj:`bool`, defaults to :obj:`True`):
+                Whether the special tokens should be removed from the decoded strings
 
         Returns:
-            A list of decoded strings
+            :obj:`List[str]`: A list of decoded strings
         """
         pass
     def token_to_id(self, token: str) -> Optional[int]:
-        """Convert the given token to its corresponding id
+        """Convert the given token to its corresponding id if it exists
 
         Args:
-            token: str:
+            token (:obj:`str`):
                 The token to convert
 
         Returns:
-            The corresponding id if it exists, None otherwise
+            :obj:`Optional[int]`: An optional id, :obj:`None` if out of vocabulary
         """
         pass
     def id_to_token(self, id: int) -> Optional[str]:
-        """Convert the given token id to its corresponding string
+        """Convert the given id to its corresponding token if it exists
 
         Args:
-            token: id:
-                The token id to convert
+            id (:obj:`int`):
+                The id to convert
 
         Returns:
-            The corresponding string if it exists, None otherwise
+            :obj:`Optional[str]`: An optional token, :obj:`None` if out of vocabulary
         """
         pass
     def add_tokens(self, tokens: List[Union[str, AddedToken]]) -> int:
         """Add the given tokens to the vocabulary
 
+        The given tokens are added only if they don't already exist in the vocabulary.
+        Each token then gets a new attributed id.
+
         Args:
-            tokens: List[Union[str, AddedToken]]:
-                A list of tokens to add to the vocabulary. Each token can either be
-                a string, or an instance of AddedToken
+            tokens (A :obj:`List` of :class:`~tokenizers.AddedToken` or :obj:`str`):
+                The list of tokens we want to add to the vocabulary. Each token can be either a
+                string or an instance of :class:`~tokenizers.AddedToken` for more customization.
 
         Returns:
-            The number of tokens that were added to the vocabulary
+            :obj:`int`: The number of tokens that were created in the vocabulary
         """
         pass
     def add_special_tokens(self, tokens: List[Union[str, AddedToken]]) -> int:
-        """Add the given special tokens to the vocabulary, and treat them as special tokens.
+        """Add the given special tokens to the Tokenizer.
 
-        The special tokens will never be processed by the model, and will be
-        removed while decoding.
+        If these tokens are already part of the vocabulary, it just let the Tokenizer know about
+        them. If they don't exist, the Tokenizer creates them, giving them a new id.
+
+        These special tokens will never be processed by the model (ie won't be split into
+        multiple tokens), and they can be removed from the output when decoding.
 
         Args:
-            tokens: List[Union[str, AddedToken]]:
-                The list of special tokens to add. Each token can either be a string
-                or an instance of AddedToken
+            tokens (A :obj:`List` of :class:`~tokenizers.AddedToken` or :obj:`str`):
+                The list of special tokens we want to add to the vocabulary. Each token can either
+                be a string or an instance of :class:`~tokenizers.AddedToken` for more
+                customization.
 
         Returns:
-            The number of tokens that were added to the vocabulary
+            :obj:`int`: The number of tokens that were created in the vocabulary
         """
         pass
     def post_process(
         self,
         encoding: Encoding,
         pair: Optional[Encoding] = None,
         add_special_tokens: bool = True,
     ) -> Encoding:
         """Apply all the post-processing steps to the given encodings.
 
         The various steps are:
-            1. Truncate according to global params (provided to `enable_truncation`)
-            2. Apply the PostProcessor
-            3. Pad according to global params. (provided to `enable_padding`)
+
+            1. Truncate according to the set truncation params (provided with
+               :meth:`~tokenizers.Tokenizer.enable_truncation`)
+            2. Apply the :class:`~tokenizers.processors.PostProcessor`
+            3. Pad according to the set padding params (provided with
+               :meth:`~tokenizers.Tokenizer.enable_padding`)
 
         Args:
-            encoding: Encoding:
-                The main Encoding to post process
+            encoding (:class:`~tokenizers.Encoding`):
+                The :class:`~tokenizers.Encoding` corresponding to the main sequence.
 
-            pair: Optional[Encoding]:
-                An optional pair Encoding
+            pair (:class:`~tokenizers.Encoding`, `optional`):
+                An optional :class:`~tokenizers.Encoding` corresponding to the pair sequence.
 
-            add_special_tokens: bool:
-                Whether to add special tokens
+            add_special_tokens (:obj:`bool`):
+                Whether to add the special tokens
 
         Returns:
-            The resulting Encoding
+            :class:`~tokenizers.Encoding`: The final post-processed encoding
         """
         pass
```

### Comparing `tokenizers-0.9.3/py_src/tokenizers/decoders/__init__.pyi` & `tokenizers-0.9.4/py_src/tokenizers/decoders/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers/implementations/base_tokenizer.py` & `tokenizers-0.9.4/py_src/tokenizers/implementations/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers/implementations/bert_wordpiece.py` & `tokenizers-0.9.4/py_src/tokenizers/implementations/bert_wordpiece.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
             "strip_accents": strip_accents,
             "lowercase": lowercase,
             "wordpieces_prefix": wordpieces_prefix,
         }
 
         super().__init__(tokenizer, parameters)
 
+    @staticmethod
     def from_file(vocab: str, **kwargs):
         vocab = WordPiece.read_file(vocab)
         return BertWordPieceTokenizer(vocab, **kwargs)
 
     def train(
         self,
         files: Union[str, List[str]],
```

### Comparing `tokenizers-0.9.3/py_src/tokenizers/implementations/byte_level_bpe.py` & `tokenizers-0.9.4/py_src/tokenizers/implementations/byte_level_bpe.py`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers/implementations/char_level_bpe.py` & `tokenizers-0.9.4/py_src/tokenizers/implementations/char_level_bpe.py`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers/implementations/sentencepiece_bpe.py` & `tokenizers-0.9.4/py_src/tokenizers/implementations/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers/implementations/sentencepiece_unigram.py` & `tokenizers-0.9.4/py_src/tokenizers/implementations/sentencepiece_unigram.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             import sys
 
             sys.path.append(".")
 
             import sentencepiece_model_pb2 as model
         except Exception:
             raise Exception(
-                "You don't seem to have the required protobuf file, in order to use this function you need to run `pip install protobuf` and `wget https://raw.githubusercontent.com/google/sentencepiece/master/python/sentencepiece_model_pb2.py` for us to be able to read the intrinsics of your spm_file. `pip install sentencepiece` is not required."
+                "You don't seem to have the required protobuf file, in order to use this function you need to run `pip install protobuf` and `wget https://raw.githubusercontent.com/google/sentencepiece/master/python/src/sentencepiece/sentencepiece_model_pb2.py` for us to be able to read the intrinsics of your spm_file. `pip install sentencepiece` is not required."
             )
 
         m = model.ModelProto()
         m.ParseFromString(open(filename, "rb").read())
 
         precompiled_charsmap = m.normalizer_spec.precompiled_charsmap
         vocab = [(piece.piece, piece.score) for piece in m.pieces]
```

### Comparing `tokenizers-0.9.3/py_src/tokenizers/models/__init__.pyi` & `tokenizers-0.9.4/py_src/tokenizers/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers/normalizers/__init__.py` & `tokenizers-0.9.4/py_src/tokenizers/normalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers/normalizers/__init__.pyi` & `tokenizers-0.9.4/py_src/tokenizers/normalizers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers/pre_tokenizers/__init__.pyi` & `tokenizers-0.9.4/py_src/tokenizers/pre_tokenizers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers/processors/__init__.pyi` & `tokenizers-0.9.4/py_src/tokenizers/processors/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers/trainers/__init__.pyi` & `tokenizers-0.9.4/py_src/tokenizers/trainers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/py_src/tokenizers.egg-info/PKG-INFO` & `tokenizers-0.9.4/py_src/tokenizers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenizers
-Version: 0.9.3
+Version: 0.9.4
 Summary: Fast and Customizable Tokenizers
 Home-page: https://github.com/huggingface/tokenizers
 Author: Anthony MOI
 Author-email: anthony@huggingface.co
 License: Apache License 2.0
 Description: <p align="center">
             <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tokenizers Version: 0.9.3 Summary: Fast and
+Metadata-Version: 2.1 Name: tokenizers Version: 0.9.4 Summary: Fast and
 Customizable Tokenizers Home-page: https://github.com/huggingface/tokenizers
 Author: Anthony MOI Author-email: anthony@huggingface.co License: Apache
 License 2.0 Description:
 
     [https://huggingface.co/landing/assets/tokenizers/tokenizers-logo.png]
                                 _[_B_u_i_l_d_]_[_G_i_t_H_u_b_]
```

### Comparing `tokenizers-0.9.3/py_src/tokenizers.egg-info/SOURCES.txt` & `tokenizers-0.9.4/py_src/tokenizers.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -111,11 +111,12 @@
 tokenizers-lib/src/utils/cache.rs
 tokenizers-lib/src/utils/iter.rs
 tokenizers-lib/src/utils/mod.rs
 tokenizers-lib/src/utils/padding.rs
 tokenizers-lib/src/utils/parallelism.rs
 tokenizers-lib/src/utils/truncation.rs
 tokenizers-lib/tests/added_tokens.rs
+tokenizers-lib/tests/documentation.rs
 tokenizers-lib/tests/offsets.rs
 tokenizers-lib/tests/serialization.rs
 tokenizers-lib/tests/unigram.rs
 tokenizers-lib/tests/common/mod.rs
```

### Comparing `tokenizers-0.9.3/setup.py` & `tokenizers-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools_rust import Binding, RustExtension
 
 extras = {}
 extras["testing"] = ["pytest"]
 
 setup(
     name="tokenizers",
-    version="0.9.3",
+    version="0.9.4",
     description="Fast and Customizable Tokenizers",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="NLP tokenizer BPE transformer deep learning",
     author="Anthony MOI",
     author_email="anthony@huggingface.co",
     url="https://github.com/huggingface/tokenizers",
```

### Comparing `tokenizers-0.9.3/src/decoders.rs` & `tokenizers-0.9.4/src/decoders.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/src/error.rs` & `tokenizers-0.9.4/src/error.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/src/lib.rs` & `tokenizers-0.9.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/src/models.rs` & `tokenizers-0.9.4/src/models.rs`

 * *Files 0% similar despite different names*

```diff
@@ -364,20 +364,22 @@
         let unk_token = PyWordLevel::get_unk(kwargs)?;
 
         if let Some(vocab) = vocab {
             let model = match vocab {
                 PyVocab::Vocab(vocab) => WordLevel::builder()
                     .vocab(vocab)
                     .unk_token(unk_token)
-                    .build(),
+                    .build()
+                    .expect("Can only fail when loading from files"),
                 PyVocab::Filename(vocab_filename) => {
                     deprecation_warning(
-                    "0.9.0",
-                    "WordLevel.__init__ will not create from files anymore, try `WordLevel.from_file` instead",
-                )?;
+                        "0.9.0",
+                        "WordLevel.__init__ will not create from files anymore, \
+                            try `WordLevel.from_file` instead",
+                    )?;
                     WordLevel::from_file(vocab_filename, unk_token).map_err(|e| {
                         exceptions::PyException::new_err(format!(
                             "Error while loading WordLevel: {}",
                             e
                         ))
                     })?
                 }
```

### Comparing `tokenizers-0.9.3/src/normalizers.rs` & `tokenizers-0.9.4/src/normalizers.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/src/pre_tokenizers.rs` & `tokenizers-0.9.4/src/pre_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/src/processors.rs` & `tokenizers-0.9.4/src/processors.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/src/token.rs` & `tokenizers-0.9.4/src/token.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/src/trainers.rs` & `tokenizers-0.9.4/src/trainers.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/src/utils/mod.rs` & `tokenizers-0.9.4/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/src/utils/normalization.rs` & `tokenizers-0.9.4/src/utils/normalization.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/src/utils/pretokenization.rs` & `tokenizers-0.9.4/src/utils/pretokenization.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/CHANGELOG.md` & `tokenizers-0.9.4/tokenizers-lib/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/Cargo.toml` & `tokenizers-0.9.4/tokenizers-lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/Makefile` & `tokenizers-0.9.4/tokenizers-lib/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 BENCHMARK_DIR = benches
 TESTS_DIR = tests
 
 dir_guard=@mkdir -p $(@D)
 
 SHARED_RESOURCES = $(DATA_DIR)/gpt2-vocab.json $(DATA_DIR)/gpt2-merges.txt $(DATA_DIR)/bert-base-uncased-vocab.txt $(DATA_DIR)/big.txt $(DATA_DIR)/small.txt
 BENCHMARK_RESOURCES = $(SHARED_RESOURCES)
-TESTS_RESOURCES = $(SHARED_RESOURCES) $(DATA_DIR)/unigram.json $(DATA_DIR)/unigram_wagahaiwa_nekodearu.txt $(DATA_DIR)/albert-base-v1-tokenizer.json
+TESTS_RESOURCES = $(SHARED_RESOURCES) $(DATA_DIR)/unigram.json $(DATA_DIR)/unigram_wagahaiwa_nekodearu.txt $(DATA_DIR)/albert-base-v1-tokenizer.json $(DATA_DIR)/roberta.json $(DATA_DIR)/tokenizer-wiki.json $(DATA_DIR)/bert-wiki.json
 
 .PHONY : build
 build :
 	cargo build --all-targets
 
 .PHONY : release
 release :
@@ -63,7 +63,19 @@
 
 $(DATA_DIR)/big.txt :
 	$(dir_guard)
 	wget https://norvig.com/big.txt -O $@
 
 $(DATA_DIR)/small.txt : $(DATA_DIR)/big.txt
 	head -100 $(DATA_DIR)/big.txt > $@
+
+$(DATA_DIR)/roberta.json :
+	$(dir_guard)
+	wget https://storage.googleapis.com/tokenizers/roberta.json -O $@
+
+$(DATA_DIR)/tokenizer-wiki.json :
+	$(dir_guard)
+	wget https://s3.amazonaws.com/models.huggingface.co/bert/anthony/doc-quicktour/tokenizer.json -O $@
+
+$(DATA_DIR)/bert-wiki.json :
+	$(dir_guard)
+	wget https://s3.amazonaws.com/models.huggingface.co/bert/anthony/doc-pipeline/tokenizer.json -O $@
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/README.md` & `tokenizers-0.9.4/tokenizers-lib/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -83,29 +83,29 @@
             AddedToken::from(String::from("<mask>"), true),
         ])
         .build();
 
     let tokenizer = TokenizerBuilder::new()
         .with_model(BPE::default())
         .with_normalizer(Some(Sequence::new(vec![
-            NormalizerWrapper::StripNormalizer(Strip::new(true, true)),
-            NormalizerWrapper::NFC(NFC),
+            Strip::new(true, true).into(),
+            NFC.into(),
         ])))
-        .with_pre_tokenizer(Some(PreTokenizerWrapper::ByteLevel(ByteLevel::default())))
-        .with_post_processor(Some(PostProcessorWrapper::ByteLevel(ByteLevel::default())))
-        .with_decoder(Some(DecoderWrapper::ByteLevel(ByteLevel::default())))
+        .with_pre_tokenizer(Some(ByteLevel::default()))
+        .with_post_processor(Some(ByteLevel::default()))
+        .with_decoder(Some(ByteLevel::default()))
         .build()?;
 
+    let pretty = false;
     tokenizer
         .train(
             &trainer,
             vec!["path/to/vocab.txt".to_string()],
         )?
-        .get_model()
-        .save(Path::new("result-folder"), Some("some-prefix"))?;
+        .save("tokenizer.json", pretty)?;
 
     Ok(())
 }
 ```
 
 ## Additional information
```

#### html2text {}

```diff
@@ -30,20 +30,18 @@
 TokenizerBuilder}; use std::path::Path; fn main() -> Result<()> { let
 vocab_size: usize = 100; let trainer = BpeTrainerBuilder::new() .show_progress
 (true) .vocab_size(vocab_size) .min_frequency(0) .special_tokens(vec!
 [ AddedToken::from(String::from(""), true), AddedToken::from(String::from(""),
 true), AddedToken::from(String::from(""), true), AddedToken::from(String::from
 (""), true), AddedToken::from(String::from(""), true), ]) .build(); let
 tokenizer = TokenizerBuilder::new() .with_model(BPE::default())
-.with_normalizer(Some(Sequence::new(vec![ NormalizerWrapper::StripNormalizer
-(Strip::new(true, true)), NormalizerWrapper::NFC(NFC), ]))) .with_pre_tokenizer
-(Some(PreTokenizerWrapper::ByteLevel(ByteLevel::default())))
-.with_post_processor(Some(PostProcessorWrapper::ByteLevel(ByteLevel::default
-()))) .with_decoder(Some(DecoderWrapper::ByteLevel(ByteLevel::default())))
-.build()?; tokenizer .train( &trainer, vec!["path/to/vocab.txt".to_string()],
-)? .get_model() .save(Path::new("result-folder"), Some("some-prefix"))?; Ok(())
+.with_normalizer(Some(Sequence::new(vec![ Strip::new(true, true).into(),
+NFC.into(), ]))) .with_pre_tokenizer(Some(ByteLevel::default()))
+.with_post_processor(Some(ByteLevel::default())) .with_decoder(Some(ByteLevel::
+default())) .build()?; let pretty = false; tokenizer .train( &trainer, vec!
+["path/to/vocab.txt".to_string()], )? .save("tokenizer.json", pretty)?; Ok(())
 } ``` ## Additional information - tokenizers is designed to leverage CPU
 parallelism when possible. The level of parallelism is determined by the total
 number of core/threads your CPU provides but this can be tuned by setting the
 `RAYON_RS_NUM_CPUS` environment variable. As an example setting
 `RAYON_RS_NUM_CPUS=4` will allocate a maximum of 4 threads. **_Please note this
 behavior may evolve in the future_**
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/README.tpl` & `tokenizers-0.9.4/tokenizers-lib/README.tpl`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/benches/bert_benchmark.rs` & `tokenizers-0.9.4/tokenizers-lib/benches/bert_benchmark.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/benches/bpe_benchmark.rs` & `tokenizers-0.9.4/tokenizers-lib/benches/bpe_benchmark.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/benches/common/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/benches/common/mod.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/cli.rs` & `tokenizers-0.9.4/tokenizers-lib/src/cli.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/decoders/bpe.rs` & `tokenizers-0.9.4/tokenizers-lib/src/decoders/bpe.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/decoders/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/src/decoders/mod.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/decoders/wordpiece.rs` & `tokenizers-0.9.4/tokenizers-lib/src/decoders/wordpiece.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/lib.rs` & `tokenizers-0.9.4/tokenizers-lib/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -70,29 +70,29 @@
 //!             AddedToken::from(String::from("<mask>"), true),
 //!         ])
 //!         .build();
 //!
 //!     let tokenizer = TokenizerBuilder::new()
 //!         .with_model(BPE::default())
 //!         .with_normalizer(Some(Sequence::new(vec![
-//!             NormalizerWrapper::StripNormalizer(Strip::new(true, true)),
-//!             NormalizerWrapper::NFC(NFC),
+//!             Strip::new(true, true).into(),
+//!             NFC.into(),
 //!         ])))
-//!         .with_pre_tokenizer(Some(PreTokenizerWrapper::ByteLevel(ByteLevel::default())))
-//!         .with_post_processor(Some(PostProcessorWrapper::ByteLevel(ByteLevel::default())))
-//!         .with_decoder(Some(DecoderWrapper::ByteLevel(ByteLevel::default())))
+//!         .with_pre_tokenizer(Some(ByteLevel::default()))
+//!         .with_post_processor(Some(ByteLevel::default()))
+//!         .with_decoder(Some(ByteLevel::default()))
 //!         .build()?;
 //!
+//!     let pretty = false;
 //!     tokenizer
 //!         .train(
 //!             &trainer,
 //!             vec!["path/to/vocab.txt".to_string()],
 //!         )?
-//!         .get_model()
-//!         .save(Path::new("result-folder"), Some("some-prefix"))?;
+//!         .save("tokenizer.json", pretty)?;
 //!
 //!     Ok(())
 //! }
 //! ```
 //!
 //! # Additional information
 //!
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/bpe/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/bpe/mod.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/bpe/model.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/bpe/model.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/bpe/serialization.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/bpe/serialization.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/bpe/trainer.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/bpe/trainer.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/bpe/word.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/bpe/word.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/unigram/lattice.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/unigram/lattice.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/unigram/model.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/unigram/model.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/unigram/serialization.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/unigram/serialization.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/unigram/trainer.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/unigram/trainer.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/unigram/trie.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/unigram/trie.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/wordlevel/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/wordlevel/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -27,66 +27,79 @@
             ),
             Error::BadVocabulary => write!(fmt, "Bad vocabulary json file"),
         }
     }
 }
 
 struct Config {
+    files: Option<String>,
     vocab: HashMap<String, u32>,
     unk_token: String,
 }
 
 /// A `WordLevelBuilder` can be used to create a `WordLevel`
 /// model with a custom configuration.
 pub struct WordLevelBuilder {
     config: Config,
 }
 
 impl Default for WordLevelBuilder {
     fn default() -> Self {
         Self {
             config: Config {
+                files: None,
                 vocab: HashMap::new(),
                 unk_token: String::from("<unk>"),
             },
         }
     }
 }
 
 impl WordLevelBuilder {
     /// Construct a new `WordLevelBuilder`.
     pub fn new() -> Self {
         Self::default()
     }
 
+    /// Set the input files.
+    pub fn files(mut self, vocab: String) -> Self {
+        self.config.files = Some(vocab);
+        self
+    }
+
     /// Set the vocab (token -> ID) mapping.
     pub fn vocab(mut self, vocab: HashMap<String, u32>) -> Self {
         self.config.vocab = vocab;
         self
     }
 
     /// The the `UNK` token for the vocab.
     pub fn unk_token(mut self, unk_token: String) -> Self {
         self.config.unk_token = unk_token;
         self
     }
 
     /// Contructs a `WordLevel` model that uses the `WordLevelBuilder`'s configuration.
-    pub fn build(self) -> WordLevel {
+    pub fn build(mut self) -> Result<WordLevel> {
+        if let Some(vocab) = self.config.files {
+            self.config.vocab = WordLevel::read_file(&vocab)?;
+        }
+
         let vocab_r = self
             .config
             .vocab
             .iter()
             .map(|(key, val)| (*val, key.to_owned()))
             .collect();
-        WordLevel {
+
+        Ok(WordLevel {
             vocab: self.config.vocab,
             vocab_r,
             unk_token: self.config.unk_token,
-        }
+        })
     }
 }
 
 #[derive(PartialEq, Clone)]
 pub struct WordLevel {
     vocab: HashMap<String, u32>,
     vocab_r: HashMap<u32, String>,
@@ -129,15 +142,15 @@
         };
         Ok(vocab)
     }
 
     /// Initialize a WordLevel model from vocab and merges file.
     pub fn from_file(vocab_path: &str, unk_token: String) -> Result<WordLevel> {
         let vocab = WordLevel::read_file(vocab_path)?;
-        Ok(Self::builder().vocab(vocab).unk_token(unk_token).build())
+        Self::builder().vocab(vocab).unk_token(unk_token).build()
     }
 }
 
 impl Default for WordLevel {
     fn default() -> Self {
         Self {
             vocab: HashMap::new(),
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/wordlevel/serialization.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/wordlevel/serialization.rs`

 * *Files 2% similar despite different names*

```diff
@@ -43,10 +43,10 @@
         while let Some(key) = map.next_key::<String>()? {
             match key.as_ref() {
                 "vocab" => builder = builder.vocab(map.next_value()?),
                 "unk_token" => builder = builder.unk_token(map.next_value()?),
                 _ => {}
             }
         }
-        Ok(builder.build())
+        Ok(builder.build().map_err(serde::de::Error::custom)?)
     }
 }
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/wordpiece/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/wordpiece/mod.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/wordpiece/serialization.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/wordpiece/serialization.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/models/wordpiece/trainer.rs` & `tokenizers-0.9.4/tokenizers-lib/src/models/wordpiece/trainer.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/normalizers/bert.rs` & `tokenizers-0.9.4/tokenizers-lib/src/normalizers/bert.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/normalizers/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/src/normalizers/mod.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/normalizers/precompiled.rs` & `tokenizers-0.9.4/tokenizers-lib/src/normalizers/precompiled.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/normalizers/replace.rs` & `tokenizers-0.9.4/tokenizers-lib/src/normalizers/replace.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/normalizers/strip.rs` & `tokenizers-0.9.4/tokenizers-lib/src/normalizers/strip.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/normalizers/unicode.rs` & `tokenizers-0.9.4/tokenizers-lib/src/normalizers/unicode.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/normalizers/utils.rs` & `tokenizers-0.9.4/tokenizers-lib/src/normalizers/utils.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/bert.rs` & `tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/bert.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/byte_level.rs` & `tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/byte_level.rs`

 * *Files 3% similar despite different names*

```diff
@@ -198,19 +198,20 @@
             }
         }
     });
 }
 
 #[cfg(test)]
 mod tests {
-    use super::ByteLevel;
+    use super::*;
     use crate::tokenizer::{
         Decoder, Encoding, OffsetReferential, OffsetType, PostProcessor, PreTokenizedString,
         PreTokenizer,
     };
+    use std::iter::FromIterator;
 
     #[test]
     fn pre_tokenization() {
         let bytelevel = ByteLevel::default().add_prefix_space(false);
         let mut pretokenized: PreTokenizedString = "Hello my friend, how is your day going?".into();
         bytelevel.pre_tokenize(&mut pretokenized).unwrap();
         assert_eq!(
@@ -380,53 +381,71 @@
             vec!["i", "⭢", "j"]
         );
     }
 
     #[test]
     fn processor_trims_offsets() {
         let start = Encoding::new(
-            vec![],
+            vec![0; 5],
             vec![],
             vec![
                 "Ġ".into(),
                 "ĠĠĠĠHelloĠĠ".into(),
                 "ĠĠHello".into(),
                 "HelloĠĠ".into(),
                 "ĠĠĠĠ".into(),
             ],
             vec![],
             vec![(0, 1), (0, 11), (11, 18), (18, 25), (25, 29)],
             vec![],
             vec![],
             vec![],
+            HashMap::new(),
         );
         let expected = Encoding::new(
-            vec![],
+            vec![0; 5],
             vec![],
             vec![
                 "Ġ".into(),
                 "ĠĠĠĠHelloĠĠ".into(),
                 "ĠĠHello".into(),
                 "HelloĠĠ".into(),
                 "ĠĠĠĠ".into(),
             ],
             vec![],
             vec![(0, 0), (4, 9), (13, 18), (18, 23), (29, 29)],
             vec![],
             vec![],
             vec![],
+            HashMap::new(),
         );
 
         let bytelevel = ByteLevel::default().trim_offsets(true);
         assert_eq!(
             expected,
             bytelevel.process(start.clone(), None, false).unwrap()
         );
 
-        let mut pair_expected = expected.clone();
+        let mut pair_expected = Encoding::new(
+            vec![0; 5],
+            vec![],
+            vec![
+                "Ġ".into(),
+                "ĠĠĠĠHelloĠĠ".into(),
+                "ĠĠHello".into(),
+                "HelloĠĠ".into(),
+                "ĠĠĠĠ".into(),
+            ],
+            vec![],
+            vec![(0, 0), (4, 9), (13, 18), (18, 23), (29, 29)],
+            vec![],
+            vec![],
+            vec![],
+            HashMap::from_iter(vec![(0, 0..5), (1, 5..10)]),
+        );
         pair_expected.merge_with(expected, false);
         assert_eq!(
             pair_expected,
             bytelevel
                 .process(start.clone(), Some(start), false)
                 .unwrap()
         );
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/delimiter.rs` & `tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/delimiter.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/digits.rs` & `tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/digits.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/metaspace.rs` & `tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/metaspace.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/mod.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/punctuation.rs` & `tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/punctuation.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/sequence.rs` & `tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/sequence.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/unicode_scripts/pre_tokenizer.rs` & `tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/unicode_scripts/pre_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/unicode_scripts/scripts.rs` & `tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/unicode_scripts/scripts.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/pre_tokenizers/whitespace.rs` & `tokenizers-0.9.4/tokenizers-lib/src/pre_tokenizers/whitespace.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/processors/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/src/processors/mod.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/processors/roberta.rs` & `tokenizers-0.9.4/tokenizers-lib/src/processors/bert.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,69 @@
-use crate::processors::byte_level::process_offsets;
 use crate::tokenizer::{Encoding, PostProcessor, Result};
 use serde::{Deserialize, Serialize};
+use std::collections::HashMap;
+use std::iter::FromIterator;
 
-#[derive(Serialize, Deserialize, Debug, Clone, PartialEq)]
+#[derive(Serialize, Deserialize, Clone, Debug, PartialEq)]
 #[serde(tag = "type")]
-pub struct RobertaProcessing {
+pub struct BertProcessing {
     sep: (String, u32),
     cls: (String, u32),
-    trim_offsets: bool,
-    add_prefix_space: bool,
 }
 
-impl Default for RobertaProcessing {
+impl Default for BertProcessing {
     fn default() -> Self {
         Self {
-            sep: ("</s>".into(), 2),
-            cls: ("<s>".into(), 0),
-            trim_offsets: true,
-            add_prefix_space: true,
+            sep: ("[SEP]".into(), 102),
+            cls: ("[CLS]".into(), 101),
         }
     }
 }
 
-impl RobertaProcessing {
+impl BertProcessing {
     pub fn new(sep: (String, u32), cls: (String, u32)) -> Self {
-        RobertaProcessing {
-            sep,
-            cls,
-            ..Default::default()
-        }
-    }
-    pub fn trim_offsets(mut self, v: bool) -> Self {
-        self.trim_offsets = v;
-        self
-    }
-    pub fn add_prefix_space(mut self, v: bool) -> Self {
-        self.add_prefix_space = v;
-        self
+        BertProcessing { sep, cls }
     }
 }
 
-impl PostProcessor for RobertaProcessing {
+impl PostProcessor for BertProcessing {
     fn added_tokens(&self, is_pair: bool) -> usize {
         if is_pair {
-            4
+            3
         } else {
             2
         }
     }
 
     fn process(
         &self,
         mut encoding: Encoding,
-        mut pair_encoding: Option<Encoding>,
+        pair_encoding: Option<Encoding>,
         add_special_tokens: bool,
     ) -> Result<Encoding> {
-        if self.trim_offsets {
-            process_offsets(&mut encoding, self.add_prefix_space);
-            encoding
-                .get_overflowing_mut()
-                .iter_mut()
-                .for_each(|mut encoding| process_offsets(&mut encoding, self.add_prefix_space));
-
-            if let Some(mut encoding) = pair_encoding.as_mut() {
-                process_offsets(&mut encoding, self.add_prefix_space);
-                encoding
-                    .get_overflowing_mut()
-                    .iter_mut()
-                    .for_each(|mut encoding| process_offsets(&mut encoding, self.add_prefix_space));
-            }
-        }
-
         if !add_special_tokens {
             return PostProcessor::default_process(encoding, pair_encoding, add_special_tokens);
         }
 
         let ids = [&[self.cls.1], &encoding.get_ids()[..], &[self.sep.1]].concat();
         let type_ids = [&[0], &encoding.get_type_ids()[..], &[0]].concat();
         let tokens = [
             &[self.cls.0.clone()],
             &encoding.get_tokens()[..],
             &[self.sep.0.clone()],
         ]
         .concat();
-        let words = [&[None], &encoding.get_words()[..], &[None]].concat();
+        let words = [&[None], &encoding.get_word_ids()[..], &[None]].concat();
         let offsets = [&[(0, 0)], &encoding.get_offsets()[..], &[(0, 0)]].concat();
         let special_tokens = [&[1u32], &vec![0; encoding.get_ids().len()][..], &[1]].concat();
         let attention_mask = vec![1; ids.len()];
 
+        // For compatibility with `TemplateProcessing`, the sequence_ranges shouldn't contain
+        // the special tokens.
+        let sequence_ranges = HashMap::from_iter(vec![(0, 1..ids.len() - 1)]);
         let mut new_encoding = Encoding::new(
             ids,
             type_ids,
             tokens,
             words,
             offsets,
             special_tokens,
@@ -104,89 +76,92 @@
                     let type_ids = [&[0], &encoding.get_type_ids()[..], &[0]].concat();
                     let tokens = [
                         &[self.cls.0.clone()],
                         &encoding.get_tokens()[..],
                         &[self.sep.0.clone()],
                     ]
                     .concat();
-                    let words = [&[None], &encoding.get_words()[..], &[None]].concat();
+                    let words = [&[None], &encoding.get_word_ids()[..], &[None]].concat();
                     let offsets = [&[(0, 0)], &encoding.get_offsets()[..], &[(0, 0)]].concat();
                     let special_tokens =
                         [&[1u32], &vec![0; encoding.get_ids().len()][..], &[1]].concat();
                     let attention_mask = vec![1; ids.len()];
 
+                    // For compatibility with `TemplateProcessing`, the sequence_ranges shouldn't
+                    // contain the special tokens.
+                    let sequence_ranges = HashMap::from_iter(vec![(0, 1..ids.len() - 1)]);
                     Encoding::new(
                         ids,
                         type_ids,
                         tokens,
                         words,
                         offsets,
                         special_tokens,
                         attention_mask,
                         vec![],
+                        sequence_ranges,
                     )
                 })
                 .collect(),
+            sequence_ranges,
         );
 
         if let Some(mut encoding) = pair_encoding {
-            let pair_ids = [&[self.sep.1], &encoding.get_ids()[..], &[self.sep.1]].concat();
-            let pair_type_ids = vec![0; encoding.get_ids().len() + 2];
-            let pair_tokens = [
-                &[self.sep.0.clone()],
-                &encoding.get_tokens()[..],
-                &[self.sep.0.clone()],
-            ]
-            .concat();
-            let pair_words = [&[None], &encoding.get_words()[..], &[None]].concat();
-            let pair_offsets = [&[(0, 0)], &encoding.get_offsets()[..], &[(0, 0)]].concat();
+            let pair_ids = [&encoding.get_ids()[..], &[self.sep.1]].concat();
+            let pair_type_ids = [&encoding.get_type_ids()[..], &[1]].concat();
+            let pair_tokens = [&encoding.get_tokens()[..], &[self.sep.0.clone()]].concat();
+            let pair_words = [&encoding.get_word_ids()[..], &[None]].concat();
+            let pair_offsets = [&encoding.get_offsets()[..], &[(0, 0)]].concat();
             let pair_special_tokens =
-                [&[1], &vec![0u32; encoding.get_type_ids().len()][..], &[1]].concat();
+                [&vec![0u32; encoding.get_type_ids().len()][..], &[1]].concat();
             let pair_attention_mask = vec![1; pair_ids.len()];
 
+            // For compatibility with `TemplateProcessing`, the sequence_ranges shouldn't contain
+            // the special tokens.
+            let pair_sequence_ranges = HashMap::from_iter(vec![(1, 0..pair_ids.len() - 1)]);
             let new_pair_encoding = Encoding::new(
                 pair_ids,
                 pair_type_ids,
                 pair_tokens,
                 pair_words,
                 pair_offsets,
                 pair_special_tokens,
                 pair_attention_mask,
                 encoding
                     .take_overflowing()
                     .into_iter()
                     .map(|encoding| {
-                        let pair_ids =
-                            [&[self.sep.1], &encoding.get_ids()[..], &[self.sep.1]].concat();
-                        let pair_type_ids = vec![0; encoding.get_ids().len() + 2];
-                        let pair_tokens = [
-                            &[self.sep.0.clone()],
-                            &encoding.get_tokens()[..],
-                            &[self.sep.0.clone()],
-                        ]
-                        .concat();
-                        let pair_words = [&[None], &encoding.get_words()[..], &[None]].concat();
-                        let pair_offsets =
-                            [&[(0, 0)], &encoding.get_offsets()[..], &[(0, 0)]].concat();
+                        let pair_ids = [&encoding.get_ids()[..], &[self.sep.1]].concat();
+                        let pair_type_ids = [&encoding.get_type_ids()[..], &[1]].concat();
+                        let pair_tokens =
+                            [&encoding.get_tokens()[..], &[self.sep.0.clone()]].concat();
+                        let pair_words = [&encoding.get_word_ids()[..], &[None]].concat();
+                        let pair_offsets = [&encoding.get_offsets()[..], &[(0, 0)]].concat();
                         let pair_special_tokens =
-                            [&[1], &vec![0u32; encoding.get_type_ids().len()][..], &[1]].concat();
+                            [&vec![0u32; encoding.get_type_ids().len()][..], &[1]].concat();
                         let pair_attention_mask = vec![1; pair_ids.len()];
 
+                        // For compatibility with `TemplateProcessing`, the sequence_ranges
+                        // shouldn't contain the special tokens.
+                        let pair_sequence_ranges =
+                            HashMap::from_iter(vec![(1, 0..pair_ids.len() - 1)]);
                         Encoding::new(
                             pair_ids,
                             pair_type_ids,
                             pair_tokens,
                             pair_words,
                             pair_offsets,
                             pair_special_tokens,
                             pair_attention_mask,
                             vec![],
+                            pair_sequence_ranges,
                         )
                     })
                     .collect(),
+                pair_sequence_ranges,
             );
 
             new_encoding.merge_with(new_pair_encoding, false);
         }
 
         Ok(new_encoding)
     }
@@ -194,23 +169,16 @@
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
     fn serde() {
-        let roberta = RobertaProcessing::default();
-        let roberta_r = r#"{
-            "type":"RobertaProcessing",
-            "sep":["</s>",2],
-            "cls":["<s>",0],
-            "trim_offsets":true,
-            "add_prefix_space":true
-        }"#
-        .replace(char::is_whitespace, "");
-        assert_eq!(serde_json::to_string(&roberta).unwrap(), roberta_r);
+        let bert = BertProcessing::default();
+        let bert_r = r#"{"type":"BertProcessing","sep":["[SEP]",102],"cls":["[CLS]",101]}"#;
+        assert_eq!(serde_json::to_string(&bert).unwrap(), bert_r);
         assert_eq!(
-            serde_json::from_str::<RobertaProcessing>(&roberta_r).unwrap(),
-            roberta
+            serde_json::from_str::<BertProcessing>(bert_r).unwrap(),
+            bert
         );
     }
 }
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/processors/template.rs` & `tokenizers-0.9.4/tokenizers-lib/src/processors/template.rs`

 * *Files 6% similar despite different names*

```diff
@@ -515,14 +515,15 @@
         let mut ids = Vec::with_capacity(new_len);
         let mut type_ids = Vec::with_capacity(new_len);
         let mut tokens = Vec::with_capacity(new_len);
         let mut words = Vec::with_capacity(new_len);
         let mut offsets = Vec::with_capacity(new_len);
         let mut special_tokens_mask = Vec::with_capacity(new_len);
         let mut attention_mask = Vec::with_capacity(new_len);
+        let mut sequence_ranges = HashMap::new();
 
         let pair_overflowing = pair.as_mut().map_or(vec![], |e| e.take_overflowing());
         let mut overflowing = encoding
             .take_overflowing()
             .into_iter()
             .flat_map(|encoding| {
                 let mut overflowings = vec![];
@@ -560,31 +561,37 @@
 
         for piece in template {
             match piece {
                 Piece::Sequence {
                     id: Sequence::A,
                     type_id,
                 } => {
+                    let seq_start = ids.len();
+                    let seq_end = seq_start + encoding.len();
+                    sequence_ranges.insert(0, seq_start..seq_end);
                     ids.extend(encoding.get_ids());
                     type_ids.extend(std::iter::repeat(type_id).take(encoding.len()));
                     tokens.extend(encoding.get_tokens().iter().map(|s| s.to_owned()));
-                    words.extend(encoding.get_words());
+                    words.extend(encoding.get_word_ids());
                     offsets.extend(encoding.get_offsets());
                     special_tokens_mask.extend(encoding.get_special_tokens_mask());
                     attention_mask.extend(encoding.get_attention_mask());
                 }
                 Piece::Sequence {
                     id: Sequence::B,
                     type_id,
                 } => {
                     let pair = pair.as_ref().expect("Missing pair sequence, checked above");
+                    let seq_start = ids.len();
+                    let seq_end = seq_start + pair.len();
+                    sequence_ranges.insert(1, seq_start..seq_end);
                     ids.extend(pair.get_ids());
                     type_ids.extend(std::iter::repeat(type_id).take(pair.len()));
                     tokens.extend(pair.get_tokens().iter().map(|s| s.to_owned()));
-                    words.extend(pair.get_words());
+                    words.extend(pair.get_word_ids());
                     offsets.extend(pair.get_offsets());
                     special_tokens_mask.extend(pair.get_special_tokens_mask());
                     attention_mask.extend(pair.get_attention_mask());
                 }
                 Piece::SpecialToken { id, type_id } => {
                     if add_special_tokens {
                         let tok = &self.special_tokens.0[id]; // We already checked existance above
@@ -607,14 +614,15 @@
             type_ids,
             tokens,
             words,
             offsets,
             special_tokens_mask,
             attention_mask,
             overflowing,
+            sequence_ranges,
         ))
     }
 }
 
 impl PostProcessor for TemplateProcessing {
     fn added_tokens(&self, is_pair: bool) -> usize {
         if is_pair {
@@ -643,14 +651,15 @@
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use std::convert::TryInto;
+    use std::iter::FromIterator;
 
     #[test]
     fn piece_serde() {
         let seq_0 = Piece::Sequence {
             id: Sequence::A,
             type_id: 0,
         };
@@ -853,34 +862,39 @@
             vec![
                 Token::new(12, "Hello".into(), (0, 5)),
                 Token::new(14, "there".into(), (6, 11)),
             ],
             0,
         );
         let pair = Encoding::from_tokens(vec![Token::new(15, "pair".into(), (0, 4))], 0);
+        let single_encoding = processor.process(encoding.clone(), None, true).unwrap();
+        let pair_encoding = processor.process(encoding, Some(pair), true).unwrap();
         assert_eq!(
-            processor.process(encoding.clone(), None, true).unwrap(),
+            single_encoding,
             Encoding::new(
                 vec![1, 12, 14, 0],
                 vec![0, 0, 0, 0],
                 vec![
                     "[CLS]".into(),
                     "Hello".into(),
                     "there".into(),
                     "[SEP]".into()
                 ],
                 vec![None, None, None, None],
                 vec![(0, 0), (0, 5), (6, 11), (0, 0)],
                 vec![1, 0, 0, 1],
                 vec![1, 1, 1, 1],
-                vec![]
+                vec![],
+                HashMap::from_iter(vec![(0, 1..3)]),
             )
         );
+        assert_eq!(single_encoding.token_to_sequence(2), Some(0));
+        assert_eq!(single_encoding.token_to_sequence(3), None);
         assert_eq!(
-            processor.process(encoding, Some(pair), true).unwrap(),
+            pair_encoding,
             Encoding::new(
                 vec![1, 12, 14, 0, 15, 0],
                 vec![0, 0, 0, 0, 1, 1],
                 vec![
                     "[CLS]".into(),
                     "Hello".into(),
                     "there".into(),
@@ -888,17 +902,22 @@
                     "pair".into(),
                     "[SEP]".into()
                 ],
                 vec![None, None, None, None, None, None],
                 vec![(0, 0), (0, 5), (6, 11), (0, 0), (0, 4), (0, 0)],
                 vec![1, 0, 0, 1, 0, 1],
                 vec![1, 1, 1, 1, 1, 1],
-                vec![]
+                vec![],
+                HashMap::from_iter(vec![(0, 1..3), (1, 4..5)]),
             )
         );
+        assert_eq!(pair_encoding.token_to_sequence(2), Some(0));
+        assert_eq!(pair_encoding.token_to_sequence(3), None);
+        assert_eq!(pair_encoding.token_to_sequence(4), Some(1));
+        assert_eq!(pair_encoding.token_to_sequence(5), None);
     }
 
     #[test]
     fn pair_must_use_both_sequences() {
         let processor = TemplateProcessing::builder()
             .try_single("$0")
             .unwrap()
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/tokenizer/added_vocabulary.rs` & `tokenizers-0.9.4/tokenizers-lib/src/tokenizer/added_vocabulary.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/tokenizer/encoding.rs` & `tokenizers-0.9.4/tokenizers-lib/src/tokenizer/encoding.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 use crate::parallelism::*;
 use crate::tokenizer::{Offsets, Token};
 use crate::utils::padding::PaddingDirection;
 use serde::{Deserialize, Serialize};
+use std::collections::HashMap;
+use std::ops::Range;
 
 /// Represents the output of a `Tokenizer`.
 #[derive(Default, PartialEq, Debug, Clone, Serialize, Deserialize)]
 pub struct Encoding {
     /// IDs produced by the `Tokenizer`
     ids: Vec<u32>,
     /// Type of the IDs
@@ -18,49 +20,55 @@
     offsets: Vec<Offsets>,
     /// Mask identifying special tokens
     special_tokens_mask: Vec<u32>,
     /// Mask identifying padding tokens for the attention mechanism
     attention_mask: Vec<u32>,
     /// A list of overflowing Encoding generated when we got truncated
     overflowing: Vec<Encoding>,
+    /// Ranges of tokens covered by each sequence. If this is empty we consider
+    /// there is only one sequence in this Encoding, and that it covers the entire range.
+    sequence_ranges: HashMap<usize, Range<usize>>,
 }
 impl Encoding {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         ids: Vec<u32>,
         type_ids: Vec<u32>,
         tokens: Vec<String>,
         words: Vec<Option<u32>>,
         offsets: Vec<Offsets>,
         special_tokens_mask: Vec<u32>,
         attention_mask: Vec<u32>,
         overflowing: Vec<Encoding>,
+        sequence_ranges: HashMap<usize, Range<usize>>,
     ) -> Self {
         Encoding {
             ids,
             type_ids,
             tokens,
             words,
             offsets,
             special_tokens_mask,
             attention_mask,
             overflowing,
+            sequence_ranges,
         }
     }
 
     pub fn with_capacity(len: usize) -> Self {
         Encoding {
             ids: Vec::with_capacity(len),
             type_ids: Vec::with_capacity(len),
             tokens: Vec::with_capacity(len),
             words: Vec::with_capacity(len),
             offsets: Vec::with_capacity(len),
             special_tokens_mask: Vec::with_capacity(len),
             attention_mask: Vec::with_capacity(len),
             overflowing: vec![],
+            sequence_ranges: HashMap::new(),
         }
     }
 
     pub fn from_tokens(tokens: Vec<Token>, type_id: u32) -> Self {
         let length = tokens.len();
         let (ids, tokens, offsets) = tokens.into_iter().fold(
             (
@@ -81,37 +89,64 @@
             tokens,
             offsets,
             words: vec![None; length],
             type_ids: vec![type_id; length],
             attention_mask: vec![1; length],
             special_tokens_mask: vec![0; length],
             overflowing: vec![],
+            sequence_ranges: HashMap::new(),
         }
     }
 
+    /// Whether this Encoding is empty
     pub fn is_empty(&self) -> bool {
         self.ids.is_empty()
     }
 
+    /// Return the total length of this Encoding
     pub fn len(&self) -> usize {
         self.ids.len()
     }
 
+    /// Return the number of sequences combined in this Encoding
+    pub fn n_sequences(&self) -> usize {
+        if self.sequence_ranges.is_empty() {
+            1
+        } else {
+            self.sequence_ranges.len()
+        }
+    }
+
+    /// Set the given sequence id for the whole range of tokens contained in this Encoding
+    pub fn set_sequence_id(&mut self, sequence_id: usize) {
+        self.sequence_ranges.insert(sequence_id, 0..self.len());
+    }
+
     pub fn get_tokens(&self) -> &[String] {
         &self.tokens[..]
     }
 
-    pub fn get_words(&self) -> &[Option<u32>] {
+    pub fn get_word_ids(&self) -> &[Option<u32>] {
         &self.words
     }
 
-    pub fn get_words_mut(&mut self) -> &mut [Option<u32>] {
+    pub fn get_word_ids_mut(&mut self) -> &mut [Option<u32>] {
         &mut self.words
     }
 
+    pub fn get_sequence_ids(&self) -> Vec<Option<usize>> {
+        let mut sequences = vec![None; self.len()];
+        for seq_id in 0..self.n_sequences() {
+            let range = self.sequence_range(seq_id);
+            let seq_len = range.len();
+            sequences.splice(range, std::iter::repeat(Some(seq_id)).take(seq_len));
+        }
+        sequences
+    }
+
     pub fn get_ids(&self) -> &[u32] {
         &self.ids
     }
 
     pub fn get_type_ids(&self) -> &[u32] {
         &self.type_ids
     }
@@ -151,74 +186,116 @@
         self.tokens
             .iter()
             .zip(self.offsets.iter_mut())
             .enumerate()
             .for_each(func)
     }
 
+    /// Returns the range to target to retrieve something (word_id, offsets, ..) related to the
+    /// given sequence id
+    fn sequence_range(&self, sequence_id: usize) -> Range<usize> {
+        self.sequence_ranges
+            .get(&sequence_id)
+            .cloned()
+            .unwrap_or(0..self.len())
+    }
+
+    /// Returns the index of the sequence containing the given token
+    pub fn token_to_sequence(&self, token: usize) -> Option<usize> {
+        if token > self.len() {
+            None
+        } else if self.sequence_ranges.is_empty() {
+            Some(0)
+        } else {
+            self.sequence_ranges.iter().find_map(|(seq_id, range)| {
+                if range.contains(&token) {
+                    Some(*seq_id)
+                } else {
+                    None
+                }
+            })
+        }
+    }
+
     /// Get the encoded tokens corresponding to the word at the given index in the input sequence,
     /// with the form (start_token, end_token + 1)
-    pub fn word_to_tokens(&self, word: u32) -> Option<(usize, usize)> {
+    pub fn word_to_tokens(&self, word: u32, sequence_id: usize) -> Option<(usize, usize)> {
         let (mut start, mut end) = (None, None);
+        let sequence_range = self.sequence_range(sequence_id);
+
         self.words
+            .get(sequence_range.clone())?
             .iter()
             .enumerate()
             .take_while(|(_, w)| **w <= Some(word))
             .filter(|(_, w)| **w == Some(word))
             .for_each(|(i, _)| {
                 if start.is_none() || Some(i) < start {
                     start = Some(i);
                 }
                 if end.is_none() || Some(i) >= end {
                     end = Some(i + 1);
                 }
             });
 
         if let (Some(start), Some(end)) = (start, end) {
-            Some((start, end))
+            Some((sequence_range.start + start, sequence_range.start + end))
         } else {
             None
         }
     }
 
     /// Get the offsets of the word at the given index in the input sequence.
-    pub fn word_to_chars(&self, word: u32) -> Option<Offsets> {
-        self.word_to_tokens(word)
+    pub fn word_to_chars(&self, word: u32, sequence_id: usize) -> Option<Offsets> {
+        self.word_to_tokens(word, sequence_id)
             .map(|(start, end)| {
                 if end == 0 {
                     None
                 } else {
                     Some((self.offsets[start].0, self.offsets[end - 1].1))
                 }
             })
             .flatten()
     }
 
     /// Get the offsets of the token at the given index.
-    pub fn token_to_chars(&self, token: usize) -> Option<Offsets> {
-        self.offsets.get(token).copied()
+    pub fn token_to_chars(&self, token: usize) -> Option<(usize, Offsets)> {
+        Some((
+            self.token_to_sequence(token)?,
+            self.offsets.get(token).copied()?,
+        ))
     }
 
     /// Get the word that contains the token at the given index.
-    pub fn token_to_word(&self, token: usize) -> Option<u32> {
-        self.words.get(token).copied().flatten()
+    pub fn token_to_word(&self, token: usize) -> Option<(usize, u32)> {
+        Some((
+            self.token_to_sequence(token)?,
+            self.words.get(token).copied().flatten()?,
+        ))
     }
 
     /// Get the token that contains the given char.
-    pub fn char_to_token(&self, pos: usize) -> Option<usize> {
+    pub fn char_to_token(&self, pos: usize, sequence_id: usize) -> Option<usize> {
+        let sequence_range = self.sequence_range(sequence_id);
+
         self.offsets
+            .get(sequence_range.clone())?
             .iter()
             .position(|(start, end)| pos >= *start && pos < *end)
+            .map(|pos| sequence_range.start + pos)
     }
 
     /// Get the word that contains the given char.
-    pub fn char_to_word(&self, pos: usize) -> Option<u32> {
-        self.char_to_token(pos)
-            .map(|token| self.token_to_word(token))
-            .flatten()
+    pub fn char_to_word(&self, pos: usize, sequence_id: usize) -> Option<u32> {
+        Some(
+            self.char_to_token(pos, sequence_id)
+                .map(|token| self.token_to_word(token))
+                .flatten()?
+                .1,
+        )
     }
 
     /// Truncate the current `Encoding`.
     ///
     /// Panic if `stride >= max_len`
     pub fn truncate(&mut self, max_len: usize, stride: usize) {
         if max_len >= self.ids.len() {
@@ -236,14 +313,17 @@
         let o_type_ids = self.type_ids.split_off(max_len);
         let o_tokens = self.tokens.split_off(max_len);
         let o_words = self.words.split_off(max_len);
         let o_offsets = self.offsets.split_off(max_len);
         let o_spe_toks = self.special_tokens_mask.split_off(max_len);
         let o_attent = self.attention_mask.split_off(max_len);
 
+        // When truncating, we loose the `sequence_ranges` information.
+        self.sequence_ranges.clear();
+
         // Now we need to separate the overflowing part into as many Encoding as needed
         assert!(stride < max_len);
         let part_size = max_len - stride;
         let mut overflowing = vec![];
         let mut part_id = 0;
         let mut prev_encoding: &Encoding = self;
 
@@ -287,14 +367,15 @@
                     &prev_encoding.attention_mask,
                     &o_attent,
                     part_size,
                     part_id,
                     stride,
                 ),
                 overflowing: vec![],
+                sequence_ranges: HashMap::new(),
             };
 
             part_id += 1;
             overflowing.push(o);
             prev_encoding = &overflowing.last().unwrap();
         }
 
@@ -336,14 +417,23 @@
         for other_o in &pair.overflowing {
             let mut n_encoding = self.clone();
             n_encoding.merge_with(other_o.clone(), growing_offsets);
             overflowings.push(n_encoding);
         }
 
         // Finish by merging ourself with the other encoding
+        let original_self_len = self.len(); // Must be before any modification to self.ids
+
+        self.sequence_ranges
+            .extend(pair.sequence_ranges.into_iter().map(|(seq_id, range)| {
+                (
+                    seq_id,
+                    original_self_len + range.start..original_self_len + range.end,
+                )
+            }));
         self.ids.extend(pair.ids);
         self.type_ids.extend(pair.type_ids);
         self.tokens.extend(pair.tokens);
         self.words.extend(pair.words);
 
         let starting_offset = if growing_offsets {
             self.offsets.last().map_or(0, |o| o.1)
@@ -471,50 +561,51 @@
     let prev_slice = &prev[prev.len() - stride..];
     [prev_slice, curr_slice].concat()
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
+    use std::iter::FromIterator;
 
     #[test]
     fn merge_encodings() {
         let mut a = Encoding {
             ids: vec![1],
             type_ids: vec![0],
             tokens: vec![String::from("Hello ")],
             words: vec![Some(0)],
             offsets: vec![(0, 6)],
             special_tokens_mask: vec![0],
             attention_mask: vec![1],
-            overflowing: vec![],
+            ..Default::default()
         };
         let b = Encoding {
             ids: vec![2],
             type_ids: vec![1],
             tokens: vec![String::from("World!")],
             words: vec![Some(0)],
             offsets: vec![(0, 6)],
             special_tokens_mask: vec![0],
             attention_mask: vec![1],
-            overflowing: vec![],
+            ..Default::default()
         };
         a.merge_with(b, true);
 
         assert_eq!(
             a,
             Encoding {
                 ids: vec![1, 2],
                 type_ids: vec![0, 1],
                 tokens: vec![String::from("Hello "), String::from("World!")],
                 words: vec![Some(0), Some(0)],
                 offsets: vec![(0, 6), (6, 12)],
                 special_tokens_mask: vec![0, 0],
                 attention_mask: vec![1, 1],
-                overflowing: vec![],
+                ..Default::default()
             }
         );
     }
 
     #[test]
     fn truncate() {
         let mut a = Encoding {
@@ -525,15 +616,15 @@
                 String::from("World"),
                 String::from("!"),
             ],
             words: vec![Some(0), Some(1), Some(2)],
             offsets: vec![(0, 5), (6, 11), (11, 12)],
             special_tokens_mask: vec![0, 0, 0],
             attention_mask: vec![1, 1, 1],
-            overflowing: vec![],
+            ..Default::default()
         };
         a.truncate(2, 0);
 
         assert_eq!(
             a,
             Encoding {
                 ids: vec![1, 2],
@@ -547,16 +638,17 @@
                     ids: vec![3],
                     type_ids: vec![0],
                     tokens: vec![String::from("!")],
                     words: vec![Some(2)],
                     offsets: vec![(11, 12)],
                     special_tokens_mask: vec![0],
                     attention_mask: vec![1],
-                    overflowing: vec![],
-                }]
+                    ..Default::default()
+                }],
+                ..Default::default()
             }
         );
     }
 
     #[test]
     fn truncate_to_empty() {
         let mut a = Encoding {
@@ -567,97 +659,126 @@
                 String::from("World"),
                 String::from("!"),
             ],
             words: vec![Some(0), Some(1), Some(2)],
             offsets: vec![(0, 5), (6, 11), (11, 12)],
             special_tokens_mask: vec![0, 0, 0],
             attention_mask: vec![1, 1, 1],
-            overflowing: vec![],
+            ..Default::default()
         };
         a.truncate(0, 0);
 
         assert_eq!(
             a,
             Encoding {
-                ids: vec![],
-                type_ids: vec![],
-                tokens: vec![],
-                words: vec![],
-                offsets: vec![],
-                special_tokens_mask: vec![],
-                attention_mask: vec![],
                 overflowing: vec![Encoding {
                     ids: vec![1, 2, 3],
                     type_ids: vec![0, 0, 0],
                     tokens: vec![
                         String::from("Hello"),
                         String::from("World"),
                         String::from("!"),
                     ],
                     words: vec![Some(0), Some(1), Some(2)],
                     offsets: vec![(0, 5), (6, 11), (11, 12)],
                     special_tokens_mask: vec![0, 0, 0],
                     attention_mask: vec![1, 1, 1],
                     overflowing: vec![],
-                }]
+                    ..Default::default()
+                }],
+                ..Default::default()
             }
         );
     }
 
     #[test]
     fn mappings() {
         let encoding = Encoding {
+            ids: vec![0; 11], // Needed for Encoding::len
             tokens: vec![
+                // First sequence:
                 "He".into(),
                 "llo".into(),
                 "won".into(),
                 "der".into(),
                 "ful".into(),
                 "friend".into(),
                 "!".into(),
+                // Second sequence:
+                "How".into(),
+                "are".into(),
+                "you".into(),
+                "?".into(),
             ],
             offsets: vec![
+                // First sequence:
                 (0, 2),
                 (2, 5),
                 (7, 10),
                 (10, 13),
                 (13, 16),
                 (17, 23),
                 (23, 24),
+                // Second sequence:
+                (0, 3),
+                (4, 7),
+                (8, 11),
+                (11, 12),
             ],
             words: vec![
+                // First sequence:
                 Some(0),
                 Some(0),
                 Some(1),
                 Some(1),
                 Some(1),
                 Some(2),
                 Some(3),
+                // Second sequence:
+                Some(0),
+                Some(1),
+                Some(2),
+                Some(3),
             ],
+            sequence_ranges: HashMap::from_iter(vec![(0, 0..7), (1, 7..11)]),
             ..Default::default()
         };
-        assert_eq!(encoding.word_to_tokens(0), Some((0, 2)));
-        assert_eq!(encoding.word_to_tokens(1), Some((2, 5)));
-        assert_eq!(encoding.word_to_tokens(2), Some((5, 6)));
-        assert_eq!(encoding.word_to_tokens(3), Some((6, 7)));
-
-        assert_eq!(encoding.word_to_chars(0), Some((0, 5)));
-        assert_eq!(encoding.word_to_chars(1), Some((7, 16)));
-
-        assert_eq!(encoding.token_to_chars(0), Some((0, 2)));
-        assert_eq!(encoding.token_to_chars(1), Some((2, 5)));
-
-        assert_eq!(encoding.token_to_word(1), Some(0));
-        assert_eq!(encoding.token_to_word(2), Some(1));
-        assert_eq!(encoding.token_to_word(7), None);
-
-        assert_eq!(encoding.char_to_token(3), Some(1));
-        assert_eq!(encoding.char_to_token(8), Some(2));
-        assert_eq!(encoding.char_to_token(16), None);
-        assert_eq!(encoding.char_to_token(23), Some(6));
-
-        assert_eq!(encoding.char_to_word(3), Some(0));
-        assert_eq!(encoding.char_to_word(8), Some(1));
-        assert_eq!(encoding.char_to_word(16), None);
-        assert_eq!(encoding.char_to_word(23), Some(3));
+        assert_eq!(encoding.word_to_tokens(0, 0), Some((0, 2)));
+        assert_eq!(encoding.word_to_tokens(1, 0), Some((2, 5)));
+        assert_eq!(encoding.word_to_tokens(2, 0), Some((5, 6)));
+        assert_eq!(encoding.word_to_tokens(3, 0), Some((6, 7)));
+        assert_eq!(encoding.word_to_tokens(0, 1), Some((7, 8)));
+        assert_eq!(encoding.word_to_tokens(1, 1), Some((8, 9)));
+        assert_eq!(encoding.word_to_tokens(2, 1), Some((9, 10)));
+        assert_eq!(encoding.word_to_tokens(3, 1), Some((10, 11)));
+
+        assert_eq!(encoding.word_to_chars(0, 0), Some((0, 5)));
+        assert_eq!(encoding.word_to_chars(1, 0), Some((7, 16)));
+        assert_eq!(encoding.word_to_chars(0, 1), Some((0, 3)));
+        assert_eq!(encoding.word_to_chars(1, 1), Some((4, 7)));
+
+        assert_eq!(encoding.token_to_chars(0), Some((0, (0, 2))));
+        assert_eq!(encoding.token_to_chars(1), Some((0, (2, 5))));
+        assert_eq!(encoding.token_to_chars(7), Some((1, (0, 3))));
+        assert_eq!(encoding.token_to_chars(9), Some((1, (8, 11))));
+
+        assert_eq!(encoding.token_to_word(1), Some((0, 0)));
+        assert_eq!(encoding.token_to_word(2), Some((0, 1)));
+        assert_eq!(encoding.token_to_word(7), Some((1, 0)));
+        assert_eq!(encoding.token_to_word(9), Some((1, 2)));
+        assert_eq!(encoding.token_to_word(11), None);
+
+        assert_eq!(encoding.char_to_token(3, 0), Some(1));
+        assert_eq!(encoding.char_to_token(8, 0), Some(2));
+        assert_eq!(encoding.char_to_token(16, 0), None);
+        assert_eq!(encoding.char_to_token(23, 0), Some(6));
+        assert_eq!(encoding.char_to_token(2, 1), Some(7));
+        assert_eq!(encoding.char_to_token(9, 1), Some(9));
+
+        assert_eq!(encoding.char_to_word(3, 0), Some(0));
+        assert_eq!(encoding.char_to_word(8, 0), Some(1));
+        assert_eq!(encoding.char_to_word(16, 0), None);
+        assert_eq!(encoding.char_to_word(23, 0), Some(3));
+        assert_eq!(encoding.char_to_word(2, 1), Some(0));
+        assert_eq!(encoding.char_to_word(9, 1), Some(2));
     }
 }
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/tokenizer/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/src/tokenizer/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,30 @@
 };
 
 use indicatif::{ProgressBar, ProgressStyle};
 use serde::de::DeserializeOwned;
 use serde::export::Formatter;
 use serde::{Deserialize, Serialize};
 
-use crate::decoders::DecoderWrapper;
-use crate::models::ModelWrapper;
-use crate::normalizers::NormalizerWrapper;
-use crate::pre_tokenizers::PreTokenizerWrapper;
-use crate::processors::PostProcessorWrapper;
 use crate::utils::parallelism::*;
 
 mod added_vocabulary;
 mod encoding;
 pub mod normalizer;
 pub mod pattern;
 pub mod pre_tokenizer;
 mod serialization;
 
+// Re-export wrappers
+pub use crate::decoders::DecoderWrapper;
+pub use crate::models::ModelWrapper;
+pub use crate::normalizers::NormalizerWrapper;
+pub use crate::pre_tokenizers::PreTokenizerWrapper;
+pub use crate::processors::PostProcessorWrapper;
+// And some other types
 pub use crate::utils::iter::LinesWithEnding;
 pub use crate::utils::padding::{pad_encodings, PaddingDirection, PaddingParams, PaddingStrategy};
 pub use crate::utils::truncation::{truncate_encodings, TruncationParams, TruncationStrategy};
 pub use added_vocabulary::*;
 pub use encoding::*;
 pub use normalizer::{NormalizedString, OffsetReferential, SplitDelimiterBehavior};
 pub use pre_tokenizer::*;
@@ -99,15 +101,17 @@
     pub fn default_process(
         mut encoding: Encoding,
         pair_encoding: Option<Encoding>,
         _add_special_tokens: bool,
     ) -> Result<Encoding> {
         match pair_encoding {
             None => Ok(encoding),
-            Some(pair) => {
+            Some(mut pair) => {
+                encoding.set_sequence_id(0);
+                pair.set_sequence_id(1);
                 encoding.merge_with(pair, false);
                 Ok(encoding)
             }
         }
     }
 }
 
@@ -385,14 +389,22 @@
     }
     pub fn from_file<P: AsRef<Path>>(file: P) -> Result<Self> {
         let content = read_to_string(file)?;
         Ok(serde_json::from_str(&content)?)
     }
 }
 
+impl std::str::FromStr for Tokenizer {
+    type Err = Box<dyn std::error::Error + Send + Sync>;
+
+    fn from_str(s: &str) -> Result<Self> {
+        Ok(serde_json::from_str(s)?)
+    }
+}
+
 impl<M, N, PT, PP, D> From<TokenizerImpl<M, N, PT, PP, D>> for Tokenizer
 where
     M: Into<ModelWrapper>,
     N: Into<NormalizerWrapper>,
     PT: Into<PreTokenizerWrapper>,
     PP: Into<PostProcessorWrapper>,
     D: Into<DecoderWrapper>,
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/tokenizer/normalizer.rs` & `tokenizers-0.9.4/tokenizers-lib/src/tokenizer/normalizer.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/tokenizer/pattern.rs` & `tokenizers-0.9.4/tokenizers-lib/src/tokenizer/pattern.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/tokenizer/pre_tokenizer.rs` & `tokenizers-0.9.4/tokenizers-lib/src/tokenizer/pre_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/tokenizer/serialization.rs` & `tokenizers-0.9.4/tokenizers-lib/src/tokenizer/serialization.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/utils/cache.rs` & `tokenizers-0.9.4/tokenizers-lib/src/utils/cache.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/utils/iter.rs` & `tokenizers-0.9.4/tokenizers-lib/src/utils/iter.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/utils/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/utils/padding.rs` & `tokenizers-0.9.4/tokenizers-lib/src/utils/padding.rs`

 * *Files 6% similar despite different names*

```diff
@@ -80,38 +80,41 @@
     Ok(())
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::tokenizer::Encoding;
+    use std::collections::HashMap;
 
     #[test]
     fn pad_to_multiple() {
         fn get_encodings() -> [Encoding; 2] {
             [
                 Encoding::new(
                     vec![0, 1, 2, 3, 4],
                     vec![],
                     vec![],
                     vec![],
                     vec![],
                     vec![],
                     vec![],
                     vec![],
+                    HashMap::new(),
                 ),
                 Encoding::new(
                     vec![0, 1, 2],
                     vec![],
                     vec![],
                     vec![],
                     vec![],
                     vec![],
                     vec![],
                     vec![],
+                    HashMap::new(),
                 ),
             ]
         }
 
         // Test fixed
         let mut encodings = get_encodings();
         let mut params = PaddingParams {
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/utils/parallelism.rs` & `tokenizers-0.9.4/tokenizers-lib/src/utils/parallelism.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/src/utils/truncation.rs` & `tokenizers-0.9.4/tokenizers-lib/src/utils/truncation.rs`

 * *Files 2% similar despite different names*

```diff
@@ -161,38 +161,41 @@
     Ok((encoding, pair_encoding))
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::tokenizer::Encoding;
+    use std::collections::HashMap;
 
     fn get_empty() -> Encoding {
         Encoding::new(
             vec![],
             vec![],
             vec![],
             vec![],
             vec![],
             vec![],
             vec![],
             vec![],
+            HashMap::new(),
         )
     }
 
     fn get_short() -> Encoding {
         Encoding::new(
             vec![1, 2],
             vec![0, 0],
             vec![String::from("a"), String::from("b")],
             vec![Some(0), Some(1)],
             vec![(0, 1), (1, 2)],
             vec![0, 0],
             vec![1, 1],
             vec![],
+            HashMap::new(),
         )
     }
 
     fn get_medium() -> Encoding {
         Encoding::new(
             vec![3, 4, 5, 6],
             vec![0, 0, 0, 0],
@@ -203,14 +206,15 @@
                 String::from("g"),
             ],
             vec![Some(0), Some(1), Some(2), Some(3)],
             vec![(0, 1), (1, 2), (2, 3), (3, 4)],
             vec![0, 0, 0, 0],
             vec![1, 1, 1, 1],
             vec![],
+            HashMap::new(),
         )
     }
 
     fn get_long() -> Encoding {
         Encoding::new(
             vec![7, 8, 9, 10, 11, 12, 13, 14],
             vec![0, 0, 0, 0, 0, 0, 0, 0],
@@ -243,14 +247,15 @@
                 (5, 6),
                 (6, 7),
                 (6, 8),
             ],
             vec![0, 0, 0, 0, 0, 0, 0, 0],
             vec![1, 1, 1, 1, 1, 1, 1, 1],
             vec![],
+            HashMap::new(),
         )
     }
 
     fn truncate_and_assert(
         encoding1: Encoding,
         encoding2: Encoding,
         params: &TruncationParams,
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/tests/added_tokens.rs` & `tokenizers-0.9.4/tokenizers-lib/tests/added_tokens.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/tests/common/mod.rs` & `tokenizers-0.9.4/tokenizers-lib/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/tests/offsets.rs` & `tokenizers-0.9.4/tokenizers-lib/tests/offsets.rs`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             (4, 7),
             (7, 10),
             (10, 15),
             (15, 16)
         ]
     );
     assert_eq!(
-        output.get_words(),
+        output.get_word_ids(),
         &[
             Some(0),
             Some(1),
             Some(2),
             Some(3),
             Some(0),
             Some(1),
@@ -122,15 +122,15 @@
     let output = tokenizer.encode(&input[..], false).unwrap();
 
     assert_eq!(
         output.get_tokens(),
         &["ĠMy", "Ġname", "Ġis", "ĠAnth", "on", "ino"]
     );
     assert_eq!(
-        output.get_words(),
+        output.get_word_ids(),
         &[Some(0), Some(1), Some(2), Some(3), Some(3), Some(3)]
     );
     assert_eq!(
         output.get_offsets(),
         &[(0, 2), (0, 4), (0, 2), (0, 4), (4, 6), (6, 9)]
     );
 }
@@ -141,15 +141,15 @@
     let input = ["My", "name", "is", "Anthonino"];
 
     // When trimming offsets (expect same result)
     let tokenizer = get_byte_level(true, true);
     let output = tokenizer.encode(&input[..], false).unwrap();
 
     assert_eq!(
-        output.get_words(),
+        output.get_word_ids(),
         &[Some(0), Some(1), Some(2), Some(3), Some(3), Some(3)]
     );
     assert_eq!(
         output.get_offsets(),
         &[(0, 2), (0, 4), (0, 2), (0, 4), (4, 6), (6, 9)]
     );
 }
@@ -175,15 +175,15 @@
         ]
     );
     assert_eq!(
         output.get_tokens(),
         &["yesterday", "i", "saw", "a", "[MASK]", "far", "away"]
     );
     assert_eq!(
-        output.get_words(),
+        output.get_word_ids(),
         &[
             Some(0),
             Some(1),
             Some(2),
             Some(3),
             Some(4),
             Some(5),
```

### Comparing `tokenizers-0.9.3/tokenizers-lib/tests/serialization.rs` & `tokenizers-0.9.4/tokenizers-lib/tests/serialization.rs`

 * *Files identical despite different names*

### Comparing `tokenizers-0.9.3/tokenizers-lib/tests/unigram.rs` & `tokenizers-0.9.4/tokenizers-lib/tests/unigram.rs`

 * *Files identical despite different names*

