# Comparing `tmp/plone.app.discussion-4.1.1.tar.gz` & `tmp/plone.app.discussion-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.discussion-4.1.1.tar", last modified: Fri Mar 22 16:02:33 2024, max compression
+gzip compressed data, was "plone.app.discussion-4.1.2.tar", last modified: Tue Apr 16 19:31:01 2024, max compression
```

## Comparing `plone.app.discussion-4.1.1.tar` & `plone.app.discussion-4.1.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:33.027575 plone.app.discussion-4.1.1/
--rw-r--r--   0 maurits    (501) staff       (20)    45612 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      122 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    49731 2024-03-22 16:02:33.026908 plone.app.discussion-4.1.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1892 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:32.975678 plone.app.discussion-4.1.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      726 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      106 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:32.978986 plone.app.discussion-4.1.1/docs/source/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:32.980327 plone.app.discussion-4.1.1/docs/source/api/
--rw-r--r--   0 maurits    (501) staff       (20)       54 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/api/comment.txt
--rw-r--r--   0 maurits    (501) staff       (20)       59 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/api/conversation.txt
--rw-r--r--   0 maurits    (501) staff       (20)      599 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/api/index.txt
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/architecture.txt
--rw-r--r--   0 maurits    (501) staff       (20)       59 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/captcha.txt
--rw-r--r--   0 maurits    (501) staff       (20)     6706 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)       50 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/design.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2148 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/email-notification.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:32.983908 plone.app.discussion-4.1.1/docs/source/howtos/
--rw-r--r--   0 maurits    (501) staff       (20)     5493 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/howtos/howto_extend_the_comment_form.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1242 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5116 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/howtos/howto_override_comments_viewlet.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2526 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/howtos/howto_override_enable_conversation.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5038 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt
--rw-r--r--   0 maurits    (501) staff       (20)      301 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/howtos/howto_write_a_custom_email_notification.txt
--rw-r--r--   0 maurits    (501) staff       (20)      330 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/howtos/index.txt
--rw-r--r--   0 maurits    (501) staff       (20)      629 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/index.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3670 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/docs/source/workflow.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:32.984359 plone.app.discussion-4.1.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:32.988278 plone.app.discussion-4.1.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:32.999091 plone.app.discussion-4.1.1/plone/app/discussion/
--rw-r--r--   0 maurits    (501) staff       (20)     3064 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)       76 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2563 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/architecture.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:33.006617 plone.app.discussion-4.1.1/plone/app/discussion/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2792 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/captcha.py
--rw-r--r--   0 maurits    (501) staff       (20)     3641 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/captcha.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1216 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/captcha.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4035 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/comment.py
--rw-r--r--   0 maurits    (501) staff       (20)    11136 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/comments.pt
--rw-r--r--   0 maurits    (501) staff       (20)    21413 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/comments.py
--rw-r--r--   0 maurits    (501) staff       (20)     4789 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      892 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9711 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     2407 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/conversation.py
--rw-r--r--   0 maurits    (501) staff       (20)    15354 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/moderation.pt
--rw-r--r--   0 maurits    (501) staff       (20)    15100 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/moderation.py
--rw-r--r--   0 maurits    (501) staff       (20)     1421 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)     2112 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/browser/validator.py
--rw-r--r--   0 maurits    (501) staff       (20)     3787 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)    15443 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/comment.py
--rw-r--r--   0 maurits    (501) staff       (20)      394 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/comment.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4389 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2311 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/contentrules.py
--rw-r--r--   0 maurits    (501) staff       (20)     3554 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/contentrules.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    13846 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/conversation.py
--rw-r--r--   0 maurits    (501) staff       (20)      192 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/conversation.txt
--rw-r--r--   0 maurits    (501) staff       (20)     6887 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/design.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2453 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/events.py
--rw-r--r--   0 maurits    (501) staff       (20)    14014 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      501 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/notifications.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      651 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:32.969723 plone.app.discussion-4.1.1/plone/app/discussion/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:33.011289 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)     1002 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      170 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      504 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      621 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      247 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1104 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/portal_atct.xml
--rw-r--r--   0 maurits    (501) staff       (20)      261 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1189 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:33.011757 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1182 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/types/Discussion_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)      205 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:32.970686 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/workflows/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:33.012243 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     3068 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:33.012728 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/workflows/comment_review_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     7060 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml
--rw-r--r--   0 maurits    (501) staff       (20)      421 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/workflows.xml
--rw-r--r--   0 maurits    (501) staff       (20)      255 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)     2534 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/subscribers.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4037 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:33.022657 plone.app.discussion-4.1.1/plone/app/discussion/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3965 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/collection-integration-test.txt
--rw-r--r--   0 maurits    (501) staff       (20)     8931 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/functional_test_comment_review_workflow.txt
--rw-r--r--   0 maurits    (501) staff       (20)    17844 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/functional_test_comments.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:33.023673 plone.app.discussion-4.1.1/plone/app/discussion/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     2490 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/robot/test_discussion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2933 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/robot/test_moderation.robot
--rw-r--r--   0 maurits    (501) staff       (20)    20482 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)    19247 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_comment.py
--rw-r--r--   0 maurits    (501) staff       (20)    28444 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_comments_viewlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     5457 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_contentrules.py
--rw-r--r--   0 maurits    (501) staff       (20)     8117 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)    34617 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_conversation.py
--rw-r--r--   0 maurits    (501) staff       (20)     7051 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_events.py
--rw-r--r--   0 maurits    (501) staff       (20)      986 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     8559 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_indexers.py
--rw-r--r--   0 maurits    (501) staff       (20)     4544 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_moderation_multiple_state_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     7620 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_moderation_view.py
--rw-r--r--   0 maurits    (501) staff       (20)    12004 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_notifications.py
--rw-r--r--   0 maurits    (501) staff       (20)      879 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)    12734 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tests/test_workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)     2598 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/tool.py
--rw-r--r--   0 maurits    (501) staff       (20)     4400 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     3685 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/upgrades.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2425 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/plone/app/discussion/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-22 16:02:33.024268 plone.app.discussion-4.1.1/plone.app.discussion.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    49731 2024-03-22 16:02:32.000000 plone.app.discussion-4.1.1/plone.app.discussion.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4341 2024-03-22 16:02:32.000000 plone.app.discussion-4.1.1/plone.app.discussion.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-22 16:02:32.000000 plone.app.discussion-4.1.1/plone.app.discussion.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-03-22 16:02:32.000000 plone.app.discussion-4.1.1/plone.app.discussion.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-22 16:02:32.000000 plone.app.discussion-4.1.1/plone.app.discussion.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      535 2024-03-22 16:02:32.000000 plone.app.discussion-4.1.1/plone.app.discussion.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-03-22 16:02:32.000000 plone.app.discussion-4.1.1/plone.app.discussion.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4493 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-03-22 16:02:33.027701 plone.app.discussion-4.1.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2455 2024-03-22 16:02:31.000000 plone.app.discussion-4.1.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.398906 plone.app.discussion-4.1.2/
+-rw-r--r--   0 maurits    (501) staff       (20)    45984 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    50103 2024-04-16 19:31:01.398466 plone.app.discussion-4.1.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1892 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.363630 plone.app.discussion-4.1.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      726 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      106 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.365851 plone.app.discussion-4.1.2/docs/source/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.367022 plone.app.discussion-4.1.2/docs/source/api/
+-rw-r--r--   0 maurits    (501) staff       (20)       54 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/api/comment.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       59 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/api/conversation.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      599 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/api/index.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/architecture.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       59 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/captcha.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6706 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)       50 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/design.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2148 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/email-notification.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.369532 plone.app.discussion-4.1.2/docs/source/howtos/
+-rw-r--r--   0 maurits    (501) staff       (20)     5493 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/howtos/howto_extend_the_comment_form.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1242 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5116 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/howtos/howto_override_comments_viewlet.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2526 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/howtos/howto_override_enable_conversation.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5038 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      301 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/howtos/howto_write_a_custom_email_notification.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      330 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/howtos/index.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      629 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/index.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3670 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/docs/source/workflow.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.369881 plone.app.discussion-4.1.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.372776 plone.app.discussion-4.1.2/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.379859 plone.app.discussion-4.1.2/plone/app/discussion/
+-rw-r--r--   0 maurits    (501) staff       (20)     3064 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       76 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2563 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/architecture.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.385070 plone.app.discussion-4.1.2/plone/app/discussion/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2792 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/captcha.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3641 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/captcha.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1216 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/captcha.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4035 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/comment.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11136 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/comments.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    21413 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/comments.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4789 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      892 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9711 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2407 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/conversation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15046 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/moderation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    14121 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/moderation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1421 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2112 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/browser/validator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3787 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15443 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/comment.py
+-rw-r--r--   0 maurits    (501) staff       (20)      394 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/comment.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4389 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2311 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/contentrules.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3554 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/contentrules.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    13846 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/conversation.py
+-rw-r--r--   0 maurits    (501) staff       (20)      192 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/conversation.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6887 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/design.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2453 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14014 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      501 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/notifications.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      651 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.359575 plone.app.discussion-4.1.2/plone/app/discussion/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.388591 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)     1002 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      170 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      504 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      621 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      247 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1104 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/portal_atct.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      261 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1189 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.388870 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     1182 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/types/Discussion_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      205 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.360241 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/workflows/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.389179 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     3068 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.389586 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/workflows/comment_review_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     7060 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      421 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/workflows.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      255 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/subscribers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2534 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/subscribers.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4037 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.395881 plone.app.discussion-4.1.2/plone/app/discussion/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3965 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/collection-integration-test.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     8931 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/functional_test_comment_review_workflow.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    17844 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/functional_test_comments.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.396474 plone.app.discussion-4.1.2/plone/app/discussion/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     2490 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/robot/test_discussion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3314 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/robot/test_moderation.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    20482 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19247 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_comment.py
+-rw-r--r--   0 maurits    (501) staff       (20)    28444 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_comments_viewlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5457 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_contentrules.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8117 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)    34617 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_conversation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7051 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_events.py
+-rw-r--r--   0 maurits    (501) staff       (20)      986 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8559 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_indexers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4544 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_moderation_multiple_state_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7620 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_moderation_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12004 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_notifications.py
+-rw-r--r--   0 maurits    (501) staff       (20)      879 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12734 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tests/test_workflow.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2598 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/tool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4400 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3685 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2425 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/plone/app/discussion/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:31:01.396820 plone.app.discussion-4.1.2/plone.app.discussion.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    50103 2024-04-16 19:31:01.000000 plone.app.discussion-4.1.2/plone.app.discussion.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4341 2024-04-16 19:31:01.000000 plone.app.discussion-4.1.2/plone.app.discussion.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:31:01.000000 plone.app.discussion-4.1.2/plone.app.discussion.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-16 19:31:01.000000 plone.app.discussion-4.1.2/plone.app.discussion.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:31:01.000000 plone.app.discussion-4.1.2/plone.app.discussion.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      535 2024-04-16 19:31:01.000000 plone.app.discussion-4.1.2/plone.app.discussion.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-16 19:31:01.000000 plone.app.discussion-4.1.2/plone.app.discussion.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4493 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-16 19:31:01.398988 plone.app.discussion-4.1.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2455 2024-04-16 19:31:00.000000 plone.app.discussion-4.1.2/setup.py
```

### Comparing `plone.app.discussion-4.1.1/CHANGES.rst` & `plone.app.discussion-4.1.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.2 (2024-04-16)
+------------------
+
+Internal:
+
+
+- Add capture screen in robot tests to debug. @wesleybl (#235)
+- Fix robot test `Add a Comment to a Document and bulk delete it`. @wesleybl (#237)
+- Fix robot test `Add a Comment to a Document and bulk delete it` 2. @wesleybl (#238)
+- Fix robot test `Add a Comment to a Document and bulk delete it` 3. @wesleybl (#239)
+
+
 4.1.1 (2024-03-22)
 ------------------
 
 Bug fixes:
 
 
 - Apply validation for all captchas. @ksuess (#234)
```

### Comparing `plone.app.discussion-4.1.1/PKG-INFO` & `plone.app.discussion-4.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.discussion
-Version: 4.1.1
+Version: 4.1.2
 Summary: Enhanced discussion support for Plone
 Home-page: https://pypi.org/project/plone.app.discussion
 Author: Timo Stollenwerk - Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone discussion
 Classifier: Development Status :: 5 - Production/Stable
@@ -125,14 +125,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.2 (2024-04-16)
+------------------
+
+Internal:
+
+
+- Add capture screen in robot tests to debug. @wesleybl (#235)
+- Fix robot test `Add a Comment to a Document and bulk delete it`. @wesleybl (#237)
+- Fix robot test `Add a Comment to a Document and bulk delete it` 2. @wesleybl (#238)
+- Fix robot test `Add a Comment to a Document and bulk delete it` 3. @wesleybl (#239)
+
+
 4.1.1 (2024-03-22)
 ------------------
 
 Bug fixes:
 
 
 - Apply validation for all captchas. @ksuess (#234)
```

### Comparing `plone.app.discussion-4.1.1/README.rst` & `plone.app.discussion-4.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/LICENSE.GPL` & `plone.app.discussion-4.1.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/LICENSE.txt` & `plone.app.discussion-4.1.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/source/api/index.txt` & `plone.app.discussion-4.1.2/docs/source/api/index.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/source/conf.py` & `plone.app.discussion-4.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/source/email-notification.txt` & `plone.app.discussion-4.1.2/docs/source/email-notification.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/source/howtos/howto_extend_the_comment_form.txt` & `plone.app.discussion-4.1.2/docs/source/howtos/howto_extend_the_comment_form.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt` & `plone.app.discussion-4.1.2/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/source/howtos/howto_override_comments_viewlet.txt` & `plone.app.discussion-4.1.2/docs/source/howtos/howto_override_comments_viewlet.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/source/howtos/howto_override_enable_conversation.txt` & `plone.app.discussion-4.1.2/docs/source/howtos/howto_override_enable_conversation.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt` & `plone.app.discussion-4.1.2/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/source/index.txt` & `plone.app.discussion-4.1.2/docs/source/index.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/docs/source/workflow.txt` & `plone.app.discussion-4.1.2/docs/source/workflow.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/TODO.txt` & `plone.app.discussion-4.1.2/plone/app/discussion/TODO.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/architecture.txt` & `plone.app.discussion-4.1.2/plone/app/discussion/architecture.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/captcha.py` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/captcha.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/captcha.txt` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/captcha.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/captcha.zcml` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/captcha.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/comment.py` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/comment.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/comments.pt` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/comments.pt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/comments.py` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/comments.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/configure.zcml` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/controlpanel.pt` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/controlpanel.py` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/conversation.py` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/conversation.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/moderation.pt` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/moderation.pt`

 * *Files 2% similar despite different names*

```diff
@@ -223,21 +223,14 @@
                                  value   item/getPath;
                                  id      string:cb_${item/id};
                                  checked item/checked|nothing;
                                  alt     string:Select ${item/Title};
                                  title   string:Select ${item/Title};
                                "
                         />
-                        <input name="selected_obj_paths:list"
-                               type="hidden"
-                               value="#"
-                               tal:attributes="
-                                 value item/getURL;
-                               "
-                        />
                       </td>
                       <td>
                         <span tal:content="python:item.author_name or item.Creator">Name</span>
                         <tal:email tal:condition="email">
                           <br />
                           <a tal:content="email"
                              tal:attributes="
```

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/moderation.py` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/moderation.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,26 +152,14 @@
 class DeleteComment(BrowserView):
     """Delete a comment from a conversation.
 
        This view is always called directly on the comment object:
 
          http://nohost/front-page/++conversation++default/1286289644723317/\
          @@moderate-delete-comment
-
-       Each table row (comment) in the moderation view contains a hidden input
-       field with the absolute URL of the content object:
-
-         <input type="hidden"
-                value="http://nohost/front-page/++conversation++default/\
-                       1286289644723317"
-                name="selected_obj_paths:list">
-
-       This absolute URL is called from a jQuery method that is bind to the
-       'delete' button of the table row. See javascripts/moderation.js for more
-       details.
     """
 
     def __call__(self):
         comment = aq_inner(self.context)
         conversation = aq_parent(comment)
         content_object = aq_parent(conversation)
         # conditional security
@@ -236,26 +224,14 @@
 class CommentTransition(BrowserView):
     r"""Publish, reject, recall a comment or mark it as spam.
 
     This view is always called directly on the comment object:
 
         http://nohost/front-page/++conversation++default/1286289644723317/\
         @@transmit-comment
-
-    Each table row (comment) in the moderation view contains a hidden input
-    field with the absolute URL of the content object:
-
-        <input type="hidden"
-            value="http://nohost/front-page/++conversation++default/\
-                1286289644723317"
-            name="selected_obj_paths:list">
-
-    This absolute URL is called from a jQuery method that is bind to the
-    'delete' button of the table row. See javascripts/moderation.js for more
-    details.
     """
 
     def __call__(self):
         """Call CommentTransition."""
         comment = aq_inner(self.context)
         content_object = aq_parent(aq_parent(comment))
         workflow_action = self.request.form.get("workflow_action", "publish")
```

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/traversal.py` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/traversal.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/browser/validator.py` & `plone.app.discussion-4.1.2/plone/app/discussion/browser/validator.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/catalog.py` & `plone.app.discussion-4.1.2/plone/app/discussion/catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/comment.py` & `plone.app.discussion-4.1.2/plone/app/discussion/comment.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/configure.zcml` & `plone.app.discussion-4.1.2/plone/app/discussion/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/contentrules.py` & `plone.app.discussion-4.1.2/plone/app/discussion/contentrules.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/contentrules.zcml` & `plone.app.discussion-4.1.2/plone/app/discussion/contentrules.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/conversation.py` & `plone.app.discussion-4.1.2/plone/app/discussion/conversation.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/design.txt` & `plone.app.discussion-4.1.2/plone/app/discussion/design.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/events.py` & `plone.app.discussion-4.1.2/plone/app/discussion/events.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/interfaces.py` & `plone.app.discussion-4.1.2/plone/app/discussion/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/permissions.zcml` & `plone.app.discussion-4.1.2/plone/app/discussion/permissions.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/actions.xml` & `plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/controlpanel.xml` & `plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/portal_atct.xml` & `plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/portal_atct.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/rolemap.xml` & `plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/types/Discussion_Item.xml` & `plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/types/Discussion_Item.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml` & `plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml` & `plone.app.discussion-4.1.2/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/subscribers.zcml` & `plone.app.discussion-4.1.2/plone/app/discussion/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/testing.py` & `plone.app.discussion-4.1.2/plone/app/discussion/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/collection-integration-test.txt` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/collection-integration-test.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/functional_test_comment_review_workflow.txt` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/functional_test_comment_review_workflow.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/functional_test_comments.txt` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/functional_test_comments.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/robot/test_discussion.robot` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/robot/test_discussion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/robot/test_moderation.robot` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/robot/test_moderation.robot`

 * *Files 8% similar despite different names*

```diff
@@ -63,18 +63,23 @@
   Click Button  Comment
 
 I add a comment and delete it
   Wait until page contains element  id=form-widgets-comment-text
   Input Text  id=form-widgets-comment-text  This is a comment
   Click Button  Comment
   Go To  ${PLONE_URL}/@@moderate-comments?review_state=all
-  Wait Until Element Is Enabled  css=option[value=delete]
+  Wait Until Element Is Visible  css=option[value=delete]
   Wait Until Keyword Succeeds  5x  1s  Select And Check  xpath://select[@name='form.select.BulkAction']  delete
+  Wait Until Element Is Visible  css=[name=check_all]
+  Wait Until Element Is Enabled  css=[name=check_all]
+  Wait Until Element Is Visible  css=[name="paths:list"]
+  Wait Until Element Is Enabled  css=[name="paths:list"]
+  Wait for Condition   return jQuery._data( jQuery('[name=check_all]')[0], "events" )?.click?.length == 2
   Select Checkbox  name=check_all
-  Sleep  1s
+  Wait Until Element Is Visible  css=[name="paths:list"]:checked
   Wait For Then Click Element  css=button[name="form.button.BulkAction"]
   Wait Until Page Does Not Contain  This is a comment
 
 workflow multiple enabled
   Go To  ${PLONE_URL}/@@content-controlpanel?type_id=Discussion%20Item&new_workflow=comment_review_workflow
   Execute Javascript  window.scroll(0, 2000)
   Click Button  Save
```

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_catalog.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_comment.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_comments_viewlet.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_comments_viewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_contentrules.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_contentrules.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_controlpanel.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_conversation.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_conversation.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_events.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_functional.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_indexers.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_moderation_multiple_state_view.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_moderation_multiple_state_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_moderation_view.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_moderation_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_notifications.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_robot.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tests/test_workflow.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/tool.py` & `plone.app.discussion-4.1.2/plone/app/discussion/tool.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/upgrades.py` & `plone.app.discussion-4.1.2/plone/app/discussion/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/upgrades.zcml` & `plone.app.discussion-4.1.2/plone/app/discussion/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone/app/discussion/vocabularies.py` & `plone.app.discussion-4.1.2/plone/app/discussion/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone.app.discussion.egg-info/PKG-INFO` & `plone.app.discussion-4.1.2/plone.app.discussion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.discussion
-Version: 4.1.1
+Version: 4.1.2
 Summary: Enhanced discussion support for Plone
 Home-page: https://pypi.org/project/plone.app.discussion
 Author: Timo Stollenwerk - Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone discussion
 Classifier: Development Status :: 5 - Production/Stable
@@ -125,14 +125,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.2 (2024-04-16)
+------------------
+
+Internal:
+
+
+- Add capture screen in robot tests to debug. @wesleybl (#235)
+- Fix robot test `Add a Comment to a Document and bulk delete it`. @wesleybl (#237)
+- Fix robot test `Add a Comment to a Document and bulk delete it` 2. @wesleybl (#238)
+- Fix robot test `Add a Comment to a Document and bulk delete it` 3. @wesleybl (#239)
+
+
 4.1.1 (2024-03-22)
 ------------------
 
 Bug fixes:
 
 
 - Apply validation for all captchas. @ksuess (#234)
```

### Comparing `plone.app.discussion-4.1.1/plone.app.discussion.egg-info/SOURCES.txt` & `plone.app.discussion-4.1.2/plone.app.discussion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/plone.app.discussion.egg-info/requires.txt` & `plone.app.discussion-4.1.2/plone.app.discussion.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/pyproject.toml` & `plone.app.discussion-4.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.1.1/setup.py` & `plone.app.discussion-4.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.1.1"
+version = "4.1.2"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
 )
 
 install_requires = [
     "BTrees",
```

