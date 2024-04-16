# Comparing `tmp/minet-1.5.1.tar.gz` & `tmp/minet-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minet-1.5.1.tar", last modified: Thu Mar 28 13:32:21 2024, max compression
+gzip compressed data, was "minet-2.0.0.tar", last modified: Tue Apr 16 08:55:39 2024, max compression
```

## Comparing `minet-1.5.1.tar` & `minet-2.0.0.tar`

### file list

```diff
@@ -1,315 +1,312 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.012588 minet-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-28 13:31:07.000000 minet-1.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-03-28 13:32:21.012588 minet-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-03-28 13:31:07.000000 minet-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.976588 minet-1.5.1/minet/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.976588 minet-1.5.1/minet/__future__/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:31:07.000000 minet-1.5.1/minet/__future__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-03-28 13:31:07.000000 minet-1.5.1/minet/__future__/threaded_child_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-28 13:31:07.000000 minet-1.5.1/minet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-28 13:31:07.000000 minet-1.5.1/minet/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.980588 minet-1.5.1/minet/browser/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-28 13:31:07.000000 minet-1.5.1/minet/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-28 13:31:07.000000 minet-1.5.1/minet/browser/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-28 13:31:07.000000 minet-1.5.1/minet/browser/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-28 13:31:07.000000 minet-1.5.1/minet/browser/plawright_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-03-28 13:31:07.000000 minet-1.5.1/minet/browser/threadsafe_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-28 13:31:07.000000 minet-1.5.1/minet/browser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.980588 minet-1.5.1/minet/buzzsumo/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 13:31:07.000000 minet-1.5.1/minet/buzzsumo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-03-28 13:31:07.000000 minet-1.5.1/minet/buzzsumo/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-28 13:31:07.000000 minet-1.5.1/minet/buzzsumo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-03-28 13:31:07.000000 minet-1.5.1/minet/buzzsumo/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.980588 minet-1.5.1/minet/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30486 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.980588 minet-1.5.1/minet/cli/buzzsumo/
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/buzzsumo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/buzzsumo/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/buzzsumo/domain_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/buzzsumo/exact_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/buzzsumo/limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/buzzsumo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.980588 minet-1.5.1/minet/cli/cookies/
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/cookies/cookies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.980588 minet-1.5.1/minet/cli/crawl/
--rw-r--r--   0 runner    (1001) docker     (127)    14843 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/crawl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/crawl/crawl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/crawl/focus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.984588 minet-1.5.1/minet/cli/crowdtangle/
--rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/crowdtangle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/crowdtangle/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/crowdtangle/lists.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/crowdtangle/posts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/crowdtangle/posts_by_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/crowdtangle/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/crowdtangle/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/crowdtangle/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.984588 minet-1.5.1/minet/cli/dump/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/dump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/dump/dump_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/dump/dump_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/dump/dump_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.984588 minet-1.5.1/minet/cli/extract/
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/extract/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.984588 minet-1.5.1/minet/cli/facebook/
--rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/facebook/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/facebook/experimental_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/facebook/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/facebook/post_authors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/facebook/post_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/facebook/posts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/facebook/url_likes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/facebook/user_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/facebook/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.984588 minet-1.5.1/minet/cli/fetch/
--rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18298 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/fetch/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.984588 minet-1.5.1/minet/cli/google/
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/google/sheets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.988588 minet-1.5.1/minet/cli/hyphe/
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/hyphe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/hyphe/crawl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/hyphe/declare.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/hyphe/destroy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/hyphe/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/hyphe/reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/hyphe/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/hyphe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.988588 minet-1.5.1/minet/cli/instagram/
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/instagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/instagram/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/instagram/hashtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/instagram/post_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/instagram/user_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/instagram/user_following.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/instagram/user_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/instagram/user_posts.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/instagram/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15677 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/loading_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.988588 minet-1.5.1/minet/cli/mediacloud/
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/mediacloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/mediacloud/medias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/mediacloud/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.988588 minet-1.5.1/minet/cli/mediacloud/topic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/mediacloud/topic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/mediacloud/topic/stories.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/mediacloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/reporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.988588 minet-1.5.1/minet/cli/scrape/
--rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/scrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/scrape/scrape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.988588 minet-1.5.1/minet/cli/telegram/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/telegram/channel_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/telegram/channel_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.988588 minet-1.5.1/minet/cli/tiktok/
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/tiktok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/tiktok/search_videos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.992588 minet-1.5.1/minet/cli/twitter/
--rw-r--r--   0 runner    (1001) docker     (127)    24913 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/attrition.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/followers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/followers_you_know.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/friends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/legacy_tweets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/list_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/list_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/retweeters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/scrape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/tweet_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/tweet_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/tweet_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/tweets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/user_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/user_tweets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/twitter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.992588 minet-1.5.1/minet/cli/url_extract/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/url_extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/url_extract/url_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.992588 minet-1.5.1/minet/cli/url_join/
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/url_join/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/url_join/url_join.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.992588 minet-1.5.1/minet/cli/url_parse/
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/url_parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/url_parse/url_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.992588 minet-1.5.1/minet/cli/user_agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/user_agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/user_agents/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/user_agents/random.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/user_agents/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.992588 minet-1.5.1/minet/cli/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/wikipedia/pageviews.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.996588 minet-1.5.1/minet/cli/youtube/
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/youtube/captions.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/youtube/channel_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/youtube/channel_videos.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/youtube/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/youtube/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/youtube/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cli/youtube/videos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-28 13:31:07.000000 minet-1.5.1/minet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-28 13:31:07.000000 minet-1.5.1/minet/cookies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.996588 minet-1.5.1/minet/crawl/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crawl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20721 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crawl/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crawl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crawl/focus.py
--rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crawl/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crawl/spiders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crawl/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crawl/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crawl/url_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:20.996588 minet-1.5.1/minet/crowdtangle/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/posts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-03-28 13:31:07.000000 minet-1.5.1/minet/crowdtangle/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-28 13:31:07.000000 minet-1.5.1/minet/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-03-28 13:31:07.000000 minet-1.5.1/minet/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-03-28 13:31:07.000000 minet-1.5.1/minet/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24355 2024-03-28 13:31:07.000000 minet-1.5.1/minet/executors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-03-28 13:31:07.000000 minet-1.5.1/minet/extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.000588 minet-1.5.1/minet/facebook/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-28 13:31:07.000000 minet-1.5.1/minet/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-28 13:31:07.000000 minet-1.5.1/minet/facebook/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-03-28 13:31:07.000000 minet-1.5.1/minet/facebook/emulated_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-28 13:31:07.000000 minet-1.5.1/minet/facebook/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-03-28 13:31:07.000000 minet-1.5.1/minet/facebook/mobile_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-28 13:31:07.000000 minet-1.5.1/minet/facebook/post_id_from_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-03-28 13:31:07.000000 minet-1.5.1/minet/facebook/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-28 13:31:07.000000 minet-1.5.1/minet/facebook/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-03-28 13:31:07.000000 minet-1.5.1/minet/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.000588 minet-1.5.1/minet/google/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-28 13:31:07.000000 minet-1.5.1/minet/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-28 13:31:07.000000 minet-1.5.1/minet/google/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-28 13:31:07.000000 minet-1.5.1/minet/google/sheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-28 13:31:07.000000 minet-1.5.1/minet/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-28 13:31:07.000000 minet-1.5.1/minet/heuristics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.000588 minet-1.5.1/minet/hyphe/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-28 13:31:07.000000 minet-1.5.1/minet/hyphe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-03-28 13:31:07.000000 minet-1.5.1/minet/hyphe/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-28 13:31:07.000000 minet-1.5.1/minet/hyphe/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-28 13:31:07.000000 minet-1.5.1/minet/hyphe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-28 13:31:07.000000 minet-1.5.1/minet/hyphe/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-28 13:31:07.000000 minet-1.5.1/minet/hyphe/spider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.000588 minet-1.5.1/minet/instagram/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-28 13:31:07.000000 minet-1.5.1/minet/instagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16806 2024-03-28 13:31:07.000000 minet-1.5.1/minet/instagram/api_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-28 13:31:07.000000 minet-1.5.1/minet/instagram/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-28 13:31:07.000000 minet-1.5.1/minet/instagram/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-03-28 13:31:07.000000 minet-1.5.1/minet/instagram/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-28 13:31:07.000000 minet-1.5.1/minet/instagram/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-28 13:31:07.000000 minet-1.5.1/minet/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.000588 minet-1.5.1/minet/mediacloud/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-28 13:31:07.000000 minet-1.5.1/minet/mediacloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-28 13:31:07.000000 minet-1.5.1/minet/mediacloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-28 13:31:07.000000 minet-1.5.1/minet/mediacloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-28 13:31:07.000000 minet-1.5.1/minet/mediacloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-28 13:31:07.000000 minet-1.5.1/minet/mediacloud/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-28 13:31:07.000000 minet-1.5.1/minet/mediacloud/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-03-28 13:31:07.000000 minet-1.5.1/minet/mediacloud/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-28 13:31:07.000000 minet-1.5.1/minet/mediacloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-28 13:31:07.000000 minet-1.5.1/minet/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-03-28 13:31:07.000000 minet-1.5.1/minet/pycurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-03-28 13:31:07.000000 minet-1.5.1/minet/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.004588 minet-1.5.1/minet/scrape/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.004588 minet-1.5.1/minet/scrape/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.004588 minet-1.5.1/minet/scrape/classes/named/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/named/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/named/canonical.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/named/europresse.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/named/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/named/metas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/named/rss.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/named/title.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/named/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/classes/named/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11035 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/soup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/std.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/straining.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-28 13:31:07.000000 minet-1.5.1/minet/scrape/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-03-28 13:31:07.000000 minet-1.5.1/minet/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-03-28 13:31:07.000000 minet-1.5.1/minet/sqlar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.008588 minet-1.5.1/minet/telegram/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-28 13:31:07.000000 minet-1.5.1/minet/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-28 13:31:07.000000 minet-1.5.1/minet/telegram/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-28 13:31:07.000000 minet-1.5.1/minet/telegram/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-03-28 13:31:07.000000 minet-1.5.1/minet/telegram/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-28 13:31:07.000000 minet-1.5.1/minet/telegram/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.008588 minet-1.5.1/minet/tiktok/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 13:31:07.000000 minet-1.5.1/minet/tiktok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-03-28 13:31:07.000000 minet-1.5.1/minet/tiktok/api_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-28 13:31:07.000000 minet-1.5.1/minet/tiktok/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-28 13:31:07.000000 minet-1.5.1/minet/tiktok/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-03-28 13:31:07.000000 minet-1.5.1/minet/tiktok/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.008588 minet-1.5.1/minet/twitter/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-28 13:31:07.000000 minet-1.5.1/minet/twitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-28 13:31:07.000000 minet-1.5.1/minet/twitter/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    36164 2024-03-28 13:31:07.000000 minet-1.5.1/minet/twitter/api_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-28 13:31:07.000000 minet-1.5.1/minet/twitter/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-03-28 13:31:07.000000 minet-1.5.1/minet/twitter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-28 13:31:07.000000 minet-1.5.1/minet/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.008588 minet-1.5.1/minet/user_agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-28 13:31:07.000000 minet-1.5.1/minet/user_agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-03-28 13:31:07.000000 minet-1.5.1/minet/user_agents/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-03-28 13:31:07.000000 minet-1.5.1/minet/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    40330 2024-03-28 13:31:07.000000 minet-1.5.1/minet/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.008588 minet-1.5.1/minet/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-28 13:31:07.000000 minet-1.5.1/minet/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-28 13:31:07.000000 minet-1.5.1/minet/wikipedia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-28 13:31:07.000000 minet-1.5.1/minet/wikipedia/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-03-28 13:31:07.000000 minet-1.5.1/minet/wikipedia/wikimedia_rest_api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.012588 minet-1.5.1/minet/youtube/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-28 13:31:07.000000 minet-1.5.1/minet/youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-03-28 13:31:07.000000 minet-1.5.1/minet/youtube/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-28 13:31:07.000000 minet-1.5.1/minet/youtube/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-28 13:31:07.000000 minet-1.5.1/minet/youtube/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-03-28 13:31:07.000000 minet-1.5.1/minet/youtube/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-03-28 13:31:07.000000 minet-1.5.1/minet/youtube/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-28 13:31:07.000000 minet-1.5.1/minet/youtube/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-28 13:31:07.000000 minet-1.5.1/minet/youtube/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:21.012588 minet-1.5.1/minet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-03-28 13:32:20.000000 minet-1.5.1/minet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-03-28 13:32:20.000000 minet-1.5.1/minet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:32:20.000000 minet-1.5.1/minet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 13:32:20.000000 minet-1.5.1/minet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-28 13:32:20.000000 minet-1.5.1/minet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 13:32:20.000000 minet-1.5.1/minet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:32:20.000000 minet-1.5.1/minet.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 13:32:21.012588 minet-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-28 13:31:07.000000 minet-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.049679 minet-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 08:54:31.000000 minet-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-16 08:55:39.049679 minet-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-04-16 08:54:31.000000 minet-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.013680 minet-2.0.0/minet/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 08:54:31.000000 minet-2.0.0/minet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 08:54:31.000000 minet-2.0.0/minet/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.013680 minet-2.0.0/minet/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-16 08:54:31.000000 minet-2.0.0/minet/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 08:54:31.000000 minet-2.0.0/minet/browser/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-16 08:54:31.000000 minet-2.0.0/minet/browser/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-16 08:54:31.000000 minet-2.0.0/minet/browser/plawright_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-16 08:54:31.000000 minet-2.0.0/minet/browser/threadsafe_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-16 08:54:31.000000 minet-2.0.0/minet/browser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.013680 minet-2.0.0/minet/buzzsumo/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-16 08:54:31.000000 minet-2.0.0/minet/buzzsumo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-16 08:54:31.000000 minet-2.0.0/minet/buzzsumo/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-16 08:54:31.000000 minet-2.0.0/minet/buzzsumo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-16 08:54:31.000000 minet-2.0.0/minet/buzzsumo/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.017680 minet-2.0.0/minet/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30498 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.017680 minet-2.0.0/minet/cli/buzzsumo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/buzzsumo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/buzzsumo/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/buzzsumo/domain_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/buzzsumo/exact_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/buzzsumo/limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/buzzsumo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.017680 minet-2.0.0/minet/cli/cookies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/cookies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/cookies/cookies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.017680 minet-2.0.0/minet/cli/crawl/
+-rw-r--r--   0 runner    (1001) docker     (127)    14843 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/crawl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/crawl/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/crawl/focus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.017680 minet-2.0.0/minet/cli/crowdtangle/
+-rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/crowdtangle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/crowdtangle/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/crowdtangle/lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/crowdtangle/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/crowdtangle/posts_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/crowdtangle/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/crowdtangle/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/crowdtangle/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.021679 minet-2.0.0/minet/cli/dump/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/dump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/dump/dump_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/dump/dump_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/dump/dump_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.021679 minet-2.0.0/minet/cli/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/extract/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.021679 minet-2.0.0/minet/cli/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/facebook/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/facebook/experimental_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/facebook/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/facebook/post_authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/facebook/post_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/facebook/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/facebook/url_likes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/facebook/user_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/facebook/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.021679 minet-2.0.0/minet/cli/fetch/
+-rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/fetch/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.021679 minet-2.0.0/minet/cli/google/
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/google/sheets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.025679 minet-2.0.0/minet/cli/hyphe/
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/hyphe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/hyphe/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/hyphe/declare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/hyphe/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/hyphe/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/hyphe/reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/hyphe/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/hyphe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.025679 minet-2.0.0/minet/cli/instagram/
+-rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/instagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/instagram/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/instagram/hashtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/instagram/post_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/instagram/user_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/instagram/user_following.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/instagram/user_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/instagram/user_posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/instagram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15677 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/loading_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.025679 minet-2.0.0/minet/cli/mediacloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/mediacloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/mediacloud/medias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/mediacloud/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.025679 minet-2.0.0/minet/cli/mediacloud/topic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/mediacloud/topic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/mediacloud/topic/stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/mediacloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/reporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.025679 minet-2.0.0/minet/cli/scrape/
+-rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/scrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/scrape/scrape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.025679 minet-2.0.0/minet/cli/telegram/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/telegram/channel_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/telegram/channel_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.025679 minet-2.0.0/minet/cli/tiktok/
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/tiktok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/tiktok/search_videos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.029679 minet-2.0.0/minet/cli/twitter/
+-rw-r--r--   0 runner    (1001) docker     (127)    24913 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/attrition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/followers_you_know.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/friends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/legacy_tweets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/list_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/list_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/retweeters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/scrape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/tweet_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/tweet_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/tweet_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/tweets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/user_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/user_tweets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/twitter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.029679 minet-2.0.0/minet/cli/url_extract/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/url_extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/url_extract/url_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.029679 minet-2.0.0/minet/cli/url_join/
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/url_join/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/url_join/url_join.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.029679 minet-2.0.0/minet/cli/url_parse/
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/url_parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/url_parse/url_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.029679 minet-2.0.0/minet/cli/user_agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/user_agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/user_agents/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/user_agents/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/user_agents/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.033679 minet-2.0.0/minet/cli/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/wikipedia/pageviews.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.033679 minet-2.0.0/minet/cli/youtube/
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/youtube/captions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/youtube/channel_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/youtube/channel_videos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/youtube/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/youtube/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/youtube/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cli/youtube/videos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-16 08:54:31.000000 minet-2.0.0/minet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-16 08:54:31.000000 minet-2.0.0/minet/cookies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.033679 minet-2.0.0/minet/crawl/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crawl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crawl/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crawl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crawl/focus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19409 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crawl/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crawl/spiders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crawl/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crawl/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crawl/url_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.037679 minet-2.0.0/minet/crowdtangle/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-16 08:54:31.000000 minet-2.0.0/minet/crowdtangle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-16 08:54:31.000000 minet-2.0.0/minet/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-16 08:54:31.000000 minet-2.0.0/minet/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-16 08:54:31.000000 minet-2.0.0/minet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-04-16 08:54:31.000000 minet-2.0.0/minet/executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-16 08:54:31.000000 minet-2.0.0/minet/extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.037679 minet-2.0.0/minet/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-16 08:54:31.000000 minet-2.0.0/minet/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-16 08:54:31.000000 minet-2.0.0/minet/facebook/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-16 08:54:31.000000 minet-2.0.0/minet/facebook/emulated_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-16 08:54:31.000000 minet-2.0.0/minet/facebook/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-04-16 08:54:31.000000 minet-2.0.0/minet/facebook/mobile_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-16 08:54:31.000000 minet-2.0.0/minet/facebook/post_id_from_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-16 08:54:31.000000 minet-2.0.0/minet/facebook/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-16 08:54:31.000000 minet-2.0.0/minet/facebook/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8754 2024-04-16 08:54:31.000000 minet-2.0.0/minet/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.037679 minet-2.0.0/minet/google/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 08:54:31.000000 minet-2.0.0/minet/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-16 08:54:31.000000 minet-2.0.0/minet/google/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-16 08:54:31.000000 minet-2.0.0/minet/google/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-16 08:54:31.000000 minet-2.0.0/minet/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-16 08:54:31.000000 minet-2.0.0/minet/heuristics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.037679 minet-2.0.0/minet/hyphe/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-16 08:54:31.000000 minet-2.0.0/minet/hyphe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-16 08:54:31.000000 minet-2.0.0/minet/hyphe/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-16 08:54:31.000000 minet-2.0.0/minet/hyphe/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-16 08:54:31.000000 minet-2.0.0/minet/hyphe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-16 08:54:31.000000 minet-2.0.0/minet/hyphe/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-16 08:54:31.000000 minet-2.0.0/minet/hyphe/spider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.037679 minet-2.0.0/minet/instagram/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 08:54:31.000000 minet-2.0.0/minet/instagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16806 2024-04-16 08:54:31.000000 minet-2.0.0/minet/instagram/api_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-16 08:54:31.000000 minet-2.0.0/minet/instagram/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-16 08:54:31.000000 minet-2.0.0/minet/instagram/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-04-16 08:54:31.000000 minet-2.0.0/minet/instagram/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 08:54:31.000000 minet-2.0.0/minet/instagram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-16 08:54:31.000000 minet-2.0.0/minet/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.041679 minet-2.0.0/minet/mediacloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 08:54:31.000000 minet-2.0.0/minet/mediacloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-16 08:54:31.000000 minet-2.0.0/minet/mediacloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-16 08:54:31.000000 minet-2.0.0/minet/mediacloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-16 08:54:31.000000 minet-2.0.0/minet/mediacloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-16 08:54:31.000000 minet-2.0.0/minet/mediacloud/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-16 08:54:31.000000 minet-2.0.0/minet/mediacloud/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-16 08:54:31.000000 minet-2.0.0/minet/mediacloud/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-16 08:54:31.000000 minet-2.0.0/minet/mediacloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-16 08:54:31.000000 minet-2.0.0/minet/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-16 08:54:31.000000 minet-2.0.0/minet/pycurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-16 08:54:31.000000 minet-2.0.0/minet/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.041679 minet-2.0.0/minet/scrape/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.041679 minet-2.0.0/minet/scrape/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.045679 minet-2.0.0/minet/scrape/classes/named/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/named/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/named/canonical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/named/europresse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/named/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/named/metas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/named/rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/named/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/named/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/classes/named/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11035 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/soup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/straining.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-16 08:54:31.000000 minet-2.0.0/minet/scrape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-16 08:54:31.000000 minet-2.0.0/minet/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-16 08:54:31.000000 minet-2.0.0/minet/sqlar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.045679 minet-2.0.0/minet/telegram/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 08:54:31.000000 minet-2.0.0/minet/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 08:54:31.000000 minet-2.0.0/minet/telegram/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-16 08:54:31.000000 minet-2.0.0/minet/telegram/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-04-16 08:54:31.000000 minet-2.0.0/minet/telegram/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-16 08:54:31.000000 minet-2.0.0/minet/telegram/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.045679 minet-2.0.0/minet/tiktok/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 08:54:31.000000 minet-2.0.0/minet/tiktok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-16 08:54:31.000000 minet-2.0.0/minet/tiktok/api_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-16 08:54:31.000000 minet-2.0.0/minet/tiktok/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-16 08:54:31.000000 minet-2.0.0/minet/tiktok/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-16 08:54:31.000000 minet-2.0.0/minet/tiktok/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.045679 minet-2.0.0/minet/twitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 08:54:31.000000 minet-2.0.0/minet/twitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-16 08:54:31.000000 minet-2.0.0/minet/twitter/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36164 2024-04-16 08:54:31.000000 minet-2.0.0/minet/twitter/api_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-16 08:54:31.000000 minet-2.0.0/minet/twitter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-16 08:54:31.000000 minet-2.0.0/minet/twitter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-16 08:54:31.000000 minet-2.0.0/minet/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.045679 minet-2.0.0/minet/user_agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-16 08:54:31.000000 minet-2.0.0/minet/user_agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-16 08:54:31.000000 minet-2.0.0/minet/user_agents/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-16 08:54:31.000000 minet-2.0.0/minet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40358 2024-04-16 08:54:31.000000 minet-2.0.0/minet/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.045679 minet-2.0.0/minet/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-16 08:54:31.000000 minet-2.0.0/minet/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-16 08:54:31.000000 minet-2.0.0/minet/wikipedia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 08:54:31.000000 minet-2.0.0/minet/wikipedia/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-16 08:54:31.000000 minet-2.0.0/minet/wikipedia/wikimedia_rest_api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.049679 minet-2.0.0/minet/youtube/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-16 08:54:31.000000 minet-2.0.0/minet/youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-04-16 08:54:31.000000 minet-2.0.0/minet/youtube/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-16 08:54:31.000000 minet-2.0.0/minet/youtube/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-16 08:54:31.000000 minet-2.0.0/minet/youtube/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-16 08:54:31.000000 minet-2.0.0/minet/youtube/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-16 08:54:31.000000 minet-2.0.0/minet/youtube/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-16 08:54:31.000000 minet-2.0.0/minet/youtube/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-16 08:54:31.000000 minet-2.0.0/minet/youtube/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:55:39.049679 minet-2.0.0/minet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-16 08:55:38.000000 minet-2.0.0/minet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-16 08:55:38.000000 minet-2.0.0/minet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:55:38.000000 minet-2.0.0/minet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 08:55:38.000000 minet-2.0.0/minet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-16 08:55:38.000000 minet-2.0.0/minet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 08:55:38.000000 minet-2.0.0/minet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:55:38.000000 minet-2.0.0/minet.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:55:39.049679 minet-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-16 08:54:31.000000 minet-2.0.0/setup.py
```

### Comparing `minet-1.5.1/LICENSE.txt` & `minet-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/PKG-INFO` & `minet-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: minet
-Version: 1.5.1
+Version: 2.0.0
 Summary: A webmining CLI tool & library for python.
 Home-page: http://github.com/medialab/minet
 Author: Guillaume Plique, Pauline Breteau, Jules Farjas, Héloïse Théro, Jean Descamps, Amélie Pellé, Laura Miguel, César Pichon, Kelly Christensen
 License: GPL-3.0
 Keywords: webmining
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: about-time<5,>=4
 Requires-Dist: beautifulsoup4<5,>=4.7.1
 Requires-Dist: browser-cookie3==0.19.1
 Requires-Dist: casanova<3,>=2.0.1
 Requires-Dist: charset-normalizer<4,>=3
 Requires-Dist: dateparser>=1.1.1
 Requires-Dist: ebbe<2,>=1.13
 Requires-Dist: json5>=0.8.5
-Requires-Dist: lxml>=4.3.0
+Requires-Dist: lxml<5.2,>=4.3.0
 Requires-Dist: nanoid<3,>=2
-Requires-Dist: playwright<1.36,>=1.35
-Requires-Dist: playwright_stealth<2,>=1
+Requires-Dist: playwright<1.44,>=1.43
+Requires-Dist: playwright_stealth<2,>=1.0.6
 Requires-Dist: pyyaml
 Requires-Dist: quenouille<2,>=1.9.1
 Requires-Dist: rich<14,>=13
 Requires-Dist: rich-argparse<2,>=1
 Requires-Dist: soupsieve<3,>=2.1
 Requires-Dist: tenacity<9,>=8
-Requires-Dist: trafilatura<1.8,>=1.7
+Requires-Dist: trafilatura<1.9,>=1.8.1
 Requires-Dist: twitwi<0.19,>=0.18.2
 Requires-Dist: ural<2,>=1.3.2
 Requires-Dist: urllib3<2,>=1.26.16
 Requires-Dist: typing_extensions>=4.3; python_version < "3.11"
 
 [![Build Status](https://github.com/medialab/minet/workflows/Tests/badge.svg)](https://github.com/medialab/minet/actions) [![DOI](https://zenodo.org/badge/169059797.svg)](https://zenodo.org/badge/latestdoi/169059797) [![download number](https://static.pepy.tech/badge/minet)](https://pepy.tech/project/minet)
```

### Comparing `minet-1.5.1/README.md` & `minet-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/browser/extensions.py` & `minet-2.0.0/minet/browser/extensions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/browser/plawright_shim.py` & `minet-2.0.0/minet/browser/plawright_shim.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 from minet.browser.utils import get_browsers_path
 
 
 def run_playwright(*args: str) -> int:
     env = get_driver_env()
     env.setdefault("PLAYWRIGHT_BROWSERS_PATH", get_browsers_path())
 
-    driver_executable = compute_driver_executable()
+    node, pw = compute_driver_executable()
+
     completed_process = subprocess.run(
-        [str(driver_executable), *args], env=env, stdout=subprocess.DEVNULL
+        [node, pw, *args], env=env, stdout=subprocess.DEVNULL
     )
 
     return completed_process.returncode
 
 
 def install_browser(name: str) -> None:
     path = join(get_browsers_path(), name + "-*")
```

### Comparing `minet-1.5.1/minet/browser/threadsafe_browser.py` & `minet-2.0.0/minet/browser/threadsafe_browser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,49 @@
-from typing import Callable, TypeVar, Awaitable, Set, Optional, Union
-from minet.types import Literal, Concatenate, ParamSpec
+from typing import (
+    Callable,
+    TypeVar,
+    Awaitable,
+    Set,
+    Optional,
+    Union,
+    Literal,
+    Container,
+)
+from minet.types import Concatenate, ParamSpec
 
 import os
 import asyncio
-import platform
 from shutil import rmtree
 from concurrent.futures import Future
 from threading import Thread, Event, Lock
-from playwright.async_api import async_playwright, Browser, BrowserContext
-
-from minet.exceptions import UnknownBrowserError
+from playwright.async_api import (
+    async_playwright,
+    Browser,
+    BrowserContext,
+    Error as PlaywrightError,
+    TimeoutError as PlaywrightTimeoutError,
+)
+from urllib3._collections import HTTPHeaderDict
+
+from minet.constants import REDIRECT_STATUSES
+from minet.exceptions import (
+    UnknownBrowserError,
+    BrowserYetUnimplementedError,
+    InvalidStatusError,
+)
+from minet.web import Response
 from minet.browser.plawright_shim import install_browser
-from minet.browser.utils import get_browsers_path, get_temp_persistent_context_path
+from minet.browser.utils import (
+    get_browsers_path,
+    get_temp_persistent_context_path,
+    convert_playwright_error,
+)
 from minet.browser.extensions import get_extension_path, ensure_extension_is_downloaded
+from minet.types import Redirection
 
-UNIX = "windows" not in platform.system().lower()
-LTE_PY37 = platform.python_version_tuple()[:2] <= ("3", "7")
 SUPPORTED_BROWSERS = ("chromium", "firefox")
 
 
 BrowserName = Literal["chromium", "firefox"]
 T = TypeVar("T")
 P = ParamSpec("P")
 BrowserOrBrowserContext = Union[Browser, BrowserContext]
@@ -62,21 +86,14 @@
         self.requires_extensions = bool(self.extensions)
         self.persistent_user_data_dir = None
         self.persistent = self.requires_extensions
 
         if self.requires_extensions and browser != "chromium":
             raise TypeError("adblock and automatic_consent only work with chromium")
 
-        # NOTE: on unix python 3.7, child watching does not
-        # work properly when asyncio is not running from the main thread
-        if UNIX and LTE_PY37:
-            from minet.__future__.threaded_child_watcher import ThreadedChildWatcher
-
-            asyncio.set_child_watcher(ThreadedChildWatcher())
-
         self.browser_name: str = browser
         self.browser: Optional[Browser] = None
         self.default_browser_context: Optional[BrowserContext] = None
         self.headless = headless
         self.width = width
         self.height = height
 
@@ -233,7 +250,86 @@
         assert target is not None
 
         future = asyncio.run_coroutine_threadsafe(
             fn(target, *args, **kwargs), self.loop
         )
 
         return self.__handle_future(future)
+
+    async def __request(
+        self,
+        context: BrowserContext,
+        url: str,
+        raise_on_statuses: Optional[Container[int]] = None,
+    ) -> Response:
+        async with await context.new_page() as page:
+            try:
+                emulated_response = await page.goto(url)
+            except (PlaywrightError, PlaywrightTimeoutError) as e:
+                error = convert_playwright_error(e)
+
+                if isinstance(error, BrowserYetUnimplementedError):
+                    raise e
+
+                raise error
+
+            assert emulated_response is not None
+
+            # Invalid status?
+            if (
+                raise_on_statuses is not None
+                and emulated_response.status in raise_on_statuses
+            ):
+                raise InvalidStatusError(emulated_response.status)
+
+            # Collection redirections
+            responses = []
+
+            current = emulated_response
+
+            while True:
+                responses.append(current)
+
+                if not current.request.redirected_from:
+                    break
+
+                current = await current.request.redirected_from.response()
+
+                assert current is not None
+
+            redirection_stack = []
+
+            for r in reversed(responses):
+                redirection_stack.append(
+                    Redirection(
+                        r.url,
+                        "hit"
+                        if r.status not in REDIRECT_STATUSES
+                        else "location-header",
+                        status=r.status,
+                    )
+                )
+
+            # Building headers
+            headers = HTTPHeaderDict()
+
+            for header in await emulated_response.headers_array():
+                headers[header["name"]] = header["value"]
+
+            # Building response
+            response = Response(
+                url,
+                redirection_stack,
+                headers,
+                emulated_response.status,
+                (await page.content()).encode(),  # NOTE: we can do better
+                known_encoding="utf-8",
+            )
+
+            return response
+
+    def request(
+        self, url: str, raise_on_statuses: Optional[Container[int]] = None
+    ) -> Response:
+        return self.run_in_default_context(
+            self.__request, url, raise_on_statuses=raise_on_statuses
+        )
```

### Comparing `minet-1.5.1/minet/browser/utils.py` & `minet-2.0.0/minet/browser/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from minet.exceptions import (
     BrowserError,
     BrowserNameNotResolvedError,
     BrowserConnectionAbortedError,
     BrowserConnectionRefusedError,
     BrowserConnectionClosedError,
     BrowserTimeoutError,
-    BrowserUnknownError,
+    BrowserYetUnimplementedError,
     BrowserSSLError,
     BrowserHTTPResponseCodeFailureError,
     BrowserConnectionTimeoutError,
     BrowserContextAlreadyClosedError,
     BrowserSocketError,
 )
 from minet.browser.constants import BROWSERS_PATH
@@ -65,15 +65,15 @@
         or "maybe frame was detached?" in lower_message
     ):
         return BrowserContextAlreadyClosedError()
 
     if "net::ERR_SOCKET_NOT_CONNECTED" in error.message:
         return BrowserSocketError()
 
-    return BrowserUnknownError()
+    return BrowserYetUnimplementedError()
 
 
 def get_browsers_path() -> str:
     return expanduser(join("~", BROWSERS_PATH))
 
 
 def get_temp_persistent_context_path() -> str:
```

### Comparing `minet-1.5.1/minet/buzzsumo/client.py` & `minet-2.0.0/minet/buzzsumo/client.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/buzzsumo/exceptions.py` & `minet-2.0.0/minet/buzzsumo/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/buzzsumo/types.py` & `minet-2.0.0/minet/buzzsumo/types.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/argparse.py` & `minet-2.0.0/minet/cli/argparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,16 +429,15 @@
         setattr(
             cli_args,
             self.dest,
             False if option_string in self.false_options else True,
         )
 
 
-class DummyCSVInput(object):
-    ...
+class DummyCSVInput(object): ...
 
 
 class SingleColumnDummyCSVInput(DummyCSVInput):
     def __init__(self, column, dest):
         self.column = column
         self.dest = dest
 
@@ -636,19 +635,21 @@
         rc_key,
         default=None,
         plural=False,
         required=False,
         **kwargs,
     ):
         if "help" in kwargs:
-            kwargs["help"] = kwargs["help"].rstrip(
-                "."
-            ) + '. Can also be configured in a .minetrc file as "%s" or read from the %s env variable.' % (
-                ".".join(rc_key),
-                rc_key_to_env_var(rc_key),
+            kwargs["help"] = (
+                kwargs["help"].rstrip(".")
+                + '. Can also be configured in a .minetrc file as "%s" or read from the %s env variable.'
+                % (
+                    ".".join(rc_key),
+                    rc_key_to_env_var(rc_key),
+                )
             )
 
         self.plural = plural
 
         if plural:
             self.list_values = []
 
@@ -824,17 +825,15 @@
 
         . Here is how to indicate that the CSV column may contain multiple
           values separated by a special character:
             $ {name} {cmd} column_name -i file.csv --explode "|"
 
         . This also works with single values:
             $ {name} {cmd} "value1,value2" --explode ","
-        """.format(
-                name=name, cmd=cmd
-            )
+        """.format(name=name, cmd=cmd)
 
     if select or variadic_input is not None:
         # TODO: actually one can use xan mini dsl here
         args.append(
             {
                 "flags": ["-s", "--select"],
                 "help": "Columns of -i/--input CSV file to include in the output (separated by `,`). Use an empty string if you don't want to keep anything: --select ''.",
```

### Comparing `minet-1.5.1/minet/cli/buzzsumo/__init__.py` & `minet-2.0.0/minet/cli/buzzsumo/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/buzzsumo/domain.py` & `minet-2.0.0/minet/cli/buzzsumo/domain.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/buzzsumo/domain_summary.py` & `minet-2.0.0/minet/cli/buzzsumo/domain_summary.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/buzzsumo/exact_url.py` & `minet-2.0.0/minet/cli/buzzsumo/exact_url.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/buzzsumo/limit.py` & `minet-2.0.0/minet/cli/buzzsumo/limit.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/buzzsumo/utils.py` & `minet-2.0.0/minet/cli/buzzsumo/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/commands.py` & `minet-2.0.0/minet/cli/commands.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/console.py` & `minet-2.0.0/minet/cli/console.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/cookies/__init__.py` & `minet-2.0.0/minet/cli/cookies/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/cookies/cookies.py` & `minet-2.0.0/minet/cli/cookies/cookies.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/crawl/__init__.py` & `minet-2.0.0/minet/cli/crawl/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/crawl/crawl.py` & `minet-2.0.0/minet/cli/crawl/crawl.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/crawl/focus.py` & `minet-2.0.0/minet/cli/crawl/focus.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/crowdtangle/__init__.py` & `minet-2.0.0/minet/cli/crowdtangle/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/crowdtangle/leaderboard.py` & `minet-2.0.0/minet/cli/crowdtangle/leaderboard.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/crowdtangle/lists.py` & `minet-2.0.0/minet/cli/crowdtangle/lists.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/crowdtangle/posts_by_id.py` & `minet-2.0.0/minet/cli/crowdtangle/posts_by_id.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/crowdtangle/search.py` & `minet-2.0.0/minet/cli/crowdtangle/search.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/crowdtangle/summary.py` & `minet-2.0.0/minet/cli/crowdtangle/summary.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/crowdtangle/utils.py` & `minet-2.0.0/minet/cli/crowdtangle/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             cli_args,
             *args,
             **{
                 "client": CrowdTangleAPIClient(
                     cli_args.token, rate_limit=cli_args.rate_limit
                 ),
                 **kwargs,
-            }
+            },
         )
 
     return wrapped
 
 
 def with_crowdtangle_utilities(fn):
     return with_crowdtangle_fatal_errors(with_crowdtangle_client(fn))
@@ -95,15 +95,15 @@
 
         iterator = create_iterator(
             *args,
             limit=cli_args.limit,
             raw=cli_args.format != "csv",
             per_call=True,
             detailed=True,
-            namespace=cli_args
+            namespace=cli_args,
         )
 
         with loading_bar:
             for _, items in iterator:
                 loading_bar.advance(len(items))
 
                 # if details is not None:
```

### Comparing `minet-1.5.1/minet/cli/dump/__init__.py` & `minet-2.0.0/minet/cli/dump/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/dump/dump_graph.py` & `minet-2.0.0/minet/cli/dump/dump_graph.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/exceptions.py` & `minet-2.0.0/minet/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/extract/__init__.py` & `minet-2.0.0/minet/cli/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/extract/extract.py` & `minet-2.0.0/minet/cli/extract/extract.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/facebook/__init__.py` & `minet-2.0.0/minet/cli/facebook/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # =============================================================================
 # Minet Facebook CLI Action
 # =============================================================================
 #
 # Logic of the `fb` action.
 #
+from casanova import RowCountResumer
+
 from minet.cli.argparse import command, ConfigAction
 
 # TODO: lazyloading issue
 from minet.facebook.constants import FACEBOOK_MOBILE_DEFAULT_THROTTLE
 
 MOBILE_ARGUMENTS = [
     {
@@ -261,14 +263,15 @@
         Examples:
 
         . Fetching user infos of a series of users in a CSV file:
             $ minet fb user-infos user_url -i fb-users.csv > user-infos.csv
     """,
     variadic_input={"dummy_column": "user_url", "item_label": "user"},
     arguments=[*MOBILE_ARGUMENTS],
+    resumer=RowCountResumer,
 )
 
 FACEBOOK_COMMAND = command(
     "facebook",
     "minet.cli.facebook",
     "Minet Facebook Command",
     aliases=["fb"],
```

### Comparing `minet-1.5.1/minet/cli/facebook/comments.py` & `minet-2.0.0/minet/cli/facebook/comments.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/facebook/experimental_comments.py` & `minet-2.0.0/minet/cli/facebook/experimental_comments.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/facebook/post.py` & `minet-2.0.0/minet/cli/facebook/post.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/facebook/post_authors.py` & `minet-2.0.0/minet/cli/facebook/post_authors.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/facebook/post_stats.py` & `minet-2.0.0/minet/cli/facebook/post_stats.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/facebook/posts.py` & `minet-2.0.0/minet/cli/facebook/posts.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/facebook/url_likes.py` & `minet-2.0.0/minet/cli/facebook/url_likes.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/facebook/user_infos.py` & `minet-2.0.0/minet/cli/facebook/user_infos.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,9 +16,13 @@
     headers=MobileFacebookUserInfo, title="Scraping user infos", unit="users"
 )
 def action(cli_args, enricher, loading_bar: LoadingBar):
     scraper = FacebookMobileScraper(cli_args.cookie, throttle=cli_args.throttle)
 
     for row, user_url in enricher.cells(cli_args.column, with_rows=True):
         with loading_bar.step():
-            user_infos = scraper.user_infos(user_url)
-            enricher.writerow(row, user_infos)
+            try:
+                user_infos = scraper.user_infos(user_url)
+                enricher.writerow(row, user_infos)
+            except TypeError:
+                enricher.writerow(row)
+                loading_bar.inc_stat("invalid-url", style="error")
```

### Comparing `minet-1.5.1/minet/cli/facebook/utils.py` & `minet-2.0.0/minet/cli/facebook/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/fetch/__init__.py` & `minet-2.0.0/minet/cli/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/fetch/fetch.py` & `minet-2.0.0/minet/cli/fetch/fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,15 @@
             for result, callback_result in executor.request(
                 enricher,
                 request_args=request_args,
                 callback=worker_callback,
                 passthrough=True,
                 use_pycurl=cli_args.pycurl,
                 compressed=cli_args.compress_transfer,
-                **common_http_imap_kwargs
+                **common_http_imap_kwargs,
             ):
                 with loading_bar.step():
                     index, row = result.item
 
                     if isinstance(result, PassthroughRequestResult):
                         enricher.writerow(index, row)
                         loading_bar.inc_stat("filtered", style="warning")
@@ -421,15 +421,15 @@
                 enricher,
                 resolve_args=request_args,
                 follow_meta_refresh=cli_args.follow_meta_refresh,
                 follow_js_relocation=cli_args.follow_js_relocation,
                 infer_redirection=cli_args.infer_redirection,
                 canonicalize=cli_args.canonicalize,
                 passthrough=True,
-                **common_http_imap_kwargs
+                **common_http_imap_kwargs,
             ):
                 with loading_bar.step():
                     index, row = result.item
 
                     if isinstance(result, PassthroughResolveResult):
                         enricher.writerow(index, row)
                         loading_bar.inc_stat("filtered", style="warning")
@@ -464,15 +464,15 @@
         import asyncio
         from playwright.async_api import (
             Error as PlaywrightError,
             TimeoutError as PlaywrightTimeoutError,
         )
 
         from minet.browser.utils import convert_playwright_error
-        from minet.exceptions import BrowserUnknownError
+        from minet.exceptions import BrowserYetUnimplementedError
         from minet.serialization import serialize_error_as_slug
 
         goto_timeout = int(
             (cli_args.timeout if cli_args.timeout is not None else 30) * 1000
         )
 
         async def screenshot(
@@ -484,15 +484,15 @@
                         payload.url,
                         timeout=goto_timeout,
                         wait_until=cli_args.wait_until,
                     )
                 except (PlaywrightError, PlaywrightTimeoutError) as e:
                     error = convert_playwright_error(e)
 
-                    if isinstance(error, BrowserUnknownError):
+                    if isinstance(error, BrowserYetUnimplementedError):
                         raise e
 
                     return ScreenshotAddendum(
                         screenshot_error=serialize_error_as_slug(error)
                     )
 
                 assert response is not None
@@ -537,15 +537,15 @@
                 )
 
         with BrowserThreadPoolExecutor(
             width=cli_args.width,
             height=cli_args.height,
             adblock=cli_args.adblock,
             automatic_consent=cli_args.automatic_consent,
-            **common_executor_kwargs
+            **common_executor_kwargs,
         ) as executor:
             loading_bar.append_to_title(" (t=%i)" % executor.max_workers)
 
             for result in executor.run(
                 enricher, screenshot, passthrough=True, **common_imap_kwargs
             ):
                 with loading_bar.step():
```

### Comparing `minet-1.5.1/minet/cli/google/__init__.py` & `minet-2.0.0/minet/cli/google/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/google/sheets.py` & `minet-2.0.0/minet/cli/google/sheets.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/hyphe/__init__.py` & `minet-2.0.0/minet/cli/hyphe/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/hyphe/crawl.py` & `minet-2.0.0/minet/cli/hyphe/crawl.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/hyphe/declare.py` & `minet-2.0.0/minet/cli/hyphe/declare.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/hyphe/destroy.py` & `minet-2.0.0/minet/cli/hyphe/destroy.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/hyphe/dump.py` & `minet-2.0.0/minet/cli/hyphe/dump.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/hyphe/reset.py` & `minet-2.0.0/minet/cli/hyphe/reset.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/hyphe/tag.py` & `minet-2.0.0/minet/cli/hyphe/tag.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/instagram/__init__.py` & `minet-2.0.0/minet/cli/instagram/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # =============================================================================
 # Minet Instagram CLI Action
 # =============================================================================
 #
 # Logic of the `insta` action.
 #
+from casanova import RowCountResumer
+
 from minet.cli.argparse import command, ConfigAction
 
 INSTAGRAM_COMMENTS_SUBCOMMAND = command(
     "comments",
     "minet.cli.instagram.comments",
     title="Instagram Comments Command",
     description="""
@@ -148,14 +150,15 @@
     """,
     variadic_input={
         "dummy_column": "post",
         "item_label": "post url, post shortcode or post id",
         "item_label_plural": "post urls, post shortcodes or post ids",
     },
     select=True,
+    resumer=RowCountResumer,
 )
 
 INSTAGRAM_USER_FOLLOWING_SUBCOMMAND = command(
     "user-following",
     "minet.cli.instagram.user_following",
     title="Instagram User Following Command",
     description="""
@@ -227,14 +230,15 @@
             $ minet instagram user-infos banksrepeta > banksrepeta_infos.csv
     """,
     variadic_input={
         "dummy_column": "user",
         "item_label": "username, user url or user id",
         "item_label_plural": "usernames, user urls or user ids",
     },
+    resumer=RowCountResumer
 )
 
 INSTAGRAM_USER_POSTS_SUBCOMMAND = command(
     "user-posts",
     "minet.cli.instagram.user_posts",
     title="Instagram User Posts Command",
     description="""
```

### Comparing `minet-1.5.1/minet/cli/instagram/comments.py` & `minet-2.0.0/minet/cli/instagram/comments.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/instagram/hashtag.py` & `minet-2.0.0/minet/cli/instagram/hashtag.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/instagram/post_infos.py` & `minet-2.0.0/minet/cli/instagram/post_infos.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,33 +2,29 @@
 # Minet Instagram Post-infos CLI Action
 # =============================================================================
 #
 # Logic of the `instagram post-infos` action.
 #
 from minet.cli.utils import with_enricher_and_loading_bar
 from minet.cli.instagram.utils import with_instagram_fatal_errors
+from minet.cli.loading_bar import LoadingBar
 from minet.instagram import InstagramAPIScraper
 from minet.instagram.types import InstagramPost
 from minet.instagram.exceptions import InstagramInvalidTargetError
 
 
 @with_instagram_fatal_errors
 @with_enricher_and_loading_bar(
     headers=InstagramPost, title="Scraping infos", unit="posts"
 )
-def action(cli_args, enricher, loading_bar):
+def action(cli_args, enricher, loading_bar: LoadingBar):
     client = InstagramAPIScraper(cookie=cli_args.cookie)
 
-    for i, row, user in enricher.enumerate_cells(
-        cli_args.column, with_rows=True, start=1
-    ):
+    for row, user in enricher.cells(cli_args.column, with_rows=True):
         with loading_bar.step():
             try:
                 result = client.post_infos(user)
-
                 enricher.writerow(row, result)
 
             except InstagramInvalidTargetError:
-                loading_bar.print(
-                    "Given post (line %i) is probably not an Instagram post: %s"
-                    % (i, user)
-                )
+                loading_bar.inc_stat("not-found", style="warning")
+                enricher.writerow(row)
```

### Comparing `minet-1.5.1/minet/cli/instagram/user_followers.py` & `minet-2.0.0/minet/cli/instagram/user_followers.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/instagram/user_following.py` & `minet-2.0.0/minet/cli/instagram/user_following.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/instagram/user_infos.py` & `minet-2.0.0/minet/cli/instagram/user_infos.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # =============================================================================
 # Minet Instagram User-infos CLI Action
 # =============================================================================
 #
 # Logic of the `instagram user-infos` action.
 #
 from minet.cli.utils import with_enricher_and_loading_bar
+from minet.cli.loading_bar import LoadingBar
 from minet.cli.instagram.utils import with_instagram_fatal_errors
 from minet.instagram import InstagramAPIScraper
 from minet.instagram.types import InstagramUserInfo
 from minet.instagram.exceptions import InstagramInvalidTargetError
 
 
 @with_instagram_fatal_errors
 @with_enricher_and_loading_bar(
     headers=InstagramUserInfo, title="Scraping infos", unit="users"
 )
-def action(cli_args, enricher, loading_bar):
+def action(cli_args, enricher, loading_bar: LoadingBar):
     client = InstagramAPIScraper(cookie=cli_args.cookie)
 
-    for i, row, user in enricher.enumerate_cells(
-        cli_args.column, with_rows=True, start=1
-    ):
+    for row, user in enricher.cells(cli_args.column, with_rows=True):
         with loading_bar.step():
             try:
                 info = client.user_infos(user)
                 enricher.writerow(row, info)
 
             except InstagramInvalidTargetError:
-                loading_bar.print(
-                    "Given user (line %i) is probably not an Instagram user: %s"
-                    % (i, user)
-                )
+                loading_bar.inc_stat("not-found", style="warning")
+                enricher.writerow(row)
```

### Comparing `minet-1.5.1/minet/cli/instagram/user_posts.py` & `minet-2.0.0/minet/cli/instagram/user_posts.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/instagram/utils.py` & `minet-2.0.0/minet/cli/instagram/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/loading_bar.py` & `minet-2.0.0/minet/cli/loading_bar.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/mediacloud/__init__.py` & `minet-2.0.0/minet/cli/mediacloud/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/mediacloud/medias.py` & `minet-2.0.0/minet/cli/mediacloud/medias.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/mediacloud/search.py` & `minet-2.0.0/minet/cli/mediacloud/search.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/mediacloud/topic/stories.py` & `minet-2.0.0/minet/cli/mediacloud/topic/stories.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/reporters.py` & `minet-2.0.0/minet/cli/reporters.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/run.py` & `minet-2.0.0/minet/cli/run.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/scrape/__init__.py` & `minet-2.0.0/minet/cli/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/scrape/scrape.py` & `minet-2.0.0/minet/cli/scrape/scrape.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/telegram/__init__.py` & `minet-2.0.0/minet/cli/telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/telegram/channel_infos.py` & `minet-2.0.0/minet/cli/telegram/channel_infos.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/telegram/channel_messages.py` & `minet-2.0.0/minet/cli/telegram/channel_messages.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/tiktok/__init__.py` & `minet-2.0.0/minet/cli/tiktok/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/tiktok/search_videos.py` & `minet-2.0.0/minet/cli/tiktok/search_videos.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/__init__.py` & `minet-2.0.0/minet/cli/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/attrition.py` & `minet-2.0.0/minet/cli/twitter/attrition.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/followers_you_know.py` & `minet-2.0.0/minet/cli/twitter/followers_you_know.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/legacy_tweets.py` & `minet-2.0.0/minet/cli/twitter/legacy_tweets.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/list_followers.py` & `minet-2.0.0/minet/cli/twitter/list_followers.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/list_members.py` & `minet-2.0.0/minet/cli/twitter/list_members.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/retweeters.py` & `minet-2.0.0/minet/cli/twitter/retweeters.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/scrape.py` & `minet-2.0.0/minet/cli/twitter/scrape.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/tweet_count.py` & `minet-2.0.0/minet/cli/twitter/tweet_count.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/tweet_date.py` & `minet-2.0.0/minet/cli/twitter/tweet_date.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/tweet_search.py` & `minet-2.0.0/minet/cli/twitter/tweet_search.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/tweets.py` & `minet-2.0.0/minet/cli/twitter/tweets.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/user_search.py` & `minet-2.0.0/minet/cli/twitter/user_search.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/user_tweets.py` & `minet-2.0.0/minet/cli/twitter/user_tweets.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/users.py` & `minet-2.0.0/minet/cli/twitter/users.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/twitter/utils.py` & `minet-2.0.0/minet/cli/twitter/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/url_extract/__init__.py` & `minet-2.0.0/minet/cli/url_extract/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/url_extract/url_extract.py` & `minet-2.0.0/minet/cli/url_extract/url_extract.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/url_join/__init__.py` & `minet-2.0.0/minet/cli/url_join/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/url_join/url_join.py` & `minet-2.0.0/minet/cli/url_join/url_join.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/url_parse/__init__.py` & `minet-2.0.0/minet/cli/url_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/url_parse/url_parse.py` & `minet-2.0.0/minet/cli/url_parse/url_parse.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/user_agents/__init__.py` & `minet-2.0.0/minet/cli/user_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/utils.py` & `minet-2.0.0/minet/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,15 +343,15 @@
             total = getattr(cli_args, "total", None)
 
             with LoadingBar(
                 total=total,
                 stats=stats,
                 refresh_per_second=getattr(cli_args, "refresh_per_second", 10),
                 simple=getattr(cli_args, "simple_progress", False),
-                **loading_bar_kwargs
+                **loading_bar_kwargs,
             ) as loading_bar:
                 additional_kwargs = {
                     "loading_bar": loading_bar,
                 }
 
                 return action(cli_args, *args, **additional_kwargs, **kwargs)
 
@@ -432,15 +432,15 @@
                     cli_args.output,
                     add=headers(cli_args)
                     if callable(headers) and not is_tabular_record_class(headers)
                     else headers,
                     select=cli_args.select,
                     total=getattr(cli_args, "total", None),
                     multiplex=multiplex,
-                    **enricher_kwargs
+                    **enricher_kwargs,
                 )
 
             completed = 0
 
             if isinstance(cli_args.output, casanova.Resumer):
                 try:
                     completed = cli_args.output.already_done_count()
```

### Comparing `minet-1.5.1/minet/cli/wikipedia/__init__.py` & `minet-2.0.0/minet/cli/wikipedia/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/wikipedia/pageviews.py` & `minet-2.0.0/minet/cli/wikipedia/pageviews.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/youtube/__init__.py` & `minet-2.0.0/minet/cli/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/youtube/captions.py` & `minet-2.0.0/minet/cli/youtube/captions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/youtube/channel_links.py` & `minet-2.0.0/minet/cli/youtube/channel_links.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/youtube/channel_videos.py` & `minet-2.0.0/minet/cli/youtube/channel_videos.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/youtube/channels.py` & `minet-2.0.0/minet/cli/youtube/channels.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/youtube/comments.py` & `minet-2.0.0/minet/cli/youtube/comments.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/youtube/search.py` & `minet-2.0.0/minet/cli/youtube/search.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cli/youtube/videos.py` & `minet-2.0.0/minet/cli/youtube/videos.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/constants.py` & `minet-2.0.0/minet/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/cookies.py` & `minet-2.0.0/minet/cookies.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crawl/crawler.py` & `minet-2.0.0/minet/crawl/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,23 @@
     Tuple,
     Any,
     Generic,
     Mapping,
     Iterable,
     Iterator,
     Union,
+    Awaitable,
+    TYPE_CHECKING,
 )
 from minet.types import ParamSpec
 
+if TYPE_CHECKING:
+    from playwright.async_api import BrowserContext
+    from minet.browser import ThreadsafeBrowser
+
 from os import makedirs
 from os.path import join
 from threading import Lock
 from urllib.parse import urljoin
 from ural import ensure_protocol, get_domain_name
 from multiprocessing import Pool
 
@@ -112,30 +118,33 @@
             Callable[
                 [
                     "Crawler",
                     SuccessfulCrawlResult[CrawlJobDataType, CrawlResultDataType],
                 ],
                 CallbackResultType,
             ]
-        ] = None
+        ] = None,
     ):
         self.crawler = crawler
         self.cancel_event = self.crawler.executor.cancel_event
         self.local_context = self.crawler.executor.local_context
         self.request_args = request_args
         self.max_depth = crawler.max_depth
         self.callback = callback
 
-        self.default_kwargs = {
-            "pool_manager": crawler.executor.pool_manager,
-            "max_redirects": max_redirects,
-            "stateful": stateful_redirects,
-            "spoof_ua": spoof_ua,
-            "cancel_event": crawler.executor.cancel_event,
-        }
+        self.default_kwargs = {}
+
+        if self.crawler.browser is None:
+            self.default_kwargs = {
+                "pool_manager": crawler.executor.pool_manager,
+                "max_redirects": max_redirects,
+                "stateful": stateful_redirects,
+                "spoof_ua": spoof_ua,
+                "cancel_event": crawler.executor.cancel_event,
+            }
 
         if use_pycurl:
             del self.default_kwargs["pool_manager"]
             self.default_kwargs["use_pycurl"] = True
 
         if compressed:
             self.default_kwargs["compressed"] = True
@@ -175,19 +184,24 @@
                 kwargs.update(self.request_args(job))
 
             if cancel_event.is_set():
                 return
 
             try:
                 retryer = getattr(self.local_context, "retryer", None)
+                request_fn = (
+                    request
+                    if self.crawler.browser is None
+                    else self.crawler.browser.request
+                )
 
                 if retryer is not None:
-                    response = retryer(request, job.url, **kwargs)
+                    response = retryer(request_fn, job.url, **kwargs)
                 else:
-                    response = request(job.url, **kwargs)
+                    response = request_fn(job.url, **kwargs)
 
                 # If end url is different from job we add the url to visited cache
                 # NOTE: this is somewhat subject to race conditions but it should
                 # be benign and still be useful in some cases.
                 if self.crawler.url_cache is not None and job.url != response.end_url:
                     with self.crawler.enqueue_lock:
                         self.crawler.url_cache.add(response.end_url)
@@ -200,15 +214,21 @@
 
             if cancel_event.is_set():
                 return
 
             spider_result = spider.process(job, response)
 
             if spider_result is not None:
-                data, next_jobs = spider_result
+                try:
+                    data, next_jobs = spider_result
+                except (ValueError, TypeError):
+                    raise TypeError(
+                        'Spider.process is expected to return either None or a 2-tuple containing data and next targets to enqueue. Got a "%s" instead.'
+                        % spider_result.__class__.__name__
+                    )
             else:
                 data = None
                 next_jobs = None
 
             if cancel_event.is_set():
                 return
 
@@ -250,14 +270,16 @@
 
 # TODO: try creating a kwarg type for those
 class Crawler(Generic[CrawlJobDataTypes, CrawlResultDataTypes]):
     executor: HTTPThreadPoolExecutor
 
     enqueue_lock: Lock
 
+    browser: Optional["ThreadsafeBrowser"]
+
     queue: CrawlerQueue
     persistent: bool
 
     state: CrawlerState
 
     started: bool
     stopped: bool
@@ -292,19 +314,35 @@
         request_args: Optional[RequestArgsType[CrawlJobDataType]] = None,
         use_pycurl: bool = False,
         compressed: bool = False,
         known_encoding: Optional[str] = None,
         max_redirects: int = DEFAULT_FETCH_MAX_REDIRECTS,
         stateful_redirects: bool = False,
         spoof_ua: bool = False,
+        browser_emulation: bool = False,
+        browser_kwargs: Dict[str, Any] = {},
+        browser_context_init: Optional[
+            Callable[["BrowserContext"], Awaitable[None]]
+        ] = None,
     ):
         # Validation
         if resume and persistent_storage_path is None:
             raise TypeError("cannot resume a non-persistent crawler")
 
+        # Browser emulation?
+        self.browser = None
+
+        if browser_emulation:
+            from minet.browser import ThreadsafeBrowser
+
+            self.browser = ThreadsafeBrowser(**browser_kwargs)
+
+            if browser_context_init is not None:
+                self.browser.run_in_default_context(browser_context_init)
+
         # Utilities
         self.file_writer = ThreadSafeFileWriter(writer_root_directory, sqlar=sqlar)
         self.process_pool = None
 
         # NOTE: if not None and not 0 basically
         if process_pool_workers:
             self.process_pool = Pool(process_pool_workers)
@@ -480,63 +518,64 @@
         self.executor.shutdown(wait=self.executor.wait)
 
         self.queue.close()
 
         if self.url_cache:
             self.url_cache.close()
 
+        if self.browser is not None:
+            self.browser.stop()
+
     def __enter__(self):
         self.start()
         return self
 
     def __exit__(self, *exc):
         self.stop()
 
     @overload
     def crawl(
         self,
         callback: None = ...,
-    ) -> Iterator[AnyCrawlResult[CrawlJobDataTypes, CrawlResultDataTypes]]:
-        ...
+    ) -> Iterator[AnyCrawlResult[CrawlJobDataTypes, CrawlResultDataTypes]]: ...
 
     @overload
     def crawl(
         self,
         callback: Callable[
             [
                 "Crawler",
                 SuccessfulCrawlResult[CrawlJobDataTypes, CrawlResultDataTypes],
             ],
-            CallbackResultType,
-        ] = ...,
+            Optional[CallbackResultType],
+        ],
     ) -> Iterator[
         Tuple[
             AnyCrawlResult[CrawlJobDataTypes, CrawlResultDataTypes],
-            CallbackResultType,
+            Optional[CallbackResultType],
         ]
-    ]:
-        ...
+    ]: ...
 
     def crawl(
         self,
         callback: Optional[
             Callable[
                 [
                     "Crawler",
                     SuccessfulCrawlResult[CrawlJobDataTypes, CrawlResultDataTypes],
                 ],
-                CallbackResultType,
+                Optional[CallbackResultType],
             ]
         ] = None,
     ) -> Union[
         Iterator[AnyCrawlResult[CrawlJobDataTypes, CrawlResultDataTypes]],
         Iterator[
             Tuple[
                 AnyCrawlResult[CrawlJobDataTypes, CrawlResultDataTypes],
-                CallbackResultType,
+                Optional[CallbackResultType],
             ]
         ],
     ]:
         worker = CrawlWorker(self, callback=callback, **self.worker_kwargs)
 
         def key(job: CrawlJob) -> Optional[str]:
             return job.group
```

### Comparing `minet-1.5.1/minet/crawl/focus.py` & `minet-2.0.0/minet/crawl/focus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import List, Optional, Any
-from minet.types import Literal
+from typing import List, Optional, Any, Literal
 
 import re
 from ural import could_be_html, normalize_url, should_follow_href
 from urllib.parse import urljoin
 from dataclasses import dataclass
 from casanova import TabularRecord
```

### Comparing `minet-1.5.1/minet/crawl/queue.py` & `minet-2.0.0/minet/crawl/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,18 @@
-from typing import Dict, List, Tuple, Iterable, Iterator, Optional, Callable, Union
-from minet.types import Literal
+from typing import (
+    Dict,
+    List,
+    Tuple,
+    Iterable,
+    Iterator,
+    Optional,
+    Callable,
+    Union,
+    Literal,
+)
 
 import sqlite3
 import pickle
 from os import makedirs
 from os.path import join, isfile
 from shutil import rmtree
 from queue import Empty
```

### Comparing `minet-1.5.1/minet/crawl/spiders.py` & `minet-2.0.0/minet/crawl/spiders.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crawl/state.py` & `minet-2.0.0/minet/crawl/state.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crawl/types.py` & `minet-2.0.0/minet/crawl/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,27 +193,37 @@
                 ("priority", self.priority or None),
                 "data",
                 "parent",
             ),
             conditionals=("data", "spider", "parent", "group", "priority"),
         )
 
+    def retry(self, priority: Optional[int] = 0) -> CrawlTarget[CrawlJobDataType]:
+        return CrawlTarget(
+            url=self.url,
+            depth=self.depth,
+            spider=self.spider,
+            priority=priority if priority is not None else self.priority,
+            data=self.data,
+        )
+
 
 class CrawlResult(Generic[CrawlJobDataType, CrawlResultDataType]):
     __slots__ = ("job", "data", "error", "response", "degree")
 
     FIELDNAMES = [
         "id",
         "parent",
         "spider",
         "depth",
         "url",
         "resolved_url",
         "error",
         "status",
+        "datetime_utc",
         "mimetype",
         "degree",
         "body_size",
         "encoding",
     ]
 
     job: CrawlJob[CrawlJobDataType]
@@ -264,14 +274,15 @@
         row.extend(
             [
                 job.depth,
                 job.url,
                 self.response.end_url if self.response else None,
                 self.error_code,
                 self.response.status if self.response else None,
+                self.response.end_datetime if self.response else None,
                 self.response.mimetype if self.response else None,
                 self.degree,
                 len(self.response) if self.response else None,
                 self.response.encoding if self.response else None,
             ]
         )
```

### Comparing `minet-1.5.1/minet/crawl/url_cache.py` & `minet-2.0.0/minet/crawl/url_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,20 +54,18 @@
                 self.__items.add(item)
 
             return len(self.__items) - len_before
 
     @overload
     def add_many_and_keep_new(
         self, items: Iterable[I], key: Callable[[I], T] = ...
-    ) -> List[I]:
-        ...
+    ) -> List[I]: ...
 
     @overload
-    def add_many_and_keep_new(self, items: Iterable[T], key: None = ...) -> List[T]:
-        ...
+    def add_many_and_keep_new(self, items: Iterable[T], key: None = ...) -> List[T]: ...
 
     def add_many_and_keep_new(self, items, key=None):
         with self.lock:
             new = []
 
             for item in items:
                 k = item if key is None else key(item)
@@ -148,20 +146,20 @@
             rows = [(item,) for item in items]
             cursor.executemany('INSERT OR IGNORE INTO "set" ("key") VALUES (?);', rows)
             return cursor.rowcount
 
     @overload
     def add_many_and_keep_new(
         self, items: Iterable[I], key: Callable[[I], str] = ...
-    ) -> List[I]:
-        ...
+    ) -> List[I]: ...
 
     @overload
-    def add_many_and_keep_new(self, items: Iterable[str], key: None = ...) -> List[str]:
-        ...
+    def add_many_and_keep_new(
+        self, items: Iterable[str], key: None = ...
+    ) -> List[str]: ...
 
     def add_many_and_keep_new(self, items, key=None):
         with self.transaction() as cursor:
             new = []
 
             for item in items:
                 try:
```

### Comparing `minet-1.5.1/minet/crowdtangle/client.py` & `minet-2.0.0/minet/crowdtangle/client.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crowdtangle/constants.py` & `minet-2.0.0/minet/crowdtangle/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crowdtangle/exceptions.py` & `minet-2.0.0/minet/crowdtangle/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crowdtangle/leaderboard.py` & `minet-2.0.0/minet/crowdtangle/leaderboard.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crowdtangle/lists.py` & `minet-2.0.0/minet/crowdtangle/lists.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crowdtangle/post.py` & `minet-2.0.0/minet/crowdtangle/post.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crowdtangle/posts.py` & `minet-2.0.0/minet/crowdtangle/posts.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def url_forge(
     token=None,
     sort_by=None,
     language=None,
     start_date=None,
     end_date=None,
     list_ids=None,
-    **kwargs
+    **kwargs,
 ):
     base_url = URL_TEMPLATE % {"sort_by": sort_by, "token": token}
 
     if language:
         base_url += "&language=%s" % language
 
     if start_date:
```

### Comparing `minet-1.5.1/minet/crowdtangle/search.py` & `minet-2.0.0/minet/crowdtangle/search.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crowdtangle/summary.py` & `minet-2.0.0/minet/crowdtangle/summary.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crowdtangle/types.py` & `minet-2.0.0/minet/crowdtangle/types.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/crowdtangle/utils.py` & `minet-2.0.0/minet/crowdtangle/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         request,
         token,
         limit=None,
         raw=False,
         per_call=False,
         detailed=False,
         namespace=None,
-        **kwargs
+        **kwargs,
     ):
         if namespace is not None:
             kwargs = vars(namespace)
         else:
             kwargs["token"] = token
 
         # Checking we have the necessary dates
```

### Comparing `minet-1.5.1/minet/dates.py` & `minet-2.0.0/minet/dates.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/encodings.py` & `minet-2.0.0/minet/encodings.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/exceptions.py` & `minet-2.0.0/minet/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 
 
 # Browser emulation
 class BrowserError(MinetError):
     pass
 
 
-class BrowserUnknownError(BrowserError):
+class BrowserYetUnimplementedError(BrowserError):
     pass
 
 
 class BrowserNameNotResolvedError(BrowserError):
     pass
```

### Comparing `minet-1.5.1/minet/executors.py` & `minet-2.0.0/minet/executors.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,17 @@
     Iterable,
     Dict,
     Union,
     Tuple,
     Awaitable,
     Any,
     TYPE_CHECKING,
+    Literal,
 )
-from minet.types import Literal, TypedDict, Unpack, NotRequired
+from minet.types import TypedDict, Unpack, NotRequired
 
 if TYPE_CHECKING:
     from minet.browser.threadsafe_browser import BrowserOrBrowserContext
 
 import urllib3
 import threading
 from threading import Event
@@ -91,28 +92,28 @@
     item: ItemType
     url: str
 
 
 ArgsCallbackType = Callable[[HTTPWorkerPayload[ItemType]], Dict]
 
 
-class ExecutorRequestKwargs(TypedDict, Generic[ItemType, CallbackResultType]):
+class ExecutorRequestKwargs(TypedDict, Generic[ItemType]):
     ordered: NotRequired[bool]
     key: NotRequired[Optional[Callable[[ItemType], Optional[str]]]]
     throttle: NotRequired[float]
     request_args: NotRequired[Optional[ArgsCallbackType[ItemType]]]
     use_pycurl: NotRequired[bool]
     compressed: NotRequired[bool]
     buffer_size: NotRequired[int]
     domain_parallelism: NotRequired[int]
     max_redirects: NotRequired[int]
     known_encoding: NotRequired[Optional[str]]
 
 
-class ExecutorResolveKwargs(TypedDict, Generic[ItemType, CallbackResultType]):
+class ExecutorResolveKwargs(TypedDict, Generic[ItemType]):
     ordered: NotRequired[bool]
     key: NotRequired[Optional[Callable[[ItemType], Optional[str]]]]
     throttle: NotRequired[float]
     resolve_args: NotRequired[Optional[ArgsCallbackType[ItemType]]]
     buffer_size: NotRequired[int]
     domain_parallelism: NotRequired[int]
     max_redirects: NotRequired[int]
@@ -540,50 +541,48 @@
     @overload
     def request(
         self,
         iterator: Iterable[ItemType],
         *,
         passthrough: Literal[False] = ...,
         callback: None = ...,
-        **kwargs: Unpack[ExecutorRequestKwargs[ItemType, CallbackResultType]],
-    ) -> Iterator[AnyActualRequestResult[ItemType]]:
-        ...
+        **kwargs: Unpack[ExecutorRequestKwargs[ItemType]],
+    ) -> Iterator[AnyActualRequestResult[ItemType]]: ...
 
     @overload
     def request(
         self,
         iterator: Iterable[ItemType],
         *,
         passthrough: Literal[True] = ...,
         callback: None = ...,
-        **kwargs: Unpack[ExecutorRequestKwargs[ItemType, CallbackResultType]],
-    ) -> Iterator[AnyRequestResult[ItemType]]:
-        ...
+        **kwargs: Unpack[ExecutorRequestKwargs[ItemType]],
+    ) -> Iterator[AnyRequestResult[ItemType]]: ...
 
     @overload
     def request(
         self,
         iterator: Iterable[ItemType],
         *,
         passthrough: Literal[False] = ...,
-        callback: Callable[[ItemType, str, Response], CallbackResultType] = ...,
-        **kwargs: Unpack[ExecutorRequestKwargs[ItemType, CallbackResultType]],
-    ) -> Iterator[Tuple[AnyActualRequestResult[ItemType], CallbackResultType]]:
-        ...
+        callback: Callable[[ItemType, str, Response], Optional[CallbackResultType]],
+        **kwargs: Unpack[ExecutorRequestKwargs[ItemType]],
+    ) -> Iterator[
+        Tuple[AnyActualRequestResult[ItemType], Optional[CallbackResultType]]
+    ]: ...
 
     @overload
     def request(
         self,
         iterator: Iterable[ItemType],
         *,
         passthrough: Literal[True] = ...,
-        callback: Callable[[ItemType, str, Response], CallbackResultType] = ...,
-        **kwargs: Unpack[ExecutorRequestKwargs[ItemType, CallbackResultType]],
-    ) -> Iterator[Tuple[AnyRequestResult[ItemType], CallbackResultType]]:
-        ...
+        callback: Callable[[ItemType, str, Response], Optional[CallbackResultType]],
+        **kwargs: Unpack[ExecutorRequestKwargs[ItemType]],
+    ) -> Iterator[Tuple[AnyRequestResult[ItemType], Optional[CallbackResultType]]]: ...
 
     def request(
         self,
         iterator: Iterable[ItemType],
         *,
         ordered: bool = False,
         key: Optional[Callable[[ItemType], Optional[str]]] = None,
@@ -592,22 +591,22 @@
         use_pycurl: bool = False,
         compressed: bool = False,
         buffer_size: int = DEFAULT_IMAP_BUFFER_SIZE,
         domain_parallelism: int = DEFAULT_DOMAIN_PARALLELISM,
         max_redirects: int = DEFAULT_FETCH_MAX_REDIRECTS,
         known_encoding: Optional[str] = None,
         callback: Optional[
-            Callable[[ItemType, str, Response], CallbackResultType]
+            Callable[[ItemType, str, Response], Optional[CallbackResultType]]
         ] = None,
         passthrough: bool = False,
     ) -> Union[
         Iterator[AnyRequestResult[ItemType]],
         Iterator[AnyActualRequestResult[ItemType]],
-        Iterator[Tuple[AnyRequestResult[ItemType], CallbackResultType]],
-        Iterator[Tuple[AnyActualRequestResult[ItemType], CallbackResultType]],
+        Iterator[Tuple[AnyRequestResult[ItemType], Optional[CallbackResultType]]],
+        Iterator[Tuple[AnyActualRequestResult[ItemType], Optional[CallbackResultType]]],
     ]:
         # TODO: validate
         worker = HTTPWorker(
             self.pool_manager,
             self.cancel_event,
             self.local_context,
             get_args=request_args,
@@ -641,50 +640,52 @@
     @overload
     def resolve(
         self,
         iterator: Iterable[ItemType],
         *,
         callback: None = ...,
         passthrough: Literal[False] = ...,
-        **kwargs: Unpack[ExecutorResolveKwargs[ItemType, CallbackResultType]],
-    ) -> Iterator[AnyActualResolveResult[ItemType]]:
-        ...
+        **kwargs: Unpack[ExecutorResolveKwargs[ItemType]],
+    ) -> Iterator[AnyActualResolveResult[ItemType]]: ...
 
     @overload
     def resolve(
         self,
         iterator: Iterable[ItemType],
         *,
         callback: None = ...,
         passthrough: Literal[True] = ...,
-        **kwargs: Unpack[ExecutorResolveKwargs[ItemType, CallbackResultType]],
-    ) -> Iterator[AnyResolveResult[ItemType]]:
-        ...
+        **kwargs: Unpack[ExecutorResolveKwargs[ItemType]],
+    ) -> Iterator[AnyResolveResult[ItemType]]: ...
 
     @overload
     def resolve(
         self,
         iterator: Iterable[ItemType],
         *,
-        callback: Callable[[ItemType, str, RedirectionStack], CallbackResultType],
+        callback: Callable[
+            [ItemType, str, RedirectionStack], Optional[CallbackResultType]
+        ],
         passthrough: Literal[False] = ...,
-        **kwargs: Unpack[ExecutorResolveKwargs[ItemType, CallbackResultType]],
-    ) -> Iterator[Tuple[AnyActualResolveResult[ItemType], CallbackResultType]]:
-        ...
+        **kwargs: Unpack[ExecutorResolveKwargs[ItemType]],
+    ) -> Iterator[
+        Tuple[AnyActualResolveResult[ItemType], Optional[CallbackResultType]]
+    ]: ...
 
     @overload
     def resolve(
         self,
         iterator: Iterable[ItemType],
         *,
-        callback: Callable[[ItemType, str, RedirectionStack], CallbackResultType],
+        callback: Callable[
+            [ItemType, str, RedirectionStack], Optional[CallbackResultType]
+        ],
         passthrough: Literal[True] = ...,
-        **kwargs: Unpack[ExecutorResolveKwargs[ItemType, CallbackResultType]],
-    ) -> Iterator[Tuple[AnyResolveResult[ItemType], CallbackResultType]]:
-        ...
+        **kwargs: Unpack[ExecutorResolveKwargs[ItemType]],
+    ) -> Iterator[Tuple[AnyResolveResult[ItemType], Optional[CallbackResultType]]]: ...
 
     def resolve(
         self,
         iterator: Iterable[ItemType],
         *,
         ordered: bool = False,
         key: Optional[Callable[[ItemType], Optional[str]]] = None,
@@ -695,22 +696,22 @@
         max_redirects: int = DEFAULT_RESOLVE_MAX_REDIRECTS,
         follow_refresh_header: bool = True,
         follow_meta_refresh: bool = False,
         follow_js_relocation: bool = False,
         infer_redirection: bool = False,
         canonicalize: bool = False,
         callback: Optional[
-            Callable[[ItemType, str, RedirectionStack], CallbackResultType]
+            Callable[[ItemType, str, RedirectionStack], Optional[CallbackResultType]]
         ] = None,
         passthrough: bool = False,
     ) -> Union[
         Iterator[AnyResolveResult[ItemType]],
         Iterator[AnyActualResolveResult[ItemType]],
-        Iterator[Tuple[AnyResolveResult[ItemType], CallbackResultType]],
-        Iterator[Tuple[AnyActualResolveResult[ItemType], CallbackResultType]],
+        Iterator[Tuple[AnyResolveResult[ItemType], Optional[CallbackResultType]]],
+        Iterator[Tuple[AnyActualResolveResult[ItemType], Optional[CallbackResultType]]],
     ]:
         # TODO: validate
         worker = HTTPWorker(
             self.pool_manager,
             self.cancel_event,
             self.local_context,
             resolving=True,
```

### Comparing `minet-1.5.1/minet/extraction.py` & `minet-2.0.0/minet/extraction.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/facebook/constants.py` & `minet-2.0.0/minet/facebook/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/facebook/emulated_scraper.py` & `minet-2.0.0/minet/facebook/emulated_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/facebook/exceptions.py` & `minet-2.0.0/minet/facebook/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/facebook/mobile_scraper.py` & `minet-2.0.0/minet/facebook/mobile_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/facebook/post_id_from_url.py` & `minet-2.0.0/minet/facebook/post_id_from_url.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/facebook/types.py` & `minet-2.0.0/minet/facebook/types.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/facebook/utils.py` & `minet-2.0.0/minet/facebook/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/fs.py` & `minet-2.0.0/minet/fs.py`

 * *Files 5% similar despite different names*

```diff
@@ -245,15 +245,14 @@
 
         return filename
 
 
 class ThreadSafeFileWriter(object):
     def __init__(self, root_directory: Optional[str] = None, sqlar: bool = False):
         self.root_directory = root_directory or ""
-        self.folder_locks = NamedLocks()
         self.file_locks = NamedLocks()
         self.sqlar = sqlar
         self.archive = None
 
         if self.sqlar:
             self.root_directory += ".sqlar"
             self.archive = SQLiteArchive(self.root_directory)
@@ -269,17 +268,16 @@
 
         return normpath(abspath(full_path))
 
     def makedirs(self, directory: str) -> None:
         if not directory:
             return
 
-        # TODO: cache
-        with self.folder_locks[directory]:
-            makedirs(directory, exist_ok=True)
+        # NOTE: os.makedirs is already threadsafe
+        makedirs(directory, exist_ok=True)
 
     def write(
         self,
         filename: str,
         contents: Union[str, bytes],
         compress: bool = False,
         relative: bool = False,
```

### Comparing `minet-1.5.1/minet/google/exceptions.py` & `minet-2.0.0/minet/google/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/google/sheets.py` & `minet-2.0.0/minet/google/sheets.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/headers.py` & `minet-2.0.0/minet/headers.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/hyphe/client.py` & `minet-2.0.0/minet/hyphe/client.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/hyphe/constants.py` & `minet-2.0.0/minet/hyphe/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/hyphe/exceptions.py` & `minet-2.0.0/minet/hyphe/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/hyphe/formatters.py` & `minet-2.0.0/minet/hyphe/formatters.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/hyphe/spider.py` & `minet-2.0.0/minet/hyphe/spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import Iterable, List, Set, Iterator, Any, Optional
-from minet.types import Literal
+from typing import Iterable, List, Set, Iterator, Any, Optional, Literal
 
 from dataclasses import dataclass
 from ural.lru import CanonicalizedLRUTrie
 from ural import links_from_html, could_be_html, infer_redirection, canonicalize_url
 from casanova import TabularRecord
 from functools import lru_cache
```

### Comparing `minet-1.5.1/minet/instagram/api_scraper.py` & `minet-2.0.0/minet/instagram/api_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/instagram/constants.py` & `minet-2.0.0/minet/instagram/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/instagram/exceptions.py` & `minet-2.0.0/minet/instagram/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/instagram/types.py` & `minet-2.0.0/minet/instagram/types.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/instagram/utils.py` & `minet-2.0.0/minet/instagram/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/mediacloud/client.py` & `minet-2.0.0/minet/mediacloud/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,19 +37,19 @@
         return make_simple_call(
             self.pool_manager,
             self.token,
             "/media/single",
             MediacloudFeed.from_payload,
             arg=media_id,
             single=True,
-            **kwargs
+            **kwargs,
         )
 
     def feeds(self, media_id, **kwargs):
         return make_simple_call(
             self.pool_manager,
             self.token,
             "/feeds/list",
             MediacloudMedia.from_payload,
             query={"media_id": media_id, "rows": 100},
-            **kwargs
+            **kwargs,
         )
```

### Comparing `minet-1.5.1/minet/mediacloud/exceptions.py` & `minet-2.0.0/minet/mediacloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/mediacloud/search.py` & `minet-2.0.0/minet/mediacloud/search.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/mediacloud/topic.py` & `minet-2.0.0/minet/mediacloud/topic.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/mediacloud/types.py` & `minet-2.0.0/minet/mediacloud/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             payload["url"],
             payload["language"],
             payload["collect_date"],
             payload["publish_date"],
             payload["media_id"],
             payload["media_name"],
             payload["media_url"],
-            *explode_tags(tags)
+            *explode_tags(tags),
         )
 
 
 @dataclass
 class MediacloudMedia(TabularRecord):
     media_id: str
     media_name: str
@@ -117,15 +117,15 @@
             payload["url"],
             payload["is_healthy"],
             payload["is_monitored"],
             payload.get("public_notes"),
             payload["num_stories_90"],
             payload["num_sentences_90"],
             payload["start_date"],
-            *explode_tags(tags)
+            *explode_tags(tags),
         )
 
 
 @dataclass
 class MediacloudFeed(TabularRecord):
     name: str
     url: str
```

### Comparing `minet-1.5.1/minet/mediacloud/utils.py` & `minet-2.0.0/minet/mediacloud/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/multiprocessing.py` & `minet-2.0.0/minet/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/pycurl.py` & `minet-2.0.0/minet/pycurl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Optional, Dict, List, Union
-from minet.types import AnyTimeout, RedirectionStack, Redirection, HTTPHeaderDict
+from minet.types import AnyTimeout, RedirectionStack, Redirection
 
 import pycurl
 import certifi
 from dataclasses import dataclass
 from ebbe import format_repr, format_filesize
 from threading import Event
 from ural import is_url
 from urllib3 import Timeout
 from urllib.parse import urljoin
 from urllib3.util.url import parse_url
+from urllib3._collections import HTTPHeaderDict
 
 from minet.constants import REDIRECT_STATUSES
 from minet.exceptions import (
     CancelledRequestError,
     MaxRedirectsError,
     InvalidURLError,
     PycurlError,
```

### Comparing `minet-1.5.1/minet/rate_limiting.py` & `minet-2.0.0/minet/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/__init__.py` & `minet-2.0.0/minet/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/analysis.py` & `minet-2.0.0/minet/scrape/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # =============================================================================
 # Minet Scraper Analysis
 # =============================================================================
 #
 # Functions performing analysis of scraper definitions.
 #
-from typing import Optional, List
-from minet.types import Literal
+from typing import Optional, List, Literal
 
 import ast
 import soupsieve
 from soupsieve import SelectorSyntaxError
 
 from minet.scrape.utils import get_sel, get_iterator
 from minet.scrape.constants import (
```

### Comparing `minet-1.5.1/minet/scrape/classes/base.py` & `minet-2.0.0/minet/scrape/classes/base.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/classes/definition.py` & `minet-2.0.0/minet/scrape/classes/definition.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/classes/function.py` & `minet-2.0.0/minet/scrape/classes/function.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-from typing import Union, Optional, Callable, Any, cast, Dict, List
+from typing import (
+    Union,
+    Optional,
+    Callable,
+    Any,
+    cast,
+    Dict,
+    List,
+    get_origin,
+    get_args,
+    get_type_hints,
+)
 
 import inspect
 
 from casanova import RowWrapper
 from bs4 import SoupStrainer
 
-from minet.types import get_type_hints, get_origin, get_args
 from minet.scrape.classes.base import ScraperBase
 from minet.scrape.soup import WonderfulSoup
 from minet.scrape.straining import strainer_from_css
 from minet.scrape.utils import ensure_soup
 from minet.scrape.types import AnyScrapableTarget
```

### Comparing `minet-1.5.1/minet/scrape/classes/named/__init__.py` & `minet-2.0.0/minet/scrape/classes/named/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/classes/named/canonical.py` & `minet-2.0.0/minet/scrape/classes/named/canonical.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/classes/named/europresse.py` & `minet-2.0.0/minet/scrape/classes/named/europresse.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/classes/named/images.py` & `minet-2.0.0/minet/scrape/classes/named/images.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/classes/named/metas.py` & `minet-2.0.0/minet/scrape/classes/named/metas.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/classes/named/rss.py` & `minet-2.0.0/minet/scrape/classes/named/rss.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/classes/named/types.py` & `minet-2.0.0/minet/scrape/classes/named/types.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/classes/named/urls.py` & `minet-2.0.0/minet/scrape/classes/named/urls.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/compiler.py` & `minet-2.0.0/minet/scrape/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,25 +67,25 @@
     def print(self, string, **kwargs):
         self.printer(
             string,
             level=self.level,
             parent=self.parent.identifier,
             id=self.identifier,
             next=self.identifier + 1,
-            **kwargs
+            **kwargs,
         )
 
     def yield_to_parent(self, expr, **kwargs):
         if self.parent.container_type == "list":
             self.print("value_{parent}.append(%s)" % expr, **kwargs)
         elif self.parent.container_type == "dict":
             self.print(
                 "value_{parent}[%s] = %s"
                 % (escape_string_as_literal(self.parent.container_key), expr),
-                **kwargs
+                **kwargs,
             )
         else:
             self.print("value_{parent} = %s" % expr, **kwargs)
 
 
 class FieldsNode(object):
     def __init__(self, definition):
```

### Comparing `minet-1.5.1/minet/scrape/constants.py` & `minet-2.0.0/minet/scrape/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/exceptions.py` & `minet-2.0.0/minet/scrape/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/interpreter.py` & `minet-2.0.0/minet/scrape/interpreter.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/regex.py` & `minet-2.0.0/minet/scrape/regex.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/soup.py` & `minet-2.0.0/minet/scrape/soup.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,20 +91,18 @@
     def get_outer_html(self) -> str:
         return str(self).strip()
 
     def __getitem__(self, name: str) -> str:
         return cast(str, super().__getitem__(name))
 
     @overload
-    def get(self, name: str, default: str = ...) -> str:
-        ...
+    def get(self, name: str, default: str = ...) -> str: ...
 
     @overload
-    def get(self, name: str, default: None = ...) -> Optional[str]:
-        ...
+    def get(self, name: str, default: None = ...) -> Optional[str]: ...
 
     def get(self, name: str, default: Optional[str] = None) -> Optional[str]:
         return cast(Optional[str], super().get(name, default))
 
     def get_list(self, name: str) -> List[str]:
         value = super().get(name)
 
@@ -125,15 +123,21 @@
 
     def __init__(
         self,
         markup: str,
         features: str = "lxml",
         parse_only: Optional[SoupStrainer] = None,
     ) -> None:
-        super().__init__(markup, features, element_classes=WONDERFUL_ELEMENT_CLASSES, parse_only=parse_only, multi_valued_attributes=None)  # type: ignore
+        super().__init__(
+            markup,
+            features,
+            element_classes=WONDERFUL_ELEMENT_CLASSES,
+            parse_only=parse_only,
+            multi_valued_attributes=None,
+        )  # type: ignore
 
 
 @contextmanager
 def suppress_xml_parsed_as_html_warnings(bypass=False):
     try:
         if XMLParsedAsHTMLWarning is None or bypass:
             yield
```

### Comparing `minet-1.5.1/minet/scrape/std.py` & `minet-2.0.0/minet/scrape/std.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/straining.py` & `minet-2.0.0/minet/scrape/straining.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/scrape/utils.py` & `minet-2.0.0/minet/scrape/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/serialization.py` & `minet-2.0.0/minet/serialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     PycurlHostResolutionError,
     PycurlTimeoutError,
     PycurlConnectionRefusedError,
     PycurlSSLError,
     PycurlReceiveError,
     PycurlSendError,
     #
-    BrowserUnknownError,
+    BrowserYetUnimplementedError,
     BrowserNameNotResolvedError,
     BrowserConnectionAbortedError,
     BrowserConnectionRefusedError,
     BrowserConnectionClosedError,
     BrowserTimeoutError,
     BrowserSSLError,
     BrowserHTTPResponseCodeFailureError,
@@ -122,15 +122,15 @@
     PycurlHostResolutionError: "unknown-host",
     PycurlTimeoutError: "timeout",
     PycurlConnectionRefusedError: "connection-refused",
     PycurlSSLError: "ssl",
     PycurlReceiveError: "receive-error",
     PycurlSendError: "send-error",
     #
-    BrowserUnknownError: "unknown-browser-error",
+    BrowserYetUnimplementedError: "unknown-browser-error",
     BrowserNameNotResolvedError: "unknown-host",
     BrowserConnectionAbortedError: "connection-aborted",
     BrowserConnectionRefusedError: "connection-refused",
     BrowserConnectionClosedError: "connection-closed",
     BrowserTimeoutError: "timeout",
     BrowserSSLError: "ssl",
     BrowserHTTPResponseCodeFailureError: "http-response-code-failure",
```

### Comparing `minet-1.5.1/minet/sqlar.py` & `minet-2.0.0/minet/sqlar.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/telegram/scraper.py` & `minet-2.0.0/minet/telegram/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,16 +78,15 @@
     if channel_description:
         description = channel_description.get_text()
 
     # NOTE: the counter_type can be singular or plural, so we normalize
     counters_infos = {
         counter.select_one("span[class='counter_type']")
         .get_text()
-        .rstrip("s"): counter.select_one("span[class='counter_value']")
-        .get_text()
+        .rstrip("s"): counter.select_one("span[class='counter_value']").get_text()
         for counter in channel_infos.select("div[class='tgme_channel_info_counter']")
     }
 
     nb_subscribers = counters_infos["subscriber"]
     nb_photos = counters_infos["photo"]
     nb_videos = counters_infos["video"]
     nb_links = counters_infos["link"]
```

### Comparing `minet-1.5.1/minet/telegram/types.py` & `minet-2.0.0/minet/telegram/types.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/tiktok/api_scraper.py` & `minet-2.0.0/minet/tiktok/api_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/tiktok/exceptions.py` & `minet-2.0.0/minet/tiktok/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/tiktok/types.py` & `minet-2.0.0/minet/tiktok/types.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/twitter/api_client.py` & `minet-2.0.0/minet/twitter/api_client.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/twitter/api_scraper.py` & `minet-2.0.0/minet/twitter/api_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/twitter/constants.py` & `minet-2.0.0/minet/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/twitter/exceptions.py` & `minet-2.0.0/minet/twitter/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/types.py` & `minet-2.0.0/minet/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 import sys
-from typing import Union, List, Optional
+from typing import Union, List, Optional, Literal
 from os import PathLike
 from io import FileIO
-from bs4 import BeautifulSoup
 from urllib3 import Timeout
 from ebbe import format_repr
 
 # NOTE: yes this is repetitive, but mypy only understands this, don't ask questions...
-if sys.version_info >= (3, 8):
-    from typing import Literal, get_origin, get_type_hints, get_args
-else:
-    from typing_extensions import Literal, get_origin, get_type_hints, get_args
-
 if sys.version_info >= (3, 10):
     from typing import TypeGuard, Concatenate, ParamSpec
 else:
     from typing_extensions import TypeGuard, Concatenate, ParamSpec
 
 if sys.version_info >= (3, 11):
     from typing import TypedDict, Required, NotRequired, Unpack
 else:
     from typing_extensions import TypedDict, Required, NotRequired, Unpack
 
-# Useful conditional imports
-try:
-    from urllib3 import HTTPHeaderDict
-except ImportError:
-    from urllib3._collections import HTTPHeaderDict
-
 # Useful Any types
 AnyPath = Union[str, PathLike]
 AnyFileTarget = Union[AnyPath, FileIO]
 AnyTimeout = Union[float, Timeout]
 
 # Redirection types
 RedirectionType = Literal[
```

### Comparing `minet-1.5.1/minet/user_agents/__init__.py` & `minet-2.0.0/minet/user_agents/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Tuple, List
 
+import json
 import random
 from os.path import join, dirname
 
 import minet.user_agents.data as data
 from minet.exceptions import UserAgentsUpdateError
 
 
@@ -14,19 +15,21 @@
         yield d
 
 
 def update_user_agents(transient: bool = False) -> None:
     from minet.web import request
 
     def download_useragentsme_data() -> List[Tuple[float, str]]:
-        response = request("https://www.useragents.me/api")
-        results = response.json()
+        response = request("https://www.useragents.me")
+        json_text = response.soup().force_select_one("#most-common-desktop-useragents-json-csv textarea").get_text()
+        data = json.loads(json_text)
+
         return [
             (row["pct"], row["ua"])
-            for row in results.get("data", [])
+            for row in data
             if not "Trident" in row["ua"]  # Filtering out windows shenanigans etc.
         ]
 
     try:
         data.USER_AGENTS = download_useragentsme_data()
 
         probs = [pct for (pct, _) in data.USER_AGENTS]
```

### Comparing `minet-1.5.1/minet/utils.py` & `minet-2.0.0/minet/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/web.py` & `minet-2.0.0/minet/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     OrderedDict,
     List,
     Mapping,
     Any,
     Dict,
     Container,
 )
-from minet.types import AnyTimeout, Redirection, RedirectionStack, HTTPHeaderDict
+from minet.types import AnyTimeout, Redirection, RedirectionStack
 
 import re
 import cgi
 import certifi
 import random
 import urllib3
 import urllib3.exceptions as urllib3_exceptions
@@ -36,14 +36,15 @@
 from timeit import default_timer as timer
 from io import BytesIO
 from threading import Event
 from urllib.parse import urljoin, quote
 from urllib.request import Request
 from urllib3.util.ssl_ import create_urllib3_context
 from urllib3.util.request import ACCEPT_ENCODING
+from urllib3._collections import HTTPHeaderDict
 from ebbe import rcompose, noop, format_filesize, format_repr
 from tenacity import (
     Retrying,
     RetryCallState,
     retry_if_exception,
     stop_after_attempt,
     stop_when_event_set,
@@ -121,18 +122,18 @@
 def looks_like_html(html_chunk: bytes) -> bool:
     return HTML_RE.match(html_chunk) is not None
 
 
 def create_pool_manager(
     proxy: Optional[str] = None,
     parallelism: int = 1,
-    num_pools: Optional[int] = None,
+    num_pools: int = 4,
     insecure: bool = False,
     spoof_tls_ciphers: bool = False,
-    **kwargs
+    **kwargs,
 ) -> urllib3.PoolManager:
     """
     Helper function returning a urllib3 pool manager with sane defaults.
     """
 
     manager_kwargs: Dict[str, Any] = {"timeout": DEFAULT_URLLIB3_TIMEOUT}
 
@@ -898,15 +899,15 @@
         return self.__text  # type: ignore # If we don't raise, this IS a string
 
     def json(self):
         return json.loads(self.text())
 
     def soup(
         self,
-        engine: str = "lxml",
+        engine: str = "html.parser",
         ignore_xhtml_warning=False,
         strainer: Optional[SoupStrainer] = None,
     ) -> WonderfulSoup:
         with suppress_xml_parsed_as_html_warnings(bypass=not ignore_xhtml_warning):
             return WonderfulSoup(self.text(), engine, parse_only=strainer)
 
     def links(self, unique: bool = True, strip_fragment: bool = False) -> List[str]:
@@ -1118,15 +1119,15 @@
 
 
 def request_jsonrpc(
     url: str,
     method: str,
     pool_manager: urllib3.PoolManager = DEFAULT_POOL_MANAGER,
     *args,
-    **kwargs
+    **kwargs,
 ) -> Response:
     params = []
 
     if len(args) > 0:
         params = args
     elif len(kwargs) > 0:
         params = kwargs
```

### Comparing `minet-1.5.1/minet/wikipedia/wikimedia_rest_api_client.py` & `minet-2.0.0/minet/wikipedia/wikimedia_rest_api_client.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/youtube/client.py` & `minet-2.0.0/minet/youtube/client.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/youtube/constants.py` & `minet-2.0.0/minet/youtube/constants.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/youtube/exceptions.py` & `minet-2.0.0/minet/youtube/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/youtube/scraper.py` & `minet-2.0.0/minet/youtube/scraper.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/youtube/types.py` & `minet-2.0.0/minet/youtube/types.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/youtube/urls.py` & `minet-2.0.0/minet/youtube/urls.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet/youtube/utils.py` & `minet-2.0.0/minet/youtube/utils.py`

 * *Files identical despite different names*

### Comparing `minet-1.5.1/minet.egg-info/PKG-INFO` & `minet-2.0.0/minet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: minet
-Version: 1.5.1
+Version: 2.0.0
 Summary: A webmining CLI tool & library for python.
 Home-page: http://github.com/medialab/minet
 Author: Guillaume Plique, Pauline Breteau, Jules Farjas, Héloïse Théro, Jean Descamps, Amélie Pellé, Laura Miguel, César Pichon, Kelly Christensen
 License: GPL-3.0
 Keywords: webmining
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: about-time<5,>=4
 Requires-Dist: beautifulsoup4<5,>=4.7.1
 Requires-Dist: browser-cookie3==0.19.1
 Requires-Dist: casanova<3,>=2.0.1
 Requires-Dist: charset-normalizer<4,>=3
 Requires-Dist: dateparser>=1.1.1
 Requires-Dist: ebbe<2,>=1.13
 Requires-Dist: json5>=0.8.5
-Requires-Dist: lxml>=4.3.0
+Requires-Dist: lxml<5.2,>=4.3.0
 Requires-Dist: nanoid<3,>=2
-Requires-Dist: playwright<1.36,>=1.35
-Requires-Dist: playwright_stealth<2,>=1
+Requires-Dist: playwright<1.44,>=1.43
+Requires-Dist: playwright_stealth<2,>=1.0.6
 Requires-Dist: pyyaml
 Requires-Dist: quenouille<2,>=1.9.1
 Requires-Dist: rich<14,>=13
 Requires-Dist: rich-argparse<2,>=1
 Requires-Dist: soupsieve<3,>=2.1
 Requires-Dist: tenacity<9,>=8
-Requires-Dist: trafilatura<1.8,>=1.7
+Requires-Dist: trafilatura<1.9,>=1.8.1
 Requires-Dist: twitwi<0.19,>=0.18.2
 Requires-Dist: ural<2,>=1.3.2
 Requires-Dist: urllib3<2,>=1.26.16
 Requires-Dist: typing_extensions>=4.3; python_version < "3.11"
 
 [![Build Status](https://github.com/medialab/minet/workflows/Tests/badge.svg)](https://github.com/medialab/minet/actions) [![DOI](https://zenodo.org/badge/169059797.svg)](https://zenodo.org/badge/latestdoi/169059797) [![download number](https://static.pepy.tech/badge/minet)](https://pepy.tech/project/minet)
```

### Comparing `minet-1.5.1/minet.egg-info/SOURCES.txt` & `minet-2.0.0/minet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,14 @@
 minet.egg-info/PKG-INFO
 minet.egg-info/SOURCES.txt
 minet.egg-info/dependency_links.txt
 minet.egg-info/entry_points.txt
 minet.egg-info/requires.txt
 minet.egg-info/top_level.txt
 minet.egg-info/zip-safe
-minet/__future__/__init__.py
-minet/__future__/threaded_child_watcher.py
 minet/browser/__init__.py
 minet/browser/constants.py
 minet/browser/extensions.py
 minet/browser/plawright_shim.py
 minet/browser/threadsafe_browser.py
 minet/browser/utils.py
 minet/buzzsumo/__init__.py
```

### Comparing `minet-1.5.1/setup.py` & `minet-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,36 +18,36 @@
     description="A webmining CLI tool & library for python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/medialab/minet",
     author="Guillaume Plique, Pauline Breteau, Jules Farjas, Héloïse Théro, Jean Descamps, Amélie Pellé, Laura Miguel, César Pichon, Kelly Christensen",
     keywords="webmining",
     license="GPL-3.0",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     packages=packages,
     install_requires=[
         "about-time>=4,<5",
         "beautifulsoup4>=4.7.1,<5",
         "browser-cookie3==0.19.1",
         "casanova>=2.0.1,<3",
         "charset-normalizer>=3,<4",
         "dateparser>=1.1.1",
         "ebbe>=1.13,<2",
         "json5>=0.8.5",
-        "lxml>=4.3.0",
+        "lxml>=4.3.0,<5.2",
         "nanoid>=2,<3",
-        "playwright>=1.35,<1.36",
-        "playwright_stealth>=1,<2",
+        "playwright>=1.43,<1.44",
+        "playwright_stealth>=1.0.6,<2",
         "pyyaml",
         "quenouille>=1.9.1,<2",
         "rich>=13,<14",
         "rich-argparse>=1,<2",
         "soupsieve>=2.1,<3",
         "tenacity>=8,<9",
-        "trafilatura>=1.7,<1.8",
+        "trafilatura>=1.8.1,<1.9",
         "twitwi>=0.18.2,<0.19",
         "ural>=1.3.2,<2",
         "urllib3>=1.26.16,<2",
     ],
     extras_require={
         ":python_version<'3.11'": ["typing_extensions>=4.3"],
     },
```

