# Comparing `tmp/twikit-1.5.0.tar.gz` & `tmp/twikit-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.5.0.tar", last modified: Mon Apr 15 14:52:51 2024, max compression
+gzip compressed data, was "twikit-1.5.1.tar", last modified: Tue Apr 16 15:19:30 2024, max compression
```

## Comparing `twikit-1.5.0.tar` & `twikit-1.5.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 14:52:51.348049 twikit-1.5.0/
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-04-15 14:52:51.345054 twikit-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 14:52:51.349044 twikit-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:52:51.263274 twikit-1.5.0/twikit/
--rw-rw-rw-   0        0        0      620 2024-04-15 14:49:26.000000 twikit-1.5.0/twikit/__init__.py
--rw-rw-rw-   0        0        0   131589 2024-04-15 14:28:49.000000 twikit-1.5.0/twikit/client.py
--rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.0/twikit/community.py
--rw-rw-rw-   0        0        0     2626 2024-04-14 11:15:08.000000 twikit-1.5.0/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.0/twikit/group.py
--rw-rw-rw-   0        0        0     2095 2024-04-14 11:11:34.000000 twikit-1.5.0/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.0/twikit/notification.py
--rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/trend.py
--rw-rw-rw-   0        0        0    20744 2024-04-14 15:05:06.000000 twikit-1.5.0/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:52:51.342062 twikit-1.5.0/twikit/twikit_async/
--rw-rw-rw-   0        0        0      572 2024-04-15 14:48:54.000000 twikit-1.5.0/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0   133874 2024-04-15 14:40:16.000000 twikit-1.5.0/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.0/twikit/twikit_async/community.py
--rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.0/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    20613 2024-04-14 11:18:02.000000 twikit-1.5.0/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-04-14 04:11:42.000000 twikit-1.5.0/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-04-14 04:11:03.000000 twikit-1.5.0/twikit/user.py
--rw-rw-rw-   0        0        0    24789 2024-04-15 12:37:05.000000 twikit-1.5.0/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:52:51.287209 twikit-1.5.0/twikit.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-04-15 14:52:50.000000 twikit-1.5.0/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2024-04-15 14:52:51.000000 twikit-1.5.0/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 14:52:50.000000 twikit-1.5.0/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-15 14:52:50.000000 twikit-1.5.0/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 14:52:50.000000 twikit-1.5.0/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 15:19:30.407811 twikit-1.5.1/
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-16 15:19:30.404823 twikit-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 15:19:30.407811 twikit-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:19:30.293120 twikit-1.5.1/twikit/
+-rw-rw-rw-   0        0        0      620 2024-04-16 15:17:55.000000 twikit-1.5.1/twikit/__init__.py
+-rw-rw-rw-   0        0        0   132489 2024-04-16 15:17:16.000000 twikit-1.5.1/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.1/twikit/community.py
+-rw-rw-rw-   0        0        0     2626 2024-04-14 11:15:08.000000 twikit-1.5.1/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.1/twikit/group.py
+-rw-rw-rw-   0        0        0     2095 2024-04-14 11:11:34.000000 twikit-1.5.1/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.1/twikit/notification.py
+-rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/trend.py
+-rw-rw-rw-   0        0        0    20836 2024-04-16 15:06:59.000000 twikit-1.5.1/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:19:30.401828 twikit-1.5.1/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      572 2024-04-15 14:48:54.000000 twikit-1.5.1/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0   134756 2024-04-16 15:17:50.000000 twikit-1.5.1/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.1/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.1/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    20701 2024-04-15 15:04:49.000000 twikit-1.5.1/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14740 2024-04-14 04:11:42.000000 twikit-1.5.1/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14517 2024-04-14 04:11:03.000000 twikit-1.5.1/twikit/user.py
+-rw-rw-rw-   0        0        0    24789 2024-04-15 12:37:05.000000 twikit-1.5.1/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:19:30.313065 twikit-1.5.1/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-16 15:19:29.000000 twikit-1.5.1/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2024-04-16 15:19:30.000000 twikit-1.5.1/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 15:19:29.000000 twikit-1.5.1/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-16 15:19:29.000000 twikit-1.5.1/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 15:19:29.000000 twikit-1.5.1/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.5.0/LICENSE` & `twikit-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/PKG-INFO` & `twikit-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.0
+Version: 1.5.1
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.0/README.md` & `twikit-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/setup.py` & `twikit-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/__init__.py` & `twikit-1.5.1/twikit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========================
 Twikit Twitter API Wrapper
 ==========================
 
 A Python library for interacting with the Twitter API.
 """
 
-__version__ = '1.5.0'
+__version__ = '1.5.1'
 
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .errors import *
 from .group import Group, GroupMessage
 from .list import List
```

### Comparing `twikit-1.5.0/twikit/client.py` & `twikit-1.5.1/twikit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -901,15 +901,17 @@
         self,
         text: str = '',
         media_ids: list[str] | None = None,
         poll_uri: str | None = None,
         reply_to: str | None = None,
         conversation_control: Literal[
             'followers', 'verified', 'mentioned'] | None = None,
-        attachment_url: str | None = None
+        attachment_url: str | None = None,
+        community_id: str | None = None,
+        share_with_followers: bool = False
     ) -> Tweet:
         """
         Creates a new tweet on Twitter with the specified
         text, media, and poll.
 
         Parameters
         ----------
@@ -1003,14 +1005,22 @@
             variables['conversation_control'] = {
                 'mode': limit_mode
             }
 
         if attachment_url is not None:
             variables['attachment_url'] = attachment_url
 
+        if community_id is not None:
+            variables['semantic_annotation_ids'] = [{
+                'entity_id': community_id,
+                'group_id': '8',
+                'domain_id': '31'
+            }]
+            variables['broadcast'] = share_with_followers
+
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_TWEET),
             'features': FEATURES,
         }
         response = self.http.post(
             Endpoint.CREATE_TWEET,
@@ -2382,15 +2392,16 @@
 
     def get_trends(
         self,
         category: Literal[
             'trending', 'for-you', 'news', 'sports', 'entertainment'
         ],
         count: int = 20,
-        retry: bool = True
+        retry: bool = True,
+        additional_request_params: dict | None = None
     ) -> list[Trend]:
         """
         Retrieves trending topics on Twitter.
 
         Parameters
         ----------
         category : {'trending', 'for-you', 'news', 'sports', 'entertainment'}
@@ -2400,14 +2411,19 @@
             - 'news': News-related trends.
             - 'sports': Sports-related trends.
             - 'entertainment': Entertainment-related trends.
         count : :class:`int`, default=20
             The number of trends to retrieve.
         retry : :class:`bool`, default=True
             If no trends are fetched continuously retry to fetch trends.
+        additional_request_params : :class:`dict`, default=None
+            Parameters to be added on top of the existing trends API
+            parameters. Typically, it is used as `additional_request_params =
+            {'candidate_source': 'trends'}` when this function doesn't work
+            otherwise.
 
         Returns
         -------
         list[:class:`Trend`]
             A list of Trend objects representing the retrieved trends.
 
         Examples
@@ -2423,14 +2439,16 @@
         if category in ['news', 'sports', 'entertainment']:
             category += '_unified'
         params = {
             'count': count,
             'include_page_configuration': True,
             'initial_tab_id': category
         }
+        if additional_request_params is not None:
+            params |= additional_request_params
         response = self.http.get(
             Endpoint.TREND,
             params=params,
             headers=self._base_headers
         ).json()
 
         entry_id_prefix = 'trends' if category == 'trending' else 'Guide'
@@ -2440,15 +2458,17 @@
         ]
 
         if not entries:
             if not retry:
                 return []
             # Recall the method again, as the trend information
             # may not be returned due to a Twitter error.
-            return self.get_trends(category, count, retry)
+            return self.get_trends(
+                category, count, retry, additional_request_params
+            )
 
         items = entries[-1]['content']['timelineModule']['items']
 
         results = []
         for item in items:
             trend_info = item['item']['content']['trend']
             results.append(Trend(self, trend_info))
```

### Comparing `twikit-1.5.0/twikit/community.py` & `twikit-1.5.1/twikit/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/errors.py` & `twikit-1.5.1/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/group.py` & `twikit-1.5.1/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/http.py` & `twikit-1.5.1/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/list.py` & `twikit-1.5.1/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/message.py` & `twikit-1.5.1/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/notification.py` & `twikit-1.5.1/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/trend.py` & `twikit-1.5.1/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/tweet.py` & `twikit-1.5.1/twikit/tweet.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,16 @@
             hashtags = legacy['entities'].get('hashtags', [])
         self.hashtags: list[str] = [
             i['text'] for i in hashtags
         ]
 
         if (
             'card' in data and
+            'legacy' in data['card'] and
+            'name' in data['card']['legacy'] and
             data['card']['legacy']['name'].startswith('poll')
         ):
             self._poll_data = data['card']
         else:
             self._poll_data = None
 
     @property
```

### Comparing `twikit-1.5.0/twikit/twikit_async/__init__.py` & `twikit-1.5.1/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/twikit_async/client.py` & `twikit-1.5.1/twikit/twikit_async/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,18 @@
     build_tweet_data,
     build_user_data,
     find_dict,
     flatten_params,
     get_query_id,
     urlencode
 )
-from .community import CommunityRule, Community, CommunityCreator, CommunityMember
+from .community import (
+    Community,
+    CommunityMember
+)
 from .group import Group, GroupMessage
 from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Trend
 from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet
@@ -912,15 +915,17 @@
         self,
         text: str = '',
         media_ids: list[str] | None = None,
         poll_uri: str | None = None,
         reply_to: str | None = None,
         conversation_control: Literal[
             'followers', 'verified', 'mentioned'] | None = None,
-        attachment_url: str | None = None
+        attachment_url: str | None = None,
+        community_id: str | None = None,
+        share_with_followers: bool = False
     ) -> Tweet:
         """
         Creates a new tweet on Twitter with the specified
         text, media, and poll.
 
         Parameters
         ----------
@@ -1014,14 +1019,22 @@
             variables['conversation_control'] = {
                 'mode': limit_mode
             }
 
         if attachment_url is not None:
             variables['attachment_url'] = attachment_url
 
+        if community_id is not None:
+            variables['semantic_annotation_ids'] = [{
+                'entity_id': community_id,
+                'group_id': '8',
+                'domain_id': '31'
+            }]
+            variables['broadcast'] = share_with_followers
+
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_TWEET),
             'features': FEATURES,
         }
         response = (await self.http.post(
             Endpoint.CREATE_TWEET,
@@ -2400,15 +2413,16 @@
 
     async def get_trends(
         self,
         category: Literal[
             'trending', 'for-you', 'news', 'sports', 'entertainment'
         ],
         count: int = 20,
-        retry: bool = True
+        retry: bool = True,
+        additional_request_params: dict | None = None
     ) -> list[Trend]:
         """
         Retrieves trending topics on Twitter.
 
         Parameters
         ----------
         category : {'trending', 'for-you', 'news', 'sports', 'entertainment'}
@@ -2418,14 +2432,19 @@
             - 'news': News-related trends.
             - 'sports': Sports-related trends.
             - 'entertainment': Entertainment-related trends.
         count : :class:`int`, default=20
             The number of trends to retrieve.
         retry : :class:`bool`, default=True
             If no trends are fetched continuously retry to fetch trends.
+        additional_request_params : :class:`dict`, default=None
+            Parameters to be added on top of the existing trends API
+            parameters. Typically, it is used as `additional_request_params =
+            {'candidate_source': 'trends'}` when this function doesn't work
+            otherwise.
 
         Returns
         -------
         list[:class:`Trend`]
             A list of Trend objects representing the retrieved trends.
 
         Examples
@@ -2441,14 +2460,16 @@
         if category in ['news', 'sports', 'entertainment']:
             category += '_unified'
         params = {
             'count': count,
             'include_page_configuration': True,
             'initial_tab_id': category
         }
+        if additional_request_params is not None:
+            params |= additional_request_params
         response = (await self.http.get(
             Endpoint.TREND,
             params=params,
             headers=self._base_headers
         )).json()
 
         entry_id_prefix = 'trends' if category == 'trending' else 'Guide'
@@ -2458,15 +2479,17 @@
         ]
 
         if not entries:
             if not retry:
                 return []
             # Recall the method again, as the trend information
             # may not be returned due to a Twitter error.
-            return await self.get_trends(category, count, retry)
+            return await self.get_trends(
+                category, count, retry, additional_request_params
+            )
 
         items = entries[-1]['content']['timelineModule']['items']
 
         results = []
         for item in items:
             trend_info = item['item']['content']['trend']
             results.append(Trend(self, trend_info))
```

### Comparing `twikit-1.5.0/twikit/twikit_async/community.py` & `twikit-1.5.1/twikit/twikit_async/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/twikit_async/errors.py` & `twikit-1.5.1/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/twikit_async/group.py` & `twikit-1.5.1/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/twikit_async/http.py` & `twikit-1.5.1/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/twikit_async/list.py` & `twikit-1.5.1/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/twikit_async/message.py` & `twikit-1.5.1/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/twikit_async/notification.py` & `twikit-1.5.1/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/twikit_async/trend.py` & `twikit-1.5.1/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/twikit_async/tweet.py` & `twikit-1.5.1/twikit/twikit_async/tweet.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,18 +166,20 @@
                 hashtags = []
         else:
             hashtags = legacy['entities'].get('hashtags', [])
         self.hashtags: list[str] = [
             i['text'] for i in hashtags
         ]
 
-        if (
-            'card' in data and
+        if all([
+            'card' in data,
+            'legacy' in data['card'],
+            'name' in data['card']['legacy'],
             data['card']['legacy']['name'].startswith('poll')
-        ):
+        ]):
             self._poll_data = data['card']
         else:
             self._poll_data = None
 
     @property
     def created_at_datetime(self) -> datetime:
         return timestamp_to_datetime(self.created_at)
```

### Comparing `twikit-1.5.0/twikit/twikit_async/user.py` & `twikit-1.5.1/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/twikit_async/utils.py` & `twikit-1.5.1/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/user.py` & `twikit-1.5.1/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit/utils.py` & `twikit-1.5.1/twikit/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.0/twikit.egg-info/PKG-INFO` & `twikit-1.5.1/twikit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.0
+Version: 1.5.1
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.0/twikit.egg-info/SOURCES.txt` & `twikit-1.5.1/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

