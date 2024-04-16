# Comparing `tmp/nio-bot-1.1.0b1.tar.gz` & `tmp/nio-bot-1.1.0b1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nio-bot-1.1.0b1.tar", last modified: Mon Oct 16 13:47:25 2023, max compression
+gzip compressed data, was "nio-bot-1.1.0b1.post1.tar", last modified: Mon Oct 16 14:00:02 2023, max compression
```

## Comparing `nio-bot-1.1.0b1.tar` & `nio-bot-1.1.0b1.post1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.557714 nio-bot-1.1.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.545714 nio-bot-1.1.0b1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.545714 nio-bot-1.1.0b1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.545714 nio-bot-1.1.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.545714 nio-bot-1.1.0b1/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.idea/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.545714 nio-bot-1.1.0b1/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.idea/markdown.xml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.idea/nio-bot.iml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2023-10-16 13:47:25.553714 nio-bot-1.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7303 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.545714 nio-bot-1.1.0b1/dev/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1094 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/dev/release.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.545714 nio-bot-1.1.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.541714 nio-bot-1.1.0b1/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.541714 nio-bot-1.1.0b1/docs/assets/guides/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.541714 nio-bot-1.1.0b1/docs/assets/guides/images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.545714 nio-bot-1.1.0b1/docs/assets/guides/images/sending-attachments/
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/assets/guides/images/sending-attachments/blurhash-dehashed.avif
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/assets/guides/images/sending-attachments/blurhash-hashed.avif
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/assets/guides/images/sending-attachments/file-send.avif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.545714 nio-bot-1.1.0b1/docs/assets/guides/text/
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/assets/guides/text/example_ffprobe.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/assets/guides/text/example_identify.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.545714 nio-bot-1.1.0b1/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/guides/a-simple-bot.md
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/guides/creating-custom-parsers.md
--rw-r--r--   0 runner    (1001) docker     (127)    15178 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/guides/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/guides/sending-attachments.md
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.545714 nio-bot-1.1.0b1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/attachment.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/client.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/commands.md
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/context.md
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/events.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/exceptions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.549714 nio-bot-1.1.0b1/docs/reference/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/utils/federation.md
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/utils/help_command.md
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/utils/parsers.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/utils/string_view.md
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/utils/typing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/docs/reference/utils/unblock.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.549714 nio-bot-1.1.0b1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/examples/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 13:47:25.557714 nio-bot-1.1.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.541714 nio-bot-1.1.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.549714 nio-bot-1.1.0b1/src/nio_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2023-10-16 13:47:25.000000 nio-bot-1.1.0b1/src/nio_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-10-16 13:47:25.000000 nio-bot-1.1.0b1/src/nio_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 13:47:25.000000 nio-bot-1.1.0b1/src/nio_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-16 13:47:25.000000 nio-bot-1.1.0b1/src/nio_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-10-16 13:47:25.000000 nio-bot-1.1.0b1/src/nio_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-16 13:47:25.000000 nio-bot-1.1.0b1/src/nio_bot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.549714 nio-bot-1.1.0b1/src/niobot/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14042 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-10-16 13:47:25.000000 nio-bot-1.1.0b1/src/niobot/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/_event_stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    45168 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    42438 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18474 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.549714 nio-bot-1.1.0b1/src/niobot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/utils/federation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/utils/help_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/utils/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18133 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/utils/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/utils/string_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/niobot/utils/unblocking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.549714 nio-bot-1.1.0b1/src/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:47:25.553714 nio-bot-1.1.0b1/src/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/tests/assets/CREDITS.md
--rw-r--r--   0 runner    (1001) docker     (127)    29517 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/tests/assets/sample-15s.ogg
--rw-r--r--   0 runner    (1001) docker     (127)  1407681 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/tests/assets/sample-5s-compressed.mp4
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/tests/assets/sample-clouds.avif
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/tests/assets/sample-lipsum-10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/tests/test_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/src/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-10-16 13:47:12.000000 nio-bot-1.1.0b1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.791439 nio-bot-1.1.0b1.post1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.775439 nio-bot-1.1.0b1.post1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.775439 nio-bot-1.1.0b1.post1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.775439 nio-bot-1.1.0b1.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.779439 nio-bot-1.1.0b1.post1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.idea/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.779439 nio-bot-1.1.0b1.post1/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.idea/markdown.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.idea/nio-bot.iml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2023-10-16 14:00:02.791439 nio-bot-1.1.0b1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7303 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.779439 nio-bot-1.1.0b1.post1/dev/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1094 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/dev/release.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.779439 nio-bot-1.1.0b1.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.767439 nio-bot-1.1.0b1.post1/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.767439 nio-bot-1.1.0b1.post1/docs/assets/guides/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.767439 nio-bot-1.1.0b1.post1/docs/assets/guides/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.783439 nio-bot-1.1.0b1.post1/docs/assets/guides/images/sending-attachments/
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/assets/guides/images/sending-attachments/blurhash-dehashed.avif
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/assets/guides/images/sending-attachments/blurhash-hashed.avif
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/assets/guides/images/sending-attachments/file-send.avif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.783439 nio-bot-1.1.0b1.post1/docs/assets/guides/text/
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/assets/guides/text/example_ffprobe.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/assets/guides/text/example_identify.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.783439 nio-bot-1.1.0b1.post1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/guides/a-simple-bot.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/guides/creating-custom-parsers.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15178 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/guides/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/guides/sending-attachments.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.783439 nio-bot-1.1.0b1.post1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/attachment.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/client.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/commands.md
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/events.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/exceptions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.787439 nio-bot-1.1.0b1.post1/docs/reference/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/utils/federation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/utils/help_command.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/utils/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/utils/string_view.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/utils/typing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/docs/reference/utils/unblock.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.787439 nio-bot-1.1.0b1.post1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/examples/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 14:00:02.791439 nio-bot-1.1.0b1.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.771439 nio-bot-1.1.0b1.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.787439 nio-bot-1.1.0b1.post1/src/nio_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2023-10-16 14:00:02.000000 nio-bot-1.1.0b1.post1/src/nio_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-10-16 14:00:02.000000 nio-bot-1.1.0b1.post1/src/nio_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 14:00:02.000000 nio-bot-1.1.0b1.post1/src/nio_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-16 14:00:02.000000 nio-bot-1.1.0b1.post1/src/nio_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2023-10-16 14:00:02.000000 nio-bot-1.1.0b1.post1/src/nio_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-16 14:00:02.000000 nio-bot-1.1.0b1.post1/src/nio_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.787439 nio-bot-1.1.0b1.post1/src/niobot/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14042 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2023-10-16 14:00:02.000000 nio-bot-1.1.0b1.post1/src/niobot/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/_event_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45168 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42521 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18474 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.787439 nio-bot-1.1.0b1.post1/src/niobot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/utils/federation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/utils/help_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/utils/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18133 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/utils/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/utils/string_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/niobot/utils/unblocking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.787439 nio-bot-1.1.0b1.post1/src/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:00:02.791439 nio-bot-1.1.0b1.post1/src/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/tests/assets/CREDITS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    29517 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/tests/assets/sample-15s.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)  1407681 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/tests/assets/sample-5s-compressed.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/tests/assets/sample-clouds.avif
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/tests/assets/sample-lipsum-10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/tests/test_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/src/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-10-16 13:59:50.000000 nio-bot-1.1.0b1.post1/tox.ini
```

### Comparing `nio-bot-1.1.0b1/.github/ISSUE_TEMPLATE/bug_report.md` & `nio-bot-1.1.0b1.post1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/.github/ISSUE_TEMPLATE/feature_request.md` & `nio-bot-1.1.0b1.post1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/.github/dependabot.yml` & `nio-bot-1.1.0b1.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/.github/workflows/python-package.yml` & `nio-bot-1.1.0b1.post1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/.github/workflows/python-publish.yml` & `nio-bot-1.1.0b1.post1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/.gitignore` & `nio-bot-1.1.0b1.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/.idea/inspectionProfiles/Project_Default.xml` & `nio-bot-1.1.0b1.post1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/CONTRIBUTING.md` & `nio-bot-1.1.0b1.post1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/Dockerfile` & `nio-bot-1.1.0b1.post1/Dockerfile`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/LICENSE` & `nio-bot-1.1.0b1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/PKG-INFO` & `nio-bot-1.1.0b1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nio-bot
-Version: 1.1.0b1
+Version: 1.1.0b1.post1
 Summary: Making matrix bots simple
 Author-email: Nexus <pip@nexy7574.co.uk>
 License: GNU GPLv3
 Project-URL: Source, https://github.com/nexy7574/niobot
 Project-URL: Tracker, https://github.com/nexy7574/niobot/issues
 Project-URL: Documentation, https://nexy7574.github.io/niobot/
 Project-URL: Matrix Room, https://matrix.to/#/#niobot:nexy7574.co.uk
```

### Comparing `nio-bot-1.1.0b1/README.md` & `nio-bot-1.1.0b1.post1/README.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/SECURITY.md` & `nio-bot-1.1.0b1.post1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/dev/release.sh` & `nio-bot-1.1.0b1.post1/dev/release.sh`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/assets/guides/images/sending-attachments/blurhash-dehashed.avif` & `nio-bot-1.1.0b1.post1/docs/assets/guides/images/sending-attachments/blurhash-dehashed.avif`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/assets/guides/images/sending-attachments/blurhash-hashed.avif` & `nio-bot-1.1.0b1.post1/docs/assets/guides/images/sending-attachments/blurhash-hashed.avif`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/assets/guides/images/sending-attachments/file-send.avif` & `nio-bot-1.1.0b1.post1/docs/assets/guides/images/sending-attachments/file-send.avif`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/assets/guides/text/example_ffprobe.json` & `nio-bot-1.1.0b1.post1/docs/assets/guides/text/example_ffprobe.json`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/guides/a-simple-bot.md` & `nio-bot-1.1.0b1.post1/docs/guides/a-simple-bot.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/guides/creating-custom-parsers.md` & `nio-bot-1.1.0b1.post1/docs/guides/creating-custom-parsers.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/guides/getting-started.md` & `nio-bot-1.1.0b1.post1/docs/guides/getting-started.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/guides/sending-attachments.md` & `nio-bot-1.1.0b1.post1/docs/guides/sending-attachments.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/index.md` & `nio-bot-1.1.0b1.post1/docs/index.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/reference/context.md` & `nio-bot-1.1.0b1.post1/docs/reference/context.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/reference/events.md` & `nio-bot-1.1.0b1.post1/docs/reference/events.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/reference/utils/help_command.md` & `nio-bot-1.1.0b1.post1/docs/reference/utils/help_command.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/reference/utils/parsers.md` & `nio-bot-1.1.0b1.post1/docs/reference/utils/parsers.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/reference/utils/string_view.md` & `nio-bot-1.1.0b1.post1/docs/reference/utils/string_view.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/reference/utils/typing.md` & `nio-bot-1.1.0b1.post1/docs/reference/utils/typing.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/docs/reference/utils/unblock.md` & `nio-bot-1.1.0b1.post1/docs/reference/utils/unblock.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/mkdocs.yml` & `nio-bot-1.1.0b1.post1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/pyproject.toml` & `nio-bot-1.1.0b1.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/nio_bot.egg-info/PKG-INFO` & `nio-bot-1.1.0b1.post1/src/nio_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nio-bot
-Version: 1.1.0b1
+Version: 1.1.0b1.post1
 Summary: Making matrix bots simple
 Author-email: Nexus <pip@nexy7574.co.uk>
 License: GNU GPLv3
 Project-URL: Source, https://github.com/nexy7574/niobot
 Project-URL: Tracker, https://github.com/nexy7574/niobot/issues
 Project-URL: Documentation, https://nexy7574.github.io/niobot/
 Project-URL: Matrix Room, https://matrix.to/#/#niobot:nexy7574.co.uk
```

### Comparing `nio-bot-1.1.0b1/src/nio_bot.egg-info/SOURCES.txt` & `nio-bot-1.1.0b1.post1/src/nio_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/__init__.py` & `nio-bot-1.1.0b1.post1/src/niobot/__init__.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/__main__.py` & `nio-bot-1.1.0b1.post1/src/niobot/__main__.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/_event_stubs.py` & `nio-bot-1.1.0b1.post1/src/niobot/_event_stubs.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/attachment.py` & `nio-bot-1.1.0b1.post1/src/niobot/attachment.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/client.py` & `nio-bot-1.1.0b1.post1/src/niobot/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,22 +394,23 @@
                         len(set(instance.list_commands())),
                         instance.__class__.__qualname__,
                     )
                 else:
                     self.log.debug("%r does not appear to be a niobot module", item)
         return added
 
-    def unmount_module(self, import_path: str) -> None:
+    def unmount_module(self, module: Module) -> None:
         """
         Does the opposite of mounting the module.
         This will remove any commands that have been added to the bot from the given module.
 
-        :param import_path:
-        :return:
+        :param module: The module to unmount
         """
+        self.log.debug("Unmounting module %r", module)
+        module.__teardown__()
 
     @property
     def commands(self) -> dict[str, Command]:
         """Returns the internal command register.
 
         !!! warning
             Modifying any values here will update the internal register too.
```

### Comparing `nio-bot-1.1.0b1/src/niobot/commands.py` & `nio-bot-1.1.0b1.post1/src/niobot/commands.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/context.py` & `nio-bot-1.1.0b1.post1/src/niobot/context.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/exceptions.py` & `nio-bot-1.1.0b1.post1/src/niobot/exceptions.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/utils/checks.py` & `nio-bot-1.1.0b1.post1/src/niobot/utils/checks.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/utils/federation.py` & `nio-bot-1.1.0b1.post1/src/niobot/utils/federation.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/utils/help_command.py` & `nio-bot-1.1.0b1.post1/src/niobot/utils/help_command.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/utils/lib.py` & `nio-bot-1.1.0b1.post1/src/niobot/utils/lib.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/utils/parsers.py` & `nio-bot-1.1.0b1.post1/src/niobot/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/utils/string_view.py` & `nio-bot-1.1.0b1.post1/src/niobot/utils/string_view.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/utils/typing.py` & `nio-bot-1.1.0b1.post1/src/niobot/utils/typing.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/niobot/utils/unblocking.py` & `nio-bot-1.1.0b1.post1/src/niobot/utils/unblocking.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/tests/assets/CREDITS.md` & `nio-bot-1.1.0b1.post1/src/tests/assets/CREDITS.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/tests/assets/sample-15s.ogg` & `nio-bot-1.1.0b1.post1/src/tests/assets/sample-15s.ogg`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/tests/assets/sample-5s-compressed.mp4` & `nio-bot-1.1.0b1.post1/src/tests/assets/sample-5s-compressed.mp4`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/tests/assets/sample-lipsum-10.txt` & `nio-bot-1.1.0b1.post1/src/tests/assets/sample-lipsum-10.txt`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/tests/test_attachment.py` & `nio-bot-1.1.0b1.post1/src/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.1.0b1/src/tests/test_parsers.py` & `nio-bot-1.1.0b1.post1/src/tests/test_parsers.py`

 * *Files identical despite different names*

