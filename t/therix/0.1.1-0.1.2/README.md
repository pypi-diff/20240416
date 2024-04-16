# Comparing `tmp/therix-0.1.1.tar.gz` & `tmp/therix-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "therix-0.1.1.tar", max compression
+gzip compressed data, was "therix-0.1.2.tar", max compression
```

## Comparing `therix-0.1.1.tar` & `therix-0.1.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.1/LICENSE
--rw-r--r--   0        0        0     1218 2024-04-12 15:05:11.676463 therix-0.1.1/README.md
--rw-r--r--   0        0        0      800 2024-04-12 15:06:37.519063 therix-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.929969 therix-0.1.1/therix/__init__.py
--rw-r--r--   0        0        0     2083 2024-04-12 14:54:15.930143 therix-0.1.1/therix/core/JSONLoader.py
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.930181 therix-0.1.1/therix/core/__init__.py
--rw-r--r--   0        0        0     1571 2024-04-12 14:54:15.930332 therix-0.1.1/therix/core/constants.py
--rw-r--r--   0        0        0      861 2024-04-12 14:54:15.930444 therix-0.1.1/therix/core/data_sources.py
--rw-r--r--   0        0        0     1610 2024-04-12 14:54:15.930567 therix-0.1.1/therix/core/embedding_models.py
--rw-r--r--   0        0        0     2302 2024-04-12 14:54:15.930687 therix-0.1.1/therix/core/inference_models.py
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.930720 therix-0.1.1/therix/core/output_source.py
--rw-r--r--   0        0        0     3286 2024-04-12 14:54:15.930842 therix-0.1.1/therix/core/pipeline.py
--rw-r--r--   0        0        0     1153 2024-04-12 14:54:15.930956 therix-0.1.1/therix/core/pipeline_component.py
--rw-r--r--   0        0        0      307 2024-04-12 14:54:15.931067 therix-0.1.1/therix/core/trace.py
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.931148 therix-0.1.1/therix/db/__init__.py
--rw-r--r--   0        0        0       83 2024-04-12 14:54:15.931283 therix-0.1.1/therix/db/base.py
--rw-r--r--   0        0        0     2941 2024-04-12 14:54:15.931402 therix-0.1.1/therix/db/db_manager.py
--rw-r--r--   0        0        0      415 2024-04-12 14:54:15.931538 therix-0.1.1/therix/db/session.py
--rw-r--r--   0        0        0      234 2024-04-12 14:54:15.931776 therix-0.1.1/therix/docs/.gitignore
--rw-r--r--   0        0        0      768 2024-04-12 14:54:15.931895 therix-0.1.1/therix/docs/README.md
--rw-r--r--   0        0        0       89 2024-04-12 14:54:15.932023 therix-0.1.1/therix/docs/babel.config.js
--rw-r--r--   0        0        0      389 2024-04-12 14:54:15.932200 therix-0.1.1/therix/docs/blog/2019-05-28-first-blog-post.md
--rw-r--r--   0        0        0     3116 2024-04-12 14:54:15.932340 therix-0.1.1/therix/docs/blog/2019-05-29-long-blog-post.md
--rw-r--r--   0        0        0      439 2024-04-12 14:54:15.932456 therix-0.1.1/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
--rw-r--r--   0        0        0    96122 2024-04-12 14:54:15.932858 therix-0.1.1/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
--rw-r--r--   0        0        0      783 2024-04-12 14:54:15.933048 therix-0.1.1/therix/docs/blog/2021-08-26-welcome/index.md
--rw-r--r--   0        0        0      447 2024-04-12 14:54:15.933157 therix-0.1.1/therix/docs/blog/authors.yml
--rw-r--r--   0        0        0     1411 2024-04-12 14:54:15.933315 therix-0.1.1/therix/docs/docs/intro.md
--rw-r--r--   0        0        0      180 2024-04-12 14:54:15.933452 therix-0.1.1/therix/docs/docs/tutorial-basics/_category_.json
--rw-r--r--   0        0        0     1078 2024-04-12 14:54:15.933560 therix-0.1.1/therix/docs/docs/tutorial-basics/congratulations.md
--rw-r--r--   0        0        0      886 2024-04-12 14:54:15.933661 therix-0.1.1/therix/docs/docs/tutorial-basics/create-a-blog-post.md
--rw-r--r--   0        0        0     1042 2024-04-12 14:54:15.933784 therix-0.1.1/therix/docs/docs/tutorial-basics/create-a-document.md
--rw-r--r--   0        0        0     1015 2024-04-12 14:54:15.933895 therix-0.1.1/therix/docs/docs/tutorial-basics/create-a-page.md
--rw-r--r--   0        0        0      702 2024-04-12 14:54:15.934002 therix-0.1.1/therix/docs/docs/tutorial-basics/deploy-your-site.md
--rw-r--r--   0        0        0     3006 2024-04-12 14:54:15.934112 therix-0.1.1/therix/docs/docs/tutorial-basics/markdown-features.mdx
--rw-r--r--   0        0        0       99 2024-04-12 14:54:15.934248 therix-0.1.1/therix/docs/docs/tutorial-extras/_category_.json
--rw-r--r--   0        0        0    25427 2024-04-12 14:54:15.934440 therix-0.1.1/therix/docs/docs/tutorial-extras/img/docsVersionDropdown.png
--rw-r--r--   0        0        0    27841 2024-04-12 14:54:15.934733 therix-0.1.1/therix/docs/docs/tutorial-extras/img/localeDropdown.png
--rw-r--r--   0        0        0     1232 2024-04-12 14:54:15.934904 therix-0.1.1/therix/docs/docs/tutorial-extras/manage-docs-versions.md
--rw-r--r--   0        0        0     1587 2024-04-12 14:54:15.935005 therix-0.1.1/therix/docs/docs/tutorial-extras/translate-your-site.md
--rw-r--r--   0        0        0     3605 2024-04-12 14:54:15.935114 therix-0.1.1/therix/docs/docusaurus.config.js
--rw-r--r--   0        0        0   573996 2024-04-12 14:54:15.936314 therix-0.1.1/therix/docs/package-lock.json
--rw-r--r--   0        0        0     1061 2024-04-12 14:54:15.936493 therix-0.1.1/therix/docs/package.json
--rw-r--r--   0        0        0      779 2024-04-12 14:54:15.936597 therix-0.1.1/therix/docs/sidebars.js
--rw-r--r--   0        0        0     1721 2024-04-12 14:54:15.936828 therix-0.1.1/therix/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      138 2024-04-12 14:54:15.936929 therix-0.1.1/therix/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     2239 2024-04-12 14:54:15.937061 therix-0.1.1/therix/docs/src/css/custom.css
--rw-r--r--   0        0        0      365 2024-04-12 14:54:15.937193 therix-0.1.1/therix/docs/src/pages/index.module.css
--rw-r--r--   0        0        0      118 2024-04-12 14:54:15.937292 therix-0.1.1/therix/docs/src/pages/markdown-page.md
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.937368 therix-0.1.1/therix/docs/static/.nojekyll
--rw-r--r--   0        0        0    21038 2024-04-12 14:54:15.937664 therix-0.1.1/therix/docs/static/img/coditas.png
--rw-r--r--   0        0        0     5277 2024-04-12 14:54:15.937878 therix-0.1.1/therix/docs/static/img/coditasLogo.svg
--rw-r--r--   0        0        0    55746 2024-04-12 14:54:15.938169 therix-0.1.1/therix/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0     5142 2024-04-12 14:54:15.938362 therix-0.1.1/therix/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0     3626 2024-04-12 14:54:15.938464 therix-0.1.1/therix/docs/static/img/favicon.ico
--rw-r--r--   0        0        0      506 2024-04-12 14:54:15.938561 therix-0.1.1/therix/docs/static/img/icon.svg
--rw-r--r--   0        0        0     6438 2024-04-12 14:54:15.938694 therix-0.1.1/therix/docs/static/img/logo.svg
--rw-r--r--   0        0        0    31486 2024-04-12 14:54:15.938840 therix-0.1.1/therix/docs/static/img/undraw_docusaurus_mountain.svg
--rw-r--r--   0        0        0    36002 2024-04-12 14:54:15.939041 therix-0.1.1/therix/docs/static/img/undraw_docusaurus_react.svg
--rw-r--r--   0        0        0    11887 2024-04-12 14:54:15.939300 therix-0.1.1/therix/docs/static/img/undraw_docusaurus_tree.svg
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.939374 therix-0.1.1/therix/entities/__init__.py
--rw-r--r--   0        0        0     2205 2024-04-12 14:54:15.939477 therix-0.1.1/therix/entities/models.py
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.939553 therix-0.1.1/therix/services/__init__.py
--rw-r--r--   0        0        0     3137 2024-04-12 14:54:15.939692 therix-0.1.1/therix/services/pipeline_service.py
--rw-r--r--   0        0        0     1434 2024-04-12 14:54:15.939755 therix-0.1.1/therix/services/web_crawling.py
--rw-r--r--   0        0        0    10364 2024-04-12 14:54:15.939955 therix-0.1.1/therix/utils/rag.py
--rw-r--r--   0        0        0     2335 1970-01-01 00:00:00.000000 therix-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1218 2024-04-12 15:05:11.676463 therix-0.1.2/README.md
+-rw-r--r--   0        0        0      841 2024-04-16 06:14:22.172351 therix-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 14:54:15.929969 therix-0.1.2/therix/__init__.py
+-rw-r--r--   0        0        0     2083 2024-04-12 14:54:15.930143 therix-0.1.2/therix/core/JSONLoader.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:54:15.930181 therix-0.1.2/therix/core/__init__.py
+-rw-r--r--   0        0        0     1571 2024-04-12 14:54:15.930332 therix-0.1.2/therix/core/constants.py
+-rw-r--r--   0        0        0      854 2024-04-16 06:13:24.884093 therix-0.1.2/therix/core/data_sources.py
+-rw-r--r--   0        0        0     1676 2024-04-16 06:13:24.884272 therix-0.1.2/therix/core/embedding_models.py
+-rw-r--r--   0        0        0     2381 2024-04-16 06:13:24.884478 therix-0.1.2/therix/core/inference_models.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:54:15.930720 therix-0.1.2/therix/core/output_source.py
+-rw-r--r--   0        0        0     3422 2024-04-16 06:13:24.884674 therix-0.1.2/therix/core/pipeline.py
+-rw-r--r--   0        0        0     1153 2024-04-12 14:54:15.930956 therix-0.1.2/therix/core/pipeline_component.py
+-rw-r--r--   0        0        0      299 2024-04-16 06:13:24.884857 therix-0.1.2/therix/core/trace.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:54:15.931148 therix-0.1.2/therix/db/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-12 14:54:15.931283 therix-0.1.2/therix/db/base.py
+-rw-r--r--   0        0        0     2936 2024-04-16 06:13:24.885055 therix-0.1.2/therix/db/db_manager.py
+-rw-r--r--   0        0        0      410 2024-04-16 06:13:24.885241 therix-0.1.2/therix/db/session.py
+-rw-r--r--   0        0        0      234 2024-04-12 14:54:15.931776 therix-0.1.2/therix/docs/.gitignore
+-rw-r--r--   0        0        0      768 2024-04-12 14:54:15.931895 therix-0.1.2/therix/docs/README.md
+-rw-r--r--   0        0        0       89 2024-04-12 14:54:15.932023 therix-0.1.2/therix/docs/babel.config.js
+-rw-r--r--   0        0        0      389 2024-04-12 14:54:15.932200 therix-0.1.2/therix/docs/blog/2019-05-28-first-blog-post.md
+-rw-r--r--   0        0        0     3116 2024-04-12 14:54:15.932340 therix-0.1.2/therix/docs/blog/2019-05-29-long-blog-post.md
+-rw-r--r--   0        0        0      439 2024-04-12 14:54:15.932456 therix-0.1.2/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
+-rw-r--r--   0        0        0    96122 2024-04-12 14:54:15.932858 therix-0.1.2/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
+-rw-r--r--   0        0        0      783 2024-04-12 14:54:15.933048 therix-0.1.2/therix/docs/blog/2021-08-26-welcome/index.md
+-rw-r--r--   0        0        0      447 2024-04-12 14:54:15.933157 therix-0.1.2/therix/docs/blog/authors.yml
+-rw-r--r--   0        0        0     1411 2024-04-12 14:54:15.933315 therix-0.1.2/therix/docs/docs/intro.md
+-rw-r--r--   0        0        0      180 2024-04-12 14:54:15.933452 therix-0.1.2/therix/docs/docs/tutorial-basics/_category_.json
+-rw-r--r--   0        0        0     1078 2024-04-12 14:54:15.933560 therix-0.1.2/therix/docs/docs/tutorial-basics/congratulations.md
+-rw-r--r--   0        0        0      886 2024-04-12 14:54:15.933661 therix-0.1.2/therix/docs/docs/tutorial-basics/create-a-blog-post.md
+-rw-r--r--   0        0        0     1042 2024-04-12 14:54:15.933784 therix-0.1.2/therix/docs/docs/tutorial-basics/create-a-document.md
+-rw-r--r--   0        0        0     1015 2024-04-12 14:54:15.933895 therix-0.1.2/therix/docs/docs/tutorial-basics/create-a-page.md
+-rw-r--r--   0        0        0      702 2024-04-12 14:54:15.934002 therix-0.1.2/therix/docs/docs/tutorial-basics/deploy-your-site.md
+-rw-r--r--   0        0        0     3006 2024-04-12 14:54:15.934112 therix-0.1.2/therix/docs/docs/tutorial-basics/markdown-features.mdx
+-rw-r--r--   0        0        0       99 2024-04-12 14:54:15.934248 therix-0.1.2/therix/docs/docs/tutorial-extras/_category_.json
+-rw-r--r--   0        0        0    25427 2024-04-12 14:54:15.934440 therix-0.1.2/therix/docs/docs/tutorial-extras/img/docsVersionDropdown.png
+-rw-r--r--   0        0        0    27841 2024-04-12 14:54:15.934733 therix-0.1.2/therix/docs/docs/tutorial-extras/img/localeDropdown.png
+-rw-r--r--   0        0        0     1232 2024-04-12 14:54:15.934904 therix-0.1.2/therix/docs/docs/tutorial-extras/manage-docs-versions.md
+-rw-r--r--   0        0        0     1587 2024-04-12 14:54:15.935005 therix-0.1.2/therix/docs/docs/tutorial-extras/translate-your-site.md
+-rw-r--r--   0        0        0     3605 2024-04-12 14:54:15.935114 therix-0.1.2/therix/docs/docusaurus.config.js
+-rw-r--r--   0        0        0   573996 2024-04-12 14:54:15.936314 therix-0.1.2/therix/docs/package-lock.json
+-rw-r--r--   0        0        0     1061 2024-04-12 14:54:15.936493 therix-0.1.2/therix/docs/package.json
+-rw-r--r--   0        0        0      779 2024-04-12 14:54:15.936597 therix-0.1.2/therix/docs/sidebars.js
+-rw-r--r--   0        0        0     1721 2024-04-12 14:54:15.936828 therix-0.1.2/therix/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      138 2024-04-12 14:54:15.936929 therix-0.1.2/therix/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     2239 2024-04-12 14:54:15.937061 therix-0.1.2/therix/docs/src/css/custom.css
+-rw-r--r--   0        0        0      365 2024-04-12 14:54:15.937193 therix-0.1.2/therix/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0      118 2024-04-12 14:54:15.937292 therix-0.1.2/therix/docs/src/pages/markdown-page.md
+-rw-r--r--   0        0        0        0 2024-04-12 14:54:15.937368 therix-0.1.2/therix/docs/static/.nojekyll
+-rw-r--r--   0        0        0    21038 2024-04-12 14:54:15.937664 therix-0.1.2/therix/docs/static/img/coditas.png
+-rw-r--r--   0        0        0     5277 2024-04-12 14:54:15.937878 therix-0.1.2/therix/docs/static/img/coditasLogo.svg
+-rw-r--r--   0        0        0    55746 2024-04-12 14:54:15.938169 therix-0.1.2/therix/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0     5142 2024-04-12 14:54:15.938362 therix-0.1.2/therix/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0     3626 2024-04-12 14:54:15.938464 therix-0.1.2/therix/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0      506 2024-04-12 14:54:15.938561 therix-0.1.2/therix/docs/static/img/icon.svg
+-rw-r--r--   0        0        0     6438 2024-04-12 14:54:15.938694 therix-0.1.2/therix/docs/static/img/logo.svg
+-rw-r--r--   0        0        0    31486 2024-04-12 14:54:15.938840 therix-0.1.2/therix/docs/static/img/undraw_docusaurus_mountain.svg
+-rw-r--r--   0        0        0    36002 2024-04-12 14:54:15.939041 therix-0.1.2/therix/docs/static/img/undraw_docusaurus_react.svg
+-rw-r--r--   0        0        0    11887 2024-04-12 14:54:15.939300 therix-0.1.2/therix/docs/static/img/undraw_docusaurus_tree.svg
+-rw-r--r--   0        0        0        0 2024-04-12 14:54:15.939374 therix-0.1.2/therix/entities/__init__.py
+-rw-r--r--   0        0        0     2205 2024-04-12 14:54:15.939477 therix-0.1.2/therix/entities/models.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:54:15.939553 therix-0.1.2/therix/services/__init__.py
+-rw-r--r--   0        0        0     3411 2024-04-16 06:13:24.885453 therix-0.1.2/therix/services/pipeline_service.py
+-rw-r--r--   0        0        0     1434 2024-04-12 14:54:15.939755 therix-0.1.2/therix/services/web_crawling.py
+-rw-r--r--   0        0        0    10269 2024-04-16 06:13:24.885743 therix-0.1.2/therix/utils/rag.py
+-rw-r--r--   0        0        0     2348 1970-01-01 00:00:00.000000 therix-0.1.2/PKG-INFO
```

### Comparing `therix-0.1.1/LICENSE` & `therix-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/README.md` & `therix-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/pyproject.toml` & `therix-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "therix"
-version = "0.1.1"
+version = "0.1.2"
 description = "Therix is the SDK for langchain based applications."
 authors = ["Ajinath"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
@@ -20,15 +20,15 @@
 langfuse = "2.21.1"
 alembic-postgresql-enum = "1.1.2"
 greenlet = "^3.0.3"
 youtube-transcript-api = "^0.6.2"
 pytube = "^15.0.0"
 bs4 = "^0.0.2"
 selenium = "^4.19.0"
-psycopg = "^3.1.18"
+psycopg = {extras = ["binary", "pool"], version = "^3.1.18"}
 langchain-groq = "^0.1.0"
 boto3 = "^1.34.81"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 poetry-dotenv = "0.4.0"
```

### Comparing `therix-0.1.1/therix/core/JSONLoader.py` & `therix-0.1.2/therix/core/JSONLoader.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/core/constants.py` & `therix-0.1.2/therix/core/constants.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/core/data_sources.py` & `therix-0.1.2/therix/core/data_sources.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
-from therix_core.core.constants import DataSourceMaster
+from therix.core.constants import DataSourceMaster
 from .pipeline_component import DataSource
 
+
 class PDFDataSource(DataSource):
     def __init__(self, config):
         super().__init__(DataSourceMaster.PDF, config)
 
+
 class WebsiteDataSource(DataSource):
     def __init__(self, config):
         super().__init__(DataSourceMaster.WEBSITE, config)
 
+
 class CSVDataSource(DataSource):
     def __init__(self, config):
         super().__init__(DataSourceMaster.CSV, config)
 
+
 class DatabaseDataSource(DataSource):
     def __init__(self, config):
         super().__init__(DataSourceMaster.DATABASE, config)
 
+
 class DOCXDataSource(DataSource):
     def __init__(self, config):
         super().__init__(DataSourceMaster.DOCX, config)
-        
+
+
 class YoutubeDataSource(DataSource):
     def __init__(self, config):
-         super().__init__(DataSourceMaster.YOUTUBE, config)
+        super().__init__(DataSourceMaster.YOUTUBE, config)
```

### Comparing `therix-0.1.1/therix/core/embedding_models.py` & `therix-0.1.2/therix/core/embedding_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,52 @@
-
-from therix_core.core.constants import EmbeddingModelMaster
-from therix_core.core.pipeline_component import EmbeddingModel
+from therix.core.constants import EmbeddingModelMaster
+from therix.core.pipeline_component import EmbeddingModel
 
 
 class OpenAITextAdaEmbeddingModel(EmbeddingModel):
     def __init__(self, **kwargs):
         super().__init__(name=EmbeddingModelMaster.OPENAI_TEXT_ADA, **kwargs)
 
+
 class OpenAITextEmbedding3SmallEmbeddingModel(EmbeddingModel):
     def __init__(self, **kwargs):
-        super().__init__(name=EmbeddingModelMaster.OPENAI_TEXT_EMBEDDING_3_SMALL, **kwargs)
+        super().__init__(
+            name=EmbeddingModelMaster.OPENAI_TEXT_EMBEDDING_3_SMALL, **kwargs
+        )
+
 
 class OpenAITextEmbedding3LargeEmbeddingModel(EmbeddingModel):
     def __init__(self, **kwargs):
-        super().__init__(name=EmbeddingModelMaster.OPENAI_TEXT_EMBEDDING_3_LARGE, **kwargs)
-        
+        super().__init__(
+            name=EmbeddingModelMaster.OPENAI_TEXT_EMBEDDING_3_LARGE, **kwargs
+        )
+
+
 class AzureOpenAIEmbedding3SmallEmbeddingModel(EmbeddingModel):
     def __init__(self, **kwargs):
-        super().__init__(name=EmbeddingModelMaster.AZURE_TEXT_EMBEDDING_3_SMALL, **kwargs)
-        
+        super().__init__(
+            name=EmbeddingModelMaster.AZURE_TEXT_EMBEDDING_3_SMALL, **kwargs
+        )
+
+
 class AzureOpenAITextAdaEmbeddingModel(EmbeddingModel):
     def __init__(self, **kwargs):
         super().__init__(name=EmbeddingModelMaster.AZURE_TEXT_ADA, **kwargs)
-        
+
+
 class AzureOpenAIEmbedding3LargeEmbeddingModel(EmbeddingModel):
     def __init__(self, **kwargs):
-        super().__init__(name=EmbeddingModelMaster.AZURE_TEXT_EMBEDDING_3_LARGE, **kwargs)
-        
+        super().__init__(
+            name=EmbeddingModelMaster.AZURE_TEXT_EMBEDDING_3_LARGE, **kwargs
+        )
+
+
 class BedrockTitanEmbedding(EmbeddingModel):
     def __init__(self, **kwargs):
         super().__init__(name=EmbeddingModelMaster.BEDROCK_TITAN_EMBEDDING, **kwargs)
-        
+
+
 class BedrockTitanMultiModalEmbedding(EmbeddingModel):
     def __init__(self, **kwargs):
-        super().__init__(name=EmbeddingModelMaster.BEDROCK_TITAN_MULTIMODAL_EMBEDDING, **kwargs)
+        super().__init__(
+            name=EmbeddingModelMaster.BEDROCK_TITAN_MULTIMODAL_EMBEDDING, **kwargs
+        )
```

### Comparing `therix-0.1.1/therix/core/inference_models.py` & `therix-0.1.2/therix/core/inference_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,72 @@
-from therix_core.core.constants import InferenceModelMaster
-from therix_core.core.pipeline_component import InferenceModel
+from therix.core.constants import InferenceModelMaster
+from therix.core.pipeline_component import InferenceModel
 
 
 class OpenAIGPT35TurboInferenceModel(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(name=InferenceModelMaster.OPENAI_GPT_3_5_TURBO, config=config)
 
+
 class OpenAIGPT4InferenceModel(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(name=InferenceModelMaster.OPENAI_GPT_4, config=config)
 
+
 class OpenAIGPT4TurboPreviewInferenceModel(InferenceModel):
     def __init__(self, config: dict):
-        super().__init__(name=InferenceModelMaster.OPENAI_GPT_4_TURBO_PREVIEW, config=config)
+        super().__init__(
+            name=InferenceModelMaster.OPENAI_GPT_4_TURBO_PREVIEW, config=config
+        )
+
 
 class AzureOpenAIGPT3TurboPreviewInferenceModel(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(name=InferenceModelMaster.AZURE_GPT_3_5_TURBO, config=config)
-        
+
+
 class AzureOpenAIGPT3TurboInstructnferenceModel(InferenceModel):
     def __init__(self, config: dict):
-        super().__init__(name=InferenceModelMaster.AZURE_GPT_3_5_TURBO_INSTRUCT, config=config)
+        super().__init__(
+            name=InferenceModelMaster.AZURE_GPT_3_5_TURBO_INSTRUCT, config=config
+        )
+
 
 class AzureOpenAIGPT4InferenceModel(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(name=InferenceModelMaster.AZURE_GPT_4, config=config)
-        
+
+
 class AzureOpenAIGPT4TurboPreviewInferenceModel(InferenceModel):
     def __init__(self, config: dict):
-        super().__init__(name=InferenceModelMaster.AZURE_GPT_4_TURBO_PREVIEW, config=config)
-        
+        super().__init__(
+            name=InferenceModelMaster.AZURE_GPT_4_TURBO_PREVIEW, config=config
+        )
+
 
 class GroqMixtral87bInferenceModel(InferenceModel):
     def __init__(self, config: dict):
-        super().__init__(name=InferenceModelMaster.GROQ_LLM_MIXTRAL_8_7_B, config=config)
-        
+        super().__init__(
+            name=InferenceModelMaster.GROQ_LLM_MIXTRAL_8_7_B, config=config
+        )
+
+
 class GroqGemma7B(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(name=InferenceModelMaster.GROQ_LLM_GEMMA7B, config=config)
 
+
 class GroqLlama270b(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(name=InferenceModelMaster.GROQ_LLM_LLAMA2_70B, config=config)
+
+
 class BedrockTextExpressV1(InferenceModel):
     def __init__(self, config: dict):
-        super().__init__(name=InferenceModelMaster.BEDROCK_TEXT_EXPRES_V1, config=config)
+        super().__init__(
+            name=InferenceModelMaster.BEDROCK_TEXT_EXPRES_V1, config=config
+        )
+
 
 class BedrockTextExpressV1(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(name=InferenceModelMaster.BEDROCK_TEXT_LITE_G1, config=config)
```

### Comparing `therix-0.1.1/therix/core/pipeline.py` & `therix-0.1.2/therix/core/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from uuid import uuid4
-from therix_core.core.pipeline_component import PipelineComponent
+from therix.core.pipeline_component import PipelineComponent
 from .constants import DataSourceMaster, EmbeddingModelMaster  # Import your constants
 from ..services.pipeline_service import PipelineService  # Import your service
 from ..entities.models import ConfigType  # Import your ConfigType enum
 
+
 class Pipeline:
 
-    def __init__(self, name, status='IN_DRAFT'):
-        self.pipeline_data = {'name': name, 'status': status}
+    def __init__(self, name, status="IN_DRAFT"):
+        self.pipeline_data = {"name": name, "status": status}
         self.components = []
         self.pipeline_service = PipelineService()
-    
+
     @classmethod
     def from_id(cls, pipeline_id):
         pipeline = cls.__new__(cls)
         pipeline.__init__(None)
         pipeline.load(pipeline_id)
         return pipeline
 
@@ -38,40 +39,51 @@
 
     def add_output_source(self, name, config):
         output_source = PipelineComponent(ConfigType.OUTPUT_SOURCE, name, config)
         return self.add(output_source)
 
     def save(self):
         configurations_data = [
-            {'config_type': component.type.value, 'name': component.name, 'config': component.config}
+            {
+                "config_type": component.type.value,
+                "name": component.name,
+                "config": component.config,
+            }
             for component in self.components
         ]
         # Save the pipeline and its components to the database
-        self.pipeline_data = self.pipeline_service.create_pipeline_with_configurations(self.pipeline_data, configurations_data)
+        self.pipeline_data = self.pipeline_service.create_pipeline_with_configurations(
+            self.pipeline_data, configurations_data
+        )
         self.id = self.pipeline_data.id
         self.name = self.pipeline_data.name
         return self.pipeline_data
 
     def publish(self):
         return self.pipeline_service.publish_pipeline(self.pipeline_data)
-    
+
     def load(self, pipeline_id):
         self.pipeline_data = self.pipeline_service.get_pipeline(pipeline_id)
         self.id = self.pipeline_data.id
         self.name = self.pipeline_data.name
         return self.pipeline_data
 
     def preprocess_data(self):
         self.pipeline_service.preprocess_data(self.pipeline_data.id)
 
     def invoke(self, question, session_id=None):
         if session_id == None:
             session_id = uuid4()
-        pipeline_trace_config = self.pipeline_service.get_pipeline_configuraitons_by_type(self.pipeline_data.id, ConfigType.TRACE_DETAILS)
+        pipeline_trace_config = (
+            self.pipeline_service.get_pipeline_configuraitons_by_type(
+                self.pipeline_data.id, ConfigType.TRACE_DETAILS
+            )
+        )
         if pipeline_trace_config:
             trace_details = pipeline_trace_config[0].config
         else:
             trace_details = None
         # trace_details = { "name": self.pipeline_data.name, "id": self.pipeline_data.id}
         answer = self.pipeline_service.invoke_pipeline(
-            self.pipeline_data.id, question, session_id, trace_details)
+            self.pipeline_data.id, question, session_id, trace_details
+        )
         return {"answer": answer, "session_id": session_id}
```

### Comparing `therix-0.1.1/therix/core/pipeline_component.py` & `therix-0.1.2/therix/core/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/db/db_manager.py` & `therix-0.1.2/therix/db/db_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.exc import SQLAlchemyError
 from alembic.config import Config
 from alembic import command
 import logging
 import os
 
-from therix_core.db.base import Base
+from therix.db.base import Base
 
 
 # Configure logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
```

### Comparing `therix-0.1.1/therix/docs/README.md` & `therix-0.1.2/therix/docs/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/blog/2019-05-29-long-blog-post.md` & `therix-0.1.2/therix/docs/blog/2019-05-29-long-blog-post.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg` & `therix-0.1.2/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/blog/2021-08-26-welcome/index.md` & `therix-0.1.2/therix/docs/blog/2021-08-26-welcome/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docs/intro.md` & `therix-0.1.2/therix/docs/docs/intro.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docs/tutorial-basics/congratulations.md` & `therix-0.1.2/therix/docs/docs/tutorial-basics/congratulations.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docs/tutorial-basics/create-a-blog-post.md` & `therix-0.1.2/therix/docs/docs/tutorial-basics/create-a-blog-post.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docs/tutorial-basics/create-a-document.md` & `therix-0.1.2/therix/docs/docs/tutorial-basics/create-a-document.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docs/tutorial-basics/create-a-page.md` & `therix-0.1.2/therix/docs/docs/tutorial-basics/create-a-page.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docs/tutorial-basics/deploy-your-site.md` & `therix-0.1.2/therix/docs/docs/tutorial-basics/deploy-your-site.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docs/tutorial-basics/markdown-features.mdx` & `therix-0.1.2/therix/docs/docs/tutorial-basics/markdown-features.mdx`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docs/tutorial-extras/img/docsVersionDropdown.png` & `therix-0.1.2/therix/docs/docs/tutorial-extras/img/docsVersionDropdown.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docs/tutorial-extras/img/localeDropdown.png` & `therix-0.1.2/therix/docs/docs/tutorial-extras/img/localeDropdown.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docs/tutorial-extras/manage-docs-versions.md` & `therix-0.1.2/therix/docs/docs/tutorial-extras/manage-docs-versions.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docs/tutorial-extras/translate-your-site.md` & `therix-0.1.2/therix/docs/docs/tutorial-extras/translate-your-site.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/docusaurus.config.js` & `therix-0.1.2/therix/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/package-lock.json` & `therix-0.1.2/therix/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/package.json` & `therix-0.1.2/therix/docs/package.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/sidebars.js` & `therix-0.1.2/therix/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/src/components/HomepageFeatures/index.js` & `therix-0.1.2/therix/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/src/css/custom.css` & `therix-0.1.2/therix/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/static/img/coditas.png` & `therix-0.1.2/therix/docs/static/img/coditas.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/static/img/coditasLogo.svg` & `therix-0.1.2/therix/docs/static/img/coditasLogo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/static/img/docusaurus-social-card.jpg` & `therix-0.1.2/therix/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/static/img/docusaurus.png` & `therix-0.1.2/therix/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/static/img/favicon.ico` & `therix-0.1.2/therix/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/static/img/logo.svg` & `therix-0.1.2/therix/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/static/img/undraw_docusaurus_mountain.svg` & `therix-0.1.2/therix/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/static/img/undraw_docusaurus_react.svg` & `therix-0.1.2/therix/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/docs/static/img/undraw_docusaurus_tree.svg` & `therix-0.1.2/therix/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/entities/models.py` & `therix-0.1.2/therix/entities/models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/services/pipeline_service.py` & `therix-0.1.2/therix/services/pipeline_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,93 @@
 import json
 import os
 import urllib
-from therix_core.services.web_crawling import crawl_website
-from therix_core.utils.rag import chat, create_embeddings, get_vectorstore
+from therix.services.web_crawling import crawl_website
+from therix.utils.rag import chat, create_embeddings, get_vectorstore
 from ..db.session import SessionLocal
 from ..entities.models import Pipeline, PipelineConfiguration
-from therix_core.utils.rag import chat, create_embeddings, get_vectorstore
+from therix.utils.rag import chat, create_embeddings, get_vectorstore
+
+
 class PipelineService:
     def __init__(self):
         self.db_session = SessionLocal()
 
     def create_pipeline_with_configurations(self, pipeline_data, configurations_data):
         new_pipeline = Pipeline(**pipeline_data)
         self.db_session.add(new_pipeline)
         self.db_session.flush()  # Flush to assign an ID to the new_pipeline
 
         for config_data in configurations_data:
-            config_data['pipeline_id'] = new_pipeline.id
+            config_data["pipeline_id"] = new_pipeline.id
             new_config = PipelineConfiguration(**config_data)
             self.db_session.add(new_config)
 
         self.db_session.commit()
         return new_pipeline
-    
+
     def publish_pipeline(self, pipeline_data):
-        pipeline = self.db_session.query(Pipeline).filter_by(id=pipeline_data.id).first()
-        pipeline.status = 'PUBLISHED'
+        pipeline = (
+            self.db_session.query(Pipeline).filter_by(id=pipeline_data.id).first()
+        )
+        pipeline.status = "PUBLISHED"
         self.db_session.commit()
         return pipeline
-    
+
     def get_pipeline(self, pipeline_id):
         return self.db_session.query(Pipeline).filter_by(id=pipeline_id).first()
-    
+
     def get_pipeline_configurations(self, pipeline_id):
-        return self.db_session.query(PipelineConfiguration).filter_by(pipeline_id=pipeline_id).all()
-    
+        return (
+            self.db_session.query(PipelineConfiguration)
+            .filter_by(pipeline_id=pipeline_id)
+            .all()
+        )
+
     def get_pipeline_configuraitons_by_type(self, pipeline_id, config_type):
-        return self.db_session.query(PipelineConfiguration).filter_by(pipeline_id=pipeline_id, config_type=config_type).all()
+        return (
+            self.db_session.query(PipelineConfiguration)
+            .filter_by(pipeline_id=pipeline_id, config_type=config_type)
+            .all()
+        )
 
     def preprocess_data(self, pipeline_id):
-        data_sources = self.get_pipeline_configuraitons_by_type(pipeline_id, 'INPUT_SOURCE')
+        data_sources = self.get_pipeline_configuraitons_by_type(
+            pipeline_id, "INPUT_SOURCE"
+        )
         output_file = None
-        if 'website' in data_sources[0].config:
-            website_url = data_sources[0].config['website']
+        if "website" in data_sources[0].config:
+            website_url = data_sources[0].config["website"]
             web_content = crawl_website(website_url)
             domain_name = urllib.parse.urlparse(website_url).netloc
             output_file = f"{domain_name}_data.json"
             with open(output_file, "w") as f:
                 json.dump(web_content, f, indent=4)
-            data_sources[0].config['files'] = [output_file]
-        embedding_model = self.get_pipeline_configuraitons_by_type(pipeline_id, 'EMBEDDING_MODEL')
+            data_sources[0].config["files"] = [output_file]
+        embedding_model = self.get_pipeline_configuraitons_by_type(
+            pipeline_id, "EMBEDDING_MODEL"
+        )
         create_embeddings(data_sources, embedding_model[0], str(pipeline_id))
-        if 'website' in data_sources[0].config:
+        if "website" in data_sources[0].config:
             os.remove(output_file)
-    
+
     def invoke_pipeline(self, pipeline_id, question, session_id, trace_details=None):
-        embedding_model = self.get_pipeline_configuraitons_by_type(pipeline_id, 'EMBEDDING_MODEL')
+        embedding_model = self.get_pipeline_configuraitons_by_type(
+            pipeline_id, "EMBEDDING_MODEL"
+        )
         store = get_vectorstore(embedding_model[0], str(pipeline_id))
         retreiver = store.as_retriever()
-        inference_model = self.get_pipeline_configuraitons_by_type(pipeline_id, 'INFERENCE_MODEL')
-        return chat(question, retreiver, inference_model[0], embedding_model, session_id, pipeline_id, trace_details)
+        inference_model = self.get_pipeline_configuraitons_by_type(
+            pipeline_id, "INFERENCE_MODEL"
+        )
+        return chat(
+            question,
+            retreiver,
+            inference_model[0],
+            embedding_model,
+            session_id,
+            pipeline_id,
+            trace_details,
+        )
 
     def __del__(self):
         self.db_session.close()
```

### Comparing `therix-0.1.1/therix/services/web_crawling.py` & `therix-0.1.2/therix/services/web_crawling.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.1/therix/utils/rag.py` & `therix-0.1.2/therix/utils/rag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,193 +1,198 @@
 import json
 from operator import itemgetter
 from pathlib import Path
 from langchain.docstore.document import Document
 from langchain_community.document_loaders import TextLoader, PyPDFLoader
 from langchain_community.vectorstores.pgvector import PGVector
 from langchain_openai import OpenAIEmbeddings, ChatOpenAI
-from langchain_openai import AzureOpenAI 
+from langchain_openai import AzureOpenAI
 from langchain_groq import ChatGroq
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_community.document_loaders import YoutubeLoader
 from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
 from langchain_openai import AzureOpenAIEmbeddings
 
-from therix_core.core.JSONLoader import JSONLoader
+from therix.core.JSONLoader import JSONLoader
 from langchain_community.embeddings import BedrockEmbeddings
 import boto3
 from langchain_community.llms import Bedrock
-from therix_core.core.constants import (
+from therix.core.constants import (
     DataSourceMaster,
     EmbeddingModelMaster,
     InferenceModelMaster,
 )
-from therix_core.db.session import SQLALCHEMY_DATABASE_URL
+from therix.db.session import SQLALCHEMY_DATABASE_URL
 from langfuse.callback import CallbackHandler
 from langchain_core.prompts import PromptTemplate
 from langchain_community.vectorstores.pgvector import PGVector
 from langchain.memory import PostgresChatMessageHistory
 from langchain.prompts import PromptTemplate
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.runnables import RunnablePassthrough
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.messages import get_buffer_string
 from langchain_core.prompts import format_document
 from langchain_core.runnables import RunnableParallel
 from operator import itemgetter
 
+
 def sanitize_text(text):
     # Remove null characters (0x00) from the text
-    sanitized_text = text.replace('\x00', '')
+    sanitized_text = text.replace("\x00", "")
     return sanitized_text
 
 
-def get_loader(file_type, file_path,config):
+def get_loader(file_type, file_path, config):
     if file_type == DataSourceMaster.TEXT:
         return TextLoader(file_path)
     elif file_type == DataSourceMaster.PDF:
         return PyPDFLoader(file_path)
     elif file_type == DataSourceMaster.YOUTUBE:
         return YoutubeLoader.from_youtube_url(
-            file_path ,add_video_info=True,
-             language=[config['language'], "id"],
-             translation="en",
+            file_path,
+            add_video_info=True,
+            language=[config["language"], "id"],
+            translation="en",
         )
-        return  PyPDFLoader(file_path)
+        return PyPDFLoader(file_path)
     elif file_type == DataSourceMaster.WEBSITE:
         return JSONLoader(file_path)
     else:
         raise ValueError(f"Unknown data source type: {file_type}")
 
 
 def get_embedding_model(embedding_model_name, config):
     print(embedding_model_name, config)
     if (
         embedding_model_name == EmbeddingModelMaster.OPENAI_TEXT_ADA
         or embedding_model_name == EmbeddingModelMaster.OPENAI_TEXT_EMBEDDING_3_SMALL
         or embedding_model_name == EmbeddingModelMaster.OPENAI_TEXT_EMBEDDING_3_LARGE
-    ) and("api_key" in config):
+    ) and ("api_key" in config):
         return OpenAIEmbeddings(
             openai_api_key=config["api_key"], model=embedding_model_name
         )
     elif (
-         embedding_model_name == EmbeddingModelMaster.AZURE_TEXT_ADA
+        embedding_model_name == EmbeddingModelMaster.AZURE_TEXT_ADA
         or embedding_model_name == EmbeddingModelMaster.AZURE_TEXT_EMBEDDING_3_LARGE
-        or embedding_model_name == EmbeddingModelMaster.AZURE_TEXT_EMBEDDING_3_SMALL) and (
-            "azure_api_key"   in config
-        ):
-            return AzureOpenAIEmbeddings(
-            api_key=config["azure_api_key"], 
+        or embedding_model_name == EmbeddingModelMaster.AZURE_TEXT_EMBEDDING_3_SMALL
+    ) and ("azure_api_key" in config):
+        return AzureOpenAIEmbeddings(
+            api_key=config["azure_api_key"],
             model=embedding_model_name,
             azure_endpoint=config["azure_endpoint"],
             openai_api_version=config["openai_api_version"],
             azure_deployment=config["azure_deployment"],
         )
-        
-    elif(
+
+    elif (
         embedding_model_name == EmbeddingModelMaster.BEDROCK_TITAN_EMBEDDING
-        or embedding_model_name == EmbeddingModelMaster.BEDROCK_TITAN_MULTIMODAL_EMBEDDING
-        ) and ("bedrock_aws_session_token" in config ):
-        bedrock_client=boto3.client(
-            service_name='bedrock-runtime', 
+        or embedding_model_name
+        == EmbeddingModelMaster.BEDROCK_TITAN_MULTIMODAL_EMBEDDING
+    ) and ("bedrock_aws_session_token" in config):
+        bedrock_client = boto3.client(
+            service_name="bedrock-runtime",
             aws_access_key_id=config["bedrock_aws_access_key_id"],
             aws_secret_access_key=config["bedrock_aws_secret_access_key"],
             aws_session_token=config["bedrock_aws_session_token"],
-            region_name=config['bedrock_region_name']
+            region_name=config["bedrock_region_name"],
         )
-    
+
         return BedrockEmbeddings(
             credentials_profile_name="bedrock-admin",
             client=bedrock_client,
             model_id=embedding_model_name,
-            region_name=config['bedrock_region_name']
+            region_name=config["bedrock_region_name"],
         )
     else:
         raise ValueError(f"Unknown embedding model: {embedding_model_name}")
 
 
 def get_inference_model(inference_model_name, config):
     if (
         inference_model_name == InferenceModelMaster.OPENAI_GPT_3_5_TURBO
         or inference_model_name == InferenceModelMaster.OPENAI_GPT_3_5_TURBO_INSTRUCT
         or inference_model_name == InferenceModelMaster.OPENAI_GPT_4
         or inference_model_name == InferenceModelMaster.OPENAI_GPT_4_TURBO_PREVIEW
     ) and ("api_key" in config):
         return ChatOpenAI(openai_api_key=config["api_key"], model=inference_model_name)
-    elif(
-         inference_model_name == InferenceModelMaster.OPENAI_GPT_3_5_TURBO
+    elif (
+        inference_model_name == InferenceModelMaster.OPENAI_GPT_3_5_TURBO
         or inference_model_name == InferenceModelMaster.OPENAI_GPT_3_5_TURBO_INSTRUCT
         or inference_model_name == InferenceModelMaster.OPENAI_GPT_4
-        or inference_model_name == InferenceModelMaster.OPENAI_GPT_4_TURBO_PREVIEW) and (
-             "azure_api_key" in config
-        ):
+        or inference_model_name == InferenceModelMaster.OPENAI_GPT_4_TURBO_PREVIEW
+    ) and ("azure_api_key" in config):
         return AzureOpenAI(
-            api_key=config["azure_api_key"], 
+            api_key=config["azure_api_key"],
             model=inference_model_name,
             deployment_name=config["deployment_name"],
             azure_endpoint=config["azure_endpoint"],
             api_version=config["openai_api_version"],
-            )
-    elif(
-        inference_model_name == InferenceModelMaster.GROQ_LLM_MIXTRAL_8_7_B or
-        inference_model_name == InferenceModelMaster.GROQ_LLM_LLAMA2_70B or
-        inference_model_name == InferenceModelMaster.GROQ_LLM_GEMMA7B
-        ) and('groq_api_key' in config):
-        return ChatGroq(
-            groq_api_key=config["groq_api_key"],
-            model=inference_model_name
         )
-    
-    elif(
+    elif (
+        inference_model_name == InferenceModelMaster.GROQ_LLM_MIXTRAL_8_7_B
+        or inference_model_name == InferenceModelMaster.GROQ_LLM_LLAMA2_70B
+        or inference_model_name == InferenceModelMaster.GROQ_LLM_GEMMA7B
+    ) and ("groq_api_key" in config):
+        return ChatGroq(groq_api_key=config["groq_api_key"], model=inference_model_name)
 
-        inference_model_name == InferenceModelMaster.BEDROCK_TEXT_EXPRES_V1 
+    elif (
+        inference_model_name == InferenceModelMaster.BEDROCK_TEXT_EXPRES_V1
         or inference_model_name == InferenceModelMaster.BEDROCK_TEXT_LITE_G1
-        ) and ("bedrock_aws_session_token" in config ):
-        bedrock_client=boto3.client(
-            service_name='bedrock-runtime', 
+    ) and ("bedrock_aws_session_token" in config):
+        bedrock_client = boto3.client(
+            service_name="bedrock-runtime",
             aws_access_key_id=config["bedrock_aws_access_key_id"],
             aws_secret_access_key=config["bedrock_aws_secret_access_key"],
             aws_session_token=config["bedrock_aws_session_token"],
-            region_name=config['bedrock_region_name']
+            region_name=config["bedrock_region_name"],
         )
         return Bedrock(
             credentials_profile_name="bedrock-admin",
             model_id=inference_model_name,
             client=bedrock_client,
-            region_name=config['bedrock_region_name']
+            region_name=config["bedrock_region_name"],
         )
     else:
         raise ValueError(f"Unknown inference model: {inference_model_name}")
 
 
 def create_embeddings(data_sources, embedding_model, collection_name):
     store = get_vectorstore(embedding_model, collection_name)
     for data_source in data_sources:
         # data_source = {'name': 'PDF', 'config': {'files': ['path/to/file', 'path/to/file']}}
         for file_path in data_source.config["files"]:
-            loader = get_loader(data_source.name, file_path,data_source.config)
+            loader = get_loader(data_source.name, file_path, data_source.config)
             pages = loader.load_and_split()
             # text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
-            
+
             store.add_documents(pages)
             return "embedding created"
 
 
 def get_vectorstore(embedding_model, collection_name):
     embeddings = get_embedding_model(embedding_model.name, embedding_model.config)
     store = PGVector(
         collection_name=collection_name,
         connection_string=SQLALCHEMY_DATABASE_URL,
         embedding_function=embeddings,
     )
     return store
 
 
-def chat(question, retriever, inference_model, embed_model, session_id, pipeline_id, trace_details=None):
+def chat(
+    question,
+    retriever,
+    inference_model,
+    embed_model,
+    session_id,
+    pipeline_id,
+    trace_details=None,
+):
 
     print(trace_details)
 
     chain_callbacks = []
     if trace_details is not None:
         langfuse_handler = CallbackHandler(
             secret_key=trace_details["secret_key"],
@@ -196,15 +201,15 @@
             trace_name=trace_details["identifier"],
         )
         chain_callbacks.append(langfuse_handler)
 
     history = PostgresChatMessageHistory(
         connection_string=SQLALCHEMY_DATABASE_URL,
         table_name="chat_history",
-        session_id=str(session_id)
+        session_id=str(session_id),
     )
     chat_history = history.messages
 
     template = """Answer the question based only on the following context:
                      {context}
 
                     Question: {question}
@@ -213,20 +218,20 @@
     _template = """Given the following conversation and a follow up question, rephrase the follow up question to be a standalone question, in its original language.
                     Chat History:
                     {chat_history}
                     Follow Up Input: {question}
                     Standalone question:"""
 
     CONDENSE_QUESTION_PROMPT = PromptTemplate.from_template(_template)
-    DEFAULT_DOCUMENT_PROMPT = PromptTemplate.from_template(
-        template="{page_content}")
+    DEFAULT_DOCUMENT_PROMPT = PromptTemplate.from_template(template="{page_content}")
 
-    def _combine_documents(docs, document_prompt=DEFAULT_DOCUMENT_PROMPT, document_separator="\n\n"):
-        doc_strings = [format_document(
-            doc, document_prompt) for doc in docs]
+    def _combine_documents(
+        docs, document_prompt=DEFAULT_DOCUMENT_PROMPT, document_separator="\n\n"
+    ):
+        doc_strings = [format_document(doc, document_prompt) for doc in docs]
         return document_separator.join(doc_strings)
 
     model = get_inference_model(inference_model.name, inference_model.config)
 
     _inputs = RunnableParallel(
         standalone_question=RunnablePassthrough.assign(
             chat_history=lambda x: get_buffer_string(x["chat_history"])
@@ -236,15 +241,14 @@
         | StrOutputParser(),
     )
     _context = {
         "context": itemgetter("standalone_question") | retriever | _combine_documents,
         "question": lambda x: x["standalone_question"],
     }
     conversational_qa_chain = _inputs | _context | ANSWER_PROMPT | model
-    result = conversational_qa_chain.invoke({
-        "question": question,
-        "chat_history": chat_history
-    })
+    result = conversational_qa_chain.invoke(
+        {"question": question, "chat_history": chat_history}
+    )
 
     history.add_user_message(question)
     history.add_ai_message(result)
     return json.loads(result.json())["content"]
```

### Comparing `therix-0.1.1/PKG-INFO` & `therix-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: therix
-Version: 0.1.1
+Version: 0.1.2
 Summary: Therix is the SDK for langchain based applications.
 License: MIT
 Author: Ajinath
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
@@ -14,16 +14,16 @@
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Requires-Dist: langchain (==0.1.13)
 Requires-Dist: langchain-groq (>=0.1.0,<0.2.0)
 Requires-Dist: langchain-openai (==0.1.1)
 Requires-Dist: langfuse (==2.21.1)
 Requires-Dist: pgvector (==0.2.5)
-Requires-Dist: psycopg (>=3.1.18,<4.0.0)
 Requires-Dist: psycopg2-binary (==2.9.9)
+Requires-Dist: psycopg[binary,pool] (>=3.1.18,<4.0.0)
 Requires-Dist: pypdf (==4.1.0)
 Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: selenium (>=4.19.0,<5.0.0)
 Requires-Dist: sqlalchemy (==2.0.28)
 Requires-Dist: tiktoken (==0.6.0)
 Requires-Dist: wheel (>=0.43.0,<0.44.0)
 Requires-Dist: youtube-transcript-api (>=0.6.2,<0.7.0)
```

