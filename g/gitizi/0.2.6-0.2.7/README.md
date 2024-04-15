# Comparing `tmp/gitizi-0.2.6.tar.gz` & `tmp/gitizi-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitizi-0.2.6.tar", last modified: Fri Feb  2 11:11:01 2024, max compression
+gzip compressed data, was "gitizi-0.2.7.tar", last modified: Mon Apr 15 22:34:37 2024, max compression
```

## Comparing `gitizi-0.2.6.tar` & `gitizi-0.2.7.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 11:11:01.547945 gitizi-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-02 11:10:53.000000 gitizi-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-02 11:11:01.547945 gitizi-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-02 11:10:53.000000 gitizi-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 11:11:01.543945 gitizi-0.2.6/gitizi/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-02 11:10:53.000000 gitizi-0.2.6/gitizi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 11:11:01.543945 gitizi-0.2.6/gitizi/ai/
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-02-02 11:10:53.000000 gitizi-0.2.6/gitizi/ai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 11:11:01.547945 gitizi-0.2.6/gitizi/ai/context/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-02 11:10:53.000000 gitizi-0.2.6/gitizi/ai/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-02-02 11:10:53.000000 gitizi-0.2.6/gitizi/ai/context/squash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-02-02 11:10:53.000000 gitizi-0.2.6/gitizi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-02 11:10:53.000000 gitizi-0.2.6/gitizi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-02-02 11:10:53.000000 gitizi-0.2.6/gitizi/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 11:11:01.547945 gitizi-0.2.6/gitizi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-02 11:11:01.000000 gitizi-0.2.6/gitizi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-02 11:11:01.000000 gitizi-0.2.6/gitizi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 11:11:01.000000 gitizi-0.2.6/gitizi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-02 11:11:01.000000 gitizi-0.2.6/gitizi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-02 11:11:01.000000 gitizi-0.2.6/gitizi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-02 11:11:01.000000 gitizi-0.2.6/gitizi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-02 11:10:53.000000 gitizi-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-02 11:10:53.000000 gitizi-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 11:11:01.547945 gitizi-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:34:37.565591 gitizi-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 22:34:33.000000 gitizi-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-15 22:34:37.565591 gitizi-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-15 22:34:33.000000 gitizi-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:34:37.561591 gitizi-0.2.7/gitizi/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 22:34:33.000000 gitizi-0.2.7/gitizi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:34:37.561591 gitizi-0.2.7/gitizi/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-15 22:34:33.000000 gitizi-0.2.7/gitizi/ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:34:37.561591 gitizi-0.2.7/gitizi/ai/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-15 22:34:33.000000 gitizi-0.2.7/gitizi/ai/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-15 22:34:33.000000 gitizi-0.2.7/gitizi/ai/context/squash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-15 22:34:33.000000 gitizi-0.2.7/gitizi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 22:34:33.000000 gitizi-0.2.7/gitizi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-15 22:34:33.000000 gitizi-0.2.7/gitizi/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:34:37.561591 gitizi-0.2.7/gitizi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-15 22:34:37.000000 gitizi-0.2.7/gitizi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-15 22:34:37.000000 gitizi-0.2.7/gitizi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 22:34:37.000000 gitizi-0.2.7/gitizi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 22:34:37.000000 gitizi-0.2.7/gitizi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-15 22:34:37.000000 gitizi-0.2.7/gitizi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 22:34:37.000000 gitizi-0.2.7/gitizi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-15 22:34:33.000000 gitizi-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 22:34:33.000000 gitizi-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-15 22:34:33.000000 gitizi-0.2.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 22:34:37.565591 gitizi-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:34:37.561591 gitizi-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-15 22:34:33.000000 gitizi-0.2.7/tests/test_unit.py
```

### Comparing `gitizi-0.2.6/LICENSE` & `gitizi-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gitizi-0.2.6/gitizi/ai/__init__.py` & `gitizi-0.2.7/gitizi/ai/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 """
 Git IZI : AI
 """
 
 from json import JSONDecodeError
 
-from aiohttp import WSServerHandshakeError, ClientOSError
+from aiohttp import ClientOSError, WSServerHandshakeError
 
 from gitizi.util import suppress_output
+
 from ..exceptions import GitiziException, GitiziParseException
 
 with suppress_output():
     import g4f
 
-from g4f.Provider import (
-    Bing,
-)
+from g4f.Provider import Bing  # pylint:disable=wrong-import-order
 
 from .context import Context
-
-from .context.squash import (
-    CONTEXT as S_CONTEXT,
-    USER_MSG_WRAPPER as S_WRAPPER,
-    retrieve_response as S_RESPONSE,
-)
+from .context.squash import CONTEXT as S_CONTEXT
+from .context.squash import USER_MSG_WRAPPER as S_WRAPPER
+from .context.squash import retrieve_response as S_RESPONSE
 
 
 def contextualize(msg: str, ctx: Context = Context.ASK) -> list[dict]:
     """Contextualize message"""
     match ctx:
         case Context.SQUASH:
             ai_ctx = S_CONTEXT
@@ -61,9 +57,8 @@
                     messages=messages,
                     provider=Bing,
                     auth=True,
                 )
                 return parse_response(msg=response, ctx=ctx)
             except (WSServerHandshakeError, ClientOSError, GitiziParseException, ConnectionResetError):
                 pass
-        else:
-            raise GitiziException("Connection error")
+        raise GitiziException("Connection error")
```

### Comparing `gitizi-0.2.6/gitizi/ai/context/squash.py` & `gitizi-0.2.7/gitizi/ai/context/squash.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     },
 ]
 
 USER_MSG_WRAPPER = "Squashed commit message:\n <message>{user_message}</message>"
 
 
 def retrieve_response(response: str):
+    """Retrieve response from AI"""
     try:
         message: str = json.loads(response)["message"]
         if not message:
             raise GitiziParseException
         if not message[0].isalpha() and not re.match(r"^\[Bump .*\].*$", message):
             raise GitiziParseException
         return message
```

### Comparing `gitizi-0.2.6/gitizi/cli.py` & `gitizi-0.2.7/gitizi/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 Git IZI : CLI
 """
 
 import sys
 
 import click
 
-from .ai import ask as ask_ai, Context
-from .exceptions import GitiziException
+from .ai import Context
+from .ai import ask as ask_ai
 from .util import (
-    default_remote_branch,
-    default_local_branch,
-    current_synced,
-    default_synced,
-    reset_default,
-    is_current_default,
-    current_branch,
-    default_remote,
-    all_commited,
-    checkout,
     commit,
-    fetch_default,
-    merge_to_current,
-    last_shared,
-    get_log_until,
+    checkout,
     get_hash,
+    last_shared,
+    all_commited,
     reset_branch,
     delete_branch,
+    fetch_default,
+    get_log_until,
+    reset_default,
+    current_branch,
+    current_synced,
+    default_remote,
+    default_synced,
+    merge_to_current,
     ammend_commit_msg,
+    is_current_default,
+    default_local_branch,
+    default_remote_branch,
 )
+from .exceptions import GitiziException
 
 
 @click.group()
 def main():
     """Git IZI entrypoint command"""
 
 
@@ -44,17 +45,15 @@
     )
 
     if reset:
         checked = False
         old_branch = None
         if not is_current_default():
             if not all_commited():
-                click.echo(
-                    "All local changes have to be commited or stashed before reset"
-                )
+                click.echo("All local changes have to be commited or stashed before reset")
                 raise click.Abort
             checked, old_branch = checkout()
         if not default_synced():
             reset_default()
             if checked:
                 checkout(old_branch)
             click.echo(f"Default branch [{default_local_branch()}] synchronised")
@@ -80,17 +79,15 @@
 def current():
     """Operations on current branch"""
 
 
 @current.command()
 def info():
     """Current branch info"""
-    click.echo(
-        f"Current branch is: {current_branch()}, is default: {is_current_default()}"
-    )
+    click.echo(f"Current branch is: {current_branch()}, is default: {is_current_default()}")
     click.echo(
         f"Default branch is: {default_local_branch()}, is in sync with remote [{default_remote()}]: {default_synced()}"
     )
 
 
 def _squash(force: bool = False):
     """Squash current commit"""
@@ -106,26 +103,25 @@
             raise click.Abort
         commit()
     click.echo("Everything is commited, continuing...")
 
     if not default_synced():
         if not force:
             click.echo(
-                f"Default branch [{default_local_branch()}] is not in sync with remote default [{default_remote_branch()}]"
+                f"Default branch [{default_local_branch()}] is not in sync with "
+                f"remote default [{default_remote_branch()}]"
             )
             raise click.Abort
         _default(reset=True)
-        # TODO: Pull default -- check if reset is all that's needed
+        # TODO: Pull default -- check if reset is all that's needed  pylint:disable=fixme
     click.echo("Default branch is in sync with remote, continuing...")
 
     if not current_synced(can_ahead=True):
         if not force:
-            click.echo(
-                f"Current branch [{current_branch()}] is behind with local default [{default_local_branch()}]"
-            )
+            click.echo(f"Current branch [{current_branch()}] is behind with local default [{default_local_branch()}]")
             raise click.Abort
         merge_to_current()
     click.echo("Default branch is ahead or in sync with default, continuing...")
 
     shared = last_shared()
     logs = get_log_until(commit_hash=shared)
 
@@ -157,20 +153,22 @@
     "-f",
     "--force",
     is_flag=True,
     default=False,
     help="Try to perform all actions needed to create a squashed commit.",
 )
 def squash(force: bool = False):
+    """Command to squash, optionally forceful"""
     _squash(force=force)
 
 
 @main.command()
 @click.argument("message")
 def ask(message: str):
     """Ask AI"""
     click.echo(ask_ai(message))
 
 
 @click.command()
 def main_squash():
+    """Command to squash with force - please know what you're doing"""
     _squash(force=True)
```

### Comparing `gitizi-0.2.6/gitizi/util.py` & `gitizi-0.2.7/gitizi/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Git IZI : Util
 """
 
 import os
 import sys
-
 from contextlib import contextmanager, redirect_stderr, redirect_stdout
 
-import click
 import git
+import click
 
 from .exceptions import GitiziException
 
 
 @contextmanager
 def suppress_output():
     """A context manager that redirects stdout and stderr to devnull"""
@@ -36,17 +35,15 @@
             return remote
     return repo.remotes[0]
 
 
 def default_remote_branch(remote: str | git.Remote | None = None) -> git.Reference:
     """Get default branch"""
     remote = (
-        remote
-        if isinstance(remote, git.Remote)
-        else git.Remote(repo=repo, name=remote) if remote else default_remote()
+        remote if isinstance(remote, git.Remote) else git.Remote(repo=repo, name=remote) if remote else default_remote()
     )
 
     return next(filter(lambda ref: ref.name == f"{remote.name}/HEAD", remote.refs)).ref
 
 
 def default_local_branch() -> git.Reference:
     """Get default local branch"""
@@ -112,17 +109,15 @@
         count_ahead = 0
 
     return count_behind == 0 and count_ahead == 0
 
 
 def reset_default():
     """Fully resets default branch to be in-line with its remote"""
-    repo.head.reset(
-        commit=f"{default_remote()}/HEAD", index=True, working_tree=True, paths=None
-    )
+    repo.head.reset(commit=f"{default_remote()}/HEAD", index=True, working_tree=True, paths=None)
 
 
 def all_commited() -> bool:
     """Check if everything is commited and we can safely check out"""
     return not repo.is_dirty()
 
 
@@ -148,17 +143,15 @@
         repo.git.checkout(*args)
         return True, curr_branch
     return False, curr_branch
 
 
 def fetch_default():
     """Fetch default branch from default remote"""
-    default_remote().fetch(
-        refspec=f"refs/heads/{default_local_branch().name}:{default_remote_branch().path}"
-    )
+    default_remote().fetch(refspec=f"refs/heads/{default_local_branch().name}:{default_remote_branch().path}")
 
 
 def commit(with_no_edit: bool = False):
     """Create a commit with all uncommited changes"""
     files = repo.git.diff(None, name_only=True)
     for f in files.split("\n"):
         if f:
```

