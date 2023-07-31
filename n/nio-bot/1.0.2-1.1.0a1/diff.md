# Comparing `tmp/nio-bot-1.0.2.tar.gz` & `tmp/nio-bot-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nio-bot-1.0.2.tar", last modified: Sun Jul 16 14:34:50 2023, max compression
+gzip compressed data, was "nio-bot-1.1.0a1.tar", last modified: Mon Jul 31 17:59:31 2023, max compression
```

## Comparing `nio-bot-1.0.2.tar` & `nio-bot-1.1.0a1.tar`

### file list

```diff
@@ -1,84 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.352550 nio-bot-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/markdown.xml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/nio-bot.iml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-16 14:34:38.000000 nio-bot-1.0.2/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-16 14:34:38.000000 nio-bot-1.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 14:34:38.000000 nio-bot-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-07-16 14:34:50.352550 nio-bot-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-07-16 14:34:38.000000 nio-bot-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/docs/assets/guides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/docs/assets/guides/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/assets/guides/images/sending-attachments/
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/assets/guides/images/sending-attachments/blurhash-dehashed.avif
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/assets/guides/images/sending-attachments/blurhash-hashed.avif
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/assets/guides/images/sending-attachments/file-send.avif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/assets/guides/text/
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/assets/guides/text/example_ffprobe.json
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/assets/guides/text/example_identify.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/guides/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/guides/sending-attachments.md
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/attachment.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/client.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/commands.md
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/context.md
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/exceptions.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/docs/reference/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/federation.md
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/help_command.md
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/parsers.md
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/string_view.md
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/typing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-16 14:34:38.000000 nio-bot-1.0.2/docs/reference/utils/unblock.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-16 14:34:38.000000 nio-bot-1.0.2/examples/access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-16 14:34:38.000000 nio-bot-1.0.2/examples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-16 14:34:38.000000 nio-bot-1.0.2/examples/uploading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-16 14:34:38.000000 nio-bot-1.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-16 14:34:38.000000 nio-bot-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-16 14:34:38.000000 nio-bot-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 14:34:50.352550 nio-bot-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.344550 nio-bot-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.348550 nio-bot-1.0.2/src/nio_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/nio_bot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.352550 nio-bot-1.0.2/src/niobot/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-16 14:34:50.000000 nio-bot-1.0.2/src/niobot/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34066 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    33431 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:34:50.352550 nio-bot-1.0.2/src/niobot/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/federation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/help_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/string_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-16 14:34:38.000000 nio-bot-1.0.2/src/niobot/utils/unblocking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.618183 nio-bot-1.1.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.610182 nio-bot-1.1.0a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.610182 nio-bot-1.1.0a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.610182 nio-bot-1.1.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.610182 nio-bot-1.1.0a1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.idea/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.610182 nio-bot-1.1.0a1/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.idea/markdown.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.idea/nio-bot.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-07-31 17:59:31.618183 nio-bot-1.1.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.610182 nio-bot-1.1.0a1/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/dev/release.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.610182 nio-bot-1.1.0a1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.606181 nio-bot-1.1.0a1/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.606181 nio-bot-1.1.0a1/docs/assets/guides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.606181 nio-bot-1.1.0a1/docs/assets/guides/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.614182 nio-bot-1.1.0a1/docs/assets/guides/images/sending-attachments/
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/assets/guides/images/sending-attachments/blurhash-dehashed.avif
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/assets/guides/images/sending-attachments/blurhash-hashed.avif
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/assets/guides/images/sending-attachments/file-send.avif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.614182 nio-bot-1.1.0a1/docs/assets/guides/text/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/assets/guides/text/example_ffprobe.json
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/assets/guides/text/example_identify.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.614182 nio-bot-1.1.0a1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/guides/a-simple-bot.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/guides/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/guides/sending-attachments.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.614182 nio-bot-1.1.0a1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/attachment.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/client.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/context.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/events.md
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/exceptions.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.614182 nio-bot-1.1.0a1/docs/reference/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/utils/federation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/utils/help_command.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/utils/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/utils/string_view.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/utils/typing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/docs/reference/utils/unblock.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.614182 nio-bot-1.1.0a1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/examples/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/examples/uploading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 17:59:31.618183 nio-bot-1.1.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.606181 nio-bot-1.1.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.614182 nio-bot-1.1.0a1/src/nio_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-07-31 17:59:31.000000 nio-bot-1.1.0a1/src/nio_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-31 17:59:31.000000 nio-bot-1.1.0a1/src/nio_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:59:31.000000 nio-bot-1.1.0a1/src/nio_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 17:59:31.000000 nio-bot-1.1.0a1/src/nio_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-31 17:59:31.000000 nio-bot-1.1.0a1/src/nio_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 17:59:31.000000 nio-bot-1.1.0a1/src/nio_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.618183 nio-bot-1.1.0a1/src/niobot/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 17:59:31.000000 nio-bot-1.1.0a1/src/niobot/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/_event_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40912 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14936 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:59:31.618183 nio-bot-1.1.0a1/src/niobot/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/utils/federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/utils/help_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/utils/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/utils/string_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-31 17:59:16.000000 nio-bot-1.1.0a1/src/niobot/utils/unblocking.py
```

### Comparing `nio-bot-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `nio-bot-1.1.0a1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md` & `nio-bot-1.1.0a1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/.github/workflows/python-package.yml` & `nio-bot-1.1.0a1/.github/workflows/python-package.yml`

 * *Files 16% similar despite different names*

```diff
@@ -22,12 +22,12 @@
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
-        python -m pip install --upgrade pytest pip
-        pip install -r requirements.txt
-    - name: Test metadata
+        python -m pip install --upgrade pytest pip wheel setuptools
+        pip install -r requirements.txt build
+    - name: build
       run: |
-        python3 src/niobot/setup.py test -m -s
+        python3 -m build
```

### Comparing `nio-bot-1.0.2/.github/workflows/python-publish.yml` & `nio-bot-1.1.0a1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/.gitignore` & `nio-bot-1.1.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/.idea/inspectionProfiles/Project_Default.xml` & `nio-bot-1.1.0a1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/Dockerfile` & `nio-bot-1.1.0a1/Dockerfile`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/LICENSE` & `nio-bot-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/PKG-INFO` & `nio-bot-1.1.0a1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,55 @@
 Metadata-Version: 2.1
 Name: nio-bot
-Version: 1.0.2
+Version: 1.1.0a1
 Summary: Making matrix bots simple
-Author-email: Nexus <packages@nexy7574.co.uk>
+Author-email: Nexus <pip@nexy7574.co.uk>
 License: GNU GPLv3
 Project-URL: Source, https://github.com/eekim10/niobot
 Project-URL: Tracker, https://github.com/eekim10/niobot/issues
 Project-URL: Documentation, https://eekim10.github.io/niobot/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: e2ee
 Provides-Extra: cli
 Provides-Extra: dev
 License-File: LICENSE
 
 # NioBot
-A simple, easy to use python Matrix bot library, based on the excellent 
+A simple, easy to use python Matrix bot library, based on the excellent
 [matrix-nio](https://pypi.org/project/matrix-nio/) library.
 
 NioBot is designed to have a similar (as similar as reasonably possible) design and feel to the
 [discord.py](https://pypi.org/project/discord.py) library, which should hopefully give it a familiar feel if you're
 coming from a discord background.
 
 Please note that there *will* be teething problems, and as such some advanced features may not be
 available, as with any client.
 
 ## Need help?
-Take a look at the [docs!](https://eekim10.github.io/niobot)
+Take a look at the [docs!](https://eekim10.github.io/niobot), or
+[![Chat on Matrix](https://matrix.to/img/matrix-badge.svg)](https://matrix.to/#/#niobot:nexy7574.co.uk)
+(dedicated support room)
 
 ---
 
 Alternatively, take a look at my [dev bot](https://github.com/EEKIM10/niobot-test), which is a bot that I use to test
 features of nio-bot before they're released.
 This bot is very advanced as, since I developed the library, I know exactly how it works, and will have bleeding-edge
 features built into it, which a lot of users may not use yet.
 
 It is, however, a great example of how an advanced, full feature bot can be created using this library.
 
 You can see it live [here](https://matrix.to/#/@jimmy-bot:nexy7574.co.uk)
-(DM it, the prefix is ?, and full end-to-end encryption is supported. Average response time is ~300-500ms)
+(DM it, the prefix is ?, and full end-to-end encryption is supported(*). Average response time is ~300-500ms)
 
-## Installation
-### Versions
-NioBot uses SemVer (semantic versioning) for versioning. This means that the version number is split into three parts:
-`Major`, `Minor` and `Patch`. As per the versioning, `Major` versions are not guaranteed to be backwards compatible,
-however `Minor` and `Patch` versions are.
-
-This means that there will always be a new `Major` increment when a backwards incompatible change is made, and a new
-`Minor` increment when a backwards compatible change is made. `Patch` versions are almost always bug fixes, and are
-always backwards compatible. If a bug fix is not backwards compatible, a new `Major` version will be released.
-
-Major changes may be pushed into their own branches for "feature previews". These branches will be prefixed with
-`feature/`, and will be merged into `master` when they are ready for release. For example, `feature/my-thing`,
-which means you can install it using `niobot @ git+https://github.com/EEKIM10/niobot.git@feature/my-thing`.
-This minimises the number of breaking releases.
+(\* May not always work due to key store issues, but it should work most of the time, especially if its your first
+time using it.)
 
+## Installation
 ### Release versions
 You can use the [PyPi](https://pypi.org/project/niobot) releases:
 ```python
 niobot==1.0.0  # or whatever version
 # Or to install it with extras
 niobot[e2ee,cli]==1.0.0
 ```
@@ -70,21 +61,17 @@
 # Or with e2ee support (note you will need libolm)
 matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git
 ```
 You can figure out how to install it in other ways.
 
 ## Features
 NioBot aims to be as easy to use as possible, so form is preferred over function.
-Some features you'd normally expect may not be implemented (yet, feel free to open a pull request!) or may not work as 
+Some features you'd normally expect may not be implemented (yet, feel free to open a pull request!) or may not work as
 intended or how you'd expect, however as with any matrix client.
 
-However, like any good client, NioBot tries to adhere to the 
-[Matrix Spec](https://spec.matrix.org/v1.7/client-server-api) (in terms of design at least, all the hard work is 
-done by matrix-nio)
-
 ## Quickstart
 ```python
 import time
 from niobot import Bot, Context
 
 bot = Bot(
     homeserver="https://matrix.org",  # your homeserver
@@ -139,51 +126,51 @@
 
 bot.run(password="password")
 ```
 
 When you call `mount_module`, it effectively calls `import module` under the hood, and then does one of the following:
 
 1. Calls the `module.setup(bot)` function, if it exists
-2. Discovers all classes that subclass `niolib.Module` in the module, and calls their `__setup__`, adding all commands
+2. Discovers all classes that subclass `niobot.Module` in the module, and calls their `__setup__`, adding all commands
 registered under that class
 
 Take the following file as ping.py:
 ```python
 import niobot
 
 
-class MyPingModule(niolib.Module):
-    # This class is a subclass of niolib.Module, so it will be automatically discovered and loaded
+class MyPingModule(niobot.Module):
+    # This class is a subclass of niobot.Module, so it will be automatically discovered and loaded
     # It also has two attributes defined that you can use:
     # * self.bot: the instance of the bot
     # * self.log: An instance of logging.Logger, which you can use to log messages to the console or log file.
     #   It is recommended to use this instead of print().
-    
+
     # Now we will define a command
     @niobot.command()
-    async def ping(self, ctx: niolib.Context):
+    async def ping(self, ctx: niobot.Context):
         """Shows the latency"""
-        roundtrip = (time.time() * 1000 - ctx.event.server_timestamp)
+        roundtrip = ctx.bot.latency(ctx.message)
         await ctx.reply("Pong! Took {:,.2f}ms".format(roundtrip))
 ```
 
-Notice how here, we use `@niolib.command`, instead of `@bot.command`? They work the same, however
-`niolib.command` is designed to be loaded in a module context, where you usually don't have the bot instance at runtime
+Notice how here, we use `@niobot.command`, instead of `@bot.command`? They work the same, however
+`niobot.command` is designed to be loaded in a module context, where you usually don't have the bot instance at runtime
 (since that is injected by `NioBot.mount_module`). If you do have the bot instance, you can use `@bot.command` instead,
 which will register your command instantly.
 
 Once `mount_module` is called, it will scan through `ping.py`. It will find `MyPingModule`, realise it is a subclass
-of `Module`, and will automatically add any commands defined by `@niolib.command`.
+of `Module`, and will automatically add any commands defined by `@niobot.command`.
 
 After all of this, `[prefix]ping` is now available!
 
 ---
 
 You can customise the behaviour of the loading process at two-levels:
 
 1. By overriding `Module.__setup__`, you can customise how the module is loaded. By default, it will scan through the
-class' functions and detect any that're annotated with `@niolib.command`, and register them. You can override this
+class' functions and detect any that're annotated with `@niobot.command`, and register them. You can override this
 to do whatever you want.
 2. Providing a `setup(niobot)` function in your module. This will be called when the module is loaded, and you can
 do whatever you want in here. This is useful if you want to do something that isn't related to commands, such as
 registering event handlers. Note that defining `setup` must be outside any classes, and it will disable the
 auto-discovery of commands.
```

### Comparing `nio-bot-1.0.2/README.md` & `nio-bot-1.1.0a1/src/nio_bot.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,55 @@
+Metadata-Version: 2.1
+Name: nio-bot
+Version: 1.1.0a1
+Summary: Making matrix bots simple
+Author-email: Nexus <pip@nexy7574.co.uk>
+License: GNU GPLv3
+Project-URL: Source, https://github.com/eekim10/niobot
+Project-URL: Tracker, https://github.com/eekim10/niobot/issues
+Project-URL: Documentation, https://eekim10.github.io/niobot/
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: e2ee
+Provides-Extra: cli
+Provides-Extra: dev
+License-File: LICENSE
+
 # NioBot
-A simple, easy to use python Matrix bot library, based on the excellent 
+A simple, easy to use python Matrix bot library, based on the excellent
 [matrix-nio](https://pypi.org/project/matrix-nio/) library.
 
 NioBot is designed to have a similar (as similar as reasonably possible) design and feel to the
 [discord.py](https://pypi.org/project/discord.py) library, which should hopefully give it a familiar feel if you're
 coming from a discord background.
 
 Please note that there *will* be teething problems, and as such some advanced features may not be
 available, as with any client.
 
 ## Need help?
-Take a look at the [docs!](https://eekim10.github.io/niobot)
+Take a look at the [docs!](https://eekim10.github.io/niobot), or
+[![Chat on Matrix](https://matrix.to/img/matrix-badge.svg)](https://matrix.to/#/#niobot:nexy7574.co.uk)
+(dedicated support room)
 
 ---
 
 Alternatively, take a look at my [dev bot](https://github.com/EEKIM10/niobot-test), which is a bot that I use to test
 features of nio-bot before they're released.
 This bot is very advanced as, since I developed the library, I know exactly how it works, and will have bleeding-edge
 features built into it, which a lot of users may not use yet.
 
 It is, however, a great example of how an advanced, full feature bot can be created using this library.
 
 You can see it live [here](https://matrix.to/#/@jimmy-bot:nexy7574.co.uk)
-(DM it, the prefix is ?, and full end-to-end encryption is supported. Average response time is ~300-500ms)
+(DM it, the prefix is ?, and full end-to-end encryption is supported(*). Average response time is ~300-500ms)
 
-## Installation
-### Versions
-NioBot uses SemVer (semantic versioning) for versioning. This means that the version number is split into three parts:
-`Major`, `Minor` and `Patch`. As per the versioning, `Major` versions are not guaranteed to be backwards compatible,
-however `Minor` and `Patch` versions are.
-
-This means that there will always be a new `Major` increment when a backwards incompatible change is made, and a new
-`Minor` increment when a backwards compatible change is made. `Patch` versions are almost always bug fixes, and are
-always backwards compatible. If a bug fix is not backwards compatible, a new `Major` version will be released.
-
-Major changes may be pushed into their own branches for "feature previews". These branches will be prefixed with
-`feature/`, and will be merged into `master` when they are ready for release. For example, `feature/my-thing`,
-which means you can install it using `niobot @ git+https://github.com/EEKIM10/niobot.git@feature/my-thing`.
-This minimises the number of breaking releases.
+(\* May not always work due to key store issues, but it should work most of the time, especially if its your first
+time using it.)
 
+## Installation
 ### Release versions
 You can use the [PyPi](https://pypi.org/project/niobot) releases:
 ```python
 niobot==1.0.0  # or whatever version
 # Or to install it with extras
 niobot[e2ee,cli]==1.0.0
 ```
@@ -54,21 +61,17 @@
 # Or with e2ee support (note you will need libolm)
 matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git
 ```
 You can figure out how to install it in other ways.
 
 ## Features
 NioBot aims to be as easy to use as possible, so form is preferred over function.
-Some features you'd normally expect may not be implemented (yet, feel free to open a pull request!) or may not work as 
+Some features you'd normally expect may not be implemented (yet, feel free to open a pull request!) or may not work as
 intended or how you'd expect, however as with any matrix client.
 
-However, like any good client, NioBot tries to adhere to the 
-[Matrix Spec](https://spec.matrix.org/v1.7/client-server-api) (in terms of design at least, all the hard work is 
-done by matrix-nio)
-
 ## Quickstart
 ```python
 import time
 from niobot import Bot, Context
 
 bot = Bot(
     homeserver="https://matrix.org",  # your homeserver
@@ -123,51 +126,51 @@
 
 bot.run(password="password")
 ```
 
 When you call `mount_module`, it effectively calls `import module` under the hood, and then does one of the following:
 
 1. Calls the `module.setup(bot)` function, if it exists
-2. Discovers all classes that subclass `niolib.Module` in the module, and calls their `__setup__`, adding all commands
+2. Discovers all classes that subclass `niobot.Module` in the module, and calls their `__setup__`, adding all commands
 registered under that class
 
 Take the following file as ping.py:
 ```python
 import niobot
 
 
-class MyPingModule(niolib.Module):
-    # This class is a subclass of niolib.Module, so it will be automatically discovered and loaded
+class MyPingModule(niobot.Module):
+    # This class is a subclass of niobot.Module, so it will be automatically discovered and loaded
     # It also has two attributes defined that you can use:
     # * self.bot: the instance of the bot
     # * self.log: An instance of logging.Logger, which you can use to log messages to the console or log file.
     #   It is recommended to use this instead of print().
-    
+
     # Now we will define a command
     @niobot.command()
-    async def ping(self, ctx: niolib.Context):
+    async def ping(self, ctx: niobot.Context):
         """Shows the latency"""
-        roundtrip = (time.time() * 1000 - ctx.event.server_timestamp)
+        roundtrip = ctx.bot.latency(ctx.message)
         await ctx.reply("Pong! Took {:,.2f}ms".format(roundtrip))
 ```
 
-Notice how here, we use `@niolib.command`, instead of `@bot.command`? They work the same, however
-`niolib.command` is designed to be loaded in a module context, where you usually don't have the bot instance at runtime
+Notice how here, we use `@niobot.command`, instead of `@bot.command`? They work the same, however
+`niobot.command` is designed to be loaded in a module context, where you usually don't have the bot instance at runtime
 (since that is injected by `NioBot.mount_module`). If you do have the bot instance, you can use `@bot.command` instead,
 which will register your command instantly.
 
 Once `mount_module` is called, it will scan through `ping.py`. It will find `MyPingModule`, realise it is a subclass
-of `Module`, and will automatically add any commands defined by `@niolib.command`.
+of `Module`, and will automatically add any commands defined by `@niobot.command`.
 
 After all of this, `[prefix]ping` is now available!
 
 ---
 
 You can customise the behaviour of the loading process at two-levels:
 
 1. By overriding `Module.__setup__`, you can customise how the module is loaded. By default, it will scan through the
-class' functions and detect any that're annotated with `@niolib.command`, and register them. You can override this
+class' functions and detect any that're annotated with `@niobot.command`, and register them. You can override this
 to do whatever you want.
 2. Providing a `setup(niobot)` function in your module. This will be called when the module is loaded, and you can
 do whatever you want in here. This is useful if you want to do something that isn't related to commands, such as
 registering event handlers. Note that defining `setup` must be outside any classes, and it will disable the
 auto-discovery of commands.
```

### Comparing `nio-bot-1.0.2/docs/assets/guides/images/sending-attachments/blurhash-dehashed.avif` & `nio-bot-1.1.0a1/docs/assets/guides/images/sending-attachments/blurhash-dehashed.avif`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/docs/assets/guides/images/sending-attachments/blurhash-hashed.avif` & `nio-bot-1.1.0a1/docs/assets/guides/images/sending-attachments/blurhash-hashed.avif`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/docs/assets/guides/images/sending-attachments/file-send.avif` & `nio-bot-1.1.0a1/docs/assets/guides/images/sending-attachments/file-send.avif`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/docs/assets/guides/text/example_ffprobe.json` & `nio-bot-1.1.0a1/docs/assets/guides/text/example_ffprobe.json`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/docs/guides/getting-started.md` & `nio-bot-1.1.0a1/docs/guides/getting-started.md`

 * *Files 4% similar despite different names*

```diff
@@ -219,16 +219,16 @@
 the same session, and to avoid having to use your password in your code.
 
 You can get your password with `niocli get-access-token`.
 For example:
 ```bash
 (venv) [me@host test-niobot]$ niocli get-access-token
 User ID (@username:homeserver.tld): @test:matrix.org
-Password (will not echo): 
-Device ID (a memorable display name for this login, such as 'bot-production') [host]: 
+Password (will not echo):
+Device ID (a memorable display name for this login, such as 'bot-production') [host]:
 Resolving homeserver... OK
 Getting access token... OK
 Access token: syt_<...>
 ```
 
 What you're going to do now, is copy the full access token string, and open `config.py` again
 Now, replace `PASSWORD=...` with `ACCESS_TOKEN="syt_<...>"`. Make sure to keep the quotes!
@@ -253,15 +253,15 @@
 
 !!! warning "Its taking FOREVER to log in! is something going wrong?"
     Nope. It can often take a while (upwards of five minutes in some cases!) for the bot to log in.
     This is because, when you first start the bot, it has to *sync* your entire state with the server.
     This often results in a LOT of IO, and a lot of network waiting, etc.
 
     You can speed up this process in the future by:
-    
+
     * Making sure you have `store_path` and a valid store in your configuration. Stores mean that the bot doesn't have
       to re-sync everything every time it starts up.
     * Using an access token instead of a password. This means that the bot doesn't have to log in, and can just start
       syncing immediately, even from the last time it was stopped, which saves a very very large portion of the time
       taken
 
 #### Interesting log output
@@ -301,46 +301,74 @@
 
     ```python
     import niobot
     import logging
     import config
 
     logging.basicConfig(level=logging.INFO, filename="bot.log")
-    
+
     bot = niobot.NioBot(
         homeserver=config.HOMESERVER,
         user_id=config.USER_ID,
         device_id='my-device-id',
         store_path='./store',
         command_prefix="!",
         owner_id="@my-matrix-username:matrix.org"
     )
     # We also want to load `fun.py`'s commands before starting:
     bot.mount_module("fun")
-    
+
     @bot.on_event("ready")
     async def on_ready(_):
         # That first argument is needed as the first result of the sync loop is passed to ready. Without it, this event
         # will fail to fire, and will cause a potentially catasrophic failure.
         print("Bot is ready!")
-    
-    
+
+
     @bot.command()
     async def ping(ctx):  # can be invoked with "!ping"
         await ctx.reply("Pong!")
-    
+
     bot.run(access_token=config.ACCESS_TOKEN)
     ```
 
 ??? abstract "fun.py"
     ```python
     import niobot
 
 
     class MyFunModule(niobot.Module):  # subclassing niobot.Module is mandatory for auto-detection.
         def __init__(self, bot):
             self.bot = bot  # bot is the NioBot instance you made in main.py!
-    
+
         @niobot.command()
         async def hello(self, ctx):
             await ctx.reply("Hello %s!" % ctx.event.sender)
     ```
+
+## Why is logging in with a password so bad?
+
+You may get a notice in your console when you try to log in with a password.
+
+This is because logging in with a password is actually an awful idea.
+It will create an entirely new session, 9 times out of 10 a hard-coded password, can cause issues with e2ee, and is
+generally just a bad idea.
+
+What you **should** do instead is get an access token.
+
+If you already know how to get yours, that's great! Otherwise, `niocli` has the solution:
+
+```bash
+$ niocli get-access-token
+```
+
+This will log into the account when prompted, and will grab you an access token, spitting it out into your terminal.
+
+From there, you can replace `bot.run(password="...")` with `bot.run(access_token="...")`, and you're good to go!
+
+!!! tip
+    You'll also notice that the bot starts up in a matter of seconds when using an access token.
+    This is because the client has already logged in before, so rather than having to sync the entire state and history,
+    it only downloads and syncs new events and data.
+
+    In comparison to using a password, which creates a new session, meaning the client has to download and sync the
+    entire history yet again.
```

### Comparing `nio-bot-1.0.2/docs/guides/sending-attachments.md` & `nio-bot-1.1.0a1/docs/guides/sending-attachments.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/docs/reference/context.md` & `nio-bot-1.1.0a1/docs/reference/context.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/docs/reference/utils/help_command.md` & `nio-bot-1.1.0a1/docs/reference/utils/help_command.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/docs/reference/utils/parsers.md` & `nio-bot-1.1.0a1/docs/reference/utils/parsers.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/docs/reference/utils/string_view.md` & `nio-bot-1.1.0a1/docs/reference/utils/string_view.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/docs/reference/utils/typing.md` & `nio-bot-1.1.0a1/docs/reference/utils/typing.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/docs/reference/utils/unblock.md` & `nio-bot-1.1.0a1/docs/reference/utils/unblock.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/examples/access_token.py` & `nio-bot-1.1.0a1/examples/access_token.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/examples/hello_world.py` & `nio-bot-1.1.0a1/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/examples/uploading.py` & `nio-bot-1.1.0a1/examples/uploading.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.2/pyproject.toml` & `nio-bot-1.1.0a1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -6,30 +6,50 @@
 [project]
 name = "nio-bot"
 description = "Making matrix bots simple"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.11"
 license = { text = "GNU GPLv3" }
 authors = [
-    {name = "Nexus", email = "packages@nexy7574.co.uk"}
+    {name = "Nexus", email = "pip@nexy7574.co.uk"}
 ]
 dynamic = ["version", "dependencies"]
 
 [project.urls]
 Source = "https://github.com/eekim10/niobot"
 Tracker = "https://github.com/eekim10/niobot/issues"
 Documentation = "https://eekim10.github.io/niobot/"
 
 
 [project.optional-dependencies]
 e2ee = ['matrix-nio[e2e]']
 cli = ['httpx', 'click']
-dev = ['mkdocs', 'mkdocs-material', 'black', 'mkdocs-autorefs', 'mkdocs-glightbox']
+dev = [
+    'mkdocs',
+    'mkdocs-material',
+    'black',
+    'mkdocs-autorefs',
+    'mkdocs-glightbox',
+    'mkdocstrings[python]',
+    'mkdocs-git-revision-date-localized-plugin',
+    'isort',
+    'build',
+    'pep440'
+]
 
 [project.scripts]
 niocli = "niobot.__main__:cli_root [cli]"
 
 [tool.setuptools_scm]
 write_to = "src/niobot/__version__.py"
 
 [tool.setuptools.dynamic]
-dependencies = {file = "requirements.txt"}
+dependencies = {file = "requirements.txt"}
+
+[tool.black]
+line-length = 120
+target-version = ["py311"]
+include = 'src/niobot(/utils)?/.+\.py'
+
+[tool.isort]
+profile = "black"
+src_paths = ["src/niobot"]
```

### Comparing `nio-bot-1.0.2/src/nio_bot.egg-info/SOURCES.txt` & `nio-bot-1.1.0a1/src/nio_bot.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 .gitignore
+.pre-commit-config.yaml
+CONTRIBUTING.md
 Dockerfile
 LICENSE
 README.md
+SECURITY.md
 mkdocs.yml
 pyproject.toml
 requirements.txt
+.github/FUNDING.yml
+.github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 .idea/.gitignore
 .idea/markdown.xml
 .idea/misc.xml
 .idea/modules.xml
 .idea/nio-bot.iml
 .idea/vcs.xml
 .idea/inspectionProfiles/Project_Default.xml
 .idea/inspectionProfiles/profiles_settings.xml
+dev/release.sh
 docs/index.md
 docs/assets/guides/images/sending-attachments/blurhash-dehashed.avif
 docs/assets/guides/images/sending-attachments/blurhash-hashed.avif
 docs/assets/guides/images/sending-attachments/file-send.avif
 docs/assets/guides/text/example_ffprobe.json
 docs/assets/guides/text/example_identify.json
+docs/guides/a-simple-bot.md
 docs/guides/getting-started.md
 docs/guides/sending-attachments.md
 docs/reference/attachment.md
 docs/reference/client.md
 docs/reference/commands.md
 docs/reference/context.md
+docs/reference/events.md
 docs/reference/exceptions.md
 docs/reference/utils/federation.md
 docs/reference/utils/help_command.md
 docs/reference/utils/parsers.md
 docs/reference/utils/string_view.md
 docs/reference/utils/typing.md
 docs/reference/utils/unblock.md
@@ -44,19 +52,21 @@
 src/nio_bot.egg-info/dependency_links.txt
 src/nio_bot.egg-info/entry_points.txt
 src/nio_bot.egg-info/requires.txt
 src/nio_bot.egg-info/top_level.txt
 src/niobot/__init__.py
 src/niobot/__main__.py
 src/niobot/__version__.py
+src/niobot/_event_stubs.py
 src/niobot/attachment.py
 src/niobot/client.py
 src/niobot/commands.py
 src/niobot/context.py
 src/niobot/exceptions.py
 src/niobot/utils/__init__.py
+src/niobot/utils/checks.py
 src/niobot/utils/federation.py
 src/niobot/utils/help_command.py
 src/niobot/utils/parsers.py
 src/niobot/utils/string_view.py
 src/niobot/utils/typing.py
 src/niobot/utils/unblocking.py
```

### Comparing `nio-bot-1.0.2/src/niobot/__init__.py` & `nio-bot-1.1.0a1/src/niobot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from nio import *
+
 from . import utils
-from .utils import *
+from .attachment import *
 from .client import *
 from .commands import *
 from .context import *
 from .exceptions import *
-from .attachment import *
+from .utils import *
 
 try:
     import __version__ as version_meta
 except ImportError:
+
     class __VersionMeta:
         __version__ = "0.0.dev0+gFFFFFF"
         __version_tuple__ = (0, 0, "dev0", "gFFFFFF")
+
     version_meta = __VersionMeta()
 
 __author__ = "Nexus <pip@nexy7574.co.uk>"
 __license__ = "GNU GPLv3"
 __url__ = "https://github.com/EEKIM10/niobot"
 __title__ = "niobot"
 __description__ = "A Matrix bot framework written in Python built on matrix-nio."
```

### Comparing `nio-bot-1.0.2/src/niobot/__main__.py` & `nio-bot-1.1.0a1/src/niobot/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
 import datetime
+import importlib.metadata
+import logging
 import os
 import pathlib
 import re
 import sys
-import logging
 
 import niobot
-import importlib.metadata
 
 try:
     import click
     import httpx
 except ImportError:
     print("Missing CLI dependencies. Did you install CLI extras?", file=sys.stderr)
     sys.exit(1)
@@ -58,17 +58,15 @@
 
 bot.run(password="{password}")
 """
 
 
 @click.group()
 @click.option(
-    "--log-level", "-L",
-    type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]),
-    default="WARNING"
+    "--log-level", "-L", type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]), default="WARNING"
 )
 @click.pass_context
 def cli_root(ctx, log_level: str):
     """CLI utilities for nio-bot."""
     logging.basicConfig(
         level=getattr(logging, log_level),
     )
@@ -78,99 +76,86 @@
     except ImportError:
         logger.warning("Failed to import version metadata.")
         __version__ = "unknown"
         __version_tuple__ = (0, 0, "unknown", "gunknown.d19991231")
     else:
         logger.debug("Version: %s", __version__)
 
-    ctx.obj = {
-        "timestamp": datetime.datetime.now(),
-        "version_info": __version__,
-        "version_tuple": __version_tuple__
-    }
+    ctx.obj = {"timestamp": datetime.datetime.now(), "version_info": __version__, "version_tuple": __version_tuple__}
 
 
 @cli_root.command()
 @click.option("--no-colour", "--no-color", "-C", is_flag=True, default=False)
-@click.option("--homeserver", "-H", default=None, help="An optional homeserver to display information about.")
 @click.pass_context
 def version(ctx, no_colour: bool):
     """Shows version information."""
     logger.info("Gathering version info...")
     import platform
+
     from nio.crypto import ENCRYPTION_ENABLED
 
     logger.debug("Attempting to resolve matrix-nio via importlib...")
     nio_version = None
     try:
         nio_version = importlib.metadata.version("matrix-nio")
     except importlib.metadata.PackageNotFoundError:
         logger.critical("Failed to resolve nio version information via importlib.")
 
     if not nio_version:
         logger.debug("Attempting to resolve matrix-nio version information via pip...")
-        command = [
-            "pip",
-            "show",
-            "matrix-nio"
-        ]
+        command = ["pip", "show", "matrix-nio"]
         result = subprocess.run(command, capture_output=True, text=True)
         if result.returncode != 0:
             logger.critical("Failed to resolve nio version information via pip.")
             nio_version = "0.0.0"
         else:
             logger.debug("Successfully resolved nio version information via pip.")
             nio_version = result.stdout.splitlines()[1].split(": ")[1]
 
     t = ctx.obj["version_tuple"]
     if len(t) > 3:
-        t3 = t[3] or 'gN/A.d%s' % (datetime.datetime.now().strftime("%Y%m%d"))
+        t3 = t[3] or "gN/A.d%s" % (datetime.datetime.now().strftime("%Y%m%d"))
         try:
             t3_commit, t3_date_raw = t3.split(".", 1)
         except ValueError:
             t3_commit = t3
             t3_date = datetime.datetime.now()
             t3_date_raw = t3_date.strftime("%Y%m%d")
         t3_date = datetime.datetime.strptime(t3_date_raw[1:], "%Y%m%d")
     else:
         t3_commit = "<release>"
         mtime = pathlib.Path(__file__).stat().st_mtime
         t3_date = datetime.datetime.fromtimestamp(mtime)
 
-    bot_version_deep = {
-        "version": "%d.%d" % (t[0], t[1]),
-        "build": t[2],
-        "commit": t3_commit,
-        "date": t3_date
-    }
+    bot_version_deep = {"version": "%d.%d" % (t[0], t[1]), "build": t[2], "commit": t3_commit, "date": t3_date}
 
     bot_version = "%s (Version %s, build %s, commit %r, built %r)" % (
         ctx.obj["version_info"],
         bot_version_deep["version"],
         bot_version_deep["build"],
         bot_version_deep["commit"][1:],
-        bot_version_deep["date"].strftime("%d/%m/%Y")
+        bot_version_deep["date"].strftime("%d/%m/%Y"),
     )
 
     _os = platform.platform()
     if hasattr(platform, "freedesktop_os_release"):
         try:
             _os_info = platform.freedesktop_os_release()
         except OSError:
             pass
         else:
             _os += " ({0}/{1} - {2})".format(
                 _os_info.get("NAME", "Unknown"),
                 _os_info.get("VERSION", "Unknown"),
-                _os_info.get("PRETTY_NAME", "Unknown")
+                _os_info.get("PRETTY_NAME", "Unknown"),
             )
 
     lines = [
         ["NioBot version", bot_version, lambda x: True],
-        ["matrix-nio version", nio_version, lambda x: x.startswith("0.20")],
+        ["matrix-nio version", nio_version, lambda x: x.startswith(("0.20", "0.21"))],
         ["Python version", platform.python_version(), lambda x: x.split(".")[0] == "3" and int(x.split(".")[1]) >= 9],
         ["Python implementation", platform.python_implementation(), lambda x: x == "CPython"],
         ["Operating System", _os, lambda val: val.startswith(("Windows", "Linux"))],
         ["Architecture", platform.machine(), lambda x: x == "x86_64"],
         ["OLM Installed", "Yes" if ENCRYPTION_ENABLED else "No", lambda x: x != "No"],
     ]
 
@@ -180,27 +165,27 @@
 
     click.echo()
     for line in lines:
         if no_colour:
             click.echo("%s: %s" % tuple(line)[:2])
         else:
             click.echo(
-                click.style(line[0], fg="cyan") + ": " +
-                click.style(line[1], fg="green" if line[2](line[1]) else "red")
+                click.style(line[0], fg="cyan") + ": " + click.style(line[1], fg="green" if line[2](line[1]) else "red")
             )
     click.echo()
 
 
 @cli_root.command(name="test-homeserver")
 @click.argument("homeserver")
 def test_homeserver(homeserver: str):
     """Walks through resolving and testing a given homeserver."""
-    import httpx
     import urllib.parse
 
+    import httpx
+
     if homeserver.startswith("@"):
         _, homeserver = homeserver.split(":", 1)
 
     logger.debug("Parsing given input %r as a URL...", homeserver)
     parsed = urllib.parse.urlparse(homeserver)
     if not parsed.scheme:
         logger.info("No scheme found, assuming HTTPS.")
@@ -211,18 +196,15 @@
         logger.critical("URI parsed to: %r", parsed)
         return
 
     logger.debug("Attempting to resolve %r...", parsed.netloc)
     logger.info("Trying well-known of %r...", parsed.netloc)
     base_url = None
     try:
-        response = httpx.get(
-            "https://%s/.well-known/matrix/client" % parsed.netloc,
-            timeout=30
-        )
+        response = httpx.get("https://%s/.well-known/matrix/client" % parsed.netloc, timeout=30)
     except httpx.HTTPError as e:
         logger.critical("Failed to get well-known: %r", e)
         return
     else:
         logger.debug("Got response: %r", response)
         cors = response.headers.get("Access-Control-Allow-Origin", None)
         if not cors:
@@ -230,15 +212,15 @@
         elif cors != "*":
             logger.warning(
                 "CORS header found, but not set to wildcard. "
                 "This homeserver will be unusable in most web-based clients!"
             )
 
         if response.status_code != 404:
-            if response.status_code != 200 or len(response.content or b'') == 0:
+            if response.status_code != 200 or len(response.content or b"") == 0:
                 logger.critical("Well-known returned non-404, but no content. Failing.")
                 return
             else:
                 data = response.json()
                 logger.debug("Well-known data: %r", data)
                 if "m.homeserver" not in data:
                     logger.critical("Well-known data does not contain m.homeserver. Failing.")
@@ -253,18 +235,15 @@
         logger.info("No well-known found. Assuming %r as homeserver.", parsed.netloc)
         base_url = urllib.parse.urlparse("https://" + parsed.netloc)
 
     base_url = base_url.geturl()
     logger.info("Using %r as homeserver.", base_url)
     logger.info("Validating homeserver...")
     try:
-        response = httpx.get(
-            base_url + "/_matrix/client/versions",
-            timeout=30
-        )
+        response = httpx.get(base_url + "/_matrix/client/versions", timeout=30)
     except httpx.HTTPError as e:
         logger.critical("Failed to get versions: %r", e)
         return
     else:
         data = response.json()
         logger.debug("Got response: %r", data)
         if "versions" not in data:
@@ -279,17 +258,20 @@
 
 
 @cli_root.command(name="get-access-token")
 @click.option("--username", "-U", default=None, help="The username part (without @)")
 @click.option("--password", "-P", default=None, help="The password to use (will be prompted if not given)")
 @click.option("--homeserver", "-H", default=None, help="The homeserver to use (will be prompted if not given)")
 @click.option(
-    "--device-id", "-D", "--session", "--session-id",
+    "--device-id",
+    "-D",
+    "--session",
+    "--session-id",
     default=None,
-    help="The device ID to use (will be prompted if not given)"
+    help="The device ID to use (will be prompted if not given)",
 )
 @click.pass_context
 def get_access_token(ctx, username: str, password: str, homeserver: str, device_id: str):
     """Fetches your access token from your homeserver."""
     if not username:
         username = ""
 
@@ -304,16 +286,15 @@
         password = click.prompt("Password (will not echo)", hide_input=True)
 
     if not homeserver:
         homeserver = click.prompt("Homeserver URL")
 
     if not device_id:
         device_id = click.prompt(
-            "Device ID (a memorable display name for this login, such as 'bot-production')",
-            default=os.uname().nodename
+            "Device ID (a memorable display name for this login, such as 'bot-production')", default=os.uname().nodename
         )
 
     click.secho("Resolving homeserver... ", fg="cyan", nl=False)
     try:
         homeserver = asyncio.run(niobot.resolve_homeserver(homeserver))
     except ConnectionError:
         click.secho("Failed!", fg="red")
@@ -323,22 +304,19 @@
     click.secho("Getting access token... ", fg="cyan", nl=False)
     status_code = None
     try:
         response = httpx.post(
             homeserver + "/_matrix/client/r0/login",
             json={
                 "type": "m.login.password",
-                "identifier": {
-                    "type": "m.id.user",
-                    "user": username
-                },
+                "identifier": {"type": "m.id.user", "user": username},
                 "password": password,
                 "device_id": device_id,
-                "initial_device_display_name": device_id
-            }
+                "initial_device_display_name": device_id,
+            },
         )
         status_code = response.status_code
         if status_code == 429:
             click.secho("Failed!", fg="red", nl=False)
             click.secho(" (Rate limited for {:.0f} seconds)".format(response.json()["retry_after_ms"] / 1000), bg="red")
             return
         response.raise_for_status()
@@ -362,35 +340,37 @@
 @click.option("--homeserver", "-H", prompt=True)
 @click.option("--device-id", "-D", prompt=True)
 @click.option("--store-path", "-S", prompt=True)
 @click.option("--prefix", "-P", prompt=True)
 @click.option("--owner-id", "-O", prompt=True)
 @click.pass_context
 def bot(
-        ctx,
-        path: str,
-        password: str,
-        homeserver: str,
-        user_id: str,
-        device_id: str,
-        store_path: str,
-        prefix: str,
-        owner_id: str
+    ctx,
+    path: str,
+    password: str,
+    homeserver: str,
+    user_id: str,
+    device_id: str,
+    store_path: str,
+    prefix: str,
+    owner_id: str,
 ):
     """Creates a new bot with two basic commands from the template. Easy quickstart."""
     with open(path, "w") as f:
-        f.write(DEFAULT_BOT_TEMPLATE.format(
-            password=password,
-            homeserver=homeserver,
-            user_id=user_id,
-            device_id=device_id,
-            store_path=store_path,
-            prefix=prefix,
-            owner_id=owner_id,
-            timestamp=datetime.datetime.utcnow().isoformat(),
-            version_info=ctx.obj["version_info"]
-        ))
+        f.write(
+            DEFAULT_BOT_TEMPLATE.format(
+                password=password,
+                homeserver=homeserver,
+                user_id=user_id,
+                device_id=device_id,
+                store_path=store_path,
+                prefix=prefix,
+                owner_id=owner_id,
+                timestamp=datetime.datetime.utcnow().isoformat(),
+                version_info=ctx.obj["version_info"],
+            )
+        )
     click.echo("Created bot file at %r" % path)
 
 
 if __name__ == "__main__":
     cli_root()
```

### Comparing `nio-bot-1.0.2/src/niobot/attachment.py` & `nio-bot-1.1.0a1/src/niobot/attachment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 """
 Matrix file attachments. Full e2ee support is implemented.
 """
 import abc
-import tempfile
-import warnings
-
-import nio
-import subprocess
-import json
+import enum
 import io
+import json
+import logging
 import os
 import pathlib
+import re
 import shutil
-import magic
+import subprocess
+import tempfile
+import time
 import typing
-import enum
+import urllib.parse
+import warnings
+
 import aiofiles
-import logging
+import aiohttp
 import blurhash
+import magic
+import nio
 
+from .exceptions import (
+    MediaCodecWarning,
+    MediaDownloadException,
+    MediaUploadException,
+    MetadataDetectionException,
+)
 from .utils import run_blocking
-from .exceptions import MediaUploadException, MetadataDetectionException, MediaCodecWarning
 
 if typing.TYPE_CHECKING:
     from .client import NioBot
 
 
 log = logging.getLogger(__name__)
 
@@ -38,14 +47,15 @@
     "first_frame",
     "BaseAttachment",
     "FileAttachment",
     "ImageAttachment",
     "VideoAttachment",
     "AudioAttachment",
     "AttachmentType",
+    "which",
     "SUPPORTED_CODECS",
     "SUPPORTED_VIDEO_CODECS",
     "SUPPORTED_AUDIO_CODECS",
     "SUPPORTED_IMAGE_CODECS",
 )
 
 SUPPORTED_VIDEO_CODECS = [
@@ -62,23 +72,17 @@
     "aac",
     "mp3",
     "vorbis",
     "flac",
     "mp2",
 ]
 # All of the above codecs were played in Element Desktop. A bunch were cut out, as the list was far too long.
-# Realistically, I don't see the warning being useful to too many people, its literally only in to help people figure
+# Realistically, I don't see the warning being useful to too many people, it's literally only in to help people figure
 # out why their media isn't playing.
-SUPPORTED_IMAGE_CODECS = [
-    "mjpeg",
-    "gif",
-    "png",
-    "av1",
-    "webp"
-]
+SUPPORTED_IMAGE_CODECS = ["mjpeg", "gif", "png", "av1", "webp"]
 # Probably not all of them but close enough
 SUPPORTED_CODECS = SUPPORTED_VIDEO_CODECS + SUPPORTED_AUDIO_CODECS + SUPPORTED_IMAGE_CODECS
 
 
 def detect_mime_type(file: typing.Union[str, io.BytesIO, pathlib.Path]) -> str:
     """
     Detect the mime type of a file.
@@ -88,19 +92,24 @@
     """
     if isinstance(file, str):
         file = pathlib.Path(file)
 
     if isinstance(file, io.BytesIO):
         current_position = file.tell()
         file.seek(0)
+        start = time.perf_counter()
         mt = magic.from_buffer(file.read(), mime=True)
+        log.debug("Took %f seconds to detect mime type", time.perf_counter() - start)
         file.seek(current_position)  # Reset the file position
         return mt
     elif isinstance(file, pathlib.Path):
-        return magic.from_file(str(file), mime=True)
+        start = time.perf_counter()
+        mt = magic.from_file(str(file), mime=True)
+        log.debug("Took %f seconds to detect mime type", time.perf_counter() - start)
+        return mt
     else:
         raise TypeError("File must be a string, BytesIO, or Path object.")
 
 
 def get_metadata_ffmpeg(file: typing.Union[str, pathlib.Path]) -> typing.Dict[str, typing.Any]:
     """
     Gets metadata for a file via ffprobe.
@@ -108,31 +117,23 @@
     [example output (JSON)](https://github.com/EEKIM10/niobot/raw/master/docs/assets/guides/text/example_ffprobe.json)
 
     :param file: The file to get metadata for. **Must be a path-like object**
     :return: A dictionary containing the metadata.
     """
     if not shutil.which("ffprobe"):
         raise FileNotFoundError("ffprobe is not installed. If it is, check your $PATH.")
-    command = [
-        "ffprobe",
-        "-of",
-        "json",
-        "-loglevel",
-        "9",
-        "-show_format",
-        "-show_streams",
-        "-i",
-        str(file)
-    ]
+    command = ["ffprobe", "-of", "json", "-loglevel", "9", "-show_format", "-show_streams", "-i", str(file)]
+    start = time.perf_counter()
     try:
         result = subprocess.run(command, capture_output=True, encoding="utf-8", errors="replace", check=True)
     except subprocess.SubprocessError as e:
         raise MetadataDetectionException("Failed to get metadata for file.", exception=e)
+    log.debug("Took %f seconds to run ffprobe", time.perf_counter() - start)
     log.debug("ffprobe output (%d): %s", result.returncode, result.stdout)
-    data = json.loads(result.stdout or '{}')
+    data = json.loads(result.stdout or "{}")
     log.debug("parsed ffprobe output:\n%s", json.dumps(data, indent=4))
     return data
 
 
 def get_metadata_imagemagick(file: pathlib.Path) -> typing.Dict[str, typing.Any]:
     """The same as `get_metadata_ffmpeg` but for ImageMagick.
 
@@ -141,25 +142,24 @@
 
     [example output (JSON)](https://github.com/EEKIM10/niobot/raw/master/docs/assets/guides/text/example_identify.json)
 
     :param file: The file to get metadata for. **Must be a path object**
     :return: A slimmed-down dictionary containing the metadata.
     """
     file = file.resolve(True)
-    command = [
-        "identify",
-        str(file)
-    ]
+    command = ["identify", str(file)]
+    start = time.perf_counter()
     try:
         result = subprocess.run(command, capture_output=True, encoding="utf-8", errors="replace", check=True)
     except subprocess.SubprocessError as e:
         raise MetadataDetectionException("Failed to get metadata for file.", exception=e)
     log.debug("identify output (%d): %s", result.returncode, result.stdout)
+    log.debug("identify took %f seconds", time.perf_counter() - start)
     stdout = result.stdout
-    stdout = stdout[len(str(file)) + 1:]
+    stdout = stdout[len(str(file)) + 1 :]
     img_format, img_size, *_ = stdout.split()
     data = {
         "streams": [
             {
                 "index": 0,
                 "codec_name": img_format,
                 "codec_long_name": img_format,
@@ -168,15 +168,15 @@
                 "width": int(img_size.split("x")[0]),
             }
         ],
         "format": {
             "filename": str(file),
             "format_long_name": img_format,
             "size": str(file.stat().st_size),
-        }
+        },
     }
     log.debug("Parsed identify output:\n%s", json.dumps(data, indent=4))
     return data
 
 
 def get_metadata(file: typing.Union[str, pathlib.Path], mime_type: str = None) -> typing.Dict[str, typing.Any]:
     """
@@ -196,19 +196,25 @@
     if mime == "image":
         if not shutil.which("identify"):
             log.warning(
                 "Imagemagick identify not found, falling back to ffmpeg for image metadata detection. "
                 "Check your $PATH."
             )
         else:
-            return get_metadata_imagemagick(file)
+            start = time.perf_counter()
+            r = get_metadata_imagemagick(file)
+            log.debug("get_metadata_imagemagick took %f seconds", time.perf_counter() - start)
+            return r
 
     if mime not in ["audio", "video", "image"]:
         raise MetadataDetectionException("Unsupported mime type. Must be an audio clip, video, or image.")
-    return get_metadata_ffmpeg(file)
+    start = time.perf_counter()
+    r = get_metadata_ffmpeg(file)
+    log.debug("get_metadata_ffmpeg took %f seconds", time.perf_counter() - start)
+    return r
 
 
 def first_frame(file: str | pathlib.Path, file_format: str = "webp") -> bytes:
     """
     Gets the first frame of a video file.
 
     !!! Danger "This function creates a file on disk"
@@ -222,33 +228,20 @@
     :param file: The file to get the first frame of. **Must be a path-like object**
     :param file_format: The format to save the frame as. Defaults to webp.
     :return: The first frame of the video in bytes.
     """
     if not shutil.which("ffmpeg"):
         raise FileNotFoundError("ffmpeg is not installed. If it is, check your $PATH.")
     with tempfile.NamedTemporaryFile(suffix=f".{file_format}") as f:
-        command = [
-            "ffmpeg",
-            "-loglevel",
-            "9",
-            "-i",
-            str(file),
-            "-frames:v",
-            "1",
-            '-y',
-            '-strict',
-            '-2',
-            f.name
-        ]
-        log.debug("Extracting first frame of %r: %s", file, ' '.join(command))
+        command = ["ffmpeg", "-loglevel", "9", "-i", str(file), "-frames:v", "1", "-y", "-strict", "-2", f.name]
+        log.debug("Extracting first frame of %r: %s", file, " ".join(command))
         try:
-            log.debug(
-                "Extraction return code: %d",
-                subprocess.run(command, capture_output=True, check=True).returncode
-            )
+            start = time.perf_counter()
+            log.debug("Extraction return code: %d", subprocess.run(command, capture_output=True, check=True).returncode)
+            log.debug("Extraction took %f seconds", time.perf_counter() - start)
         except subprocess.SubprocessError as e:
             raise MediaUploadException("Failed to extract first frame of video.", exception=e)
         f.seek(0)
         return f.read()
 
 
 def generate_blur_hash(file: str | pathlib.Path | io.BytesIO, *parts: int) -> str:
@@ -265,18 +258,24 @@
     """
     if not parts:
         parts = 4, 3
     file = _to_path(file)
     if not isinstance(file, io.BytesIO):
         with file.open("rb") as fd:
             log.info("Generating blurhash for %s", file)
-            return blurhash.encode(fd, *parts)
+            start = time.perf_counter()
+            x = blurhash.encode(fd, *parts)
+            log.debug("Generating blurhash took %f seconds", time.perf_counter() - start)
+            return x
     else:
         log.info("Generating blurhash for BytesIO object")
-        return blurhash.encode(file, *parts)
+        start = time.perf_counter()
+        x = blurhash.encode(file, *parts)
+        log.debug("Generating blurhash took %f seconds", time.perf_counter() - start)
+        return x
 
 
 def _file_okay(file: pathlib.Path | io.BytesIO) -> typing.Literal[True]:
     """Checks if a file exists, is a file, and can be read."""
     if isinstance(file, io.BytesIO):
         if file.closed:
             raise ValueError("BytesIO object is closed.")
@@ -313,23 +312,69 @@
 def _size(file: pathlib.Path | io.BytesIO) -> int:
     """Gets the size of a file."""
     if isinstance(file, io.BytesIO):
         return len(file.getbuffer())
     return file.stat().st_size
 
 
+def which(
+    file: io.BytesIO | pathlib.Path | str, mime_type: str = None
+) -> typing.Union[
+    typing.Type["FileAttachment"],
+    typing.Type["ImageAttachment"],
+    typing.Type["AudioAttachment"],
+    typing.Type["VideoAttachment"],
+]:
+    """
+    Gets the correct attachment type for a file.
+
+    This function will provide either Image/Video/Audio attachment where possible, or FileAttachment otherwise.
+
+    For example, `image/png` (from `my_image.png`) will see `image/` and will return [`ImageAttachment`][niobot.ImageAttachment],
+    and `video/mp4` (from `my_video.mp4`) will see `video/` and will return [`VideoAttachment`][niobot.VideoAttachment].
+
+    If the mime type cannot be mapped to an attachment type, this function will return [`FileAttachment`][niobot.FileAttachment].
+
+    ??? example "Usage"
+        ```python
+        import niobot
+        import pathlib
+
+        my_file = pathlib.Path("/tmp/foo.bar")
+        attachment = await niobot.which(my_file).from_file(my_file)
+        # or
+        attachment_type = niobot.which(my_file)  # one of the BaseAttachment subclasses
+        attachment = await attachment_type.from_file(my_file)
+        ```
+
+    :param file: The file or BytesIO to investigate
+    :param mime_type: The optional pre-detected mime type. If this is not provided, it will be detected.
+    :return: The correct type for this attachment (not instantiated)
+    """
+    values = {
+        "image": ImageAttachment,
+        "audio": AudioAttachment,
+        "video": VideoAttachment,
+    }
+    if not mime_type:
+        mime_type = detect_mime_type(file)
+    mime_start = mime_type.split("/")[0].lower()
+    return values.get(mime_start, FileAttachment)
+
+
 class AttachmentType(enum.Enum):
     """
     Enumeration containing the different types of media.
 
     :var FILE: A generic file.
     :var AUDIO: An audio file.
     :var VIDEO: A video file.
     :var IMAGE: An image file.
     """
+
     if typing.TYPE_CHECKING:
         FILE: "AttachmentType"
         AUDIO: "AttachmentType"
         VIDEO: "AttachmentType"
         IMAGE: "AttachmentType"
     FILE = "m.file"
     AUDIO = "m.audio"
@@ -357,47 +402,50 @@
     :ivar file_name: The name of the file. If `file` was a string or `Path`, this will be the name of the file.
     :ivar mime_type: The mime type of the file.
     :ivar size: The size of the file in bytes.
     :ivar type: The type of attachment.
     :ivar url: The URL of the uploaded file. This is set after the file is uploaded.
     :ivar keys: The encryption keys for the file. This is set after the file is uploaded.
     """
+
     if typing.TYPE_CHECKING:
         file: typing.Union[pathlib.Path, io.BytesIO]
         file_name: str
         mime_type: str
         size: int
         type: AttachmentType
 
         url: str | None
         keys: typing.Dict[str, str] | None
 
     def __init__(
-            self,
-            file: typing.Union[str, io.BytesIO, pathlib.Path],
-            file_name: str = None,
-            mime_type: str = None,
-            size_bytes: int = None,
-            *,
-            attachment_type: AttachmentType = AttachmentType.FILE
+        self,
+        file: typing.Union[str, io.BytesIO, pathlib.Path],
+        file_name: str = None,
+        mime_type: str = None,
+        size_bytes: int = None,
+        *,
+        attachment_type: AttachmentType = AttachmentType.FILE,
     ):
         self.file = _to_path(file)
         self.file_name = self.file.name if isinstance(self.file, pathlib.Path) else file_name
         if not self.file_name:
             raise ValueError("file_name must be specified when uploading a BytesIO object.")
         self.mime_type = mime_type or detect_mime_type(self.file)
         self.size = size_bytes or os.path.getsize(self.file)
 
         self.type = attachment_type
         self.url = None
         self.keys = None
 
     def __repr__(self):
-        return "<{0.__class__.__name__} file={0.file!r} file_name={0.file_name!r} " \
-               "mime_type={0.mime_type!r} size={0.size!r} type={0.type!r}>".format(self)
+        return (
+            "<{0.__class__.__name__} file={0.file!r} file_name={0.file_name!r} "
+            "mime_type={0.mime_type!r} size={0.size!r} type={0.type!r}>".format(self)
+        )
 
     def as_body(self, body: str = None) -> dict:
         """
         Generates the body for the attachment for sending. The attachment must've been uploaded first.
 
         :param body: The body to use (should be a textual description). Defaults to the file name.
         :return:
@@ -414,17 +462,17 @@
         }
         if self.keys:
             body["file"] = self.keys
         return body
 
     @classmethod
     async def from_file(
-            cls,
-            file: typing.Union[str, io.BytesIO, pathlib.Path],
-            file_name: str = None,
+        cls,
+        file: typing.Union[str, io.BytesIO, pathlib.Path],
+        file_name: str = None,
     ) -> "BaseAttachment":
         """
         Creates an attachment from a file.
 
         You should use this method instead of the constructor, as it will automatically detect all other values
 
         :param file: The file or BytesIO to attach
@@ -439,67 +487,161 @@
             if not file_name:
                 file_name = file.name
 
         mime_type = await run_blocking(detect_mime_type, file)
         size = _size(file)
         return cls(file, file_name, mime_type, size)
 
+    @classmethod
+    async def from_mxc(
+        cls, client: "NioBot", url: str, *, force_write: bool | pathlib.Path = False
+    ) -> "BaseAttachment":
+        """
+        Creates an attachment from an MXC URL.
+
+        :param client: The current client instance (used to download the attachment)
+        :param url: The MXC:// url to download
+        :param force_write: Whether to force writing downloaded attachments to a temporary file.
+        :return: The downloaded and probed attachment.
+        """
+        # !!! warning "This function loads the entire attachment into memory."
+        #     If you are downloading large attachments, you should set `force_write` to `True`, otherwise the downloaded
+        #     attachment is pushed into an [`io.BytesIO`][] object (for speed benefits), which can cause memory issues
+        #     on low-memory systems.
+        #
+        #     Bear in mind that most attachments are <= 100 megabytes. Also, forcing temp file writes may not be useful
+        #     unless your temporary file directory is backed by a physical disk, because otherwise you're just loading
+        #     into RAM with extra steps (for example, by default, `/tmp` is in-memory on linux, but `/var/tmp` is not).
+        if force_write is not None:
+            raise NotImplementedError("force_write is not implemented yet.")
+        response = await client.download(url)
+        if isinstance(response, nio.DownloadResponse):
+            return await cls.from_file(io.BytesIO(response.body), response.filename)
+        raise MediaDownloadException("Failed to download attachment.", response)
+
+    @classmethod
+    async def from_http(
+        cls,
+        url: str,
+        client_session: aiohttp.ClientSession = None,
+        *,
+        force_write: bool | pathlib.Path = False,
+    ) -> "BaseAttachment":
+        """
+        Creates an attachment from an HTTP URL.
+
+        This is not necessarily just for images, video, or other media - it can be used for any HTTP resource.
+
+        :param url: The http/s URL to download
+        :param client_session: The aiohttp client session to use. If not specified, a new one will be created.
+        :param force_write: Whether to force stream the download to the file system, instead of into memory.
+            See: [niobot.BaseAttachment.from_mxc][]
+        :return: The downloaded and probed attachment.
+        :raises: niobot.MediaDownloadException if the download failed.
+        :raises: aiohttp.ClientError if the download failed.
+        :raises niobot.MediaDetectionException: if the MIME type could not be detected.
+        """
+        if not client_session:
+            from . import __user_agent__
+
+            async with aiohttp.ClientSession(headers={"User-Agent": __user_agent__}) as session:
+                return await cls.from_http(url, session, force_write=force_write)
+
+        async with client_session.get(url) as response:
+            try:
+                response.raise_for_status()
+            except aiohttp.ClientResponseError as err:
+                raise MediaDownloadException("Failed to download attachment.", exception=err)
+            save_path = None
+            if force_write is not None:
+                if force_write is True:
+                    tempdir = tempfile.gettempdir()
+                elif isinstance(force_write, pathlib.Path):
+                    tempdir = force_write
+
+                file_name = response.headers.get("Content-Disposition")
+                if file_name:
+                    file_name = re.search(r"filename=\"(.+)\"", file_name)
+                    if file_name:
+                        file_name = file_name.group(1)
+
+                if not file_name:
+                    u = urllib.parse.urlparse(url)
+                    file_name = os.path.basename(u.path)
+
+                if os.path.isdir(tempdir):
+                    save_path = os.path.join(tempdir, file_name)
+                else:
+                    save_path = tempdir
+
+            if save_path is not None:
+                async with aiofiles.open(save_path, "wb") as fh:
+                    async for chunk in response.content.iter_chunked(1024):
+                        await fh.write(chunk)
+                return await cls.from_file(save_path, file_name)
+            else:
+                return await cls.from_file(io.BytesIO(await response.read()), file_name)
+
     @property
     def size_bytes(self) -> int:
         """Returns the size of this attachment in bytes."""
         return self.size
 
     def size_as(
-            self,
-            unit: typing.Literal[
-                'b',
-                'kb',
-                'kib',
-                'mb',
-                'mib',
-                'gb',
-                'gib',
-            ]
+        self,
+        unit: typing.Literal[
+            "b",
+            "kb",
+            "kib",
+            "mb",
+            "mib",
+            "gb",
+            "gib",
+        ],
     ) -> typing.Union[int, float]:
         """
         Helper function to convert the size of this attachment into a different unit.
 
-        ??? note "Example"
+        ??? example "Example"
             ```python
             >>> import niobot
-            >>> attachment = niobot.FileAttachment("test.txt", "text/plain")
+            >>> attachment = niobot.FileAttachment("background.png", "image/png")
             >>> attachment.size_bytes
-            1024
+            329945
             >>> attachment.size_as("kb")
-            1.024
+            329.945
+            >>> attachment.size_as("kib")
+            322.2119140625
             >>> attachment.size_as("mb")
-            0.001024
+            0.329945
+            >>> attachment.size_as("mib")
+            0.31466007232666016
             ```
             *Note that due to the nature of floats, precision may be lost, especially the larger in units you go.*
 
         :param unit: The unit to convert into
         :return: The converted size
         """
         multi = {
-            'b': 1,
-            'kb': 1000,
-            'kib': 1024,
-            'mb': 1000 ** 2,
-            'mib': 1024 ** 2,
-            'gb': 1000 ** 3,
-            'gib': 1024 ** 3,
+            "b": 1,
+            "kb": 1000,
+            "kib": 1024,
+            "mb": 1000**2,
+            "mib": 1024**2,
+            "gb": 1000**3,
+            "gib": 1024**3,
         }
         return self.size_bytes / multi[unit]
 
     async def upload(self, client: "NioBot", encrypted: bool = False) -> "BaseAttachment":
         """
         Uploads the file to matrix.
 
         :param client: The client to upload
-        :param encrypted: Whether to encrypt the thumbnail or not
+        :param encrypted: Whether to encrypt the attachment or not
         :return: The attachment
         """
         if self.keys or self.url:
             raise RuntimeError("This attachment has already been uploaded.")
         if self.file_name is None:
             if hasattr(self.file, "name"):
                 self.file_name = self.file.name
@@ -544,27 +686,28 @@
 class SupportXYZAmorganBlurHash(BaseAttachment):
     """
     Represents an attachment that supports blurhashes.
 
     :param xyz_amorgan_blurhash: The blurhash of the attachment
     :ivar xyz_amorgan_blurhash: The blurhash of the attachment
     """
+
     if typing.TYPE_CHECKING:
         xyz_amorgan_blurhash: str
 
     def __init__(self, *args, xyz_amorgan_blurhash: str = None, **kwargs):
         super().__init__(*args, **kwargs)
         self.xyz_amorgan_blurhash = xyz_amorgan_blurhash
 
     @classmethod
     async def from_file(
-            cls,
-            file: typing.Union[str, io.BytesIO, pathlib.Path],
-            file_name: str = None,
-            xyz_amorgan_blurhash: str | bool = None,
+        cls,
+        file: typing.Union[str, io.BytesIO, pathlib.Path],
+        file_name: str = None,
+        xyz_amorgan_blurhash: str | bool = None,
     ) -> "SupportXYZAmorganBlurHash":
         file = _to_path(file)
         if isinstance(file, io.BytesIO):
             if not file_name:
                 raise ValueError("file_name must be specified when uploading a BytesIO object.")
         else:
             if not file_name:
@@ -607,20 +750,21 @@
     This is for everything else.
 
     :param file: The file to upload
     :param file_name: The name of the file
     :param mime_type: The mime type of the file
     :param size_bytes: The size of the file in bytes
     """
+
     def __init__(
-            self,
-            file: typing.Union[str, io.BytesIO, pathlib.Path],
-            file_name: str = None,
-            mime_type: str = None,
-            size_bytes: int = None,
+        self,
+        file: typing.Union[str, io.BytesIO, pathlib.Path],
+        file_name: str = None,
+        mime_type: str = None,
+        size_bytes: int = None,
     ):
         super().__init__(file, file_name, mime_type, size_bytes, attachment_type=AttachmentType.FILE)
 
 
 class ImageAttachment(SupportXYZAmorganBlurHash):
     """
     Represents an image attachment.
@@ -633,52 +777,53 @@
     :param width: The width of the image in pixels (e.g. 1920)
     :param thumbnail: A thumbnail of the image. NOT a blurhash.
     :param xyz_amorgan_blurhash: The blurhash of the image
 
     :ivar info: A dict of info about the image. Contains `h`, `w`, `mimetype`, and `size` keys.
     :ivar thumbnail: A thumbnail of the image. NOT a blurhash.
     """
+
     def __init__(
-            self,
-            file: typing.Union[str, io.BytesIO, pathlib.Path],
-            file_name: str = None,
-            mime_type: str = None,
-            size_bytes: int = None,
-            height: int = None,
-            width: int = None,
-            thumbnail: "ImageAttachment" = None,
-            xyz_amorgan_blurhash: str = None,
+        self,
+        file: typing.Union[str, io.BytesIO, pathlib.Path],
+        file_name: str = None,
+        mime_type: str = None,
+        size_bytes: int = None,
+        height: int = None,
+        width: int = None,
+        thumbnail: "ImageAttachment" = None,
+        xyz_amorgan_blurhash: str = None,
     ):
         super().__init__(
             file,
             file_name,
             mime_type,
             size_bytes,
             xyz_amorgan_blurhash=xyz_amorgan_blurhash,
-            attachment_type=AttachmentType.IMAGE
+            attachment_type=AttachmentType.IMAGE,
         )
         self.info = {
             "h": height,
             "w": width,
             "mimetype": mime_type,
             "size": size_bytes,
         }
         self.thumbnail = thumbnail
 
     @classmethod
     async def from_file(
-            cls,
-            file: typing.Union[str, io.BytesIO, pathlib.Path],
-            file_name: str = None,
-            height: int = None,
-            width: int = None,
-            thumbnail: "ImageAttachment" = None,
-            generate_blurhash: bool = True,
-            *,
-            unsafe: bool = False
+        cls,
+        file: typing.Union[str, io.BytesIO, pathlib.Path],
+        file_name: str = None,
+        height: int = None,
+        width: int = None,
+        thumbnail: "ImageAttachment" = None,
+        generate_blurhash: bool = True,
+        *,
+        unsafe: bool = False,
     ) -> "ImageAttachment":
         """
         Generates an image attachment
 
         :param file: The file to upload
         :param file_name: The name of the file (only used if file is a `BytesIO`)
         :param height: The height, in pixels, of this image
@@ -739,51 +884,46 @@
     :param mime_type: The mime type of the file
     :param size_bytes: The size of the file in bytes
     :param height: The height of the video in pixels (e.g. 1080)
     :param width: The width of the video in pixels (e.g. 1920)
     :param duration: The duration of the video in seconds
     :param thumbnail: A thumbnail of the video. NOT a blurhash.
     """
+
     def __init__(
-            self,
-            file: typing.Union[str, io.BytesIO, pathlib.Path],
-            file_name: str = None,
-            mime_type: str = None,
-            size_bytes: int = None,
-            duration: int = None,
-            height: int = None,
-            width: int = None,
-            thumbnail: "ImageAttachment" = None,
+        self,
+        file: typing.Union[str, io.BytesIO, pathlib.Path],
+        file_name: str = None,
+        mime_type: str = None,
+        size_bytes: int = None,
+        duration: int = None,
+        height: int = None,
+        width: int = None,
+        thumbnail: "ImageAttachment" = None,
     ):
-        super().__init__(
-            file,
-            file_name,
-            mime_type,
-            size_bytes,
-            attachment_type=AttachmentType.VIDEO
-        )
+        super().__init__(file, file_name, mime_type, size_bytes, attachment_type=AttachmentType.VIDEO)
         self.info = {
             "duration": round(duration * 1000) if duration else None,
             "h": height,
             "w": width,
             "mimetype": mime_type,
             "size": size_bytes,
         }
         self.thumbnail = thumbnail
 
     @classmethod
     async def from_file(
-            cls,
-            file: typing.Union[str, io.BytesIO, pathlib.Path],
-            file_name: str = None,
-            duration: int = None,
-            height: int = None,
-            width: int = None,
-            thumbnail: ImageAttachment | typing.Literal[False] = None,
-            generate_blurhash: bool = True,
+        cls,
+        file: typing.Union[str, io.BytesIO, pathlib.Path],
+        file_name: str = None,
+        duration: int = None,
+        height: int = None,
+        width: int = None,
+        thumbnail: ImageAttachment | typing.Literal[False] = None,
+        generate_blurhash: bool = True,
     ) -> "VideoAttachment":
         """
         Generates a video attachment
 
         !!! warning "This function auto-generates a thumbnail!"
             As thumbnails greatly improve user experience, even with blurhashes enabled, this function will by default
             create a thumbnail of the first frame of the given video if you do not provide one yourself.
@@ -813,16 +953,19 @@
             if not file_name:
                 file_name = file.name
 
             if height is None or width is None or duration is None:
                 metadata = await run_blocking(get_metadata, file)
                 for stream in metadata["streams"]:
                     if stream["codec_type"] == "video":
-                        if stream["codec_name"].lower() not in SUPPORTED_VIDEO_CODECS \
-                                or not stream["codec_name"].startswith("pcm_"):  # usually, pcm is supported.
+                        if stream["codec_name"].lower() not in SUPPORTED_VIDEO_CODECS or not stream[
+                            "codec_name"
+                        ].startswith(
+                            "pcm_"
+                        ):  # usually, pcm is supported.
                             warning = MediaCodecWarning(stream["codec_name"], *SUPPORTED_VIDEO_CODECS)
                             warnings.warn(warning)
                         height = stream["height"]
                         width = stream["width"]
                         duration = round(float(metadata["format"]["duration"]) * 1000)
                         break
                 else:
@@ -871,41 +1014,36 @@
         return body
 
 
 class AudioAttachment(BaseAttachment):
     """
     Represents an audio attachment.
     """
+
     def __init__(
-            self,
-            file: typing.Union[str, io.BytesIO, pathlib.Path],
-            file_name: str = None,
-            mime_type: str = None,
-            size_bytes: int = None,
-            duration: int = None,
+        self,
+        file: typing.Union[str, io.BytesIO, pathlib.Path],
+        file_name: str = None,
+        mime_type: str = None,
+        size_bytes: int = None,
+        duration: int = None,
     ):
-        super().__init__(
-            file,
-            file_name,
-            mime_type,
-            size_bytes,
-            attachment_type=AttachmentType.AUDIO
-        )
+        super().__init__(file, file_name, mime_type, size_bytes, attachment_type=AttachmentType.AUDIO)
         self.info = {
             "duration": round(duration * 1000) if duration else None,
             "mimetype": mime_type,
             "size": size_bytes,
         }
 
     @classmethod
     async def from_file(
-            cls,
-            file: typing.Union[str, io.BytesIO, pathlib.Path],
-            file_name: str = None,
-            duration: int = None,
+        cls,
+        file: typing.Union[str, io.BytesIO, pathlib.Path],
+        file_name: str = None,
+        duration: int = None,
     ) -> "AudioAttachment":
         """
         Generates an audio attachment
 
         :param file: The file to upload
         :param file_name: The name of the file (only used if file is a `BytesIO`)
         :param duration: The duration of the audio, in seconds
```

### Comparing `nio-bot-1.0.2/src/niobot/client.py` & `nio-bot-1.1.0a1/src/niobot/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import asyncio
+import importlib
+import inspect
 import logging
 import os
-import importlib
+import re
 import time
-import inspect
 import typing
 from collections import deque
 
+import marko
 import nio
 from nio.crypto import ENCRYPTION_ENABLED
-import marko
 
 try:
     from .attachment import BaseAttachment
 except ImportError:
     BaseAttachment = None
-from .exceptions import *
-from .utils import run_blocking, Typing, force_await
-from .utils.help_command import help_command_callback
 from .commands import Command, Module
+from .exceptions import *
+from .utils import Typing, force_await, run_blocking
+from .utils.help_command import default_help_command
 
-
-__all__ = (
-    "NioBot",
-)
+__all__ = ("NioBot",)
 
 
 class NioBot(nio.AsyncClient):
     """
     The main client for NioBot.
 
     :param homeserver: The homeserver to connect to. e.g. https://matrix-client.matrix.org
@@ -38,45 +36,47 @@
     :param case_insensitive: Whether to ignore case when checking for commands. If True, this lower()s
      incoming messages for parsing.
     :param global_message_type: The message type to default to. Defaults to m.notice
     :param ignore_old_events: Whether to simply discard events before the bot's login.
     :param auto_join_rooms: Whether to automatically join rooms the bot is invited to.
     :param automatic_markdown_renderer: Whether to automatically render markdown in messages when sending/editing.
     :param owner_id: The user ID of the bot owner. If set, only this user can run owner-only commands, etc.
+    :param max_message_cache: The maximum number of messages to cache. Defaults to 1000.
     """
+
     def __init__(
-            self,
-            homeserver: str,
-            user_id: str,
-            device_id: str = "nio-bot",
-            store_path: str = None,
-            *,
-            command_prefix: str,
-            case_insensitive: bool = True,
-            owner_id: str = None,
-            **kwargs
+        self,
+        homeserver: str,
+        user_id: str,
+        device_id: str = "nio-bot",
+        store_path: str = None,
+        *,
+        command_prefix: str,
+        case_insensitive: bool = True,
+        owner_id: str = None,
+        **kwargs,
     ):
+        try:
+            self.loop = asyncio.get_running_loop()
+        except RuntimeError:
+            self.loop = None
         self.log = logging.getLogger(__name__)
         if store_path:
             if not os.path.exists(store_path):
                 self.log.warning("Store path %s does not exist, creating...", store_path)
                 os.makedirs(store_path, mode=0o751, exist_ok=True)
             elif not os.path.isdir(store_path):
-                raise RuntimeError("Store path %s is not a directory!" % store_path)
+                raise FileNotFoundError("Store path %s is not a directory!" % store_path)
 
         if ENCRYPTION_ENABLED:
             if not kwargs.get("config"):
-                kwargs.setdefault(
-                    "config",
-                    nio.AsyncClientConfig(
-                        encryption_enabled=True,
-                        store_sync_tokens=True
-                    )
-                )
+                kwargs.setdefault("config", nio.AsyncClientConfig(encryption_enabled=True, store_sync_tokens=True))
                 self.log.info("Encryption support enabled automatically.")
+        else:
+            self.log.info("Encryption support is not available (are the e2ee extras installed?)")
 
         super().__init__(
             homeserver,
             user_id,
             device_id,
             store_path=store_path,
             config=kwargs.pop("config", None),
@@ -88,55 +88,77 @@
         self.store_path = store_path
         self.case_insensitive = case_insensitive
         self.command_prefix = command_prefix
         self.owner_id = owner_id
 
         if command_prefix == "/":
             self.log.warning("The prefix '/' may interfere with client-side commands on some clients, such as Element.")
-        if " " in command_prefix:
-            raise RuntimeError("Command prefix cannot contain spaces.")
+        if re.match(r"\s", command_prefix):
+            raise RuntimeError("Command prefix cannot contain whitespace.")
 
         self.start_time: float | None = None
         help_cmd = Command(
-            "help",
-            help_command_callback,
-            aliases=["h"],
-            description="Shows a list of commands for this bot"
+            "help", default_help_command, aliases=["h"], description="Shows a list of commands for this bot"
         )
-        self._commands = {
-            "help": help_cmd,
-            "h": help_cmd
-        }
+        if kwargs.get("help_command"):
+            cmd = kwargs.pop("help_command")
+            if isinstance(cmd, Command):
+                help_cmd = cmd
+            elif asyncio.iscoroutinefunction(cmd) or inspect.isfunction(cmd):
+                self.log.warning(
+                    "Manually changing default help command callback to %r. Please consider passing your own"
+                    " Command instance instead."
+                )
+                help_cmd.callback = cmd
+            else:
+                raise TypeError("help_command must be a Command instance or a coroutine/function.")
+        self._commands = {"help": help_cmd, "h": help_cmd}
         self._modules = {}
         self._events = {}
         self._event_tasks = []
-        self.global_message_type = kwargs.pop(
-            "global_message_type",
-            "m.notice"
-        )
+        self.global_message_type = kwargs.pop("global_message_type", "m.notice")
         self.ignore_old_events = kwargs.pop("ignore_old_events", True)
         self.auto_join_rooms = kwargs.pop("auto_join_rooms", True)
         self.automatic_markdown_renderer = kwargs.pop("automatic_markdown_renderer", True)
         # NOTE: `m.notice` prevents bot messages sending off room notifications, and shows darker text
         # (In element at least).
 
         # noinspection PyTypeChecker
         self.add_event_callback(self.process_message, nio.RoomMessageText)
-        self.add_event_callback(
-            self.update_read_receipts,
-            nio.RoomMessage
-        )
+        self.add_event_callback(self.update_read_receipts, nio.RoomMessage)
+        self.direct_rooms: typing.Dict[str, nio.MatrixRoom] = {}
 
         self.message_cache: typing.Deque[typing.Tuple[nio.MatrixRoom, nio.RoomMessageText]] = deque(
             maxlen=kwargs.pop("max_message_cache", 1000)
         )
+        self.is_ready = asyncio.Event()
         self._waiting_events = {}
 
-        # noinspection PyTypeChecker
-        self.add_event_callback(self._auto_join_room_backlog_callback, nio.InviteMemberEvent)
+        if self.auto_join_rooms is True:
+            self.log.info("Auto-joining rooms enabled.")
+            # noinspection PyTypeChecker
+            self.add_event_callback(self._auto_join_room_backlog_callback, nio.InviteMemberEvent)
+
+    async def sync(self, *args, **kwargs) -> nio.SyncResponse | nio.SyncError:
+        sync = await super().sync(*args, **kwargs)
+        if isinstance(sync, nio.SyncResponse):
+            self._populate_dm_rooms(sync)
+        return sync
+
+    def _populate_dm_rooms(self, sync: nio.SyncResponse):
+        # This function is a workaround until a solution is implemented upstream.
+        # This function is unreliable (see: `is_direct` below, not always provided, optional in spec)
+        # See: https://github.com/poljar/matrix-nio/issues/421
+        for room_id, room_info in sync.rooms.join.items():
+            for event in room_info.state:
+                if isinstance(event, nio.RoomMemberEvent):
+                    prev = event.prev_content or {}
+                    if event.content.get("is_direct", prev.get("is_direct", False)):
+                        self.log.debug("Found DM room in sync: %s", room_id)
+                        self.direct_rooms[event.state_key] = self.rooms[room_id]
 
     async def _auto_join_room_callback(self, room: nio.MatrixRoom, _: nio.InviteMemberEvent):
         """Callback for auto-joining rooms"""
         if self.auto_join_rooms:
             self.log.info("Joining room %s", room.room_id)
             result = await self.join(room.room_id)
             if isinstance(result, nio.JoinError):
@@ -162,16 +184,15 @@
     def dispatch(self, event_name: str, *args, **kwargs):
         """Dispatches an event to listeners"""
         if event_name in self._events:
             for handler in self._events[event_name]:
                 self.log.debug("Dispatching %s to %r" % (event_name, handler))
                 try:
                     task = asyncio.create_task(
-                        handler(*args, **kwargs),
-                        name="DISPATCH_%s_%s" % (handler.__qualname__, os.urandom(3).hex())
+                        handler(*args, **kwargs), name="DISPATCH_%s_%s" % (handler.__qualname__, os.urandom(3).hex())
                     )
                     self._event_tasks.append(task)
                     task.add_done_callback(
                         lambda *_, **__: self._event_tasks.remove(task) if task in self._event_tasks else None
                     )
                 except Exception as e:
                     self.log.exception("Error dispatching %s to %r", event_name, handler, exc_info=e)
@@ -185,23 +206,26 @@
             start_time = time.time() - 30  # relative
         else:
             start_time = self.start_time
         if self.ignore_old_events is False:
             return False
         return start_time - event.server_timestamp / 1000 > 0
 
-    async def update_read_receipts(self, room, event):
+    async def update_read_receipts(self, room: str | nio.MatrixRoom, event: nio.Event):
         """part of spec module 11.6"""
+        room = self._get_id(room)
         if self.is_old(event):
             self.log.debug("Ignoring event %s, sent before bot started.", event.event_id)
             return
-        self.log.debug("Updating read receipts for %s", room.room_id)
-        result = await self.room_read_markers(room, event.event_id, event.event_id)
+        event = event.event_id
+        result = await self.room_read_markers(room, event, event)
         if not isinstance(result, nio.RoomReadMarkersResponse):
-            self.log.warning("Failed to update read receipts for %s: %s", room.room_id, result.message)
+            self.log.warning("Failed to update read receipts for %s: %s", room, result.message)
+        else:
+            self.log.debug("Updated read receipts for %s to %s.", room, event)
 
     async def process_message(self, room: nio.MatrixRoom, event: nio.RoomMessageText):
         """Processes a message and runs the command it is trying to invoke if any."""
         self.message_cache.append((room, event))
         self.dispatch("message", room, event)
         if event.sender == self.user:
             self.log.debug("Ignoring message sent by self.")
@@ -214,42 +238,50 @@
         if self.case_insensitive:
             content = event.body.lower()
         else:
             content = event.body
 
         if content.startswith(self.command_prefix):
             try:
-                command = original_command = content[len(self.command_prefix):].splitlines()[0].split(" ")[0]
+                command = original_command = content[len(self.command_prefix) :].splitlines()[0].split(" ")[0]
             except IndexError:
                 self.log.info(
                     "Failed to parse message %r - message terminated early (was the content *just* the prefix?)",
-                    event.body
+                    event.body,
                 )
                 return
             command = self.get_command(command)
             if command:
                 if command.disabled is True:
                     raise CommandDisabledError(command)
                 context = command.construct_context(self, room, event, self.command_prefix + original_command)
                 self.dispatch("command", context)
 
                 def _task_callback(t: asyncio.Task):
                     try:
                         exc = t.exception()
                     except asyncio.CancelledError:
-                        self.dispatch('command_cancelled', context, t)
+                        self.dispatch("command_cancelled", context, t)
                     else:
                         if exc:
-                            self.dispatch('command_error', context, CommandError(exception=exc))
+                            self.dispatch("command_error", context, CommandError(exception=exc))
                         else:
-                            self.dispatch('command_complete', context, t)
+                            self.dispatch("command_complete", context, t)
+                    if hasattr(context, "_perf_timer"):
+                        self.log.debug(
+                            "Command %r finished in %.2f seconds",
+                            command.name,
+                            time.perf_counter() - context._perf_timer,
+                        )
+
                 self.log.debug(f"Running command {command.name} with context {context!r}")
                 try:
-                    task = asyncio.create_task(command.invoke(context))
+                    task = asyncio.create_task(await command.invoke(context))
                     context._task = task
+                    context._perf_timer = time.perf_counter()
                 except CommandArgumentsError as e:
                     self.dispatch("command_error", context, e)
                 except Exception as e:
                     self.log.exception("Failed to invoke command %s", command.name)
                     self.dispatch("command_error", context, CommandError(exception=e))
                 else:
                     task.add_done_callback(_task_callback)
@@ -269,14 +301,23 @@
         return self.owner_id == user_id
 
     def mount_module(self, import_path: str) -> typing.Optional[list[Command]]:
         """Mounts a module including all of its commands.
 
         Must be a subclass of niobot.commands.Module, or else this function will not work.
 
+        ??? danger "There may not be an event loop running when this function is called."
+            If you are calling this function before you call `bot.run()`, it is entirely possible that you don't have
+            a running [asyncio][] event loop. If you use the event loop in `Module.__init__`, you will get an error,
+            and the module will fail the mount.
+
+            You can get around this by deferring mounting your modules until the `bot.on_ready` event is fired,
+            at which point not only will the first full sync have completed (meaning the bot has all of its caches
+            populated), but the event loop will be running.
+
         :param import_path: The import path (such as modules.file), which would be ./modules/file.py in a file tree.
         :returns: Optional[List[Command]] - A list of commands mounted. None if the module's setup() was called.
         :raise ImportError: The module path is incorrect of there was another error while importing
         :raise TypeError: The module was not a subclass of Module.
         :raise ValueError: There was an error registering a command (e.g. name conflict)
         """
         added = []
@@ -298,15 +339,15 @@
                         raise TypeError("%r is not a subclass of Module." % instance.__class__.__name__)
                     instance.__setup__()
                     self._modules[item] = instance
                     added += list(instance.list_commands())
                     self.log.debug(
                         "Loaded %d commands from %r",
                         len(set(instance.list_commands())),
-                        instance.__class__.__qualname__
+                        instance.__class__.__qualname__,
                     )
                 else:
                     self.log.debug("%r does not appear to be a niobot module", item)
         return added
 
     @property
     def commands(self) -> typing.Dict[str, Command]:
@@ -373,14 +414,15 @@
 
         def decorator(func):
             nonlocal name
             name = name or func.__name__
             command = cls(name, func, **kwargs)
             self.add_command(command)
             return func
+
         return decorator
 
     def add_event_listener(self, event_type: str, func):
         self._events.setdefault(event_type, [])
         self._events[event_type].append(func)
         self.log.debug("Added event listener %r for %r", func, event_type)
 
@@ -391,14 +433,15 @@
             event_type = event_type[3:]
 
         def wrapper(func):
             nonlocal event_type
             event_type = event_type or func.__name__
             self.add_event_listener(event_type, func)
             return func
+
         return wrapper
 
     def remove_event_listener(self, function):
         for event_type, functions in self._events.items():
             if function in functions:
                 self._events[event_type].remove(function)
                 self.log.debug("Removed %r from event %r", function, event_type)
@@ -418,17 +461,15 @@
             room_id,
             message_type,
             content,
             tx_id,
             ignore_unverified_devices,
         )
 
-    def get_cached_message(self, event_id: str) -> typing.Optional[
-        typing.Tuple[nio.MatrixRoom, nio.RoomMessageText]
-    ]:
+    def get_cached_message(self, event_id: str) -> typing.Optional[typing.Tuple[nio.MatrixRoom, nio.RoomMessageText]]:
         """Fetches a message from the cache.
 
         This returns both the room the message was sent in, and the event itself.
 
         If the message is not in the cache, this returns None."""
         for room, event in self.message_cache:
             if event_id == event.event_id:
@@ -443,20 +484,20 @@
         result: typing.Union[nio.RoomGetEventError, nio.RoomGetEventResponse]
         result = await self.room_get_event(room_id, event_id)
         if isinstance(result, nio.RoomGetEventError):
             raise NioBotException(f"Failed to fetch message {event_id} from {room_id}: {result}", original=result)
         return result
 
     async def wait_for_message(
-            self,
-            room_id: str = None,
-            sender: str = None,
-            check: typing.Callable[[nio.MatrixRoom, nio.RoomMessageText], typing.Any] = None,
-            *,
-            timeout: float = None
+        self,
+        room_id: str = None,
+        sender: str = None,
+        check: typing.Callable[[nio.MatrixRoom, nio.RoomMessageText], typing.Any] = None,
+        *,
+        timeout: float = None,
     ) -> typing.Optional[typing.Tuple[nio.MatrixRoom, nio.RoomMessageText]]:
         """Waits for a message, optionally with a filter.
 
         If this function times out, asyncio.TimeoutError is raised."""
         event = asyncio.Event()
         value = None
 
@@ -498,70 +539,104 @@
             rendered = text
         return rendered
 
     @staticmethod
     def _get_id(obj) -> str:
         if hasattr(obj, "room_id"):
             return obj.room_id
+        if hasattr(obj, "user_id"):
+            return obj.user_id
         if hasattr(obj, "event_id"):
             return obj.event_id
         if isinstance(obj, str):
             return obj
         raise ValueError("Unable to determine ID")
 
     @staticmethod
     def generate_mx_reply(room: nio.MatrixRoom, event: nio.RoomMessageText) -> str:
         """Generates a reply string for a given event."""
         return (
             "<mx-reply>"
             "<blockquote>"
-            "<a href=\"{reply_url}\">{reply}</a> "
-            "<a href=\"{user_url}\">{user}</a><br/>"
+            '<a href="{reply_url}">{reply}</a> '
+            '<a href="{user_url}">{user}</a><br/>'
             "</blockquote>"
             "</mx-reply>".format(
                 reply_url="https://matrix.to/#/{}:{}/{}".format(
-                    room.room_id,
-                    room.machine_name.split(":")[1],
-                    event.event_id
+                    room.room_id, room.machine_name.split(":")[1], event.event_id
                 ),
                 reply=event.body,
-                user_url="https://matrix.to/#/{}".format(
-                    event.sender
-                ),
+                user_url="https://matrix.to/#/{}".format(event.sender),
                 user=event.sender,
             )
         )
 
     async def _recursively_upload_attachments(
-            self,
-            base: "BaseAttachment",
-            encrypted: bool = False,
-            __previous: list = None
+        self, base: "BaseAttachment", encrypted: bool = False, __previous: list = None
     ) -> list[typing.Union[nio.UploadResponse, nio.UploadError, type(None)]]:
         """Recursively uploads attachments."""
         previous = (__previous or []).copy()
         if not base.url:
             previous.append(await base.upload(self, encrypted))
-        if hasattr(base, 'thumbnail') and base.thumbnail and not base.url:
+        if hasattr(base, "thumbnail") and base.thumbnail and not base.url:
             previous += await self._recursively_upload_attachments(base.thumbnail, encrypted, previous)
         return previous
 
+    async def get_dm_room(self, user: nio.MatrixUser | str) -> nio.MatrixRoom:
+        """
+        Gets (or creates) a room that is a private DM room for the given user.
+
+        !!! danger "Unreliable detection"
+            Due to an [issue in `matrix-nio`](https://github.com/poljar/matrix-nio/issues/421), some clients
+            (as per the matrix spec) do not issue the flag that indicates a room is a DM room while inviting users.
+
+            Due to the lack of a native solution in matrix-nio, `niobot` has a very hacky workaround that hooks into
+            the timeline for rooms, and manually detects DM rooms.
+            Due to this being a workaround, not a full solution, this may be unreliable. You should not rely on this
+            function to reliably return an existing DM room, or a valid DM room at all.
+
+        :param user: The User or user ID to fetch a DM room for.
+        :return: The DM room, either pre-existing, or a new one.
+        :raises NioBotException: A room could not be created.
+        :raises RuntimeError: The room was created, but was not in the internal cache.
+        """
+        user_id = self._get_id(user)
+        if user_id in self.direct_rooms:
+            room = self.direct_rooms[user_id]
+            self.log.debug("%r already has a DM room: %r. Returning that.", user_id, room)
+        else:
+            self.log.debug("%r does not have a DM room. Creating one.", user_id)
+            room = await self.room_create(is_direct=True, invite=[user_id])
+            if not isinstance(room, nio.RoomCreateResponse):
+                raise NioBotException("Unable to create DM room for %r: %r" % (user_id, room), response=room)
+            self.log.debug("Created DM room for %r: %r", user_id, room)
+            room = self.rooms.get(room.room_id)
+            if not room:
+                raise RuntimeError("DM room %r was created, but could not be found in the room list!" % room.room_id)
+            self.direct_rooms[user_id] = room
+        return room
+
     async def send_message(
-            self,
-            room: nio.MatrixRoom | str,
-            content: str = None,
-            file: BaseAttachment = None,
-            reply_to: nio.RoomMessageText | str = None,
-            message_type: str = None,
-            clean_mentions: bool = False
+        self,
+        room: nio.MatrixRoom | nio.MatrixUser | str,
+        content: str = None,
+        file: BaseAttachment = None,
+        reply_to: nio.RoomMessageText | str = None,
+        message_type: str = None,
+        clean_mentions: bool = False,
     ) -> nio.RoomSendResponse:
         """
         Sends a message.
 
-        :param room: The room to send this message to
+        !!! tip "New! DMs!"
+            As of v1.1.0, you can now send messages to users (either a [nio.MatrixUser][] or a user ID string),
+            and a direct message room will automatically be created for you if one does not exist, using an existing
+            one if it does.
+
+        :param room: The room or to send this message to
         :param content: The content to send. Cannot be used with file.
         :param file: A file to send, if any. Cannot be used with content.
         :param reply_to: A message to reply to.
         :param message_type: The message type to send. If none, defaults to NioBot.global_message_type,
         which itself is `m.notice` by default.
         :param clean_mentions: Whether to escape all mentions
         :return: The response from the server.
@@ -569,14 +644,19 @@
         :raises ValueError: You specified neither file nor content.
         """
         if file and BaseAttachment is None:
             raise ValueError("You are missing required libraries to use attachments.")
         if not any((content, file)):
             raise ValueError("You must specify either content or file.")
 
+        if isinstance(room, nio.MatrixUser) or (isinstance(room, str) and room.startswith("@")):
+            room = await self.get_dm_room(room)
+
+        self.log.debug("Send message resolved room to %r", room)
+
         body = {
             "msgtype": message_type or self.global_message_type,
         }
 
         if file is not None:
             # We need to upload the file first.
             responses = await self._recursively_upload_attachments(file, encrypted=getattr(file, "encrypted", False))
@@ -585,53 +665,48 @@
                     "Failed to upload media.", tuple(filter(lambda x: isinstance(x, nio.UploadError), responses))[0]
                 )
 
             body = file.as_body(content)
         else:
             if clean_mentions:
                 content = content.replace("@", "@\u200b")
-            body['body'] = content
+            body["body"] = content
             if self.automatic_markdown_renderer:
                 parsed = await run_blocking(marko.parse, content)
                 if parsed.children:
                     rendered = await run_blocking(marko.render, parsed)
                     body["formatted_body"] = rendered
                     body["format"] = "org.matrix.custom.html"
 
                 if reply_to and isinstance(reply_to, nio.RoomMessageText) and isinstance(room, nio.MatrixRoom):
                     body["formatted_body"] = "{}{}".format(
-                        self.generate_mx_reply(room, reply_to),
-                        body.get("formatted_body", body["body"])
+                        self.generate_mx_reply(room, reply_to), body.get("formatted_body", body["body"])
                     )
                     body["format"] = "org.matrix.custom.html"
 
         if reply_to:
-            body["m.relates_to"] = {
-                "m.in_reply_to": {
-                    "event_id": self._get_id(reply_to)
-                }
-            }
+            body["m.relates_to"] = {"m.in_reply_to": {"event_id": self._get_id(reply_to)}}
         async with Typing(self, self._get_id(room)):
             response = await self.room_send(
                 self._get_id(room),
                 "m.room.message",
                 body,
             )
         if isinstance(response, nio.RoomSendError):
             raise MessageException("Failed to send message.", response)
         return response
 
     async def edit_message(
-            self,
-            room: nio.MatrixRoom | str,
-            message: nio.Event | str,
-            content: str,
-            *,
-            message_type: str = None,
-            clean_mentions: bool = False
+        self,
+        room: nio.MatrixRoom | str,
+        message: nio.Event | str,
+        content: str,
+        *,
+        message_type: str = None,
+        clean_mentions: bool = False,
     ) -> nio.RoomSendResponse:
         """
         Edit an existing message. You must be the sender of the message.
 
         You also cannot edit messages that are attachments.
 
         :param room: The room the message is in.
@@ -652,17 +727,15 @@
             "format": "org.matrix.custom.html",
             "formatted_body": await self._markdown_to_html(content),
         }
 
         body = {
             "msgtype": message_type,
             "body": " * %s" % content["body"],
-            "m.new_content": {
-                **content
-            },
+            "m.new_content": {**content},
             "m.relates_to": {
                 "rel_type": "m.replace",
                 "event_id": event_id,
             },
         }
         async with Typing(self, room.room_id):
             response = await self.room_send(
@@ -673,18 +746,15 @@
         if isinstance(response, nio.RoomSendError):
             raise MessageException("Failed to edit message.", response)
         # Forcefully clear typing
         await self.room_typing(room.room_id, False)
         return response
 
     async def delete_message(
-            self,
-            room: nio.MatrixRoom | str,
-            message_id: nio.RoomMessage | str,
-            reason: str = None
+        self, room: nio.MatrixRoom | str, message_id: nio.RoomMessage | str, reason: str = None
     ) -> nio.RoomRedactResponse:
         """
         Delete an existing message. You must be the sender of the message.
 
         :param room: The room the message is in.
         :param message_id: The message to delete.
         :param reason: The reason for deleting the message.
@@ -695,18 +765,15 @@
         message_id = self._get_id(message_id)
         response = await self.room_redact(room, message_id, reason=reason)
         if isinstance(response, nio.RoomRedactError):
             raise MessageException("Failed to delete message.", response)
         return response
 
     async def add_reaction(
-            self,
-            room: nio.MatrixRoom | str,
-            message: nio.RoomMessage | str,
-            emoji: str
+        self, room: nio.MatrixRoom | str, message: nio.RoomMessage | str, emoji: str
     ) -> nio.RoomSendResponse:
         """
         Adds an emoji "reaction" to a message.
 
         :param room: The room the message is in.
         :param message: The event ID or message object to react to.
         :param emoji: The emoji to react with (e.g. `\N{cross mark}` = ❌)
@@ -737,15 +804,22 @@
         )
         if isinstance(response, nio.RoomRedactError):
             raise MessageException("Failed to delete reaction.", response)
         return response
 
     async def start(self, password: str = None, access_token: str = None, sso_token: str = None) -> None:
         """Starts the bot, running the sync loop."""
+        self.loop = asyncio.get_event_loop()
         if password or sso_token:
+            if password:
+                self.log.critical(
+                    "Logging in with a password is insecure, slow, and clunky. "
+                    "An access token will be issued after logging in, please use that. For more information, see:"
+                    "https://eekim10.github.io/niobot/guides/faq.html#why-is-logging-in-with-a-password-so-bad"
+                )
             self.log.info("Logging in with a password or SSO token")
             login_response = await self.login(password=password, token=sso_token, device_name=self.device_id)
             if isinstance(login_response, nio.LoginError):
                 raise LoginException("Failed to log in.", login_response)
             else:
                 self.log.info("Logged in as %s", login_response.user_id)
                 self.log.debug("Logged in: {0.access_token}, {0.user_id}".format(login_response))
@@ -770,14 +844,15 @@
             if isinstance(response, nio.KeysUploadError):
                 self.log.critical("Failed to upload encryption keys. Encryption may not work.")
             self.log.info("Uploaded encryption keys.")
         self.log.info("Performing first sync...")
         result = await self.sync(timeout=30000, full_state=True, set_presence="unavailable")
         if not isinstance(result, nio.SyncResponse):
             raise NioBotException("Failed to perform first sync.", result)
+        self.is_ready.set()
         self.dispatch("ready", result)
         self.log.info("Starting sync loop")
         try:
             await self.sync_forever(
                 timeout=30000,
                 full_state=True,
                 set_presence="online",
```

### Comparing `nio-bot-1.0.2/src/niobot/commands.py` & `nio-bot-1.1.0a1/src/niobot/commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,90 +1,101 @@
-import logging
 import inspect
+import logging
 import os
+import typing
 
 import nio
-import typing
 
 from .context import Context
-from .exceptions import CommandArgumentsError
+from .exceptions import *
 
 if typing.TYPE_CHECKING:
     from .client import NioBot
 
 
-__all__ = (
-    "Command",
-    "command",
-    "event",
-    "Module",
-    "Argument"
-)
+__all__ = ("Command", "command", "event", "Module", "Argument", "check")
 
 _T = typing.TypeVar("_T")
 
 
 class Argument:
     """
     Represents a command argument.
 
     ??? example
         ```py
         from niobot import NioBot, command, Argument
 
         bot = NioBot(...)
 
-        @bot.command("echo", arguments=[Argument("message", str)])
+        @bot.command("echo")
         def echo(ctx: niobot.Context, message: str):
             await ctx.respond(message)
 
         bot.run(...)
         ```
 
     :param name: The name of the argument. Will be used to know which argument to pass to the command callback.
     :param arg_type: The type of the argument (e.g. str, int, etc. or a custom type)
     :param description: The description of the argument. Will be shown in the auto-generated help command.
     :param default: The default value of the argument
     :param required: Whether the argument is required or not. Defaults to True if default is ..., False otherwise.
     """
+
     def __init__(
-            self,
-            name: str,
-            arg_type: _T,
-            *,
-            description: str = None,
-            default: typing.Any = ...,
-            required: bool = ...,
-            parser: typing.Callable[["Context", "Argument", str], typing.Optional[_T]] = ...,
-            **kwargs
+        self,
+        name: str,
+        arg_type: _T,
+        *,
+        description: str = None,
+        default: typing.Any = ...,
+        required: bool = ...,
+        parser: typing.Callable[["Context", "Argument", str], typing.Optional[_T]] = ...,
+        **kwargs,
     ):
+        log = logging.getLogger(__name__)
         self.name = name
         self.type = arg_type
         self.description = description
         self.default = default
         self.required = required
         if self.required is ...:
             self.required = default is ...
             self.default = None
         self.extra = kwargs
         self.parser = parser
         if self.parser is ...:
-            self.parser = self.internal_parser
+            from .utils import BUILTIN_MAPPING
+
+            if self.type in BUILTIN_MAPPING:
+                log.info("Using builtin parser %r for %r", self.type, self)
+                self.parser = BUILTIN_MAPPING[self.type]
+            else:
+                for base in inspect.getmro(self.type):
+                    if base in BUILTIN_MAPPING:
+                        log.info("Using builtin parser %r for %s due to being a subclass", base, self.type)
+                        self.parser = BUILTIN_MAPPING[base]
+                        break
+                else:
+                    log.info("Using default parser for %s", self.type)
+                    self.parser = self.internal_parser
 
     def __repr__(self):
-        return "<Argument name={0.name!r} type={0.type!r} default={0.default!r} required={0.required!r} " \
-               "parser={0.parser!r}>".format(self)
+        return (
+            "<Argument name={0.name!r} type={0.type!r} default={0.default!r} required={0.required!r} "
+            "parser={0.parser!r}>".format(self)
+        )
 
     @staticmethod
     def internal_parser(_: Context, arg: "Argument", value: str) -> typing.Optional[_T]:
         """The default parser for the argument. Will try to convert the value to the argument type."""
         try:
             return arg.type(value)
         except ValueError:
-            raise CommandArgumentsError(f"Invalid value for argument {arg.name}: {value!r}")
+            raise CommandParserError(f"Invalid value for argument {arg.name}: {value!r}")
 
 
 class Command:
     """Represents a command.
 
     ??? example
         !!! note
@@ -119,40 +130,43 @@
         A list of [`Argument`][niobot.commands.Argument] instances. Will be used to parse the arguments given to the
         command.
         `ctx` is always the first argument, regardless of what you put here.
     :param usage:
         A string representing how to use this command's arguments. Will be shown in the auto-generated help.
         Do not include the command name or your bot's prefix here, only arguments.
         For example: `usage="<message> [times]"` will show up as `[p][command] <message> [times]` in the help command.
-
+    :param hidden:
+        Whether the command is hidden or not. If hidden, the command will be always hidden on the auto-generated help.
     """
-    _CTX_ARG = Argument(
-        "ctx",
-        Context,
-        description="The context for the command",
-        parser=lambda ctx, *_: ctx
-    )
+
+    _CTX_ARG = Argument("ctx", Context, description="The context for the command", parser=lambda ctx, *_: ctx)
 
     def __init__(
-            self,
-            name: str,
-            callback: callable,
-            *,
-            aliases: list[str] = None,
-            description: str = None,
-            disabled: bool = False,
-            **kwargs
+        self,
+        name: str,
+        callback: callable,
+        *,
+        aliases: list[str] = None,
+        description: str = None,
+        disabled: bool = False,
+        hidden: bool = False,
+        **kwargs,
     ):
         self.__runtime_id = os.urandom(16).hex()
         self.log = logging.getLogger(__name__)
         self.name = name
         self.callback = callback
         self.description = description
         self.disabled = disabled
         self.aliases = aliases or []
+        self.checks = kwargs.pop("checks", [])
+        if hasattr(self.callback, "__nio_checks__"):
+            for check_func in self.callback.__nio_checks__.keys():
+                self.checks.append(check_func)
+        self.hidden = hidden
         self.usage = kwargs.pop("usage", None)
         self.module = kwargs.pop("module", None)
         self.arguments = kwargs.pop("arguments", None)
         if not self.arguments:
             if self.arguments is False:  # do not autodetect arguments
                 self.arguments = []
             else:
@@ -224,47 +238,67 @@
             for arg in self.arguments[1:]:
                 if arg.required:
                     usage.append(req.format(arg.name))
                 else:
                     usage.append(opt.format(arg.name))
             return " ".join(usage)
 
-    def invoke(self, ctx: Context):
-        """Invokes the current command with the given context"""
+    async def invoke(self, ctx: Context) -> typing.Coroutine:
+        """
+        Invokes the current command with the given context
+
+        :param ctx: The current context
+        :raises CommandArgumentsError: Too many/few arguments, or an error parsing an argument.
+        :raises CheckFailure: A check failed
+        """
+        from .utils import force_await
+
+        if self.checks:
+            for chk_func in self.checks:
+                name = self.callback.__nio_checks__[chk_func]
+                try:
+                    cr = await force_await(chk_func, ctx)
+                except CheckFailure:
+                    raise  # re-raise existing check failures
+                except Exception as e:
+                    raise CheckFailure(name, exception=e) from e
+                if not cr:
+                    raise CheckFailure(name)
+
         parsed_args = []
-        for index, argument in enumerate(self.arguments[1:], 0):
+        if len(ctx.args) > (len(self.arguments) - 1):
+            raise CommandArgumentsError(f"Too many arguments given to command {self.name}")
+        for index, argument in enumerate(self.arguments[1:]):
             argument: Argument
+
             if index >= len(ctx.args):
                 if argument.required:
                     raise CommandArgumentsError(f"Missing required argument {argument.name}")
                 else:
                     parsed_args.append(argument.default)
                     continue
+
             self.log.debug("Resolved argument %s to %r", argument.name, ctx.args[index])
             try:
-                parsed_argument = argument.parser(ctx, argument, ctx.args[index])
+                parsed_argument = await force_await(argument.parser, ctx, argument, ctx.args[index])
             except Exception as e:
                 error = f"Error while parsing argument {argument.name}: {e}"
                 raise CommandArgumentsError(error) from e
             parsed_args.append(parsed_argument)
 
         parsed_args = [ctx, *parsed_args]
         self.log.debug("Arguments to pass: %r", parsed_args)
         if self.module:
             self.log.debug("Will pass module instance")
             return self.callback(self.module, *parsed_args)
         else:
             return self.callback(*parsed_args)
 
     def construct_context(
-            self,
-            client: "NioBot",
-            room: nio.MatrixRoom,
-            src_event: nio.RoomMessageText,
-            meta: str
+        self, client: "NioBot", room: nio.MatrixRoom, src_event: nio.RoomMessageText, meta: str
     ) -> Context:
         return Context(client, room, src_event, self, invoking_string=meta)
 
 
 def command(name: str = None, **kwargs) -> callable:
     """
     Allows you to register commands later on, by loading modules.
@@ -283,28 +317,56 @@
         cmd = cls(name, func, **kwargs)
         func.__nio_command__ = cmd
         return func
 
     return decorator
 
 
+def check(
+    function: typing.Callable[[Context], typing.Union[bool, typing.Coroutine[None, None, bool]]],
+    name: str = None,
+) -> callable:
+    """
+    Allows you to register checks in modules.
+
+    ```python
+    @niobot.command()
+    @niobot.check(my_check_func, name="My Check")
+    async def my_command(ctx: niobot.Context):
+        pass
+    ```
+
+    :param function: The function to register as a check
+    :param name: A human-readable name for the check. Defaults to function.__name__
+    :return: The decorated function.
+    """
+
+    def decorator(command_function):
+        if hasattr(command_function, "__nio_checks__"):
+            command_function.__nio_checks__[function] = name or function.__name__
+        else:
+            command_function.__nio_checks__ = {function: name or function.__name__}
+        return command_function
+
+    decorator.internal = function
+    return decorator
+
+
 def event(name: str) -> callable:
     """
     Allows you to register event listeners in modules.
 
-    :param name: the name of the event (no ``on_`` prefix)
+    :param name: the name of the event (no `on_` prefix)
     :return:
     """
+
     def decorator(func):
-        func.__nio_event__ = {
-            "function": func,
-            "name": name,
-            "_module_instance": None
-        }
+        func.__nio_event__ = {"function": func, "name": name, "_module_instance": None}
         return func
+
     return decorator
 
 
 class Module:
     __is_nio_module__ = True
 
     def __init__(self, bot: "NioBot"):
@@ -321,21 +383,22 @@
             if hasattr(potential_event, "__nio_event__"):
                 yield potential_event.__nio_event__
 
     def _event_handler_callback(self, function):
         # Due to the fact events are less stateful than commands, we need to manually inject self for events
         async def wrapper(*args, **kwargs):
             return await function(self, *args, **kwargs)
+
         return wrapper
 
     def __setup__(self):
         """Setup function called once by NioBot.mount_module(). Mounts every command discovered."""
         for cmd in self.list_commands():
             cmd.module = self
-            logging.getLogger(__name__).info("Discovered command %r in %s.", cmd, self.__class__.__name__)
+            logging.getLogger(__name__).debug("Discovered command %r in %s.", cmd, self.__class__.__name__)
             self.bot.add_command(cmd)
 
         for _event in self.list_events():
             _event["_module_instance"] = self
             self.bot.add_event_listener(_event["name"], self._event_handler_callback(_event["function"]))
 
     def __teardown__(self):
```

### Comparing `nio-bot-1.0.2/src/niobot/context.py` & `nio-bot-1.1.0a1/src/niobot/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import logging
 import time
+import typing
 
 import nio
-import typing
 
 from .utils.string_view import ArgumentView
 
 if typing.TYPE_CHECKING:
+    from .attachment import BaseAttachment
     from .client import NioBot
     from .commands import Command
-    from .attachment import BaseAttachment
 
 
-__all__ = (
-    "Context",
-    "ContextualResponse"
-)
+__all__ = ("Context", "ContextualResponse")
 
 logger = logging.getLogger(__name__)
 
 
 class ContextualResponse:
     """Context class for managing replies.
 
     Usage of this function is not required, however it is a useful utility."""
+
     def __init__(self, ctx: "Context", response: nio.RoomSendResponse):
         self.ctx = ctx
         self._response = response
 
     def __repr__(self):
         return "<ContextualResponse ctx={0.ctx!r} response={0.response!r}>".format(self)
 
@@ -58,124 +56,106 @@
         """
         Edits the current response.
 
         :param content: The new content to edit with
         :param kwargs: Any extra arguments to pass to Client.edit_message
         :return: self
         """
-        await self.ctx.client.edit_message(
-            self.ctx.room,
-            self._response.event_id,
-            content,
-            **kwargs
-        )
+        await self.ctx.client.edit_message(self.ctx.room, self._response.event_id, content, **kwargs)
         return self
 
     async def delete(self, reason: str = None) -> None:
         """
         Redacts the current response.
 
         :param reason: An optional reason for the redaction
         :return: None, as there will be no more response.
         """
-        await self.ctx.client.delete_message(
-            self.ctx.room,
-            self._response.event_id,
-            reason=reason
-        )
+        await self.ctx.client.delete_message(self.ctx.room, self._response.event_id, reason=reason)
 
 
 class Context:
     """Event-based context for a command callback"""
+
     def __init__(
-            self,
-            _client: "NioBot",
-            room: nio.MatrixRoom,
-            event: nio.RoomMessageText,
-            command: "Command",
-            *,
-            invoking_string: str = None
+        self,
+        _client: "NioBot",
+        room: nio.MatrixRoom,
+        event: nio.RoomMessageText,
+        command: "Command",
+        *,
+        invoking_string: str = None,
     ):
         self._init_ts = time.time()
         self._client = _client
         self._room = room
         self._event = event
         self._command = command
         self._invoking_string = invoking_string
         to_parse = event.body
         if invoking_string:
             try:
-                to_parse = event.body[len(invoking_string):]
+                to_parse = event.body[len(invoking_string) :]
             except IndexError:
                 to_parse = ""
         self._args = ArgumentView(to_parse)
         self._args.parse_arguments()
         self._original_response = None
 
+        # property aliases
+        self.bot = self.client
+        self.msg = self.event = self.message
+        self.arguments = self.args
+
     def __repr__(self):
         return "<Context room={0.room!r} event={0.event!r} command={0.command!r}>".format(self)
 
     def __eq__(self, other):
         if not isinstance(other, Context):
             return False
-        return (
-            self.room == other.room and
-            self.event == other.event and
-            self.command == other.command
-        )
+        return self.room == other.room and self.event == other.event and self.command == other.command
 
     @property
     def room(self) -> nio.MatrixRoom:
         """The room that the event was dispatched in"""
         return self._room
 
     @property
     def client(self) -> "NioBot":
         """The current instance of the client"""
         return self._client
 
-    bot = client
-
     @property
     def command(self) -> "Command":
         """The current command being invoked"""
         return self._command
 
     @property
     def args(self) -> list[str]:
         """Each argument given to this command"""
         return self._args.arguments
 
-    arguments = args
-
     @property
     def message(self) -> nio.RoomMessageText:
         """The current message"""
         return self._event
 
     @property
     def original_response(self) -> typing.Optional[nio.RoomSendResponse]:
         """The result of Context.reply(), if it exists."""
         return self._original_response
 
-    msg = event = message
-
     @property
     def latency(self) -> float:
         """Returns the current event's latency in milliseconds."""
         return self.client.latency(self.event, received_at=self._init_ts)
 
     async def respond(self, content: str = None, file: "BaseAttachment" = None) -> ContextualResponse:
         """
         Responds to the current event.
 
         :param content: The text to reply with
         :param file: A file to reply with
         :return:
         """
-        result = await self.client.send_message(
-            self.room,
-            content,
-            file,
-            self.message
-        )
+        result = await self.client.send_message(self.room, content, file, self.message)
         return ContextualResponse(self, result)
```

### Comparing `nio-bot-1.0.2/src/niobot/utils/__init__.py` & `nio-bot-1.1.0a1/src/niobot/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from .typing import *
-from .string_view import *
-from .unblocking import *
+from .checks import *
+from .federation import *
 from .help_command import *
 from .parsers import *
-from .federation import *
+from .string_view import *
+from .typing import *
+from .unblocking import *
 
 
 def deprecated(use_instead: str = None):
     """Marks a function as deprecated and will warn users on call."""
-    import warnings
     import functools
+    import warnings
 
     def wrapper(func):
         @functools.wraps(func)
         def caller(*args, **kwargs):
             value = "{} is deprecated.{}".format(
-                func.__qualname__,
-                '' if not use_instead else ' Please use %r instead.' % use_instead
+                func.__qualname__, "" if not use_instead else " Please use %r instead." % use_instead
             )
             warn = DeprecationWarning(value)
             warnings.warn(warn)
             return func(*args, **kwargs)
+
         caller.__doc__ = func.__doc__
         return caller
+
     return wrapper
```

### Comparing `nio-bot-1.0.2/src/niobot/utils/federation.py` & `nio-bot-1.1.0a1/src/niobot/utils/federation.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
-
-import aiohttp
 from urllib.parse import urlparse
 
+import aiohttp
 
 __all__ = ["resolve_homeserver"]
 
 
 async def resolve_homeserver(domain: str) -> str:
     """
     Resolves a given homeserver part to the actual homeserver
 
     :param domain: The domain to crawl
     :return: The resolved homeserver
     """
     from niobot import __user_agent__
+
     if not domain.startswith("https://"):
         domain = f"https://{domain}"
     domain = urlparse(domain).netloc
     async with aiohttp.ClientSession(headers={"User-Agent": __user_agent__}) as session:
         async with session.get(f"https://{domain}/.well-known/matrix/client") as resp:
             if resp.status == 200:
                 if resp.content_type != "application/json":
```

### Comparing `nio-bot-1.0.2/src/niobot/utils/help_command.py` & `nio-bot-1.1.0a1/src/niobot/utils/help_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
+import re
 import textwrap
 import typing
-import re
+import warnings
 
 if typing.TYPE_CHECKING:
-    from ..context import Context
     from ..commands import Command
+    from ..context import Context
 
 
 __all__ = (
     "format_command_name",
     "format_command_line",
     "get_short_description",
     "get_long_description",
     "help_command_callback",
-    "clean_output"
+    "default_help_command",
+    "clean_output",
 )
 
 
 def clean_output(
-        text: str,
-        *,
-        escape_user_mentions: bool = True,
-        escape_room_mentions: bool = True,
-        escape_room_references: bool = False,
-        escape_all_periods: bool = False,
-        escape_all_at_signs: bool = False,
-        escape_method: typing.Callable[[str], str] = None
+    text: str,
+    *,
+    escape_user_mentions: bool = True,
+    escape_room_mentions: bool = True,
+    escape_room_references: bool = False,
+    escape_all_periods: bool = False,
+    escape_all_at_signs: bool = False,
+    escape_method: typing.Callable[[str], str] = None,
 ) -> str:
     """
     Escapes given text and sanitises it, ready for outputting to the user.
 
     This should always be used when echoing any sort of user-provided content, as we all know there will be some
     annoying troll who will just go `@room` for no apparent reason every 30 seconds.
 
@@ -44,14 +46,15 @@
     :param escape_all_periods: Escape all literal `.` characters (can be used to escape all links)
     :param escape_all_at_signs: Escape all literal `@` characters (can be used to escape all mentions)
     :param escape_method: A custom escape method to use instead of the built-in one
     (which just wraps characters in `\\u200b`)
     :return: The cleaned text
     """
     if escape_method is None:
+
         def escape_method(x: str) -> str:
             return "\u200b".join(x.split())
 
     if escape_user_mentions:
         text = re.sub(r"@([A-Za-z0-9\-_=+./]+):([A-Za-z0-9\-_=+./]+)", escape_method("@\\1:\\2"), text)
     if escape_room_mentions:
         text = text.replace("@room", escape_method("@room"))
@@ -66,17 +69,15 @@
 
 
 def format_command_name(command: "Command") -> str:
     """Formats the command name with its aliases if applicable"""
     if not command.aliases:
         return command.name
     else:
-        return "[{}]".format(
-            "|".join([command.name, *command.aliases])
-        )
+        return "[{}]".format("|".join([command.name, *command.aliases]))
 
 
 def format_command_line(prefix: str, command: "Command") -> str:
     """Formats a command line, including name(s) & usage."""
     name = format_command_name(command)
     start = "{}{}".format(prefix, name)
     start += " " + command.display_usage.strip().replace("\n", "")
@@ -105,20 +106,18 @@
     """Gets the full help text for a command."""
     if not command.description:
         # Get the docstring of the callback
         description = command.callback.__doc__ or "No command description."
     else:
         description = command.description
 
-    return "\n".join(
-        "> " + x for x in description.splitlines()
-    )
+    return "\n".join("> " + x for x in description.splitlines())
 
 
-async def help_command_callback(ctx: "Context"):
+async def default_help_command(ctx: "Context"):
     """Displays help text"""
     lines = []
     if not ctx.args:
         added = []
         # Display global help.
         # noinspection PyProtectedMember
         for command in ctx.client._commands.values():
@@ -132,12 +131,18 @@
     else:
         command = ctx.client.get_command(ctx.args[0])
         if not command:
             return await ctx.respond("No command with that name found!")
 
         display = format_command_line(ctx.client.command_prefix, command)
         description = get_long_description(command)
-        lines = [
-            "* {}:".format(display),
-            *description.splitlines()
-        ]
+        lines = ["* {}:".format(display), *description.splitlines()]
         await ctx.respond(clean_output("\n".join(lines)))
+
+
+def help_command_callback(ctx: "Context"):
+    """Default help command callback"""
+    warnings.warn(
+        "help_command_callback is deprecated and will be removed in v1.2.0, please use default_help_command instead",
+        DeprecationWarning,
+    )
+    return default_help_command(ctx)
```

### Comparing `nio-bot-1.0.2/src/niobot/utils/string_view.py` & `nio-bot-1.1.0a1/src/niobot/utils/string_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import logging
+
 # Inspiration from https://github.com/Pycord-Development/pycord/blob/36fea3/discord/ext/commands/view.py#L55
 
-__all__ = (
-    "QUOTES",
-    "ArgumentView"
-)
+__all__ = ("QUOTES", "ArgumentView")
 
-QUOTES = ['"', "'", '`']
+QUOTES = ['"', "'", "`"]
 
 log = logging.getLogger(__name__)
 
 
 class ArgumentView:
     """A parser designed to allow for multi-word arguments and quotes
 
     For example, the arguments `1 "2 3" 4` would result in three items in the internal list:
     `1`, `2 3`, and `4`
 
     This is most useful when parsing arguments from a command, as it allows for multi-word arguments.
 
     :param string: The string to parse
     """
+
     def __init__(self, string: str):
         self.source = string
         self.index = 0
 
         self.arguments = []
 
     def add_arg(self, argument: str) -> None:
         """Adds an argument to the argument list
 
         :param argument: The argument to add
         :return: none"""
         if not argument:
-            log.warning("Blank argument added to ArgumentView (FIXME)")
             return
         self.arguments.append(argument)
 
     @property
     def eof(self) -> bool:
         """Returns whether the parser has reached the end of the string
```

### Comparing `nio-bot-1.0.2/src/niobot/utils/typing.py` & `nio-bot-1.1.0a1/src/niobot/utils/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import asyncio
 import typing
 
 if typing.TYPE_CHECKING:
     from ..client import NioBot
 
 
-__all__ = (
-    "Typing",
-)
+__all__ = ("Typing",)
 
 
 class Typing:
     """
     Context manager to manage typing notifications.
 
     :param client: The `NioBot` instance
     :param room_id: The room id to send the typing notification to
     :param timeout: The timeout in seconds
     :param persistent: Whether to send a typing notification every `timeout` seconds, to keep the typing status active
     """
+
     def __init__(self, client: "NioBot", room_id: str, *, timeout: int = 30, persistent: bool = True):
         self.room_id = room_id
         self.client = client
         self.persistent = persistent
         self._task = None
         self.timeout = timeout * 1000
```

### Comparing `nio-bot-1.0.2/src/niobot/utils/unblocking.py` & `nio-bot-1.1.0a1/src/niobot/utils/unblocking.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import asyncio
-import typing
 import functools
+import typing
 from typing import Any
 
-
 __all__ = ("run_blocking", "force_await")
 
 
 async def run_blocking(function: typing.Callable, *args: Any, **kwargs: Any) -> Any:
     """
     Takes a blocking function and runs it in a thread, returning the result.
 
     You should use this for any long-running functions that may take a long time to respond that are not coroutines
     that you can await. For example, running a subprocess.
 
-    ??? note "Example"
+    ??? example
         ```py
         import asyncio
         import subprocess
         from niobot.utils import run_blocking
 
         async def main():
             result = await run_blocking(subprocess.run, ["find", "*.py", "-type", "f"], capture_output=True)
@@ -51,11 +50,13 @@
     ```
 
     :param function: The function to call. Make sure you do not call it, just pass it.
     :param args: The arguments to pass to the function.
     :param kwargs: The keyword arguments to pass to the function.
     :returns: The result of the function.
     """
-    if asyncio.iscoroutinefunction(function) or asyncio.iscoroutine(function):
+    if asyncio.iscoroutinefunction(function):
         return await function(*args, **kwargs)
+    elif asyncio.iscoroutine(function):
+        return await function
     else:
         return await run_blocking(function, *args, **kwargs)
```

