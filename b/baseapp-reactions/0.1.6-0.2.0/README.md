# Comparing `tmp/baseapp-reactions-0.1.6.tar.gz` & `tmp/baseapp-reactions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseapp-reactions-0.1.6.tar", last modified: Fri Mar  1 14:50:27 2024, max compression
+gzip compressed data, was "baseapp-reactions-0.2.0.tar", last modified: Tue Apr 16 11:13:22 2024, max compression
```

## Comparing `baseapp-reactions-0.1.6.tar` & `baseapp-reactions-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:27.891110 baseapp-reactions-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-03-01 14:50:27.891110 baseapp-reactions-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:27.891110 baseapp-reactions-0.1.6/baseapp_reactions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:27.891110 baseapp-reactions-0.1.6/baseapp_reactions/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/graphql/mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/graphql/object_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/graphql/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:27.891110 baseapp-reactions-0.1.6/baseapp_reactions/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/migrations/0002_alter_reaction_id.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:27.891110 baseapp-reactions-0.1.6/baseapp_reactions/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/tests/test_graphql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/baseapp_reactions/tests/test_graphql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:27.891110 baseapp-reactions-0.1.6/baseapp_reactions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-03-01 14:50:27.000000 baseapp-reactions-0.1.6/baseapp_reactions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-01 14:50:27.000000 baseapp-reactions-0.1.6/baseapp_reactions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 14:50:27.000000 baseapp-reactions-0.1.6/baseapp_reactions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-01 14:50:27.000000 baseapp-reactions-0.1.6/baseapp_reactions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-01 14:50:27.000000 baseapp-reactions-0.1.6/baseapp_reactions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-01 14:50:27.895110 baseapp-reactions-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:27.891110 baseapp-reactions-0.1.6/testproject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/testproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-01 14:50:26.000000 baseapp-reactions-0.1.6/testproject/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:22.561099 baseapp-reactions-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-16 11:13:22.561099 baseapp-reactions-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:22.557099 baseapp-reactions-0.2.0/baseapp_reactions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:22.557099 baseapp-reactions-0.2.0/baseapp_reactions/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/graphql/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/graphql/object_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/graphql/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:22.557099 baseapp-reactions-0.2.0/baseapp_reactions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/migrations/0002_alter_reaction_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:22.557099 baseapp-reactions-0.2.0/baseapp_reactions/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/tests/test_graphql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/baseapp_reactions/tests/test_graphql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:22.557099 baseapp-reactions-0.2.0/baseapp_reactions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-16 11:13:22.000000 baseapp-reactions-0.2.0/baseapp_reactions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-16 11:13:22.000000 baseapp-reactions-0.2.0/baseapp_reactions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:13:22.000000 baseapp-reactions-0.2.0/baseapp_reactions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 11:13:22.000000 baseapp-reactions-0.2.0/baseapp_reactions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 11:13:22.000000 baseapp-reactions-0.2.0/baseapp_reactions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-16 11:13:22.561099 baseapp-reactions-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:22.557099 baseapp-reactions-0.2.0/testproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:22.561099 baseapp-reactions-0.2.0/testproject/testapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/testapp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/testapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:22.561099 baseapp-reactions-0.2.0/testproject/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 11:13:20.000000 baseapp-reactions-0.2.0/testproject/wsgi.py
```

### Comparing `baseapp-reactions-0.1.6/PKG-INFO` & `baseapp-reactions-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,86 @@
 Metadata-Version: 2.1
 Name: baseapp-reactions
-Version: 0.1.6
+Version: 0.2.0
 Summary: BaseApp Reactions
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp Reactions
         
         Reusable app to enable User's reactions on any model, features like like/dislike or any other reactions type, customizable for project's needs.
         
         ## How to install:
         
-        Add dependencies to your `requirements/base.txt` file:
+        Install in your environment:
         
+        ```bash
+        pip install baseapp-reactions
         ```
-        baseapp-core @ git+https://github.com/silverlogic/baseapp-backend.git@v0.1#subdirectory=baseapp-core
-        baseapp-reactions @ git+https://github.com/silverlogic/baseapp-backend.git@v0.1#subdirectory=baseapp-reactions
-        ```
-        
-        And run provision or manually `pip install -r requirements/base.ext`
         
         If you want to develop, [install using this other guide](#how-to-develop).
         
         ## How to use
         
         Add `baseapp_reactions` to your project's `INSTALLED_APPS`
         
+        ```python
+        INSTALLED_APPS = [
+            # ...
+            "baseapp_reactions",
+            # ...
+        ]
+        ```
+        
+        Add `baseapp_reactions.permissions.ReactionsPermissionsBackend` to the `AUTHENTICATION_BACKENDS` list in your django settings file.
+        
+        ```python
+        AUTHENTICATION_BACKENDS = [
+            # ...
+            "baseapp_reactions.permissions.ReactionsPermissionsBackend",
+            # ...
+        ]
+        ```
+        
         Now make sure all models you'd like to get reactions also inherits `ReactableModel`, like:
         
         ```python
         from baseapp_reactions.models import ReactableModel
         
         class Comment(models.Model, ReactableModel):
             body = models.Textfield()
         ```
         
-        Also make sure your GraphQL object types extends `ReactionsNode` interface:
+        Also make sure your GraphQL object types extends `ReactionsInterface` interface:
         
         ```python
-        from baseapp_reactions.graphql.object_types import ReactionsNode
+        from baseapp_reactions.graphql.object_types import ReactionsInterface
         
         class CommentNode(DjangoObjectType):
             class Meta:
-                interfaces = (relay.Node, ReactionsNode)
+                interfaces = (relay.Node, ReactionsInterface)
         ```
         
-        Expose `ReactionsMutations` and `ReactionsQuery` in your GraphQL/graphene endpoint, like:
+        Expose `ReactionsMutations` and `ReactionsQueries` in your GraphQL/graphene endpoint, like:
         
         ```python
         from baseapp_reactions.graphql.mutations import ReactionsMutations
-        from baseapp_reactions.graphql.queries import ReactionsQuery
+        from baseapp_reactions.graphql.queries import ReactionsQueries
         
-        class Query(graphene.ObjectType, ReactionsQuery):
+        class Query(graphene.ObjectType, ReactionsQueries):
             pass
         
         class Mutation(graphene.ObjectType, ReactionsMutations):
             pass
         
         schema = graphene.Schema(query=Query, mutation=Mutation)
         ```
         
-        This will expose `reactionToggle` mutation and add fields and connections to all your GraphqlQL Object Types using interface `ReactionsNode`.
+        This will expose `reactionToggle` mutation and add fields and connections to all your GraphqlQL Object Types using interface `ReactionsInterface`.
         
         Example:
         
         ```graphql
         {
             comment(id: $id) {
                 id
@@ -124,38 +139,14 @@
         
         Now in your `settings/base.py` make sure to tell baseapp-reactions what is your custom model for Reaction:
         
         ```python
         BASEAPP_REACTIONS_REACTION_MODEL = 'reactions.Reaction'
         ```
         
-        ## Writing test cases in your project
-        
-        There is a `AbstractReactionFactory` which helps you write other factories:
-        
-        ```
-        import factory
-        from baseapp_reactions.tests.factories import AbstractReactionFactory
-        
-        class CommentFactory(factory.django.DjangoModelFactory):
-            class Meta:
-                model = "comments.Comment"
-        
-        
-        class CommentReactionFactory(AbstractReactionFactory):
-            target = factory.SubFactory(CommentFactory)
-        
-            class Meta:
-                model = "baseapp_reactions.Reaction"
-                # OR if you have a custom model, point to it:
-                model = "reactions.Reaction"
-        ```
-        
-        In the above example we have a easy way to make reactions to any comment into the database for testing proporses using `CommentReactionFactory`.
-        
         ## How to develop
         
         Clone the project inside your project's backend dir:
         
         ```
         git clone git@github.com:silverlogic/baseapp-backend.git
         ```
```

### Comparing `baseapp-reactions-0.1.6/README.md` & `baseapp-reactions-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,78 @@
 # BaseApp Reactions
 
 Reusable app to enable User's reactions on any model, features like like/dislike or any other reactions type, customizable for project's needs.
 
 ## How to install:
 
-Add dependencies to your `requirements/base.txt` file:
+Install in your environment:
 
+```bash
+pip install baseapp-reactions
 ```
-baseapp-core @ git+https://github.com/silverlogic/baseapp-backend.git@v0.1#subdirectory=baseapp-core
-baseapp-reactions @ git+https://github.com/silverlogic/baseapp-backend.git@v0.1#subdirectory=baseapp-reactions
-```
-
-And run provision or manually `pip install -r requirements/base.ext`
 
 If you want to develop, [install using this other guide](#how-to-develop).
 
 ## How to use
 
 Add `baseapp_reactions` to your project's `INSTALLED_APPS`
 
+```python
+INSTALLED_APPS = [
+    # ...
+    "baseapp_reactions",
+    # ...
+]
+```
+
+Add `baseapp_reactions.permissions.ReactionsPermissionsBackend` to the `AUTHENTICATION_BACKENDS` list in your django settings file.
+
+```python
+AUTHENTICATION_BACKENDS = [
+    # ...
+    "baseapp_reactions.permissions.ReactionsPermissionsBackend",
+    # ...
+]
+```
+
 Now make sure all models you'd like to get reactions also inherits `ReactableModel`, like:
 
 ```python
 from baseapp_reactions.models import ReactableModel
 
 class Comment(models.Model, ReactableModel):
     body = models.Textfield()
 ```
 
-Also make sure your GraphQL object types extends `ReactionsNode` interface:
+Also make sure your GraphQL object types extends `ReactionsInterface` interface:
 
 ```python
-from baseapp_reactions.graphql.object_types import ReactionsNode
+from baseapp_reactions.graphql.object_types import ReactionsInterface
 
 class CommentNode(DjangoObjectType):
     class Meta:
-        interfaces = (relay.Node, ReactionsNode)
+        interfaces = (relay.Node, ReactionsInterface)
 ```
 
-Expose `ReactionsMutations` and `ReactionsQuery` in your GraphQL/graphene endpoint, like:
+Expose `ReactionsMutations` and `ReactionsQueries` in your GraphQL/graphene endpoint, like:
 
 ```python
 from baseapp_reactions.graphql.mutations import ReactionsMutations
-from baseapp_reactions.graphql.queries import ReactionsQuery
+from baseapp_reactions.graphql.queries import ReactionsQueries
 
-class Query(graphene.ObjectType, ReactionsQuery):
+class Query(graphene.ObjectType, ReactionsQueries):
     pass
 
 class Mutation(graphene.ObjectType, ReactionsMutations):
     pass
 
 schema = graphene.Schema(query=Query, mutation=Mutation)
 ```
 
-This will expose `reactionToggle` mutation and add fields and connections to all your GraphqlQL Object Types using interface `ReactionsNode`.
+This will expose `reactionToggle` mutation and add fields and connections to all your GraphqlQL Object Types using interface `ReactionsInterface`.
 
 Example:
 
 ```graphql
 {
     comment(id: $id) {
         id
@@ -116,38 +131,14 @@
 
 Now in your `settings/base.py` make sure to tell baseapp-reactions what is your custom model for Reaction:
 
 ```python
 BASEAPP_REACTIONS_REACTION_MODEL = 'reactions.Reaction'
 ```
 
-## Writing test cases in your project
-
-There is a `AbstractReactionFactory` which helps you write other factories:
-
-```
-import factory
-from baseapp_reactions.tests.factories import AbstractReactionFactory
-
-class CommentFactory(factory.django.DjangoModelFactory):
-    class Meta:
-        model = "comments.Comment"
-
-
-class CommentReactionFactory(AbstractReactionFactory):
-    target = factory.SubFactory(CommentFactory)
-
-    class Meta:
-        model = "baseapp_reactions.Reaction"
-        # OR if you have a custom model, point to it:
-        model = "reactions.Reaction"
-```
-
-In the above example we have a easy way to make reactions to any comment into the database for testing proporses using `CommentReactionFactory`.
-
 ## How to develop
 
 Clone the project inside your project's backend dir:
 
 ```
 git clone git@github.com:silverlogic/baseapp-backend.git
 ```
```

### Comparing `baseapp-reactions-0.1.6/baseapp_reactions/graphql/mutations.py` & `baseapp-reactions-0.2.0/baseapp_reactions/graphql/mutations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import graphene
 import swapper
 from baseapp_core.graphql import RelayMutation, login_required
 from baseapp_core.utils import get_content_type_by_natural_key
 from django.contrib.contenttypes.models import ContentType
 from django.utils.translation import gettext_lazy as _
 from graphql.error import GraphQLError
-from graphql_relay import to_global_id
 from graphql_relay.connection.arrayconnection import offset_to_cursor
 from graphql_relay.node.node import from_global_id
 
-from .object_types import ReactionNode, ReactionsNode, ReactionTypesEnum
+from .object_types import ReactionObjectType, ReactionsInterface, ReactionTypesEnum
 
 Reaction = swapper.load_model("baseapp_reactions", "Reaction")
 
 
 class ReactionToggle(RelayMutation):
-    reaction = graphene.Field(ReactionNode._meta.connection.Edge, required=False)
-    target = graphene.Field(ReactionsNode)
+    reaction = graphene.Field(ReactionObjectType._meta.connection.Edge, required=False)
+    target = graphene.Field(ReactionsInterface)
     reaction_deleted_id = graphene.ID(required=False)
 
     class Input:
         target_object_id = graphene.ID(required=True)
         target_content_type = graphene.String(
             required=False,
             description=_(
@@ -40,54 +39,53 @@
         target_content_type = input.get("target_content_type")
         if target_content_type:
             content_type = get_content_type_by_natural_key(target_content_type)
             target = content_type.get_object_for_this_type(pk=gid)
         else:
             content_type = ContentType.objects.get_for_model(target)
 
-        # check https://github.com/queplanta/backend/blob/master/accounts/permissions.py#L9
-        if "reaction-add" not in target.get_my_permissions(info.context):
+        if not info.context.user.has_perm("baseapp_reactions.add_reaction", target):
             raise GraphQLError(
                 str(_("You don't have permission to perform this action")),
                 extensions={"code": "permission_required"},
             )
-            # return cls(e)
-        # target.has_permission(info.context, 'reaction')
 
         reaction, created = Reaction.objects.get_or_create(
             user=info.context.user,
             target_object_id=target.pk,
             target_content_type=content_type,
             defaults={"reaction_type": reaction_type},
         )
         if not created:
             if reaction.reaction_type == reaction_type:
-                if "reaction-delete" not in target.get_my_permissions(info.context):
+                if not info.context.user.has_perm("baseapp_reactions.delete_reaction", reaction):
                     raise GraphQLError(
                         str(_("You don't have permission to perform this action")),
                         extensions={"code": "permission_required"},
                     )
 
-                reaction_deleted_id = to_global_id(ReactionNode._meta.name, reaction.pk)
+                reaction_deleted_id = reaction.relay_id
                 reaction.delete()
                 target.refresh_from_db()
                 return ReactionToggle(target=target, reaction_deleted_id=reaction_deleted_id)
 
-            if "reaction-change" not in target.get_my_permissions(info.context):
+            if not info.context.user.has_perm("baseapp_reactions.change_reaction", reaction):
                 raise GraphQLError(
                     str(_("You don't have permission to perform this action")),
                     extensions={"code": "permission_required"},
                 )
 
             reaction.reaction_type = reaction_type
             reaction.save()
 
         target.refresh_from_db()
 
         return ReactionToggle(
-            reaction=ReactionNode._meta.connection.Edge(node=reaction, cursor=offset_to_cursor(0)),
+            reaction=ReactionObjectType._meta.connection.Edge(
+                node=reaction, cursor=offset_to_cursor(0)
+            ),
             target=target,
         )
 
 
 class ReactionsMutations(object):
     reaction_toggle = ReactionToggle.Field()
```

### Comparing `baseapp-reactions-0.1.6/baseapp_reactions/graphql/object_types.py` & `baseapp-reactions-0.2.0/baseapp_reactions/graphql/object_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import graphene
 import graphene_django_optimizer as gql_optimizer
 import swapper
 from baseapp_core.graphql import DjangoObjectType
+from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from graphene import relay
 from graphene_django.filter import DjangoFilterConnectionField
 
 Reaction = swapper.load_model("baseapp_reactions", "Reaction")
 
 ReactionTypesEnum = graphene.Enum.from_enum(Reaction.ReactionTypes)
@@ -18,20 +19,30 @@
     fields["total"] = graphene.Int()
     return type(name, (graphene.ObjectType,), fields)
 
 
 ReactionsCount = create_object_type_from_enum("ReactionsCount", Reaction.ReactionTypes)
 
 
-class ReactionsNode(relay.Node):
+class ReactionsInterface(relay.Node):
     reactions_count = graphene.Field(ReactionsCount)
-    reactions = DjangoFilterConnectionField(lambda: ReactionNode)
-    my_reaction = graphene.Field(lambda: ReactionNode, required=False)
+    reactions = DjangoFilterConnectionField(lambda: ReactionObjectType)
+    is_reactions_enabled = graphene.Boolean(required=True)
+    my_reaction = graphene.Field(lambda: ReactionObjectType, required=False)
 
     def resolve_reactions(self, info, **kwargs):
+        if not getattr(self, "is_reactions_enabled", True):
+            return Reaction.objects.none()
+
+        CAN_ANONYMOUS_VIEW_REACTIONS = getattr(
+            settings, "BASEAPP_REACTIONS_CAN_ANONYMOUS_VIEW_REACTIONSS", True
+        )
+        if not CAN_ANONYMOUS_VIEW_REACTIONS and not info.context.user.is_authenticated:
+            return Reaction.objects.none()
+
         target_content_type = ContentType.objects.get_for_model(self)
         return Reaction.objects.filter(
             target_content_type=target_content_type,
             target_object_id=self.pk,
         ).order_by("-created")
 
     def resolve_my_reaction(self, info, **kwargs):
@@ -40,15 +51,15 @@
             return Reaction.objects.filter(
                 target_content_type=target_content_type,
                 target_object_id=self.pk,
                 user=info.context.user,
             ).first()
 
 
-class ReactionNode(gql_optimizer.OptimizedDjangoObjectType, DjangoObjectType):
+class ReactionObjectType(gql_optimizer.OptimizedDjangoObjectType, DjangoObjectType):
     target = graphene.Field(relay.Node)
     reaction_type = graphene.Field(ReactionTypesEnum)
 
     class Meta:
         interfaces = (relay.Node,)
         model = Reaction
         fields = (
@@ -58,7 +69,14 @@
             "created",
             "modified",
             "target",
         )
         filter_fields = {
             "id": ["exact"],
         }
+
+    @classmethod
+    def get_node(self, info, id):
+        node = super().get_node(info, id)
+        if not info.context.user.has_perm("baseapp_comments.view_comment", node):
+            return None
+        return node
```

### Comparing `baseapp-reactions-0.1.6/baseapp_reactions/migrations/0001_initial.py` & `baseapp-reactions-0.2.0/baseapp_reactions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `baseapp-reactions-0.1.6/baseapp_reactions/models.py` & `baseapp-reactions-0.2.0/baseapp_reactions/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import swapper
+from baseapp_core.graphql import RelayModel
 from django.conf import settings
 from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from model_utils.models import TimeStampedModel
 
@@ -14,15 +15,15 @@
 
     for reaction_type in ReactionModel.ReactionTypes:
         d[reaction_type.name] = 0
 
     return d
 
 
-class AbstractBaseReaction(TimeStampedModel):
+class AbstractBaseReaction(TimeStampedModel, RelayModel):
     class ReactionTypes(models.IntegerChoices):
         LIKE = 1, _("like")
         DISLIKE = -1, _("dislike")
 
         @property
         def description(self):
             return self.label
@@ -95,19 +96,17 @@
 
 SwappedReaction = swapper.load_model(
     "baseapp_reactions", "Reaction", required=False, require_ready=False
 )
 
 
 class ReactableModel(models.Model):
-    reactions_count = models.JSONField(default=default_reactions_count)
+    reactions_count = models.JSONField(default=default_reactions_count, editable=False)
     reactions = GenericRelation(
         SwappedReaction,
         content_type_field="target_content_type",
-        object_id_field="target_object_id"
+        object_id_field="target_object_id",
     )
+    is_reactions_enabled = models.BooleanField(default=True)
 
     class Meta:
         abstract = True
-
-    def get_my_permissions(self, request):
-        raise NotImplementedError
```

### Comparing `baseapp-reactions-0.1.6/baseapp_reactions/tests/test_graphql_queries.py` & `baseapp-reactions-0.2.0/baseapp_reactions/tests/test_graphql_queries.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 import pytest
-from baseapp_comments.tests.factories import ClassroomCommentFactory
+from baseapp_comments.tests.factories import CommentFactory
 
-from .factories import CommentReactionFactory
+from .factories import ReactionFactory
 
 pytestmark = pytest.mark.django_db
 
-
-def test_student_can_see_reactions(django_user_student, graphql_user_student):
-    user = django_user_student.user
-    classroom = django_user_student.member.classroom
-    comment = ClassroomCommentFactory(target=classroom, user=user)
-    CommentReactionFactory(target=comment)
-    response = graphql_user_student(
-        "query { allClassrooms { totalCount edges { node { id commentsCount comments { edges { node { id content reactionsCount { total }}}} } } } }"
-    )
-    content = response.json()
-    assert content["data"]["allClassrooms"]["totalCount"] == 1
-    assert len(content["data"]["allClassrooms"]["edges"]) == 1
-    assert (
-        content["data"]["allClassrooms"]["edges"][0]["node"]["comments"]["edges"][0]["node"][
-            "reactionsCount"
-        ]["total"]
-        == 1
-    )
-
-
-def test_instructor_can_see_reactions(django_user_instructor, graphql_user_instructor):
-    user = django_user_instructor.user
-    classroom = django_user_instructor.member.classroom
-    comment = ClassroomCommentFactory(target=classroom, user=user)
-    CommentReactionFactory(target=comment)
-    response = graphql_user_instructor(
-        "query { allClassrooms { totalCount edges { node { id commentsCount comments { edges { node { id content reactionsCount { total }}}} } } } }"
-    )
+VIEW_QUERY = """
+    query GetObject($id: ID!) {
+        node(id: $id) {
+            ... on ReactionsInterface {
+                reactionsCount {
+                    total
+                }
+                reactions {
+                    edges {
+                        node {
+                            id
+                            pk
+                        }
+                    }
+                }
+            }
+        }
+    }
+"""
+
+
+def test_user_can_see_reactions(django_user_client, graphql_user_client):
+    comment = CommentFactory(user=django_user_client.user)
+    ReactionFactory(target=comment)
+    response = graphql_user_client(VIEW_QUERY, variables={"id": comment.relay_id})
     content = response.json()
-    assert content["data"]["allClassrooms"]["totalCount"] == 1
-    assert len(content["data"]["allClassrooms"]["edges"]) == 1
-    assert (
-        content["data"]["allClassrooms"]["edges"][0]["node"]["comments"]["edges"][0]["node"][
-            "reactionsCount"
-        ]["total"]
-        == 1
-    )
+    assert content["data"]["node"]["reactionsCount"]["total"] == 1
+    assert len(content["data"]["node"]["reactions"]["edges"]) == 1
+
+
+# def test_user_can_see_reactions(django_user_instructor, graphql_user_instructor):
+#     user = django_user_instructor.user
+#     classroom = django_user_instructor.member.classroom
+#     comment = ClassroomCommentFactory(target=classroom, user=user)
+#     CommentReactionFactory(target=comment)
+#     response = graphql_user_instructor(
+#         "query { allClassrooms { totalCount edges { node { id commentsCount comments { edges { node { id content reactionsCount { total }}}} } } } }"
+#     )
+#     content = response.json()
+#     assert content["data"]["allClassrooms"]["totalCount"] == 1
+#     assert len(content["data"]["allClassrooms"]["edges"]) == 1
+#     assert (
+#         content["data"]["allClassrooms"]["edges"][0]["node"]["comments"]["edges"][0]["node"][
+#             "reactionsCount"
+#         ]["total"]
+#         == 1
+#     )
```

### Comparing `baseapp-reactions-0.1.6/baseapp_reactions.egg-info/PKG-INFO` & `baseapp-reactions-0.2.0/baseapp_reactions.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,86 @@
 Metadata-Version: 2.1
 Name: baseapp-reactions
-Version: 0.1.6
+Version: 0.2.0
 Summary: BaseApp Reactions
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp Reactions
         
         Reusable app to enable User's reactions on any model, features like like/dislike or any other reactions type, customizable for project's needs.
         
         ## How to install:
         
-        Add dependencies to your `requirements/base.txt` file:
+        Install in your environment:
         
+        ```bash
+        pip install baseapp-reactions
         ```
-        baseapp-core @ git+https://github.com/silverlogic/baseapp-backend.git@v0.1#subdirectory=baseapp-core
-        baseapp-reactions @ git+https://github.com/silverlogic/baseapp-backend.git@v0.1#subdirectory=baseapp-reactions
-        ```
-        
-        And run provision or manually `pip install -r requirements/base.ext`
         
         If you want to develop, [install using this other guide](#how-to-develop).
         
         ## How to use
         
         Add `baseapp_reactions` to your project's `INSTALLED_APPS`
         
+        ```python
+        INSTALLED_APPS = [
+            # ...
+            "baseapp_reactions",
+            # ...
+        ]
+        ```
+        
+        Add `baseapp_reactions.permissions.ReactionsPermissionsBackend` to the `AUTHENTICATION_BACKENDS` list in your django settings file.
+        
+        ```python
+        AUTHENTICATION_BACKENDS = [
+            # ...
+            "baseapp_reactions.permissions.ReactionsPermissionsBackend",
+            # ...
+        ]
+        ```
+        
         Now make sure all models you'd like to get reactions also inherits `ReactableModel`, like:
         
         ```python
         from baseapp_reactions.models import ReactableModel
         
         class Comment(models.Model, ReactableModel):
             body = models.Textfield()
         ```
         
-        Also make sure your GraphQL object types extends `ReactionsNode` interface:
+        Also make sure your GraphQL object types extends `ReactionsInterface` interface:
         
         ```python
-        from baseapp_reactions.graphql.object_types import ReactionsNode
+        from baseapp_reactions.graphql.object_types import ReactionsInterface
         
         class CommentNode(DjangoObjectType):
             class Meta:
-                interfaces = (relay.Node, ReactionsNode)
+                interfaces = (relay.Node, ReactionsInterface)
         ```
         
-        Expose `ReactionsMutations` and `ReactionsQuery` in your GraphQL/graphene endpoint, like:
+        Expose `ReactionsMutations` and `ReactionsQueries` in your GraphQL/graphene endpoint, like:
         
         ```python
         from baseapp_reactions.graphql.mutations import ReactionsMutations
-        from baseapp_reactions.graphql.queries import ReactionsQuery
+        from baseapp_reactions.graphql.queries import ReactionsQueries
         
-        class Query(graphene.ObjectType, ReactionsQuery):
+        class Query(graphene.ObjectType, ReactionsQueries):
             pass
         
         class Mutation(graphene.ObjectType, ReactionsMutations):
             pass
         
         schema = graphene.Schema(query=Query, mutation=Mutation)
         ```
         
-        This will expose `reactionToggle` mutation and add fields and connections to all your GraphqlQL Object Types using interface `ReactionsNode`.
+        This will expose `reactionToggle` mutation and add fields and connections to all your GraphqlQL Object Types using interface `ReactionsInterface`.
         
         Example:
         
         ```graphql
         {
             comment(id: $id) {
                 id
@@ -124,38 +139,14 @@
         
         Now in your `settings/base.py` make sure to tell baseapp-reactions what is your custom model for Reaction:
         
         ```python
         BASEAPP_REACTIONS_REACTION_MODEL = 'reactions.Reaction'
         ```
         
-        ## Writing test cases in your project
-        
-        There is a `AbstractReactionFactory` which helps you write other factories:
-        
-        ```
-        import factory
-        from baseapp_reactions.tests.factories import AbstractReactionFactory
-        
-        class CommentFactory(factory.django.DjangoModelFactory):
-            class Meta:
-                model = "comments.Comment"
-        
-        
-        class CommentReactionFactory(AbstractReactionFactory):
-            target = factory.SubFactory(CommentFactory)
-        
-            class Meta:
-                model = "baseapp_reactions.Reaction"
-                # OR if you have a custom model, point to it:
-                model = "reactions.Reaction"
-        ```
-        
-        In the above example we have a easy way to make reactions to any comment into the database for testing proporses using `CommentReactionFactory`.
-        
         ## How to develop
         
         Clone the project inside your project's backend dir:
         
         ```
         git clone git@github.com:silverlogic/baseapp-backend.git
         ```
```

### Comparing `baseapp-reactions-0.1.6/baseapp_reactions.egg-info/SOURCES.txt` & `baseapp-reactions-0.2.0/baseapp_reactions.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 baseapp_reactions/__init__.py
 baseapp_reactions/admin.py
 baseapp_reactions/apps.py
 baseapp_reactions/models.py
+baseapp_reactions/permissions.py
 baseapp_reactions.egg-info/PKG-INFO
 baseapp_reactions.egg-info/SOURCES.txt
 baseapp_reactions.egg-info/dependency_links.txt
 baseapp_reactions.egg-info/requires.txt
 baseapp_reactions.egg-info/top_level.txt
 baseapp_reactions/graphql/__init__.py
 baseapp_reactions/graphql/mutations.py
@@ -20,8 +21,18 @@
 baseapp_reactions/migrations/__init__.py
 baseapp_reactions/tests/__init__.py
 baseapp_reactions/tests/conftest.py
 baseapp_reactions/tests/factories.py
 baseapp_reactions/tests/test_graphql_mutations.py
 baseapp_reactions/tests/test_graphql_queries.py
 testproject/__init__.py
-testproject/settings.py
+testproject/graphql.py
+testproject/settings.py
+testproject/setup.py
+testproject/urls.py
+testproject/wsgi.py
+testproject/testapp/__init__.py
+testproject/testapp/admin.py
+testproject/testapp/apps.py
+testproject/testapp/models.py
+testproject/testapp/migrations/0001_initial.py
+testproject/testapp/migrations/__init__.py
```

