# Comparing `tmp/pipeline_ai-2.1.5.tar.gz` & `tmp/pipeline_ai-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_ai-2.1.5.tar", max compression
+gzip compressed data, was "pipeline_ai-2.1.6.tar", max compression
```

## Comparing `pipeline_ai-2.1.5.tar` & `pipeline_ai-2.1.6.tar`

### file list

```diff
@@ -1,277 +1,277 @@
--rw-r--r--   0        0        0    10176 2024-04-09 15:57:04.549531 pipeline_ai-2.1.5/LICENSE
--rw-r--r--   0        0        0     8630 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/README.md
--rw-r--r--   0        0        0      281 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/__init__.py
--rw-r--r--   0        0        0      135 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/__main__.py
--rw-r--r--   0        0        0      307 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/asyncio/__init__.py
--rw-r--r--   0        0        0      993 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/asyncio/pipelines.py
--rw-r--r--   0        0        0     2602 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/compute_requirements.py
--rw-r--r--   0        0        0     8147 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/files.py
--rw-r--r--   0        0        0     9298 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/http.py
--rw-r--r--   0        0        0     2720 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/logs.py
--rw-r--r--   0        0        0     5433 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/pipelines.py
--rw-r--r--   0        0        0     1175 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/pointers.py
--rw-r--r--   0        0        0      759 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/runs.py
--rw-r--r--   0        0        0     1346 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/schemas/__init__.py
--rw-r--r--   0        0        0      104 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/schemas/cluster.py
--rw-r--r--   0        0        0     1338 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/schemas/files.py
--rw-r--r--   0        0        0     1794 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/schemas/pagination.py
--rw-r--r--   0        0        0     3324 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/schemas/pipelines.py
--rw-r--r--   0        0        0      728 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/schemas/pointers.py
--rw-r--r--   0        0        0      107 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/schemas/registry.py
--rw-r--r--   0        0        0     7923 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/cloud/schemas/runs.py
--rw-r--r--   0        0        0     4994 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/configuration/__init__.py
--rw-r--r--   0        0        0     1500 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/console/__init__.py
--rw-r--r--   0        0        0     3454 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/console/cluster.py
--rw-r--r--   0        0        0     5805 2024-04-09 15:57:04.553531 pipeline_ai-2.1.5/pipeline/console/commands.py
--rw-r--r--   0        0        0    15539 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/console/container/__init__.py
--rw-r--r--   0        0        0     1851 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/console/logs.py
--rw-r--r--   0        0        0        0 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/console/targets/__init__.py
--rw-r--r--   0        0        0      410 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/console/targets/environments.py
--rw-r--r--   0        0        0     6412 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/console/targets/files.py
--rw-r--r--   0        0        0     5432 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/console/targets/pipelines.py
--rw-r--r--   0        0        0     6148 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/console/targets/pointers.py
--rw-r--r--   0        0        0     2608 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/console/targets/resources.py
--rw-r--r--   0        0        0     6873 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/console/targets/scaling_configs.py
--rw-r--r--   0        0        0        0 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/__init__.py
--rw-r--r--   0        0        0      464 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/docker_templates/__init__.py
--rw-r--r--   0        0        0      686 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/docker_templates/dockerfile_template.txt
--rw-r--r--   0        0        0      949 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/docker_templates/pipeline_template.py
--rw-r--r--   0        0        0      522 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/docker_templates/readme_template.md
--rw-r--r--   0        0        0       69 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/.babelrc
--rw-r--r--   0        0        0     2252 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/README.md
--rw-r--r--   0        0        0   496703 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/package-lock.json
--rw-r--r--   0        0        0     2362 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/package.json
--rw-r--r--   0        0        0      161 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/postcss.config.js
--rw-r--r--   0        0        0     5200 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/Header.tsx
--rw-r--r--   0        0        0     1953 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/DynamicFieldsForm.tsx
--rw-r--r--   0        0        0    10549 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/DynamicRunInput.tsx
--rw-r--r--   0        0        0      722 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/DynamicRunInputLabel.tsx
--rw-r--r--   0        0        0     2633 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/DynamicRunInputList.tsx
--rw-r--r--   0        0        0     2375 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelineOutputColumn.tsx
--rw-r--r--   0        0        0      603 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelinePlayColumn.tsx
--rw-r--r--   0        0        0     8302 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelinePlayWrapper.tsx
--rw-r--r--   0        0        0     3988 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelinePlaygroundForm.tsx
--rw-r--r--   0        0        0     1370 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelineRunImage.tsx
--rw-r--r--   0        0        0     5256 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelineRunOutput.tsx
--rw-r--r--   0        0        0    12147 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatApp.tsx
--rw-r--r--   0        0        0     1292 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatAppForm.tsx
--rw-r--r--   0        0        0     1839 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatAppMessages.tsx
--rw-r--r--   0        0        0     1196 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatAppSettingsDialog.tsx
--rw-r--r--   0        0        0      572 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatAvatar.tsx
--rw-r--r--   0        0        0     2441 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatBubble.tsx
--rw-r--r--   0        0        0      529 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatMarkdown.tsx
--rw-r--r--   0        0        0     1707 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatPromptExamples.tsx
--rw-r--r--   0        0        0      343 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ErrorAvatar.tsx
--rw-r--r--   0        0        0      405 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/TypingAnimation.tsx
--rw-r--r--   0        0        0      549 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Badges/ApiReferenceTag.tsx
--rw-r--r--   0        0        0      943 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Badges/Badge.tsx
--rw-r--r--   0        0        0     1051 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Badges/BadgeGroup.tsx
--rw-r--r--   0        0        0     1112 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Badges/CircleBadge.tsx
--rw-r--r--   0        0        0      674 2024-04-09 15:57:04.557531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Badges/Tag.tsx
--rw-r--r--   0        0        0    12513 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Buttons/Button.tsx
--rw-r--r--   0        0        0      297 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Buttons/ButtonToggle.tsx
--rw-r--r--   0        0        0     2218 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Buttons/CodeCopyButton.tsx
--rw-r--r--   0        0        0      878 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Buttons/RefreshButton.tsx
--rw-r--r--   0        0        0      730 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Cards/ButtonCard.tsx
--rw-r--r--   0        0        0     2263 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Cards/Card.tsx
--rw-r--r--   0        0        0     2907 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Cards/CardAccordian.tsx
--rw-r--r--   0        0        0      736 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Cards/EmptyResourceCard.tsx
--rw-r--r--   0        0        0      367 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Cards/EmptyTableResourceCard.tsx
--rw-r--r--   0        0        0     3344 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Code/Code.tsx
--rw-r--r--   0        0        0     2466 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Code/syntaxHighlighterStyleNightOwl.js
--rw-r--r--   0        0        0      636 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconAlertCircle.tsx
--rw-r--r--   0        0        0     1032 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconAlertTriangle.tsx
--rw-r--r--   0        0        0      552 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconArrowDown.tsx
--rw-r--r--   0        0        0      554 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconArrowLeft.tsx
--rw-r--r--   0        0        0      556 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconArrowRight.tsx
--rw-r--r--   0        0        0      529 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconArrowTopRight.tsx
--rw-r--r--   0        0        0      517 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconArrowUp.tsx
--rw-r--r--   0        0        0      545 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconAsterisk.tsx
--rw-r--r--   0        0        0      500 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCheckmark.tsx
--rw-r--r--   0        0        0      568 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCheckmarkCircle.tsx
--rw-r--r--   0        0        0      522 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconChevronDown.tsx
--rw-r--r--   0        0        0      574 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconClock.tsx
--rw-r--r--   0        0        0      828 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCluster.tsx
--rw-r--r--   0        0        0     1274 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCoinsHand.tsx
--rw-r--r--   0        0        0      929 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCoinsStacked.tsx
--rw-r--r--   0        0        0      799 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCompass.tsx
--rw-r--r--   0        0        0     1312 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCopy.tsx
--rw-r--r--   0        0        0      607 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCpu.tsx
--rw-r--r--   0        0        0      746 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCurrencyDollarCircle.tsx
--rw-r--r--   0        0        0      800 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconDataFlow.tsx
--rw-r--r--   0        0        0     1516 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconDiscord.tsx
--rw-r--r--   0        0        0      935 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconEdit.tsx
--rw-r--r--   0        0        0      806 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconEye.tsx
--rw-r--r--   0        0        0      950 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconEyeOff.tsx
--rw-r--r--   0        0        0      713 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconFaceContent.tsx
--rw-r--r--   0        0        0      819 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconFileSearch.tsx
--rw-r--r--   0        0        0      571 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconFileText.tsx
--rw-r--r--   0        0        0      604 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconGitBranch2.tsx
--rw-r--r--   0        0        0     1137 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconGithub.tsx
--rw-r--r--   0        0        0      689 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconGlobe.tsx
--rw-r--r--   0        0        0     1101 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconGpu.tsx
--rw-r--r--   0        0        0      611 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconHeart.tsx
--rw-r--r--   0        0        0      602 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconHelpCircle.tsx
--rw-r--r--   0        0        0      519 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconInfinity.tsx
--rw-r--r--   0        0        0      720 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconInfoCircle.tsx
--rw-r--r--   0        0        0      692 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconKey.tsx
--rw-r--r--   0        0        0      667 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconList.tsx
--rw-r--r--   0        0        0      880 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconLoading.tsx
--rw-r--r--   0        0        0     3805 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconLoading2.tsx
--rw-r--r--   0        0        0      503 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconMenu2.tsx
--rw-r--r--   0        0        0      763 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconMoon.tsx
--rw-r--r--   0        0        0     1243 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconMysticFire.tsx
--rw-r--r--   0        0        0      899 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconNodePool.tsx
--rw-r--r--   0        0        0     1619 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconPause.tsx
--rw-r--r--   0        0        0      795 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconPhone.tsx
--rw-r--r--   0        0        0      984 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconPlay.tsx
--rw-r--r--   0        0        0      526 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconPlus.tsx
--rw-r--r--   0        0        0      638 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconRefresh.tsx
--rw-r--r--   0        0        0      593 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconRepeat.tsx
--rw-r--r--   0        0        0     1058 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconScale.tsx
--rw-r--r--   0        0        0      639 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSearch.tsx
--rw-r--r--   0        0        0     1220 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSend.tsx
--rw-r--r--   0        0        0      790 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSettings4.tsx
--rw-r--r--   0        0        0      644 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconShare.tsx
--rw-r--r--   0        0        0      920 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconShieldTick.tsx
--rw-r--r--   0        0        0     1177 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSocialGithub.tsx
--rw-r--r--   0        0        0     1512 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSocialGoogle.tsx
--rw-r--r--   0        0        0      610 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSpanner.tsx
--rw-r--r--   0        0        0      788 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSpeedometer.tsx
--rw-r--r--   0        0        0      774 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSun.tsx
--rw-r--r--   0        0        0      923 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconTrash.tsx
--rw-r--r--   0        0        0      610 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconUpDownArrows.tsx
--rw-r--r--   0        0        0      765 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconUpload.tsx
--rw-r--r--   0        0        0     1336 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconWrapper.tsx
--rw-r--r--   0        0        0      596 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconX.tsx
--rw-r--r--   0        0        0      624 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconXCircle.tsx
--rw-r--r--   0        0        0      645 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconXOctagon.tsx
--rw-r--r--   0        0        0      495 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconZap.tsx
--rw-r--r--   0        0        0      157 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/types.ts
--rw-r--r--   0        0        0     1677 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/InfoBlock/InfoBlock.tsx
--rw-r--r--   0        0        0      340 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/InfoBlock/InfoBlockList.tsx
--rw-r--r--   0        0        0     1604 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Checkbox.tsx
--rw-r--r--   0        0        0     1578 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/File.tsx
--rw-r--r--   0        0        0     7782 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/FileUpload.tsx
--rw-r--r--   0        0        0      370 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/HintText.tsx
--rw-r--r--   0        0        0     4634 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Input.tsx
--rw-r--r--   0        0        0      335 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/InputErrorText.tsx
--rw-r--r--   0        0        0      214 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/InputField.tsx
--rw-r--r--   0        0        0     2149 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/InputSearch.tsx
--rw-r--r--   0        0        0     1279 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/InputWithSlider.tsx
--rw-r--r--   0        0        0      486 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Label.tsx
--rw-r--r--   0        0        0     2939 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/SearchWithResults.tsx
--rw-r--r--   0        0        0     3186 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Select.tsx
--rw-r--r--   0        0        0     1151 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Slider.tsx
--rw-r--r--   0        0        0     1689 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Switch.tsx
--rw-r--r--   0        0        0     3718 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Textarea.tsx
--rw-r--r--   0        0        0     3194 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/io/IOInputAndSlider.tsx
--rw-r--r--   0        0        0     8780 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/io/PipelineFileUpload.tsx
--rw-r--r--   0        0        0      295 2024-04-09 15:57:04.561531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Loading/Loading.tsx
--rw-r--r--   0        0        0     4132 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/AwsCloudLogo.tsx
--rw-r--r--   0        0        0     1113 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/AzureCloudLogo.tsx
--rw-r--r--   0        0        0     1887 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/CurlLogo.tsx
--rw-r--r--   0        0        0     2277 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/GoogleCloudLogo.tsx
--rw-r--r--   0        0        0     1373 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/JavascriptLogo.tsx
--rw-r--r--   0        0        0     3894 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/MysticLogo.tsx
--rw-r--r--   0        0        0     3894 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/MysticLogoWhite.tsx
--rw-r--r--   0        0        0     1524 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/PhpLogo.tsx
--rw-r--r--   0        0        0     2055 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/PythonLogo.tsx
--rw-r--r--   0        0        0      213 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/index.tsx
--rw-r--r--   0        0        0     3379 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/MarkdownComponents.tsx
--rw-r--r--   0        0        0     8094 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Notifications/Notifications.tsx
--rw-r--r--   0        0        0      137 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Separators/LineSeparator.tsx
--rw-r--r--   0        0        0      324 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Separators/LineSeparatorVertical.tsx
--rw-r--r--   0        0        0      640 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Separators/OrSeparator.tsx
--rw-r--r--   0        0        0      536 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Skeletons/BlockSkeleton.tsx
--rw-r--r--   0        0        0      452 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Skeletons/TextSkeleton.tsx
--rw-r--r--   0        0        0      749 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Skeletons/TextSkeletonList.tsx
--rw-r--r--   0        0        0      563 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Statuses/StatusCircle.tsx
--rw-r--r--   0        0        0     2487 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Tabs/Tab.tsx
--rw-r--r--   0        0        0     2973 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Tabs/TabList.tsx
--rw-r--r--   0        0        0     2518 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Tabs/TabText.tsx
--rw-r--r--   0        0        0     1993 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Tooltips/Tooltip.tsx
--rw-r--r--   0        0        0     1009 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Typography/DescriptionText.tsx
--rw-r--r--   0        0        0      438 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Typography/PageTitle.tsx
--rw-r--r--   0        0        0      617 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Typography/TitleText.tsx
--rw-r--r--   0        0        0      695 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/UserProfileBox.tsx
--rw-r--r--   0        0        0      980 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/contexts/AppProviders.tsx
--rw-r--r--   0        0        0     1263 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/contexts/BannerProvider.tsx
--rw-r--r--   0        0        0      535 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/contexts/DashboardProviders.tsx
--rw-r--r--   0        0        0      736 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/contexts/TooltipProvider.tsx
--rw-r--r--   0        0        0      772 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/hooks/use-copy-to-clipboard.ts
--rw-r--r--   0        0        0      570 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/hooks/use-get-pipeline.ts
--rw-r--r--   0        0        0      882 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/hooks/use-streaming-indexes.ts
--rw-r--r--   0        0        0      941 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/hooks/use-textarea-auto-height.ts
--rw-r--r--   0        0        0      238 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/index.html
--rw-r--r--   0        0        0      579 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/index.tsx
--rw-r--r--   0        0        0     5382 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/public/gradients/gradient-mesh-04.jpg
--rw-r--r--   0        0        0     3390 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/public/gradients/gradient-mesh-17.png
--rw-r--r--   0        0        0     4840 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/public/gradients/gradient-mesh-18.png
--rw-r--r--   0        0        0     5359 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/public/gradients/gradient-mesh-3.png
--rw-r--r--   0        0        0    26167 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/styles/global.css
--rw-r--r--   0        0        0     4682 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/types.ts
--rw-r--r--   0        0        0      423 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/arrays.ts
--rw-r--r--   0        0        0      355 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/bytes.ts
--rw-r--r--   0        0        0      979 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/class-names.ts
--rw-r--r--   0        0        0        0 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/index.ts
--rw-r--r--   0        0        0    15749 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/ioVariables.tsx
--rw-r--r--   0        0        0      713 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/objects.ts
--rw-r--r--   0        0        0      513 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/queries/get-file.ts
--rw-r--r--   0        0        0      573 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/queries/get-pipeline.ts
--rw-r--r--   0        0        0      570 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/queries/post-file.ts
--rw-r--r--   0        0        0     2141 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/queries/post-run.ts
--rw-r--r--   0        0        0     3278 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/173.bundle.js
--rw-r--r--   0        0        0     2579 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/328.bundle.js
--rw-r--r--   0        0        0     3145 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/340.bundle.js
--rw-r--r--   0        0        0     2641 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/353.bundle.js
--rw-r--r--   0        0        0     2486 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/392.bundle.js
--rw-r--r--   0        0        0     2679 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/42.bundle.js
--rw-r--r--   0        0        0     4077 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/446.bundle.js
--rw-r--r--   0        0        0     8705 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/458.bundle.js
--rw-r--r--   0        0        0     2415 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/463.bundle.js
--rw-r--r--   0        0        0    25118 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/554.bundle.js
--rw-r--r--   0        0        0     2267 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/570.bundle.js
--rw-r--r--   0        0        0     2564 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/627.bundle.js
--rw-r--r--   0        0        0     5179 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/723.bundle.js
--rw-r--r--   0        0        0     2838 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/887.bundle.js
--rw-r--r--   0        0        0     2562 2024-04-09 15:57:04.565531 pipeline_ai-2.1.5/pipeline/container/frontend/static/979.bundle.js
--rw-r--r--   0        0        0  1925411 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/frontend/static/bundle.js
--rw-r--r--   0        0        0      971 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/frontend/static/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     5382 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/frontend/static/gradients/gradient-mesh-04.jpg
--rw-r--r--   0        0        0     3390 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/frontend/static/gradients/gradient-mesh-17.png
--rw-r--r--   0        0        0     4840 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/frontend/static/gradients/gradient-mesh-18.png
--rw-r--r--   0        0        0     5359 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/frontend/static/gradients/gradient-mesh-3.png
--rw-r--r--   0        0        0      257 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/frontend/static/index.html
--rw-r--r--   0        0        0    28872 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/frontend/tailwind.config.js
--rw-r--r--   0        0        0      501 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/frontend/tsconfig.json
--rw-r--r--   0        0        0     1424 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/frontend/webpack.config.js
--rw-r--r--   0        0        0     3561 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/logging.py
--rw-r--r--   0        0        0     9514 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/manager.py
--rw-r--r--   0        0        0       70 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/pipeline.py
--rw-r--r--   0        0        0      376 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/routes/__init__.py
--rw-r--r--   0        0        0      365 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/routes/play.py
--rw-r--r--   0        0        0      409 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/routes/v4/__init__.py
--rw-r--r--   0        0        0     2690 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/routes/v4/container.py
--rw-r--r--   0        0        0     2528 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/routes/v4/files.py
--rw-r--r--   0        0        0    12580 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/routes/v4/runs.py
--rw-r--r--   0        0        0     3790 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/startup.py
--rw-r--r--   0        0        0      171 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/container/status.py
--rw-r--r--   0        0        0      632 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/exceptions/__init__.py
--rw-r--r--   0        0        0      479 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/objects/__init__.py
--rw-r--r--   0        0        0     5013 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/objects/decorators.py
--rw-r--r--   0        0        0     1528 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/objects/environment/__init__.py
--rw-r--r--   0        0        0     1374 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/objects/function.py
--rw-r--r--   0        0        0    24837 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/objects/graph.py
--rw-r--r--   0        0        0     1035 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/objects/huggingface/TransformersModelForCausalLM.py
--rw-r--r--   0        0        0        0 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/objects/huggingface/__init__.py
--rw-r--r--   0        0        0      744 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/objects/model.py
--rw-r--r--   0        0        0     1773 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/objects/pipeline.py
--rw-r--r--   0        0        0     1604 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/objects/wrappers.py
--rw-r--r--   0        0        0     1359 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/util/__init__.py
--rw-r--r--   0        0        0     1612 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/util/logging.py
--rw-r--r--   0        0        0     1875 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/util/streaming.py
--rw-r--r--   0        0        0      215 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pipeline/util/torch_utils/__init__.py
--rw-r--r--   0        0        0     1345 2024-04-09 15:57:04.577531 pipeline_ai-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     9590 1970-01-01 00:00:00.000000 pipeline_ai-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0    10176 2024-04-16 10:51:58.244017 pipeline_ai-2.1.6/LICENSE
+-rw-r--r--   0        0        0     8630 2024-04-16 10:51:58.244017 pipeline_ai-2.1.6/README.md
+-rw-r--r--   0        0        0      281 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/__init__.py
+-rw-r--r--   0        0        0      135 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/__main__.py
+-rw-r--r--   0        0        0      307 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/asyncio/__init__.py
+-rw-r--r--   0        0        0      993 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/asyncio/pipelines.py
+-rw-r--r--   0        0        0     2602 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/compute_requirements.py
+-rw-r--r--   0        0        0     8147 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/files.py
+-rw-r--r--   0        0        0     9298 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/http.py
+-rw-r--r--   0        0        0     2720 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/logs.py
+-rw-r--r--   0        0        0     5433 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/pipelines.py
+-rw-r--r--   0        0        0     1175 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/pointers.py
+-rw-r--r--   0        0        0      759 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/runs.py
+-rw-r--r--   0        0        0     1346 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/schemas/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/schemas/cluster.py
+-rw-r--r--   0        0        0     1338 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/schemas/files.py
+-rw-r--r--   0        0        0     1794 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/schemas/pagination.py
+-rw-r--r--   0        0        0     3324 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/schemas/pipelines.py
+-rw-r--r--   0        0        0      728 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/schemas/pointers.py
+-rw-r--r--   0        0        0      107 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/schemas/registry.py
+-rw-r--r--   0        0        0     7923 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/cloud/schemas/runs.py
+-rw-r--r--   0        0        0     4994 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/configuration/__init__.py
+-rw-r--r--   0        0        0     1500 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/__init__.py
+-rw-r--r--   0        0        0     3454 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/cluster.py
+-rw-r--r--   0        0        0     6099 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/commands.py
+-rw-r--r--   0        0        0    17567 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/container/__init__.py
+-rw-r--r--   0        0        0     1851 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/logs.py
+-rw-r--r--   0        0        0        0 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/targets/__init__.py
+-rw-r--r--   0        0        0      410 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/targets/environments.py
+-rw-r--r--   0        0        0     6412 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/targets/files.py
+-rw-r--r--   0        0        0     5432 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/targets/pipelines.py
+-rw-r--r--   0        0        0     6148 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/targets/pointers.py
+-rw-r--r--   0        0        0     2608 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/targets/resources.py
+-rw-r--r--   0        0        0     6873 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/console/targets/scaling_configs.py
+-rw-r--r--   0        0        0        0 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/container/__init__.py
+-rw-r--r--   0        0        0      464 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/container/docker_templates/__init__.py
+-rw-r--r--   0        0        0      686 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/container/docker_templates/dockerfile_template.txt
+-rw-r--r--   0        0        0      949 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/container/docker_templates/pipeline_template.py
+-rw-r--r--   0        0        0      522 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/container/docker_templates/readme_template.md
+-rw-r--r--   0        0        0       69 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/container/frontend/.babelrc
+-rw-r--r--   0        0        0     2252 2024-04-16 10:51:58.248017 pipeline_ai-2.1.6/pipeline/container/frontend/README.md
+-rw-r--r--   0        0        0   496703 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/package-lock.json
+-rw-r--r--   0        0        0     2362 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/package.json
+-rw-r--r--   0        0        0      161 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/postcss.config.js
+-rw-r--r--   0        0        0     5200 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/Header.tsx
+-rw-r--r--   0        0        0     1953 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/DynamicFieldsForm.tsx
+-rw-r--r--   0        0        0    10549 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/DynamicRunInput.tsx
+-rw-r--r--   0        0        0      722 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/DynamicRunInputLabel.tsx
+-rw-r--r--   0        0        0     2633 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/DynamicRunInputList.tsx
+-rw-r--r--   0        0        0     2375 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelineOutputColumn.tsx
+-rw-r--r--   0        0        0      603 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelinePlayColumn.tsx
+-rw-r--r--   0        0        0     8302 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelinePlayWrapper.tsx
+-rw-r--r--   0        0        0     3988 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelinePlaygroundForm.tsx
+-rw-r--r--   0        0        0     1370 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelineRunImage.tsx
+-rw-r--r--   0        0        0     5256 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelineRunOutput.tsx
+-rw-r--r--   0        0        0    12147 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatApp.tsx
+-rw-r--r--   0        0        0     1292 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatAppForm.tsx
+-rw-r--r--   0        0        0     1839 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatAppMessages.tsx
+-rw-r--r--   0        0        0     1196 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatAppSettingsDialog.tsx
+-rw-r--r--   0        0        0      572 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatAvatar.tsx
+-rw-r--r--   0        0        0     2441 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatBubble.tsx
+-rw-r--r--   0        0        0      529 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatMarkdown.tsx
+-rw-r--r--   0        0        0     1707 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatPromptExamples.tsx
+-rw-r--r--   0        0        0      343 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ErrorAvatar.tsx
+-rw-r--r--   0        0        0      405 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/TypingAnimation.tsx
+-rw-r--r--   0        0        0      549 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Badges/ApiReferenceTag.tsx
+-rw-r--r--   0        0        0      943 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Badges/Badge.tsx
+-rw-r--r--   0        0        0     1051 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Badges/BadgeGroup.tsx
+-rw-r--r--   0        0        0     1112 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Badges/CircleBadge.tsx
+-rw-r--r--   0        0        0      674 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Badges/Tag.tsx
+-rw-r--r--   0        0        0    12513 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Buttons/Button.tsx
+-rw-r--r--   0        0        0      297 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Buttons/ButtonToggle.tsx
+-rw-r--r--   0        0        0     2218 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Buttons/CodeCopyButton.tsx
+-rw-r--r--   0        0        0      878 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Buttons/RefreshButton.tsx
+-rw-r--r--   0        0        0      730 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Cards/ButtonCard.tsx
+-rw-r--r--   0        0        0     2263 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Cards/Card.tsx
+-rw-r--r--   0        0        0     2907 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Cards/CardAccordian.tsx
+-rw-r--r--   0        0        0      736 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Cards/EmptyResourceCard.tsx
+-rw-r--r--   0        0        0      367 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Cards/EmptyTableResourceCard.tsx
+-rw-r--r--   0        0        0     3344 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Code/Code.tsx
+-rw-r--r--   0        0        0     2466 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Code/syntaxHighlighterStyleNightOwl.js
+-rw-r--r--   0        0        0      636 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconAlertCircle.tsx
+-rw-r--r--   0        0        0     1032 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconAlertTriangle.tsx
+-rw-r--r--   0        0        0      552 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconArrowDown.tsx
+-rw-r--r--   0        0        0      554 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconArrowLeft.tsx
+-rw-r--r--   0        0        0      556 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconArrowRight.tsx
+-rw-r--r--   0        0        0      529 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconArrowTopRight.tsx
+-rw-r--r--   0        0        0      517 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconArrowUp.tsx
+-rw-r--r--   0        0        0      545 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconAsterisk.tsx
+-rw-r--r--   0        0        0      500 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCheckmark.tsx
+-rw-r--r--   0        0        0      568 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCheckmarkCircle.tsx
+-rw-r--r--   0        0        0      522 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconChevronDown.tsx
+-rw-r--r--   0        0        0      574 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconClock.tsx
+-rw-r--r--   0        0        0      828 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCluster.tsx
+-rw-r--r--   0        0        0     1274 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCoinsHand.tsx
+-rw-r--r--   0        0        0      929 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCoinsStacked.tsx
+-rw-r--r--   0        0        0      799 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCompass.tsx
+-rw-r--r--   0        0        0     1312 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCopy.tsx
+-rw-r--r--   0        0        0      607 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCpu.tsx
+-rw-r--r--   0        0        0      746 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCurrencyDollarCircle.tsx
+-rw-r--r--   0        0        0      800 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconDataFlow.tsx
+-rw-r--r--   0        0        0     1516 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconDiscord.tsx
+-rw-r--r--   0        0        0      935 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconEdit.tsx
+-rw-r--r--   0        0        0      806 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconEye.tsx
+-rw-r--r--   0        0        0      950 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconEyeOff.tsx
+-rw-r--r--   0        0        0      713 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconFaceContent.tsx
+-rw-r--r--   0        0        0      819 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconFileSearch.tsx
+-rw-r--r--   0        0        0      571 2024-04-16 10:51:58.252017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconFileText.tsx
+-rw-r--r--   0        0        0      604 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconGitBranch2.tsx
+-rw-r--r--   0        0        0     1137 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconGithub.tsx
+-rw-r--r--   0        0        0      689 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconGlobe.tsx
+-rw-r--r--   0        0        0     1101 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconGpu.tsx
+-rw-r--r--   0        0        0      611 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconHeart.tsx
+-rw-r--r--   0        0        0      602 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconHelpCircle.tsx
+-rw-r--r--   0        0        0      519 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconInfinity.tsx
+-rw-r--r--   0        0        0      720 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconInfoCircle.tsx
+-rw-r--r--   0        0        0      692 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconKey.tsx
+-rw-r--r--   0        0        0      667 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconList.tsx
+-rw-r--r--   0        0        0      880 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconLoading.tsx
+-rw-r--r--   0        0        0     3805 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconLoading2.tsx
+-rw-r--r--   0        0        0      503 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconMenu2.tsx
+-rw-r--r--   0        0        0      763 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconMoon.tsx
+-rw-r--r--   0        0        0     1243 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconMysticFire.tsx
+-rw-r--r--   0        0        0      899 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconNodePool.tsx
+-rw-r--r--   0        0        0     1619 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconPause.tsx
+-rw-r--r--   0        0        0      795 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconPhone.tsx
+-rw-r--r--   0        0        0      984 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconPlay.tsx
+-rw-r--r--   0        0        0      526 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconPlus.tsx
+-rw-r--r--   0        0        0      638 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconRefresh.tsx
+-rw-r--r--   0        0        0      593 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconRepeat.tsx
+-rw-r--r--   0        0        0     1058 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconScale.tsx
+-rw-r--r--   0        0        0      639 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSearch.tsx
+-rw-r--r--   0        0        0     1220 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSend.tsx
+-rw-r--r--   0        0        0      790 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSettings4.tsx
+-rw-r--r--   0        0        0      644 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconShare.tsx
+-rw-r--r--   0        0        0      920 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconShieldTick.tsx
+-rw-r--r--   0        0        0     1177 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSocialGithub.tsx
+-rw-r--r--   0        0        0     1512 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSocialGoogle.tsx
+-rw-r--r--   0        0        0      610 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSpanner.tsx
+-rw-r--r--   0        0        0      788 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSpeedometer.tsx
+-rw-r--r--   0        0        0      774 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSun.tsx
+-rw-r--r--   0        0        0      923 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconTrash.tsx
+-rw-r--r--   0        0        0      610 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconUpDownArrows.tsx
+-rw-r--r--   0        0        0      765 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconUpload.tsx
+-rw-r--r--   0        0        0     1336 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconWrapper.tsx
+-rw-r--r--   0        0        0      596 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconX.tsx
+-rw-r--r--   0        0        0      624 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconXCircle.tsx
+-rw-r--r--   0        0        0      645 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconXOctagon.tsx
+-rw-r--r--   0        0        0      495 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconZap.tsx
+-rw-r--r--   0        0        0      157 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/types.ts
+-rw-r--r--   0        0        0     1677 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/InfoBlock/InfoBlock.tsx
+-rw-r--r--   0        0        0      340 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/InfoBlock/InfoBlockList.tsx
+-rw-r--r--   0        0        0     1604 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Checkbox.tsx
+-rw-r--r--   0        0        0     1578 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/File.tsx
+-rw-r--r--   0        0        0     7782 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/FileUpload.tsx
+-rw-r--r--   0        0        0      370 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/HintText.tsx
+-rw-r--r--   0        0        0     4634 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Input.tsx
+-rw-r--r--   0        0        0      335 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/InputErrorText.tsx
+-rw-r--r--   0        0        0      214 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/InputField.tsx
+-rw-r--r--   0        0        0     2149 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/InputSearch.tsx
+-rw-r--r--   0        0        0     1279 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/InputWithSlider.tsx
+-rw-r--r--   0        0        0      486 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Label.tsx
+-rw-r--r--   0        0        0     2939 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/SearchWithResults.tsx
+-rw-r--r--   0        0        0     3186 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Select.tsx
+-rw-r--r--   0        0        0     1151 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Slider.tsx
+-rw-r--r--   0        0        0     1689 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Switch.tsx
+-rw-r--r--   0        0        0     3718 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Textarea.tsx
+-rw-r--r--   0        0        0     3194 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/io/IOInputAndSlider.tsx
+-rw-r--r--   0        0        0     8780 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/io/PipelineFileUpload.tsx
+-rw-r--r--   0        0        0      295 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Loading/Loading.tsx
+-rw-r--r--   0        0        0     4132 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/AwsCloudLogo.tsx
+-rw-r--r--   0        0        0     1113 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/AzureCloudLogo.tsx
+-rw-r--r--   0        0        0     1887 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/CurlLogo.tsx
+-rw-r--r--   0        0        0     2277 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/GoogleCloudLogo.tsx
+-rw-r--r--   0        0        0     1373 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/JavascriptLogo.tsx
+-rw-r--r--   0        0        0     3894 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/MysticLogo.tsx
+-rw-r--r--   0        0        0     3894 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/MysticLogoWhite.tsx
+-rw-r--r--   0        0        0     1524 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/PhpLogo.tsx
+-rw-r--r--   0        0        0     2055 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/PythonLogo.tsx
+-rw-r--r--   0        0        0      213 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/index.tsx
+-rw-r--r--   0        0        0     3379 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/MarkdownComponents.tsx
+-rw-r--r--   0        0        0     8094 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Notifications/Notifications.tsx
+-rw-r--r--   0        0        0      137 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Separators/LineSeparator.tsx
+-rw-r--r--   0        0        0      324 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Separators/LineSeparatorVertical.tsx
+-rw-r--r--   0        0        0      640 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Separators/OrSeparator.tsx
+-rw-r--r--   0        0        0      536 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Skeletons/BlockSkeleton.tsx
+-rw-r--r--   0        0        0      452 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Skeletons/TextSkeleton.tsx
+-rw-r--r--   0        0        0      749 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Skeletons/TextSkeletonList.tsx
+-rw-r--r--   0        0        0      563 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Statuses/StatusCircle.tsx
+-rw-r--r--   0        0        0     2487 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Tabs/Tab.tsx
+-rw-r--r--   0        0        0     2973 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Tabs/TabList.tsx
+-rw-r--r--   0        0        0     2518 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Tabs/TabText.tsx
+-rw-r--r--   0        0        0     1993 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Tooltips/Tooltip.tsx
+-rw-r--r--   0        0        0     1009 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Typography/DescriptionText.tsx
+-rw-r--r--   0        0        0      438 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Typography/PageTitle.tsx
+-rw-r--r--   0        0        0      617 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Typography/TitleText.tsx
+-rw-r--r--   0        0        0      695 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/UserProfileBox.tsx
+-rw-r--r--   0        0        0      980 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/contexts/AppProviders.tsx
+-rw-r--r--   0        0        0     1263 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/contexts/BannerProvider.tsx
+-rw-r--r--   0        0        0      535 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/contexts/DashboardProviders.tsx
+-rw-r--r--   0        0        0      736 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/contexts/TooltipProvider.tsx
+-rw-r--r--   0        0        0      772 2024-04-16 10:51:58.256017 pipeline_ai-2.1.6/pipeline/container/frontend/src/hooks/use-copy-to-clipboard.ts
+-rw-r--r--   0        0        0      570 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/hooks/use-get-pipeline.ts
+-rw-r--r--   0        0        0      882 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/hooks/use-streaming-indexes.ts
+-rw-r--r--   0        0        0      941 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/hooks/use-textarea-auto-height.ts
+-rw-r--r--   0        0        0      238 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/index.html
+-rw-r--r--   0        0        0      579 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/index.tsx
+-rw-r--r--   0        0        0     5382 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/public/gradients/gradient-mesh-04.jpg
+-rw-r--r--   0        0        0     3390 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/public/gradients/gradient-mesh-17.png
+-rw-r--r--   0        0        0     4840 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/public/gradients/gradient-mesh-18.png
+-rw-r--r--   0        0        0     5359 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/public/gradients/gradient-mesh-3.png
+-rw-r--r--   0        0        0    26167 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/styles/global.css
+-rw-r--r--   0        0        0     4682 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/types.ts
+-rw-r--r--   0        0        0      423 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/arrays.ts
+-rw-r--r--   0        0        0      355 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/bytes.ts
+-rw-r--r--   0        0        0      979 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/class-names.ts
+-rw-r--r--   0        0        0        0 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/index.ts
+-rw-r--r--   0        0        0    15749 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/ioVariables.tsx
+-rw-r--r--   0        0        0      713 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/objects.ts
+-rw-r--r--   0        0        0      513 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/queries/get-file.ts
+-rw-r--r--   0        0        0      573 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/queries/get-pipeline.ts
+-rw-r--r--   0        0        0      570 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/queries/post-file.ts
+-rw-r--r--   0        0        0     2141 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/queries/post-run.ts
+-rw-r--r--   0        0        0     3278 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/173.bundle.js
+-rw-r--r--   0        0        0     2579 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/328.bundle.js
+-rw-r--r--   0        0        0     3145 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/340.bundle.js
+-rw-r--r--   0        0        0     2641 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/353.bundle.js
+-rw-r--r--   0        0        0     2486 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/392.bundle.js
+-rw-r--r--   0        0        0     2679 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/42.bundle.js
+-rw-r--r--   0        0        0     4077 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/446.bundle.js
+-rw-r--r--   0        0        0     8705 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/458.bundle.js
+-rw-r--r--   0        0        0     2415 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/463.bundle.js
+-rw-r--r--   0        0        0    25118 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/554.bundle.js
+-rw-r--r--   0        0        0     2267 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/570.bundle.js
+-rw-r--r--   0        0        0     2564 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/627.bundle.js
+-rw-r--r--   0        0        0     5179 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/723.bundle.js
+-rw-r--r--   0        0        0     2838 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/887.bundle.js
+-rw-r--r--   0        0        0     2562 2024-04-16 10:51:58.260017 pipeline_ai-2.1.6/pipeline/container/frontend/static/979.bundle.js
+-rw-r--r--   0        0        0  1925411 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/frontend/static/bundle.js
+-rw-r--r--   0        0        0      971 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/frontend/static/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     5382 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/frontend/static/gradients/gradient-mesh-04.jpg
+-rw-r--r--   0        0        0     3390 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/frontend/static/gradients/gradient-mesh-17.png
+-rw-r--r--   0        0        0     4840 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/frontend/static/gradients/gradient-mesh-18.png
+-rw-r--r--   0        0        0     5359 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/frontend/static/gradients/gradient-mesh-3.png
+-rw-r--r--   0        0        0      257 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/frontend/static/index.html
+-rw-r--r--   0        0        0    28872 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/frontend/tailwind.config.js
+-rw-r--r--   0        0        0      501 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/frontend/tsconfig.json
+-rw-r--r--   0        0        0     1424 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/frontend/webpack.config.js
+-rw-r--r--   0        0        0     3561 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/logging.py
+-rw-r--r--   0        0        0     9514 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/manager.py
+-rw-r--r--   0        0        0       70 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/pipeline.py
+-rw-r--r--   0        0        0      376 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/routes/__init__.py
+-rw-r--r--   0        0        0      365 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/routes/play.py
+-rw-r--r--   0        0        0      409 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/routes/v4/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/routes/v4/container.py
+-rw-r--r--   0        0        0     2528 2024-04-16 10:51:58.268017 pipeline_ai-2.1.6/pipeline/container/routes/v4/files.py
+-rw-r--r--   0        0        0    12580 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/container/routes/v4/runs.py
+-rw-r--r--   0        0        0     3790 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/container/startup.py
+-rw-r--r--   0        0        0      171 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/container/status.py
+-rw-r--r--   0        0        0      632 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/exceptions/__init__.py
+-rw-r--r--   0        0        0      479 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/objects/__init__.py
+-rw-r--r--   0        0        0     5013 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/objects/decorators.py
+-rw-r--r--   0        0        0     1528 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/objects/environment/__init__.py
+-rw-r--r--   0        0        0     1374 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/objects/function.py
+-rw-r--r--   0        0        0    24837 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/objects/graph.py
+-rw-r--r--   0        0        0     1035 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/objects/huggingface/TransformersModelForCausalLM.py
+-rw-r--r--   0        0        0        0 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/objects/huggingface/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/objects/model.py
+-rw-r--r--   0        0        0     1773 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/objects/pipeline.py
+-rw-r--r--   0        0        0     1604 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/objects/wrappers.py
+-rw-r--r--   0        0        0     1359 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/util/__init__.py
+-rw-r--r--   0        0        0     1612 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/util/logging.py
+-rw-r--r--   0        0        0     1875 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/util/streaming.py
+-rw-r--r--   0        0        0      215 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pipeline/util/torch_utils/__init__.py
+-rw-r--r--   0        0        0     1346 2024-04-16 10:51:58.272017 pipeline_ai-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0     9590 1970-01-01 00:00:00.000000 pipeline_ai-2.1.6/PKG-INFO
```

### Comparing `pipeline_ai-2.1.5/LICENSE` & `pipeline_ai-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/README.md` & `pipeline_ai-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/asyncio/pipelines.py` & `pipeline_ai-2.1.6/pipeline/cloud/asyncio/pipelines.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/compute_requirements.py` & `pipeline_ai-2.1.6/pipeline/cloud/compute_requirements.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/files.py` & `pipeline_ai-2.1.6/pipeline/cloud/files.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/http.py` & `pipeline_ai-2.1.6/pipeline/cloud/http.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/logs.py` & `pipeline_ai-2.1.6/pipeline/cloud/logs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/pipelines.py` & `pipeline_ai-2.1.6/pipeline/cloud/pipelines.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/pointers.py` & `pipeline_ai-2.1.6/pipeline/cloud/pointers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/runs.py` & `pipeline_ai-2.1.6/pipeline/cloud/runs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/schemas/__init__.py` & `pipeline_ai-2.1.6/pipeline/cloud/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/schemas/files.py` & `pipeline_ai-2.1.6/pipeline/cloud/schemas/files.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/schemas/pagination.py` & `pipeline_ai-2.1.6/pipeline/cloud/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/schemas/pipelines.py` & `pipeline_ai-2.1.6/pipeline/cloud/schemas/pipelines.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/schemas/pointers.py` & `pipeline_ai-2.1.6/pipeline/cloud/schemas/pointers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/cloud/schemas/runs.py` & `pipeline_ai-2.1.6/pipeline/cloud/schemas/runs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/configuration/__init__.py` & `pipeline_ai-2.1.6/pipeline/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/console/__init__.py` & `pipeline_ai-2.1.6/pipeline/console/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/console/cluster.py` & `pipeline_ai-2.1.6/pipeline/console/cluster.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/console/commands.py` & `pipeline_ai-2.1.6/pipeline/console/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -143,14 +143,26 @@
 
     push_parser = container_sub_parser.add_parser(
         "push",
         description="Push a pipeline container.",
         help="Push a pipeline container.",
     )
     push_parser.set_defaults(func=container._push_container)
+    push_parser.add_argument(
+        "--pointer",
+        "-p",
+        action="append",
+        help="Pointer for the container.",
+    )
+    push_parser.add_argument(
+        "--pointer-overwrite",
+        "-o",
+        action="store_true",
+        help="Overwrite existing pointers.",
+    )
 
     up_parser = container_sub_parser.add_parser(
         "up",
         description="Start a pipeline container.",
         help="Start a pipeline container.",
     )
     up_parser.set_defaults(func=container._up_container)
```

### Comparing `pipeline_ai-2.1.5/pipeline/console/container/__init__.py` & `pipeline_ai-2.1.6/pipeline/console/container/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from docker.types import DeviceRequest, LogConfig
 from pydantic import BaseModel
 
 from pipeline.cloud import http
 from pipeline.cloud.compute_requirements import Accelerator
 from pipeline.cloud.schemas import cluster as cluster_schemas
 from pipeline.cloud.schemas import pipelines as pipelines_schemas
+from pipeline.cloud.schemas import pointers as pointers_schemas
 from pipeline.cloud.schemas import registry as registry_schemas
 from pipeline.container import docker_templates
 from pipeline.util.logging import _print
 
 
 class PythonRuntime(BaseModel):
     version: str
@@ -47,14 +48,72 @@
     extras: t.Dict[str, t.Any] | None
     cluster: cluster_schemas.PipelineClusterConfig | None = None
 
     class Config:
         extra = "forbid"
 
 
+def _edit_pointer(
+    existing_pointer: str,
+    pointer_or_pipeline_id: str,
+):
+    edit_schema = pointers_schemas.PointerPatch(
+        pointer_or_pipeline_id=pointer_or_pipeline_id,
+        locked=False,
+    )
+
+    result = http.patch(
+        f"/v4/pointers/{existing_pointer}",
+        json.loads(
+            edit_schema.json(),
+        ),
+    )
+
+    if result.status_code == 200:
+        pointer = pointers_schemas.PointerGet.parse_obj(result.json())
+        _print(f"Updated pointer {pointer.pointer} -> {pointer.pipeline_id}")
+    else:
+        _print(f"Failed to edit pointer {existing_pointer}", "ERROR")
+
+
+def _create_pointer(
+    new_pointer: str,
+    pointer_or_pipeline_id: str,
+    force=False,
+) -> None:
+    create_schema = pointers_schemas.PointerCreate(
+        pointer=new_pointer,
+        pointer_or_pipeline_id=pointer_or_pipeline_id,
+        locked=False,
+    )
+    result = http.post(
+        "/v4/pointers",
+        json.loads(
+            create_schema.json(),
+        ),
+        handle_error=False,
+    )
+
+    if result.status_code == 409:
+        if force:
+            _print("Pointer already exists, forcing update", "WARNING")
+            _edit_pointer(new_pointer, pointer_or_pipeline_id)
+        else:
+            _print(
+                f"Pointer {new_pointer} already exists, use --pointer-overwrite to update",  # noqa
+                "WARNING",
+            )
+        return
+    elif result.status_code == 201:
+        pointer = pointers_schemas.PointerGet.parse_obj(result.json())
+        _print(f"Created pointer {pointer.pointer} -> {pointer.pipeline_id}")
+    else:
+        raise ValueError(f"Failed to create pointer {new_pointer}\n{result.text}")
+
+
 def _up_container(namespace: Namespace):
     _print("Starting container...", "INFO")
     config_file = Path("./pipeline.yaml")
 
     if not config_file.exists():
         raise FileNotFoundError(f"Config file {config_file} not found")
 
@@ -280,14 +339,16 @@
 
     if not config_file.exists():
         raise FileNotFoundError(f"Config file {config_file} not found")
 
     config = config_file.read_text()
     pipeline_config_yaml = yaml.load(config, Loader=yaml.FullLoader)
 
+    pointers: list | None = getattr(namespace, "pointer", None)
+
     pipeline_config = PipelineConfig.parse_obj(pipeline_config_yaml)
 
     # Check for file, transform to string, and put it back in config
     if pipeline_config.readme is not None:
         if os.path.isfile(pipeline_config.readme):
             markdown_file = Path(pipeline_config.readme)
             pipeline_config.readme = markdown_file.read_text()
@@ -448,14 +509,19 @@
     )
 
     _print(
         f"Created new pipeline deployment for {new_deployment.name} -> {new_deployment.id} (image={new_deployment.image})",  # noqa
         "SUCCESS",
     )
 
+    if pointers:
+        pointer_overwrite = getattr(namespace, "pointer_overwrite", False)
+        for pointer in pointers:
+            _create_pointer(pointer, new_deployment.id, force=pointer_overwrite)
+
 
 def _init_dir(namespace: Namespace) -> None:
     _print("Initializing directory...", "INFO")
 
     pipeline_name = getattr(namespace, "name", None)
 
     if not pipeline_name:
```

### Comparing `pipeline_ai-2.1.5/pipeline/console/logs.py` & `pipeline_ai-2.1.6/pipeline/console/logs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/console/targets/files.py` & `pipeline_ai-2.1.6/pipeline/console/targets/files.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/console/targets/pipelines.py` & `pipeline_ai-2.1.6/pipeline/console/targets/pipelines.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/console/targets/pointers.py` & `pipeline_ai-2.1.6/pipeline/console/targets/pointers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/console/targets/resources.py` & `pipeline_ai-2.1.6/pipeline/console/targets/resources.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/console/targets/scaling_configs.py` & `pipeline_ai-2.1.6/pipeline/console/targets/scaling_configs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/docker_templates/dockerfile_template.txt` & `pipeline_ai-2.1.6/pipeline/container/docker_templates/dockerfile_template.txt`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/docker_templates/pipeline_template.py` & `pipeline_ai-2.1.6/pipeline/container/docker_templates/pipeline_template.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/docker_templates/readme_template.md` & `pipeline_ai-2.1.6/pipeline/container/docker_templates/readme_template.md`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/README.md` & `pipeline_ai-2.1.6/pipeline/container/frontend/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/package-lock.json` & `pipeline_ai-2.1.6/pipeline/container/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/package.json` & `pipeline_ai-2.1.6/pipeline/container/frontend/package.json`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/Header.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/Header.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/DynamicFieldsForm.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/DynamicFieldsForm.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/DynamicRunInput.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/DynamicRunInput.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/DynamicRunInputLabel.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/DynamicRunInputLabel.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/DynamicRunInputList.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/DynamicRunInputList.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelineOutputColumn.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelineOutputColumn.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelinePlayColumn.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelinePlayColumn.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelinePlayWrapper.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelinePlayWrapper.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelinePlaygroundForm.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelinePlaygroundForm.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelineRunImage.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelineRunImage.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/PipelineRunOutput.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/PipelineRunOutput.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatApp.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatApp.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatAppForm.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatAppForm.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatAppMessages.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatAppMessages.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatAppSettingsDialog.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatAppSettingsDialog.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatAvatar.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatAvatar.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatBubble.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatBubble.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatMarkdown.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatMarkdown.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/play/chat-app/ChatPromptExamples.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/play/chat-app/ChatPromptExamples.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Badges/ApiReferenceTag.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Badges/ApiReferenceTag.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Badges/Badge.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Badges/Badge.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Badges/BadgeGroup.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Badges/BadgeGroup.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Badges/CircleBadge.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Badges/CircleBadge.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Badges/Tag.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Badges/Tag.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Buttons/Button.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Buttons/Button.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Buttons/CodeCopyButton.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Buttons/CodeCopyButton.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Buttons/RefreshButton.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Buttons/RefreshButton.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Cards/ButtonCard.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Cards/ButtonCard.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Cards/Card.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Cards/Card.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Cards/CardAccordian.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Cards/CardAccordian.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Cards/EmptyResourceCard.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Cards/EmptyResourceCard.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Code/Code.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Code/Code.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Code/syntaxHighlighterStyleNightOwl.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Code/syntaxHighlighterStyleNightOwl.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconAlertCircle.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconAlertCircle.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconAlertTriangle.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconAlertTriangle.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconArrowDown.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconArrowDown.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconArrowLeft.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconArrowLeft.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconArrowRight.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconArrowRight.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconArrowTopRight.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconArrowTopRight.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconArrowUp.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconArrowUp.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconAsterisk.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconAsterisk.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCheckmarkCircle.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCheckmarkCircle.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconChevronDown.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconChevronDown.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconClock.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconClock.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCluster.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCluster.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCoinsHand.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCoinsHand.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCoinsStacked.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCoinsStacked.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCompass.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCompass.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCopy.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCopy.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCpu.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCpu.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconCurrencyDollarCircle.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconCurrencyDollarCircle.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconDataFlow.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconDataFlow.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconDiscord.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconDiscord.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconEdit.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconEdit.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconEye.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconEye.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconEyeOff.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconEyeOff.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconFaceContent.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconFaceContent.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconFileSearch.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconFileSearch.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconFileText.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconFileText.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconGitBranch2.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconGitBranch2.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconGithub.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconGithub.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconGlobe.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconGlobe.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconGpu.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconGpu.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconHeart.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconHeart.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconHelpCircle.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconHelpCircle.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconInfinity.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconInfinity.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconInfoCircle.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconInfoCircle.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconKey.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconKey.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconList.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconList.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconLoading.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconLoading.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconLoading2.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconLoading2.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconMoon.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconMoon.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconMysticFire.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconMysticFire.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconNodePool.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconNodePool.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconPause.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconPause.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconPhone.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconPhone.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconPlay.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconPlay.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconPlus.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconPlus.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconRefresh.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconRefresh.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconRepeat.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconRepeat.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconScale.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconScale.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSearch.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSearch.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSend.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSend.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSettings4.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSettings4.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconShare.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconShare.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconShieldTick.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconShieldTick.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSocialGithub.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSocialGithub.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSocialGoogle.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSocialGoogle.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSpanner.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSpanner.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSpeedometer.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSpeedometer.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconSun.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconSun.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconTrash.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconTrash.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconUpDownArrows.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconUpDownArrows.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconUpload.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconUpload.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconWrapper.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconWrapper.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconX.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconX.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconXCircle.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconXCircle.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Icons/IconXOctagon.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Icons/IconXOctagon.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/InfoBlock/InfoBlock.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/InfoBlock/InfoBlock.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Checkbox.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Checkbox.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/File.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/File.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/FileUpload.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/FileUpload.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Input.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Input.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/InputSearch.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/InputSearch.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/InputWithSlider.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/InputWithSlider.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/SearchWithResults.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/SearchWithResults.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Select.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Select.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Slider.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Slider.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Switch.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Switch.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/Textarea.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/Textarea.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/io/IOInputAndSlider.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/io/IOInputAndSlider.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Inputs/io/PipelineFileUpload.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Inputs/io/PipelineFileUpload.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/AwsCloudLogo.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/AwsCloudLogo.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/AzureCloudLogo.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/AzureCloudLogo.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/CurlLogo.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/CurlLogo.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/GoogleCloudLogo.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/GoogleCloudLogo.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/JavascriptLogo.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/JavascriptLogo.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/MysticLogo.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/MysticLogo.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/MysticLogoWhite.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/MysticLogoWhite.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/PhpLogo.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/PhpLogo.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Logos/PythonLogo.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Logos/PythonLogo.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/MarkdownComponents.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/MarkdownComponents.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Notifications/Notifications.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Notifications/Notifications.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Separators/OrSeparator.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Separators/OrSeparator.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Skeletons/BlockSkeleton.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Skeletons/BlockSkeleton.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Skeletons/TextSkeletonList.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Skeletons/TextSkeletonList.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Statuses/StatusCircle.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Statuses/StatusCircle.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Tabs/Tab.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Tabs/Tab.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Tabs/TabList.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Tabs/TabList.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Tabs/TabText.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Tabs/TabText.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Tooltips/Tooltip.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Tooltips/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Typography/DescriptionText.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Typography/DescriptionText.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/Typography/TitleText.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/Typography/TitleText.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/components/ui/UserProfileBox.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/components/ui/UserProfileBox.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/contexts/AppProviders.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/contexts/AppProviders.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/contexts/BannerProvider.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/contexts/BannerProvider.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/contexts/DashboardProviders.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/contexts/DashboardProviders.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/contexts/TooltipProvider.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/contexts/TooltipProvider.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/hooks/use-copy-to-clipboard.ts` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/hooks/use-copy-to-clipboard.ts`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/hooks/use-get-pipeline.ts` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/hooks/use-get-pipeline.ts`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/hooks/use-streaming-indexes.ts` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/hooks/use-streaming-indexes.ts`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/hooks/use-textarea-auto-height.ts` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/hooks/use-textarea-auto-height.ts`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/index.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/public/gradients/gradient-mesh-04.jpg` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/public/gradients/gradient-mesh-04.jpg`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/public/gradients/gradient-mesh-17.png` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/public/gradients/gradient-mesh-17.png`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/public/gradients/gradient-mesh-18.png` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/public/gradients/gradient-mesh-18.png`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/public/gradients/gradient-mesh-3.png` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/public/gradients/gradient-mesh-3.png`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/styles/global.css` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/styles/global.css`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/types.ts` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/types.ts`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/class-names.ts` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/class-names.ts`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/ioVariables.tsx` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/ioVariables.tsx`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/objects.ts` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/objects.ts`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/queries/get-file.ts` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/queries/get-file.ts`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/queries/get-pipeline.ts` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/queries/get-pipeline.ts`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/queries/post-file.ts` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/queries/post-file.ts`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/src/utils/queries/post-run.ts` & `pipeline_ai-2.1.6/pipeline/container/frontend/src/utils/queries/post-run.ts`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/173.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/173.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/328.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/328.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/340.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/340.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/353.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/353.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/392.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/392.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/42.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/42.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/446.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/446.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/458.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/458.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/463.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/463.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/554.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/554.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/570.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/570.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/627.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/627.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/723.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/723.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/887.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/887.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/979.bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/979.bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/bundle.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/bundle.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/bundle.js.LICENSE.txt` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/gradients/gradient-mesh-04.jpg` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/gradients/gradient-mesh-04.jpg`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/gradients/gradient-mesh-17.png` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/gradients/gradient-mesh-17.png`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/gradients/gradient-mesh-18.png` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/gradients/gradient-mesh-18.png`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/static/gradients/gradient-mesh-3.png` & `pipeline_ai-2.1.6/pipeline/container/frontend/static/gradients/gradient-mesh-3.png`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/tailwind.config.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/frontend/webpack.config.js` & `pipeline_ai-2.1.6/pipeline/container/frontend/webpack.config.js`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/logging.py` & `pipeline_ai-2.1.6/pipeline/container/logging.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/manager.py` & `pipeline_ai-2.1.6/pipeline/container/manager.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/routes/v4/container.py` & `pipeline_ai-2.1.6/pipeline/container/routes/v4/container.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/routes/v4/files.py` & `pipeline_ai-2.1.6/pipeline/container/routes/v4/files.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/routes/v4/runs.py` & `pipeline_ai-2.1.6/pipeline/container/routes/v4/runs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/container/startup.py` & `pipeline_ai-2.1.6/pipeline/container/startup.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/exceptions/__init__.py` & `pipeline_ai-2.1.6/pipeline/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/objects/decorators.py` & `pipeline_ai-2.1.6/pipeline/objects/decorators.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/objects/environment/__init__.py` & `pipeline_ai-2.1.6/pipeline/objects/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/objects/function.py` & `pipeline_ai-2.1.6/pipeline/objects/function.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/objects/graph.py` & `pipeline_ai-2.1.6/pipeline/objects/graph.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/objects/huggingface/TransformersModelForCausalLM.py` & `pipeline_ai-2.1.6/pipeline/objects/huggingface/TransformersModelForCausalLM.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/objects/model.py` & `pipeline_ai-2.1.6/pipeline/objects/model.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/objects/pipeline.py` & `pipeline_ai-2.1.6/pipeline/objects/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/objects/wrappers.py` & `pipeline_ai-2.1.6/pipeline/objects/wrappers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/util/__init__.py` & `pipeline_ai-2.1.6/pipeline/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/util/logging.py` & `pipeline_ai-2.1.6/pipeline/util/logging.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pipeline/util/streaming.py` & `pipeline_ai-2.1.6/pipeline/util/streaming.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-2.1.5/pyproject.toml` & `pipeline_ai-2.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipeline-ai"
-version = "2.1.5"
+version = "2.1.6"
 description = "Pipelines for machine learning workloads."
 authors = [
   "Paul Hetherington <ph@mystic.ai>",
   "Ross Gray <ross@mystic.ai>",
   "Yvan Buggy <yvan@mystic.ai>",
 ]
 packages = [{ include = "pipeline" }]
@@ -61,8 +61,8 @@
 [tool.isort]
 profile = "black"
 
 [tool.poetry.scripts]
 pipeline = "pipeline.console:_run"
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
+asyncio_mode = "auto"
```

### Comparing `pipeline_ai-2.1.5/PKG-INFO` & `pipeline_ai-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-ai
-Version: 2.1.5
+Version: 2.1.6
 Summary: Pipelines for machine learning workloads.
 License: Apache-2.0
 Author: Paul Hetherington
 Author-email: ph@mystic.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

