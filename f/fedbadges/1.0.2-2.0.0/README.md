# Comparing `tmp/fedbadges-1.0.2.tar.gz` & `tmp/fedbadges-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fedbadges-1.0.2.tar", last modified: Mon Mar 25 12:49:35 2019, max compression
+gzip compressed data, was "fedbadges-2.0.0.tar", max compression
```

## Comparing `fedbadges-1.0.2.tar` & `fedbadges-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,35 @@
-drwxrwxr-x   0 cverna    (1000) cverna    (1000)        0 2019-03-25 12:49:35.000000 fedbadges-1.0.2/
--rw-rw-r--   0 cverna    (1000) cverna    (1000)    22145 2019-03-25 12:47:03.000000 fedbadges-1.0.2/CHANGELOG.rst
--rw-rw-r--   0 cverna    (1000) cverna    (1000)    18092 2019-01-21 12:29:41.000000 fedbadges-1.0.2/LICENSE
--rw-rw-r--   0 cverna    (1000) cverna    (1000)       87 2019-01-21 12:29:41.000000 fedbadges-1.0.2/MANIFEST.in
--rw-rw-r--   0 cverna    (1000) cverna    (1000)    13731 2019-03-25 12:49:35.000000 fedbadges-1.0.2/PKG-INFO
--rw-rw-r--   0 cverna    (1000) cverna    (1000)    11134 2019-02-24 20:04:47.000000 fedbadges-1.0.2/README.rst
-drwxrwxr-x   0 cverna    (1000) cverna    (1000)        0 2019-03-25 12:49:35.000000 fedbadges-1.0.2/fedbadges/
--rw-rw-r--   0 cverna    (1000) cverna    (1000)        0 2019-01-21 12:50:55.000000 fedbadges-1.0.2/fedbadges/__init__.py
--rw-rw-r--   0 cverna    (1000) cverna    (1000)     1028 2019-01-21 12:50:55.000000 fedbadges-1.0.2/fedbadges/commands.py
--rw-rw-r--   0 cverna    (1000) cverna    (1000)     9090 2019-02-26 08:47:04.000000 fedbadges-1.0.2/fedbadges/consumers.py
--rw-rw-r--   0 cverna    (1000) cverna    (1000)    17770 2019-03-25 12:45:24.000000 fedbadges-1.0.2/fedbadges/rules.py
--rw-rw-r--   0 cverna    (1000) cverna    (1000)     4013 2019-03-25 12:45:24.000000 fedbadges-1.0.2/fedbadges/utils.py
-drwxrwxr-x   0 cverna    (1000) cverna    (1000)        0 2019-03-25 12:49:35.000000 fedbadges-1.0.2/fedbadges.egg-info/
--rw-rw-r--   0 cverna    (1000) cverna    (1000)    13731 2019-03-25 12:49:35.000000 fedbadges-1.0.2/fedbadges.egg-info/PKG-INFO
--rw-rw-r--   0 cverna    (1000) cverna    (1000)      478 2019-03-25 12:49:35.000000 fedbadges-1.0.2/fedbadges.egg-info/SOURCES.txt
--rw-rw-r--   0 cverna    (1000) cverna    (1000)        1 2019-03-25 12:49:35.000000 fedbadges-1.0.2/fedbadges.egg-info/dependency_links.txt
--rw-rw-r--   0 cverna    (1000) cverna    (1000)      137 2019-03-25 12:49:35.000000 fedbadges-1.0.2/fedbadges.egg-info/entry_points.txt
--rw-rw-r--   0 cverna    (1000) cverna    (1000)        1 2019-01-21 12:38:56.000000 fedbadges-1.0.2/fedbadges.egg-info/not-zip-safe
--rw-rw-r--   0 cverna    (1000) cverna    (1000)      116 2019-03-25 12:49:35.000000 fedbadges-1.0.2/fedbadges.egg-info/requires.txt
--rw-rw-r--   0 cverna    (1000) cverna    (1000)       10 2019-03-25 12:49:35.000000 fedbadges-1.0.2/fedbadges.egg-info/top_level.txt
-drwxrwxr-x   0 cverna    (1000) cverna    (1000)        0 2019-03-25 12:49:35.000000 fedbadges-1.0.2/fedmsg.d/
--rw-rw-r--   0 cverna    (1000) cverna    (1000)     1345 2019-02-26 15:51:36.000000 fedbadges-1.0.2/fedmsg.d/badges-global.py
--rw-rw-r--   0 cverna    (1000) cverna    (1000)      106 2019-01-21 12:29:41.000000 fedbadges-1.0.2/fedmsg.d/datanommer.py
--rw-rw-r--   0 cverna    (1000) cverna    (1000)      170 2019-01-21 12:29:41.000000 fedbadges-1.0.2/fedmsg.d/endpoints.py
--rw-rw-r--   0 cverna    (1000) cverna    (1000)      116 2019-02-26 15:51:36.000000 fedbadges-1.0.2/requirements.txt
--rw-rw-r--   0 cverna    (1000) cverna    (1000)       38 2019-03-25 12:49:35.000000 fedbadges-1.0.2/setup.cfg
--rw-rw-r--   0 cverna    (1000) cverna    (1000)     1179 2019-03-25 12:47:12.000000 fedbadges-1.0.2/setup.py
+-rw-r--r--   0        0        0    22636 2024-04-16 15:45:34.113835 fedbadges-2.0.0/CHANGELOG.rst
+-rw-r--r--   0        0        0    18092 2022-06-27 10:24:28.000000 fedbadges-2.0.0/LICENSE
+-rw-r--r--   0        0        0    10839 2024-04-11 10:05:52.136691 fedbadges-2.0.0/README.rst
+-rw-r--r--   0        0        0        0 2022-06-27 10:24:28.000000 fedbadges-2.0.0/fedbadges/__init__.py
+-rw-r--r--   0        0        0     1559 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/aio.py
+-rw-r--r--   0        0        0     5857 2024-04-16 15:39:38.330818 fedbadges-2.0.0/fedbadges/consumer.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/__init__.py
+-rw-r--r--   0        0        0     1987 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/badges_dev.py
+-rw-r--r--   0        0        0     1996 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/group_membership.py
+-rw-r--r--   0        0        0     1873 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/libravatar.py
+-rw-r--r--   0        0        0     2195 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/lifecycle.py
+-rw-r--r--   0        0        0     1338 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/mirror.py
+-rw-r--r--   0        0        0      827 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/utils.py
+-rw-r--r--   0        0        0    17499 2024-04-12 17:12:53.328051 fedbadges-2.0.0/fedbadges/rules.py
+-rw-r--r--   0        0        0     3614 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/rulesrepo.py
+-rw-r--r--   0        0        0     5001 2024-04-12 17:24:32.882079 fedbadges-2.0.0/fedbadges/utils.py
+-rw-r--r--   0        0        0     5246 2024-04-11 13:38:19.306992 fedbadges-2.0.0/fedbadges.toml.example
+-rw-r--r--   0        0        0     5574 2024-04-16 15:39:38.414819 fedbadges-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-06-27 10:24:28.000000 fedbadges-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2572 2024-04-16 15:39:38.330818 fedbadges-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     1286 2022-06-27 10:24:28.000000 fedbadges-2.0.0/tests/test_badges/rules/bodhi-update-fancy.yaml
+-rw-r--r--   0        0        0      990 2022-06-27 10:24:28.000000 fedbadges-2.0.0/tests/test_badges/rules/bodhi-update-simple.yaml
+-rw-r--r--   0        0        0      986 2024-04-11 10:05:52.138691 fedbadges-2.0.0/tests/test_badges/rules/irc-speak-up.yml
+-rw-r--r--   0        0        0      919 2022-06-27 10:24:28.000000 fedbadges-2.0.0/tests/test_badges/rules/pagure-long-live.yaml
+-rw-r--r--   0        0        0     1143 2024-04-11 10:05:52.138691 fedbadges-2.0.0/tests/test_badges/rules/tagger-01.yml
+-rw-r--r--   0        0        0     2822 2024-04-12 15:35:16.765374 fedbadges-2.0.0/tests/test_complicated_recipient.py
+-rw-r--r--   0        0        0     2096 2024-04-12 15:35:28.525487 fedbadges-2.0.0/tests/test_complicated_trigger.py
+-rw-r--r--   0        0        0     6796 2024-04-12 17:21:08.460290 fedbadges-2.0.0/tests/test_criteria_datanommer.py
+-rw-r--r--   0        0        0    11977 2024-04-12 17:17:56.689566 fedbadges-2.0.0/tests/test_rule_matching.py
+-rw-r--r--   0        0        0     3171 2024-04-12 17:09:42.594579 fedbadges-2.0.0/tests/test_triggers.py
+-rw-r--r--   0        0        0     5087 2024-04-16 15:39:38.414819 fedbadges-2.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0      485 2024-04-12 14:52:01.331404 fedbadges-2.0.0/tests/test_yaml_collector.py
+-rw-r--r--   0        0        0     3348 2024-04-12 17:21:17.025367 fedbadges-2.0.0/tests/utils.py
+-rw-r--r--   0        0        0      878 2024-04-16 15:39:38.414819 fedbadges-2.0.0/tox.ini
+-rw-r--r--   0        0        0    13431 1970-01-01 00:00:00.000000 fedbadges-2.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fedbadges-1.0.2/CHANGELOG.rst` & `fedbadges-2.0.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 Changelog
 =========
 
+2.0.0
+-----
+
+- Rebase on Fedora Messaging
+- Use Poetry
+- Use FASJSON Client
+- Make it work in Openshift
+- Add CI with Github Actions
+- Drop badgrclient and go back to tahrir-api as the implementation was never finished
+- Use Black for formatting
+- Use Ruff for linting
+- Lots of other changes, see the `git log <https://github.com/fedora-infra/fedbadges/compare/1.0.3...2.0.0>`_ for details
+
+
+1.0.3
+-----
+
+- Add quick support for FASJSON (using requests, as fasjson-client is python3 only)
+
 1.0.2
 -----
 
 - Get the list of authors form pagure to query datanommer `#69 <https://github.com/fedora-infra/fedbadges/pull/69>`_
 
 1.0.1
 -----
```

### Comparing `fedbadges-1.0.2/LICENSE` & `fedbadges-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fedbadges-1.0.2/PKG-INFO` & `fedbadges-2.0.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,297 +1,276 @@
-Metadata-Version: 1.2
-Name: fedbadges
-Version: 1.0.2
-Summary: fedmsg consumer for awarding open badges
-Home-page: https://github.com/fedora-infra/fedbadges
-Author: Ross Delinger
-Author-email: rdelinge@redhat.com
-Maintainer: Ralph Bean
-Maintainer-email: rbean@redhat.com
-License: GPLv2+
-Description: Fedora Badges
-        =============
-        
-        This repo contains the consumer and the command necessary to hook the
-        badges stack (Tahrir, Tahrir-API, Tahrir-REST) into fedmsg.  It is the process
-        that runs in the background, monitoring activity of Fedora contributors, and is
-        responsible for awarding badges for activity as it happens.  It is separate
-        from and sometimes confused with the *frontend* of the badges system; that web
-        application is called `tahrir <https://github.com/fedora-infra/tahrir>`_.  This
-        project (fedbadges) writes to a database that the web frontend (tahrir) reads
-        from.
-        
-        The *actual badge rules* that we act on in Fedora Infrastructure can be
-        found `here <https://pagure.io/Fedora-Badges>`.
-        
-        Architecture
-        ------------
-        
-        fedbadges runs as a ``Consumer`` plugin to the ``fedmsg-hub`` (really,
-        a moksha-hub).  When started, it will load some initial configuration
-        and a set of ``BadgeRules`` (more on that later) and then sit quietly
-        listening to the fedmsg bus.  Each rule (composed of some metadata,
-        a ``trigger``, and a set of ``criteria``) is defined on disk as a yaml file.
-        
-        * When a new message comes along, our ``Consumer`` looks to see if it matches
-          any of the ``BadgeRules`` it has registered.
-        
-        * Each BadgeRule must define a ``trigger`` -- a `lightweight` check.
-          When processing a message, this is the first thing that is checked.  It
-          defines a *pattern* that the message must match.  If the message does not
-          match, then the current BadgeRule is discarded and processing moves to
-          the next.
-        
-          A ``trigger`` is typically something like "any bodhi message"
-          or "messages only from the failure of a koji build".  More on their
-          specification below.
-        
-        * BadgeRules must also define a set of ``criteria`` -- a more `heavyweight`
-          checks.  During the processing of a newly received message, if the
-          message matches a BadgeRule's ``trigger``, the ``criteria`` is then
-          considered.  This typically involves a more expensive query to the
-          `datanommer <https://github.com/fedora-infra/datanommer>`_ database.
-        
-          A BadgeRule ``criteria`` may read something like "$user has
-          pushed 200 bodhi updates to stable" or "$user chaired an IRC meeting".
-        
-          **Aside:** Although datanommer is the only currently supported backend, we
-          can implement other queryable backend in the future as needed like FAS2
-          (to see if the user is in X number of groups) or even off-site services
-          like libravatar (to award a badge if the user is a user of the AGPL web
-          service).
-        
-        * If a badge's ``trigger`` and ``criteria`` both match, then the badge is
-          awarded.  If the BadgeRule doesn't specify, we award the badge to all
-          usernames returned by a call to ``fedmsg.meta.msg2usernames(msg)``.
-        
-          That is usually correct -- but sometimes, a BadgeRule needs to specify
-          that one particular user (not all related users) should be recipients of
-          the badge.  In this case, the BadgeRule may define a ``recipient``
-          in dot-notation that instructs the ``Consumer`` how to extract the
-          recipient's username from the received message.
-        
-          The badge is awarded to our deserving user via the `tahrir_api
-          <https://github.com/fedora-infra/tahrir-api>`_.  At the end of the day,
-          this amounts to adding a row in a database table for the `Tahrir
-          <https://github.com/fedora-infra/tahrir>`_ application.
-        
-        There are some optimizations in place omitted above for clarity.
-        For instance, after the trigger has matched we first check if the user
-        that *would* be awarded the badge already has it.  If they do, we stop
-        processing the badge rule immediately to avoid making an unnecessary
-        expensive check against the datanommer db.
-        
-        Configuration - Global
-        ----------------------
-        
-        fedbadges needs three major pieces of global configuration.
-        All configuration is loaded in the standard fedmsg way, from
-        python files in ``/etc/fedmsg.d/``.
-        
-        First, generic and tahrir-related configuration.  See
-        `fedmsg.d/badges-global.py
-        <https://github.com/fedora-infra/fedbadges/blob/develop/fedmsg.d/badges-global.py>`_
-        in the git repo for an example.
-        
-        Second, datanommer connection information.  See
-        `fedmsg.d/datanommer.py
-        <https://github.com/fedora-infra/fedbadges/blob/develop/fedmsg.d/datanommer.py>`_
-        in the git repo for an example.
-        
-        Third, fedbadges emits its own fedmsg messages when it awards badges.  It will
-        need its own endpoint definitions for this.  See `fedmsg.d/endpoints.py
-        <https://github.com/fedora-infra/fedbadges/blob/develop/fedmsg.d/endpoints.py>`_
-        in the git repo for an example.
-        
-        Configuration - BadgeRule specification
-        ---------------------------------------
-        
-        BadgeRules are specified in `YAML <http://www.yaml.org/>`_ on the file system.
-        
-        Triggers
-        ~~~~~~~~
-        
-        Every BadgeRule must carry the following minimum set of metadata::
-        
-            # This is some metadata about the badge
-            name:           Like a Rock
-            description:    You have pushed 500 or more bodhi updates to stable status.
-            creator:        ralph
-        
-            # This is a link to the discussion about adopting this as a for-real badge.
-            discussion: http://github.com/fedora-infra/badges/pull/SOME_NUMBER
-        
-            # A link to the image for the badge
-            image_url: http://somelink.org/to-an-image.png
-        
-        Here's a simple example of a ``trigger``::
-        
-            trigger:
-              category: bodhi
-        
-        The above will match any bodhi message on any of the topics that come
-        from the bodhi update system.
-        
-        Triggers may employ a little bit of logic to make more complex
-        filters.  The following trigger will match any message that comes from
-        *either* the bodhi update system or the fedora git package repos::
-        
-            trigger:
-              category:
-                any:
-                  - bodhi
-                  - git
-        
-        At present triggers may directly compare themselves against only the
-        `category` or the `topic` of a message.  In the future we'd like to add
-        more comparisons.. in the meantime, here's an example of comparing against
-        the fully qualified message topic.  This will match any message
-        that is specifically for editing a wiki page::
-        
-            trigger:
-              topic: org.fedoraproject.prod.wiki.article.edit
-        
-        ----
-        
-        There is one additional way you can specify a trigger.  If you need more
-        flexibility than ``topic`` and
-        ``category`` allow, you may specify a custom filter expression with a
-        ``lambda`` filter.  For example::
-        
-            trigger:
-              lambda: "a string of interest" in json.dumps(msg)
-        
-        The above trigger will match if the string ``"a string of interest"`` appears
-        anywhere in the incoming message.  fedbadges takes the expression you provide
-        it and compiles it into a python callable on initialization.  Our callable
-        here serializes the message to a JSON string before doing its comparison.
-        Powerful!
-        
-        Criteria
-        ~~~~~~~~
-        
-        As mentioned above in the architecture section, we currently only support
-        datanommer as a queryable backend for criteria.  We hope to expand that
-        in the future.
-        
-        Datanommer criteria are composed of three things:
-        
-        - A **filter** limits the scope of the query to datanommer.
-        - An **operation** defines what we want to do with the filtered query.
-          Currently, we can only *count* the results.
-        - A **condition** defines how we want to compare the results of the
-          **operation** to determine if our criteria matches or not.
-        
-        Here's an example of a simple criteria definition::
-        
-            criteria:
-              filter:
-                topics:
-                - "%(topic)s"
-              operation: count
-              condition:
-                greater than or equal to: 2
-        
-        The above criteria will match if there is more than one message in datanommer
-        with the same topic as the incoming message being handled.  Here, ``"%(topic)s"``
-        is a `template variable`.  Template variables will have their values
-        substituted before the expensive check is made against datanommer.
-        
-        ----
-        
-        The above example doesn't make much sense -- we'd never use it for a real
-        badge.  The criteria would be true if there were two of *any* message kicked
-        off by *any* user at any time in the past.  Pretty generic.
-        Here's a more interesting criteria definition::
-        
-            criteria:
-              filter:
-                topics:
-                - org.fedoraproject.prod.git.receive
-                usernames:
-                - "%(msg.commit.username)s"
-              operation: count
-              condition:
-                greater than or equal to: 50
-        
-        This criteria would match if there existed 50 messages of the topic
-        ``"org.fedoraproject.prod.git.receive"`` that were also kicked off by whatever
-        user is listed in the ``msg['msg']['commit']['username']`` field of the
-        message being currently processed.  In other words, this criteria would match
-        if the user has pushed to the fedora git repos 50 or more times.
-        
-        ----
-        
-        You can do some fancy things with the **condition** of a datanommer
-        filter.  Here's a list of the possible comparisons you can make:
-        
-        - ``"is greater than or equal to"`` or alternatively
-          ``"greater than or equal to"``
-        - ``"greater than"``
-        - ``"is less than or equal to"`` or alternatively
-          ``"less than or equal to"``
-        - ``"less than"``
-        - ``"equal to"`` or alternatively ``"is equal to"``
-        - ``"is not"`` or alternatively ``"is not equal to"``
-        
-        As you can see, some of them are synonyms for each other.
-        
-        ----
-        
-        If any of those don't meet your needs, you can specify a custom expression
-        by using the ``lambda`` condition whereby fedbadges will compile whatever
-        statement you provide into a callable and use that at runtime.  For example::
-        
-        
-            criteria:
-              filter:
-                topics:
-                - org.fedoraproject.prod.git.receive
-                usernames:
-                - "%(msg.commit.username)s"
-              operation: count
-              condition:
-                lambda: value != 0 and ((value & (value - 1)) == 0)
-        
-        Who knows why you would want to do this, but the above criteria check will
-        succeed if the number of messages returned from the filtered datanommer query
-        is exactly a power of 2.
-        
-        Specifying Recipients
-        ~~~~~~~~~~~~~~~~~~~~~
-        
-        By default, if the trigger and criteria match, fedbadges will award badges
-        to all the users returned by a call to ``fedmsg.meta.msg2usernames(msg)``.
-        This *usually* corresponds with "what users are responsible" for this message.
-        That is *usually* what we want to award badges for.
-        
-        There are some instances for which that is not what we want.
-        
-        Take the `org.fedoraproject.prod.fas.group.member.remove
-        <http://www.fedmsg.com/en/latest/topics/#fas-group-member-remove>`_
-        message for example.  When user A removes user B from a group, both
-        usernames are returned from a call to ``fedmsg.meta.msg2usernames(msg)``
-        with no further distinction as to which was removing and which was removed.
-        
-        Imagine we have a "Group Pruner" badge that's awarded to group admins who
-        remove inactive users from groups.  We don't want to inadvertently award
-        that badge to the persons who *were removed*, only to those who *removed
-        them*.
-        
-        To allow for this scenario, badges may optionally define a ``recipient``
-        in dotted notation that tells fedbadges where to find the username of the
-        recipient in the originating message.  For instance, the following would
-        handle the fas case we described above::
-        
-        
-            trigger:
-              topic: org.fedoraproject.prod.fas.group.member.remove
-            criteria:
-              filter:
-                topics:
-                - "%(topic)s"
-              operation: count
-              condition:
-                greater than or equal to: 1
-            recipient: "%(msg.agent.username)s"
-Platform: UNKNOWN
+Fedora Badges Message consumer
+==============================
+
+This repo contains the consumer and the command necessary to hook the
+badges stack (Tahrir, Tahrir-API, Tahrir-REST) into Fedora Messaging.
+It is the process that runs in the background, monitoring activity of Fedora
+contributors, and is responsible for awarding badges for activity as it happens.
+It is separate from and sometimes confused with the *frontend* of the badges system
+called `tahrir <https://github.com/fedora-infra/tahrir>`_.
+This project (fedbadges) writes to a database that the web frontend (tahrir) reads
+from.
+
+The *actual badge rules* that we act on in Fedora Infrastructure can be
+found `here <https://pagure.io/Fedora-Badges>`.
+
+Architecture
+------------
+
+fedbadges is a callback class for the Fedora Messaging consumer.
+When started, it will load some initial configuration
+and a set of ``BadgeRules`` (more on that later) and then sit quietly
+listening to the Fedora Messaging bus.  Each rule (composed of some metadata,
+a ``trigger``, and a set of ``criteria``) is defined on disk as a yaml file.
+
+* When a new message comes along, our callback looks to see if it matches
+  any of the ``BadgeRules`` it has registered.
+
+* Each BadgeRule must define a ``trigger`` -- a *lightweight* check.
+  When processing a message, this is the first thing that is checked.  It
+  defines a *pattern* that the message must match.  If the message does not
+  match, then the current BadgeRule is discarded and processing moves to
+  the next.
+
+  A ``trigger`` is typically something like "any bodhi message"
+  or "messages only from the failure of a koji build".  More on their
+  specification below.
+
+* BadgeRules must also define a set of ``criteria`` -- a more *heavyweight*
+  check.  During the processing of a newly received message, if the
+  message matches a BadgeRule's ``trigger``, the ``criteria`` is then
+  considered.  This typically involves a more expensive query to the
+  `datanommer <https://github.com/fedora-infra/datanommer>`_ database.
+
+  A BadgeRule ``criteria`` may read something like "$user has
+  pushed 200 bodhi updates to stable" or "$user chaired an IRC meeting".
+
+  **Aside:** Although datanommer is the only currently supported backend, we
+  can implement other queryable backend in the future as needed like FAS
+  (to see if the user is in X number of groups) or even off-site services
+  like libravatar (to award a badge if the user is a user of the AGPL web
+  service).
+
+* If a badge's ``trigger`` and ``criteria`` both match, then the badge is
+  awarded.  If the BadgeRule doesn't specify, we award the badge to all
+  usernames returned by the message's ``usernames`` property.
+
+  That is usually correct -- but sometimes, a BadgeRule needs to specify
+  that one particular user (not all related users) should be recipients of
+  the badge.  In this case, the BadgeRule may define a ``recipient``
+  in dot-notation that instructs the ``Consumer`` how to extract the
+  recipient's username from the received message.
+
+  The badge is awarded to our deserving user via the `tahrir_api
+  <https://github.com/fedora-infra/tahrir-api>`_.  At the end of the day,
+  this amounts to adding a row in a database table for the `Tahrir
+  <https://github.com/fedora-infra/tahrir>`_ application.
+
+There are some optimizations in place omitted above for clarity.
+For instance, after the trigger has matched we first check if the user
+that *would* be awarded the badge already has it.  If they do, we stop
+processing the badge rule immediately to avoid making an unnecessary
+expensive check against the datanommer db.
+
+Configuration - Global
+----------------------
+
+fedbadges needs three major pieces of global configuration.
+All configuration is loaded in the standard Fedora Messaging way, from
+the ``[consumer_config]`` section of the configuration file. See
+`fedbadges.toml.example
+<https://github.com/fedora-infra/fedbadges/blob/develop/fedbadges.toml.example>`_
+in the git repo for an example.
+
+fedbadges also emits its own messages. Please note that the ``topic_prefix`` in
+the configuration should at least be ``badges``. In the Fedora Infrastructure,
+it will be ``org.fedoraproject.prod.badges``.
+
+Configuration - BadgeRule specification
+---------------------------------------
+
+BadgeRules are specified in `YAML <http://www.yaml.org/>`_ on the file system.
+
+Triggers
+~~~~~~~~
+
+Every BadgeRule must carry the following minimum set of metadata::
+
+    # This is some metadata about the badge
+    name:           Like a Rock
+    description:    You have pushed 500 or more bodhi updates to stable status.
+    creator:        ralph
+
+    # This is a link to the discussion about adopting this as a for-real badge.
+    discussion: http://github.com/fedora-infra/badges/pull/SOME_NUMBER
+
+    # A link to the image for the badge
+    image_url: http://somelink.org/to-an-image.png
+
+Here's a simple example of a ``trigger``::
+
+    trigger:
+      category: bodhi
+
+The above will match any bodhi message on any of the topics that come
+from the bodhi update system.
+
+Triggers may employ a little bit of logic to make more complex
+filters.  The following trigger will match any message that comes from
+*either* the bodhi update system or the fedora git package repos::
+
+    trigger:
+      category:
+        any:
+          - bodhi
+          - git
+
+At present triggers may directly compare themselves against only the
+`category` or the `topic` of a message.  In the future we'd like to add
+more comparisons.. in the meantime, here's an example of comparing against
+the fully qualified message topic.  This will match any message
+that is specifically for editing a wiki page::
+
+    trigger:
+      topic: org.fedoraproject.prod.wiki.article.edit
+
+----
+
+There is one additional way you can specify a trigger.  If you need more
+flexibility than ``topic`` and
+``category`` allow, you may specify a custom filter expression with a
+``lambda`` filter.  For example::
+
+    trigger:
+      lambda: "a string of interest" in json.dumps(msg)
+
+The above trigger will match if the string ``"a string of interest"`` appears
+anywhere in the incoming message.  fedbadges takes the expression you provide
+it and compiles it into a python callable on initialization.  Our callable
+here serializes the message to a JSON string before doing its comparison.
+Powerful!
+
+Criteria
+~~~~~~~~
+
+As mentioned above in the architecture section, we currently only support
+datanommer as a queryable backend for criteria.  We hope to expand that
+in the future.
+
+Datanommer criteria are composed of three things:
+
+- A **filter** limits the scope of the query to datanommer.
+- An **operation** defines what we want to do with the filtered query.
+  Currently, we can only *count* the results.
+- A **condition** defines how we want to compare the results of the
+  **operation** to determine if our criteria matches or not.
+
+Here's an example of a simple criteria definition::
+
+    criteria:
+      filter:
+        topics:
+        - "%(topic)s"
+      operation: count
+      condition:
+        greater than or equal to: 2
+
+The above criteria will match if there is more than one message in datanommer
+with the same topic as the incoming message being handled.  Here, ``"%(topic)s"``
+is a `template variable`.  Template variables will have their values
+substituted before the expensive check is made against datanommer.
+
+----
+
+The above example doesn't make much sense -- we'd never use it for a real
+badge.  The criteria would be true if there were two of *any* message kicked
+off by *any* user at any time in the past.  Pretty generic.
+Here's a more interesting criteria definition::
+
+    criteria:
+      filter:
+        topics:
+        - org.fedoraproject.prod.git.receive
+        usernames:
+        - "%(msg.commit.username)s"
+      operation: count
+      condition:
+        greater than or equal to: 50
+
+This criteria would match if there existed 50 messages of the topic
+``"org.fedoraproject.prod.git.receive"`` that were also kicked off by whatever
+user is listed in the ``msg['msg']['commit']['username']`` field of the
+message being currently processed.  In other words, this criteria would match
+if the user has pushed to the fedora git repos 50 or more times.
+
+----
+
+You can do some fancy things with the **condition** of a datanommer
+filter.  Here's a list of the possible comparisons you can make:
+
+- ``"is greater than or equal to"`` or alternatively
+  ``"greater than or equal to"``
+- ``"greater than"``
+- ``"is less than or equal to"`` or alternatively
+  ``"less than or equal to"``
+- ``"less than"``
+- ``"equal to"`` or alternatively ``"is equal to"``
+- ``"is not"`` or alternatively ``"is not equal to"``
+
+As you can see, some of them are synonyms for each other.
+
+----
+
+If any of those don't meet your needs, you can specify a custom expression
+by using the ``lambda`` condition whereby fedbadges will compile whatever
+statement you provide into a callable and use that at runtime.  For example::
+
+
+    criteria:
+      filter:
+        topics:
+        - org.fedoraproject.prod.git.receive
+        usernames:
+        - "%(msg.commit.username)s"
+      operation: count
+      condition:
+        lambda: value != 0 and ((value & (value - 1)) == 0)
+
+Who knows why you would want to do this, but the above criteria check will
+succeed if the number of messages returned from the filtered datanommer query
+is exactly a power of 2.
+
+Specifying Recipients
+~~~~~~~~~~~~~~~~~~~~~
+
+By default, if the trigger and criteria match, fedbadges will award badges
+to all the users returned by the message's ``usernames`` property.
+This *usually* corresponds with "what users are responsible" for this message.
+That is *usually* what we want to award badges for.
+
+There are some instances for which that is not what we want.
+
+Take the `org.fedoraproject.prod.fas.group.member.sponsor
+<https://fedora-messaging.readthedocs.io/en/stable/user-guide/schemas.html#fas>`_
+message for example.  When user A sponsors user B to a group, both
+usernames are returned by the message's ``usernames`` property with no
+further distinction as to which was adding and which was added.
+
+Imagine we have a "Group Sponsor" badge that's awarded to group admins who
+sponsor users to groups.  We don't want to inadvertently award that badge
+to the persons who *were sponsored*, only to those who *sponsored them*.
+
+To allow for this scenario, badges may optionally define a ``recipient``
+in dotted notation that tells fedbadges where to find the username of the
+recipient in the originating message.  For instance, the following would
+handle the fas case we described above::
+
+    trigger:
+      topic: org.fedoraproject.prod.fas.group.member.sponsor
+    criteria:
+      filter:
+        topics:
+        - "%(topic)s"
+      operation: count
+      condition:
+        greater than or equal to: 1
+    recipient: "%(msg.agent_name)s"
```

### Comparing `fedbadges-1.0.2/README.rst` & `fedbadges-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,116 @@
-Fedora Badges
-=============
+Metadata-Version: 2.1
+Name: fedbadges
+Version: 2.0.0
+Summary: Fedora Messaging consumer for awarding open badges
+Home-page: https://github.com/fedora-infra/fedbadges
+License: GPL-2.0-or-later
+Keywords: fedora
+Author: Fedora Infrastructure
+Author-email: admin@fedoraproject.org
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: schemas
+Requires-Dist: anitya-schema ; extra == "schemas"
+Requires-Dist: backoff (>=2.2.1,<3.0.0)
+Requires-Dist: bodhi-messages ; extra == "schemas"
+Requires-Dist: bugzilla2fedmsg-schema ; extra == "schemas"
+Requires-Dist: ci-messages ; extra == "schemas"
+Requires-Dist: click (>=8.0.0,<9.0.0)
+Requires-Dist: copr-messaging ; extra == "schemas"
+Requires-Dist: datanommer-models (>=1.2.0,<2.0.0)
+Requires-Dist: discourse2fedmsg-messages ; extra == "schemas"
+Requires-Dist: fasjson-client (>=1.0.8,<2.0.0)
+Requires-Dist: fedocal-messages ; extra == "schemas"
+Requires-Dist: fedora-elections-messages ; extra == "schemas"
+Requires-Dist: fedora-messaging (>=3.5.0,<4.0.0)
+Requires-Dist: fedora-messaging-git-hook-messages ; extra == "schemas"
+Requires-Dist: fedora-messaging-the-new-hotness-schema ; extra == "schemas"
+Requires-Dist: fedora-planet-messages ; extra == "schemas"
+Requires-Dist: fedorainfra-ansible-messages ; extra == "schemas"
+Requires-Dist: fmn-messages ; extra == "schemas"
+Requires-Dist: kerneltest-messages (>=1.0.0,<2.0.0) ; extra == "schemas"
+Requires-Dist: koji-fedoramessaging-messages (>=1.2.2,<2.0.0) ; extra == "schemas"
+Requires-Dist: koschei-messages ; extra == "schemas"
+Requires-Dist: mdapi-messages ; extra == "schemas"
+Requires-Dist: mediawiki-messages ; extra == "schemas"
+Requires-Dist: meetbot-messages ; extra == "schemas"
+Requires-Dist: noggin-messages ; extra == "schemas"
+Requires-Dist: nuancier-messages ; extra == "schemas"
+Requires-Dist: pagure-messages ; extra == "schemas"
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
+Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tahrir-api (>=1.0.0,<2.0.0)
+Requires-Dist: tahrir-messages ; extra == "schemas"
+Project-URL: Repository, https://github.com/fedora-infra/fedbadges
+Description-Content-Type: text/x-rst
+
+Fedora Badges Message consumer
+==============================
 
 This repo contains the consumer and the command necessary to hook the
-badges stack (Tahrir, Tahrir-API, Tahrir-REST) into fedmsg.  It is the process
-that runs in the background, monitoring activity of Fedora contributors, and is
-responsible for awarding badges for activity as it happens.  It is separate
-from and sometimes confused with the *frontend* of the badges system; that web
-application is called `tahrir <https://github.com/fedora-infra/tahrir>`_.  This
-project (fedbadges) writes to a database that the web frontend (tahrir) reads
+badges stack (Tahrir, Tahrir-API, Tahrir-REST) into Fedora Messaging.
+It is the process that runs in the background, monitoring activity of Fedora
+contributors, and is responsible for awarding badges for activity as it happens.
+It is separate from and sometimes confused with the *frontend* of the badges system
+called `tahrir <https://github.com/fedora-infra/tahrir>`_.
+This project (fedbadges) writes to a database that the web frontend (tahrir) reads
 from.
 
 The *actual badge rules* that we act on in Fedora Infrastructure can be
 found `here <https://pagure.io/Fedora-Badges>`.
 
 Architecture
 ------------
 
-fedbadges runs as a ``Consumer`` plugin to the ``fedmsg-hub`` (really,
-a moksha-hub).  When started, it will load some initial configuration
+fedbadges is a callback class for the Fedora Messaging consumer.
+When started, it will load some initial configuration
 and a set of ``BadgeRules`` (more on that later) and then sit quietly
-listening to the fedmsg bus.  Each rule (composed of some metadata,
+listening to the Fedora Messaging bus.  Each rule (composed of some metadata,
 a ``trigger``, and a set of ``criteria``) is defined on disk as a yaml file.
 
-* When a new message comes along, our ``Consumer`` looks to see if it matches
+* When a new message comes along, our callback looks to see if it matches
   any of the ``BadgeRules`` it has registered.
 
-* Each BadgeRule must define a ``trigger`` -- a `lightweight` check.
+* Each BadgeRule must define a ``trigger`` -- a *lightweight* check.
   When processing a message, this is the first thing that is checked.  It
   defines a *pattern* that the message must match.  If the message does not
   match, then the current BadgeRule is discarded and processing moves to
   the next.
 
   A ``trigger`` is typically something like "any bodhi message"
   or "messages only from the failure of a koji build".  More on their
   specification below.
 
-* BadgeRules must also define a set of ``criteria`` -- a more `heavyweight`
-  checks.  During the processing of a newly received message, if the
+* BadgeRules must also define a set of ``criteria`` -- a more *heavyweight*
+  check.  During the processing of a newly received message, if the
   message matches a BadgeRule's ``trigger``, the ``criteria`` is then
   considered.  This typically involves a more expensive query to the
   `datanommer <https://github.com/fedora-infra/datanommer>`_ database.
 
   A BadgeRule ``criteria`` may read something like "$user has
   pushed 200 bodhi updates to stable" or "$user chaired an IRC meeting".
 
   **Aside:** Although datanommer is the only currently supported backend, we
-  can implement other queryable backend in the future as needed like FAS2
+  can implement other queryable backend in the future as needed like FAS
   (to see if the user is in X number of groups) or even off-site services
   like libravatar (to award a badge if the user is a user of the AGPL web
   service).
 
 * If a badge's ``trigger`` and ``criteria`` both match, then the badge is
   awarded.  If the BadgeRule doesn't specify, we award the badge to all
-  usernames returned by a call to ``fedmsg.meta.msg2usernames(msg)``.
+  usernames returned by the message's ``usernames`` property.
 
   That is usually correct -- but sometimes, a BadgeRule needs to specify
   that one particular user (not all related users) should be recipients of
   the badge.  In this case, the BadgeRule may define a ``recipient``
   in dot-notation that instructs the ``Consumer`` how to extract the
   recipient's username from the received message.
 
@@ -71,31 +125,23 @@
 processing the badge rule immediately to avoid making an unnecessary
 expensive check against the datanommer db.
 
 Configuration - Global
 ----------------------
 
 fedbadges needs three major pieces of global configuration.
-All configuration is loaded in the standard fedmsg way, from
-python files in ``/etc/fedmsg.d/``.
-
-First, generic and tahrir-related configuration.  See
-`fedmsg.d/badges-global.py
-<https://github.com/fedora-infra/fedbadges/blob/develop/fedmsg.d/badges-global.py>`_
+All configuration is loaded in the standard Fedora Messaging way, from
+the ``[consumer_config]`` section of the configuration file. See
+`fedbadges.toml.example
+<https://github.com/fedora-infra/fedbadges/blob/develop/fedbadges.toml.example>`_
 in the git repo for an example.
 
-Second, datanommer connection information.  See
-`fedmsg.d/datanommer.py
-<https://github.com/fedora-infra/fedbadges/blob/develop/fedmsg.d/datanommer.py>`_
-in the git repo for an example.
-
-Third, fedbadges emits its own fedmsg messages when it awards badges.  It will
-need its own endpoint definitions for this.  See `fedmsg.d/endpoints.py
-<https://github.com/fedora-infra/fedbadges/blob/develop/fedmsg.d/endpoints.py>`_
-in the git repo for an example.
+fedbadges also emits its own messages. Please note that the ``topic_prefix`` in
+the configuration should at least be ``badges``. In the Fedora Infrastructure,
+it will be ``org.fedoraproject.prod.badges``.
 
 Configuration - BadgeRule specification
 ---------------------------------------
 
 BadgeRules are specified in `YAML <http://www.yaml.org/>`_ on the file system.
 
 Triggers
@@ -247,40 +293,39 @@
 succeed if the number of messages returned from the filtered datanommer query
 is exactly a power of 2.
 
 Specifying Recipients
 ~~~~~~~~~~~~~~~~~~~~~
 
 By default, if the trigger and criteria match, fedbadges will award badges
-to all the users returned by a call to ``fedmsg.meta.msg2usernames(msg)``.
+to all the users returned by the message's ``usernames`` property.
 This *usually* corresponds with "what users are responsible" for this message.
 That is *usually* what we want to award badges for.
 
 There are some instances for which that is not what we want.
 
-Take the `org.fedoraproject.prod.fas.group.member.remove
-<http://www.fedmsg.com/en/latest/topics/#fas-group-member-remove>`_
-message for example.  When user A removes user B from a group, both
-usernames are returned from a call to ``fedmsg.meta.msg2usernames(msg)``
-with no further distinction as to which was removing and which was removed.
-
-Imagine we have a "Group Pruner" badge that's awarded to group admins who
-remove inactive users from groups.  We don't want to inadvertently award
-that badge to the persons who *were removed*, only to those who *removed
-them*.
+Take the `org.fedoraproject.prod.fas.group.member.sponsor
+<https://fedora-messaging.readthedocs.io/en/stable/user-guide/schemas.html#fas>`_
+message for example.  When user A sponsors user B to a group, both
+usernames are returned by the message's ``usernames`` property with no
+further distinction as to which was adding and which was added.
+
+Imagine we have a "Group Sponsor" badge that's awarded to group admins who
+sponsor users to groups.  We don't want to inadvertently award that badge
+to the persons who *were sponsored*, only to those who *sponsored them*.
 
 To allow for this scenario, badges may optionally define a ``recipient``
 in dotted notation that tells fedbadges where to find the username of the
 recipient in the originating message.  For instance, the following would
 handle the fas case we described above::
 
-
     trigger:
-      topic: org.fedoraproject.prod.fas.group.member.remove
+      topic: org.fedoraproject.prod.fas.group.member.sponsor
     criteria:
       filter:
         topics:
         - "%(topic)s"
       operation: count
       condition:
         greater than or equal to: 1
-    recipient: "%(msg.agent.username)s"
+    recipient: "%(msg.agent_name)s"
+
```

### Comparing `fedbadges-1.0.2/fedbadges/rules.py` & `fedbadges-2.0.0/fedbadges/rules.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,508 +1,505 @@
-# -*- coding; utf-8 -*-
 """ Models for fedbadges.
 
 The primary thing here is a "BadgeRule" which is an in-memory working
 abstraction of the trigger and criteria required to award a badge.
 
 Authors:    Ralph Bean
 """
 
 import abc
 import copy
-import json
-import types
 import functools
 import inspect
-import transaction
+import logging
 import re
 
-import fedmsg.config
-import fedmsg.meta
-import fedmsg.encoding
 import datanommer.models
+from fedora_messaging.api import Message
+from tahrir_api.dbapi import TahrirDatabase
 
 from fedbadges.utils import (
     # These are all in-process utilities
     construct_substitutions,
+    email2fas,
     format_args,
-    single_argument_lambda_factory,
-    recursive_lambda_factory,
-    graceful,
     get_pagure_authors,
-
+    graceful,
+    nick2fas,
+    recursive_lambda_factory,
+    single_argument_lambda_factory,
     # These make networked API calls
     user_exists_in_fas,
 )
 
-import logging
-log = logging.getLogger('moksha.hub')
-
 
-nick2fas = None
-try:
-    from fedmsg_meta_fedora_infrastructure.fasshim import nick2fas
-except ImportError as e:
-    log.warn("Could not import nick2fas: %r" % e)
+log = logging.getLogger(__name__)
 
 
-email2fas = None
-try:
-    from fedmsg_meta_fedora_infrastructure.fasshim import email2fas
-except ImportError as e:
-    log.warn("Could not import email2fas: %r" % e)
-
 # Match OpenID agent strings, i.e. http://FAS.id.fedoraproject.org
-def openid2fas(openid, **config):
-    m = re.search('^https?://([a-z][a-z0-9]+)\.id\.fedoraproject\.org$', openid)
+def openid2fas(openid, config):
+    id_provider_hostname = re.escape(config["id_provider_hostname"])
+    m = re.search(f"^https?://([a-z][a-z0-9]+)\\.{id_provider_hostname}$", openid)
     if m:
         return m.group(1)
     return openid
 
-operators = frozenset([
-    "all",
-    "any",
-    "not",
-])
-lambdas = frozenset([
-    "lambda",
-])
-
-operator_lookup = {
-    "any": any,
-    "all": all,
-    "not": lambda x: all([not item for item in x])
-}
-
-fedmsg_config = fedmsg.config.load_config()
-fedmsg.meta.make_processors(**fedmsg_config)
-
-
-class BadgeRule(object):
-    required = frozenset([
-        'name',
-        'image_url',
-        'description',
-        'creator',
-        'discussion',
-        'issuer_id',
-
-        'trigger',
-        'criteria',
-    ])
-
-    possible = required.union([
-        'recipient',
-        'recipient_nick2fas',
-        'recipient_email2fas',
-        'recipient_openid2fas',
-    ])
-
-    banned_usernames = frozenset([
-        'bodhi',
-        'oscar',
-        'apache',
-        'koji',
-        'bodhi',
-        'taskotron',
-    ])
 
-    def __init__(self, badge_dict, tahrir_database, issuer_id):
-        argued_fields = frozenset(badge_dict.keys())
+def github2fas(uri, config, fasjson):
+    m = re.search(r"^https?://api.github.com/users/([a-z][a-z0-9-]+)$", uri)
+    if not m:
+        log.warning("Can't extract the username from %r", uri)
+        return None
+    github_username = m.group(1)
+    result = fasjson.search_users(github_username__exact=github_username)
+    if len(result) != 1:
+        return None
+    return result[0]["username"]
 
-        if not argued_fields.issubset(self.possible):
-            raise KeyError(
-                "%r are not possible fields.  Choose from %r" % (
-                    argued_fields.difference(self.possible),
-                    self.possible
-                ))
 
-        if not self.required.issubset(argued_fields):
-            raise ValueError(
-                "BadgeRule requires %r.  Missing %r" % (
-                    self.required,
-                    self.required.difference(argued_fields),
-                ))
+def distgit2fas(uri, config):
+    distgit_hostname = re.escape(config["distgit_hostname"])
+    m = re.search(f"^https?://{distgit_hostname}/user/([a-z][a-z0-9]+)$", uri)
+    if m:
+        return m.group(1)
+    return uri
 
-        self._d = badge_dict
 
-        self.tahrir = tahrir_database
-        if self.tahrir:
-            transaction.begin()
-            self.badge_id = self._d['badge_id'] = self.tahrir.add_badge(
-                name=self._d['name'],
-                image=self._d['image_url'],
-                desc=self._d['description'],
-                criteria=self._d['discussion'],
-                tags=','.join(self._d.get('tags', [])),
-                issuer_id=issuer_id,
-            )
-            transaction.commit()
+def krb2fas(name):
+    if "/" not in name:
+        return name
+    return name.split("/")[0]
+
+
+def validate_possible(possible, fields):
+    fields_set = set(fields)
+    if not fields_set.issubset(possible):
+        raise KeyError(
+            f"{fields_set.difference(possible)!r} are not possible fields. "
+            f"Choose from {possible!r}"
+        )
+
+
+def validate_badge(required, possible, badge_dict):
+    fields = frozenset(list(badge_dict.keys()))
+    validate_possible(possible, fields)
+    if required and not required.issubset(fields):
+        raise ValueError(
+            f"BadgeRule requires {required!r}. Missing {required.difference(fields)!r}"
+        )
+
 
-        self.trigger = Trigger(self._d['trigger'], self)
-        self.criteria = Criteria(self._d['criteria'], self)
-        self.recipient_key = self._d.get('recipient')
-        self.recipient_nick2fas = self._d.get('recipient_nick2fas')
-        self.recipient_email2fas = self._d.get('recipient_email2fas')
-        self.recipient_openid2fas = self._d.get('recipient_openid2fas')
-
-        # A sanity check before we kick things off.
-        if self.recipient_nick2fas and not nick2fas:
-            raise ImportError("recipient_nick2fas specified, but "
-                              "nick2fas is not available.")
-
-        if self.recipient_email2fas and not email2fas:
-            raise ImportError("recipient_email2fas specified, but "
-                              "email2fas is not available.")
+operators = frozenset(
+    [
+        "all",
+        "any",
+        "not",
+    ]
+)
+lambdas = frozenset(
+    [
+        "lambda",
+    ]
+)
+
+operator_lookup = {"any": any, "all": all, "not": lambda x: all([not item for item in x])}
+
+
+class BadgeRule:
+    required = frozenset(
+        [
+            "name",
+            "image_url",
+            "description",
+            "creator",
+            "discussion",
+            "issuer_id",
+            "trigger",
+            "criteria",
+        ]
+    )
+
+    possible = required.union(
+        [
+            "recipient",
+            "recipient_nick2fas",
+            "recipient_email2fas",
+            "recipient_openid2fas",
+            "recipient_github2fas",
+            "recipient_distgit2fas",
+            "recipient_krb2fas",
+        ]
+    )
+
+    banned_usernames = frozenset(
+        [
+            "bodhi",
+            "oscar",
+            "apache",
+            "koji",
+            "bodhi",
+            "taskotron",
+        ]
+    )
+
+    def __init__(self, badge_dict, issuer_id, config, fasjson):
+        validate_badge(self.required, self.possible, badge_dict)
+        self._d = badge_dict
+        self.issuer_id = issuer_id
+        self.config = config
+        self.fasjson = fasjson
+
+        self.trigger = Trigger(self._d["trigger"], self)
+        self.criteria = Criteria(self._d["criteria"], self)
+        self.recipient_key = self._d.get("recipient")
+        self.recipient_nick2fas = self._d.get("recipient_nick2fas")
+        self.recipient_email2fas = self._d.get("recipient_email2fas")
+        self.recipient_openid2fas = self._d.get("recipient_openid2fas")
+        self.recipient_github2fas = self._d.get("recipient_github2fas")
+        self.recipient_distgit2fas = self._d.get("recipient_distgit2fas")
+        self.recipient_krb2fas = self._d.get("recipient_krb2fas")
+
+    def setup(self, tahrir: TahrirDatabase):
+        self.badge_id = self._d["badge_id"] = tahrir.add_badge(
+            name=self._d["name"],
+            image=self._d["image_url"],
+            desc=self._d["description"],
+            criteria=self._d["discussion"],
+            tags=",".join(self._d.get("tags", [])),
+            issuer_id=self.issuer_id,
+        )
+        tahrir.session.commit()
 
     def __getitem__(self, key):
         return self._d[key]
 
     def __repr__(self):
-        return "<fedbadges.models.BadgeRule: %r>" % self._d
+        return f"<fedbadges.models.BadgeRule: {self._d!r}>"
 
-    def matches(self, msg):
+    def matches(self, msg: Message, tahrir: TahrirDatabase):
 
         # First, do a lightweight check to see if the msg matches a pattern.
         if not self.trigger.matches(msg):
             return set()
 
         # Before proceeding further, let's see who would get this badge if
         # our more heavyweight checks matched up.  If the user specifies a
         # recipient_key, we can use that to extract the potential awardee.  If
-        # that is not specified, we just use `msg2usernames`.
+        # that is not specified, we just use `msg.usernames`.
         if self.recipient_key:
             subs = construct_substitutions(msg)
             obj = format_args(self.recipient_key, subs)
 
-            if isinstance(obj, (basestring, int, float)):
+            if isinstance(obj, (str, int, float)):
                 obj = [obj]
 
             # On the way, it is possible for the fedmsg message to contain None
             # for "agent".  A problem here though is that None is not iterable,
             # so let's replace it with an equivalently empty iterable so code
             # further down doesn't freak out.  An instance of this is when a
             # user without a fas account comments on a bodhi update.
             if obj is None:
                 obj = []
 
-
             # It is possible to recieve a list of dictionary containing the name
             # of the recipient, this is the case in the pagure's fedmsg.
             # In that case we create a new list containing the names taken from the
             # dictionnary.
 
             new_obj = get_pagure_authors(obj)
             if new_obj:
                 obj = new_obj
 
             awardees = frozenset(obj)
 
             if self.recipient_nick2fas:
-                awardees = frozenset([
-                    nick2fas(nick, **fedmsg_config) for nick in awardees
-                ])
+                awardees = frozenset([nick2fas(nick, self.fasjson) for nick in awardees])
 
             if self.recipient_email2fas:
-                awardees = frozenset([
-                    email2fas(email, **fedmsg_config) for email in awardees
-                ])
+                awardees = frozenset([email2fas(email, self.fasjson) for email in awardees])
 
             if self.recipient_openid2fas:
-                awardees = frozenset([
-                    openid2fas(openid, **fedmsg_config) for openid in awardees
-                ])
+                awardees = frozenset([openid2fas(openid, self.config) for openid in awardees])
+
+            if self.recipient_github2fas:
+                awardees = frozenset(
+                    [github2fas(uri, self.config, self.fasjson) for uri in awardees]
+                )
+
+            if self.recipient_distgit2fas:
+                awardees = frozenset([distgit2fas(uri, self.config) for uri in awardees])
+
+            if self.recipient_krb2fas:
+                awardees = frozenset([krb2fas(uri) for uri in awardees])
+
+            awardees = frozenset([e for e in awardees if e is not None])
         else:
-            usernames = fedmsg.meta.msg2usernames(msg)
-            awardees = usernames.difference(self.banned_usernames)
+            awardees = frozenset(msg.usernames)
+
+        awardees = awardees.difference(self.banned_usernames)
 
         # Strip anyone who is an IP address
-        awardees = frozenset([
-            user for user in awardees if not (
-                user.startswith('192.168.') or
-                user.startswith('10.')
-            )
-        ])
+        awardees = frozenset(
+            [
+                user
+                for user in awardees
+                if not (user.startswith("192.168.") or user.startswith("10."))
+            ]
+        )
 
         # If no-one would get the badge by default, then no reason to waste
         # time doing any further checks.  No need to query the Tahrir DB.
         if not awardees:
             return awardees
 
         # Limit awardees to only those who do not already have this badge.
-        # Do this only if we have an active connection to the Tahrir DB.
-        if self.tahrir:
-            awardees = frozenset([
-                user for user in awardees
-                if not self.tahrir.assertion_exists(
-                    self.badge_id, "%s@fedoraproject.org" % user
-                )])
-
-            # Also, exclude any potential awardees who have opted out.
-            awardees = frozenset([
-                user for user in awardees
-                if not self.tahrir.person_opted_out(
-                    "%s@fedoraproject.org" % user
-                )])
+        awardees = frozenset(
+            [
+                user
+                for user in awardees
+                if not tahrir.assertion_exists(self.badge_id, f"{user}@fedoraproject.org")
+                and not tahrir.person_opted_out(f"{user}@fedoraproject.org")
+            ]
+        )
 
         # If no-one would get the badge at this point, then no reason to waste
         # time doing any further checks.  No need to query datanommer.
         if not awardees:
             return awardees
 
         # Check our backend criteria -- likely, perform datanommer queries.
         try:
             if not self.criteria.matches(msg):
                 return set()
-        except IOError as e:
-            log.exception(e)
+        except OSError:
+            log.exception("Failed checking criteria for rule %s", self.badge_id)
             return set()
 
         # Lastly, and this is probably most expensive.  Make sure the person
         # actually has a FAS account before we award anything.
         # https://github.com/fedora-infra/tahrir/issues/225
-        awardees = set([
-            u for u in awardees if user_exists_in_fas(fedmsg_config, u)
-        ])
+        awardees = set([u for u in awardees if user_exists_in_fas(self.fasjson, u)])
 
         return awardees
 
 
-class AbstractComparator(object):
-    """ Base class for shared behavior between trigger and criteria. """
-    __metaclass__ = abc.ABCMeta
+class AbstractComparator(metaclass=abc.ABCMeta):
+    """Base class for shared behavior between trigger and criteria."""
+
     possible = required = frozenset()
     children = None
 
     def __init__(self, d, parent=None):
-        argued_fields = frozenset(d.keys())
-        if not argued_fields.issubset(self.possible):
-            raise KeyError(
-                "%r are not possible fields.  Choose from %r" % (
-                    argued_fields.difference(self.possible),
-                    self.possible
-                ))
-
-        if self.required and not self.required.issubset(argued_fields):
-            raise ValueError(
-                "%r are required fields.  Missing %r" % (
-                    self.required,
-                    self.required.difference(argued_fields),
-                ))
-
+        validate_badge(self.required, self.possible, d)
         self._d = d
         self.parent = parent
 
     def __repr__(self):
-        return "<%s: %r> which is a child of %s" % (
-            type(self).__name__, self._d, repr(self.parent)
-        )
+        return f"<{self.__class__.__name__}: {self._d!r}>, a child of {self.parent!r}"
 
     @abc.abstractmethod
     def matches(self, msg):
         pass
 
 
 class AbstractTopLevelComparator(AbstractComparator):
     def __init__(self, *args, **kwargs):
-        super(AbstractTopLevelComparator, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         cls = type(self)
 
         if len(self._d) > 1:
-            raise ValueError("No more than one trigger allowed.  "
-                             "Use an operator, one of %r" % operators)
-
-        self.attribute = self._d.keys()[0]
+            raise ValueError(
+                "No more than one trigger allowed.  " "Use an operator, one of %r" % operators
+            )
+        self.attribute = next(iter(self._d))
         self.expected_value = self._d[self.attribute]
 
         # XXX - Check if we should we recursively nest Trigger/Criteria?
 
         # First, trick negation into thinking it is not a unary operator.
-        if self.attribute == 'not':
+        if self.attribute == "not":
             self.expected_value = [self.expected_value]
 
         # Then, treat everything as if it accepts an arbitrary # of args.
         if self.attribute in operators:
             if not isinstance(self.expected_value, list):
-                raise TypeError("Operators only accept lists, not %r" %
-                                type(self.expected_value))
+                raise TypeError("Operators only accept lists, not %r" % type(self.expected_value))
             self.children = [cls(child, self) for child in self.expected_value]
 
 
 class Trigger(AbstractTopLevelComparator):
-    possible = frozenset([
-        'topic',
-        'category',
-    ]).union(operators).union(lambdas)
+    possible = (
+        frozenset(
+            [
+                "topic",
+                "category",
+            ]
+        )
+        .union(operators)
+        .union(lambdas)
+    )
 
     @graceful(set())
     def matches(self, msg):
         # Check if we should just aggregate the results of our children.
         # Otherwise, we are a leaf-node doing a straightforward comparison.
         if self.children:
-            return operator_lookup[self.attribute]((
-                child.matches(msg) for child in self.children
-            ))
-        elif self.attribute == 'lambda':
+            return operator_lookup[self.attribute](child.matches(msg) for child in self.children)
+        elif self.attribute == "lambda":
             return single_argument_lambda_factory(
-                expression=self.expected_value, argument=msg, name='msg')
-        elif self.attribute == 'category':
-            # TODO -- use fedmsg.meta.msg2processor(msg).__name__.lower()
-            return msg['topic'].split('.')[3] == self.expected_value
+                expression=self.expected_value,
+                argument={"msg": msg.body, "message": msg},
+                name="msg",
+            )
+        elif self.attribute == "category":
+            return msg.topic.split(".")[3] == self.expected_value
+        elif self.attribute == "topic":
+            return msg.topic.endswith(self.expected_value)
         else:
-            if hasattr(msg[self.attribute], 'endswith'):
-                return msg[self.attribute].endswith(self.expected_value)
-            else:
-                return msg[self.attribute] == self.expected_value
+            raise RuntimeError(f"Unexpected attribute: {self.attribute}")
 
 
 class Criteria(AbstractTopLevelComparator):
-    possible = frozenset([
-        'datanommer',
-    ]).union(operators)
+    possible = frozenset(
+        [
+            "datanommer",
+        ]
+    ).union(operators)
 
     def __init__(self, *args, **kwargs):
-        super(Criteria, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         if not self.children:
             # Then, by AbstractComparator rules, I am a leaf node.  Specialize!
             self._specialize()
 
     def _specialize(self):
-        if self.attribute == 'datanommer':
+        if self.attribute == "datanommer":
             self.specialization = DatanommerCriteria(self.expected_value)
         # TODO -- expand this with other "backends" as necessary
         # elif self.attribute == 'fas'
         else:
             raise RuntimeError("This should be impossible to reach.")
 
     @graceful(set())
     def matches(self, msg):
         if self.children:
-            return operator_lookup[self.attribute]((
-                child.matches(msg) for child in self.children
-            ))
+            return operator_lookup[self.attribute](child.matches(msg) for child in self.children)
         else:
             return self.specialization.matches(msg)
 
 
 class AbstractSpecializedComparator(AbstractComparator):
     pass
 
+
 class DatanommerCriteria(AbstractSpecializedComparator):
-    required = possible = frozenset([
-        'filter',
-        'operation',
-        'condition',
-    ])
+    required = possible = frozenset(
+        [
+            "filter",
+            "operation",
+            "condition",
+        ]
+    )
 
     condition_callbacks = {
-        'is greater than or equal to': lambda t, v: v >= t,
-        'greater than or equal to': lambda t, v: v >= t,
-        'greater than': lambda t, v: v > t,
-
-        'is less than or equal to': lambda t, v: v <= t,
-        'less than or equal to': lambda t, v: v <= t,
-        'less than': lambda t, v: v < t,
-
-        'equal to': lambda t, v: v == t,
-        'is equal to': lambda t, v: v == t,
-
-        'is not': lambda t, v: v != t,
-        'is not equal to': lambda t, v: v != t,
-
-        'lambda': single_argument_lambda_factory,
+        "is greater than or equal to": lambda t, v: v >= t,
+        "greater than or equal to": lambda t, v: v >= t,
+        "greater than": lambda t, v: v > t,
+        "is less than or equal to": lambda t, v: v <= t,
+        "less than or equal to": lambda t, v: v <= t,
+        "less than": lambda t, v: v < t,
+        "equal to": lambda t, v: v == t,
+        "is equal to": lambda t, v: v == t,
+        "is not": lambda t, v: v != t,
+        "is not equal to": lambda t, v: v != t,
+        "lambda": single_argument_lambda_factory,
     }
 
     def __init__(self, *args, **kwargs):
-        super(DatanommerCriteria, self).__init__(*args, **kwargs)
-        if len(self._d['condition']) > 1:
-            conditions = self.condition_callbacks.keys()
-            raise ValueError("No more than one condition allowed.  "
-                             "Use one of %r" % conditions)
-
-        # Determine what arguments datanommer..grep accepts
-        argspec = inspect.getargspec(datanommer.models.Message.grep)
-        irrelevant = frozenset(['defer'])
+        super().__init__(*args, **kwargs)
+        if len(self._d["condition"]) > 1:
+            conditions = list(self.condition_callbacks.keys())
+            raise ValueError("No more than one condition allowed.  " "Use one of %r" % conditions)
+
+        # Determine what arguments datanommer.models.Message.grep accepts
+        argspec = inspect.getfullargspec(datanommer.models.Message.grep)
+        irrelevant = frozenset(["defer"])
         grep_arguments = frozenset(argspec.args[1:]).difference(irrelevant)
 
         # Validate the filter
-        argued_filter_fields = frozenset(self._d['filter'].keys())
-        if not argued_filter_fields.issubset(grep_arguments):
-            raise KeyError(
-                "%r are not possible fields.  Choose from %r" % (
-                    argued_filter_fields.difference(grep_arguments),
-                    grep_arguments,
-                ))
+        validate_possible(grep_arguments, self._d["filter"])
 
         # Validate the condition
-        condition_key, condition_val = self._d['condition'].items()[0]
+        condition_key, condition_val = next(iter(self._d["condition"].items()))
         if condition_key not in self.condition_callbacks:
-            raise KeyError("%r is not a valid condition key.  Use one of %r" %
-                           (condition_key, self.condition_callbacks.keys()))
+            raise KeyError(
+                f"{condition_key!r} is not a valid condition key. "
+                f"Use one of {list(self.condition_callbacks)!r}"
+            )
 
         # Construct a condition callable for later
-        self.condition = functools.partial(
-            self.condition_callbacks[condition_key], condition_val)
+        self.condition = functools.partial(self.condition_callbacks[condition_key], condition_val)
 
     def _construct_query(self, msg):
-        """ Construct a datanommer query for this message.
+        """Construct a datanommer query for this message.
 
         The "filter" section of this criteria object will be used.  It will
         first be formatted with any substitutions present in the incoming
         message.  This is used, for instance, to construct a query like "give
         me all the messages bearing the same topic as the message that just
         arrived".
         """
         subs = construct_substitutions(msg)
-        kwargs = format_args(copy.copy(self._d['filter']), subs)
-        kwargs = recursive_lambda_factory(kwargs, msg, name='msg')
+        kwargs = format_args(copy.copy(self._d["filter"]), subs)
+        kwargs = recursive_lambda_factory(kwargs, {"msg": msg.body, "message": msg}, name="msg")
 
         # It is possible to recieve a list of dictionary containing the name
         # of the recipient, this is the case in the pagure's fedmsg.
         # In that case we create a new list containing the names taken from the
         # dictionnary.
-        if kwargs.get('users') is not None:
-            for item in kwargs['users']:
+        if kwargs.get("users") is not None:
+            for item in kwargs["users"]:
                 if isinstance(item, list):
-                    kwargs['users'] = item
-            users = get_pagure_authors(kwargs['users'])
+                    kwargs["users"] = item
+            users = get_pagure_authors(kwargs["users"])
             if users:
-                kwargs['users'] = users
-        kwargs['defer'] = True
+                kwargs["users"] = users
+        kwargs["defer"] = True
         total, pages, query = datanommer.models.Message.grep(**kwargs)
         return total, pages, query
 
     def _format_lambda_operation(self, msg):
-        """ Format the string representation of a lambda operation.
+        """Format the string representation of a lambda operation.
 
         The lambda operation can be formatted here to include strings that
         appear in the message being evaluated like
         %(msg.comment.update_submitter)s.  Placeholders like that will have
         their value substituted with whatever appears in the incoming message.
         """
         subs = construct_substitutions(msg)
-        operation = format_args(copy.copy(self._d['operation']), subs)
-        return operation['lambda']
+        operation = format_args(copy.copy(self._d["operation"]), subs)
+        return operation["lambda"]
 
-    def matches(self, msg):
-        """ A datanommer criteria check is composed of three steps.
+    def matches(self, msg: Message):
+        """A datanommer criteria check is composed of three steps.
 
         - A datanommer query is constructed by combining our yaml definition
           with the incoming fedmsg message that triggered us.
         - An operation in python is constructed by comining our yaml definition
           with the incoming fedmsg message that triggered us.  That operation
           is then executed against the datanommer query object.
         - A condition, derived from our yaml definition, is evaluated with the
           result of the operation from the previous step and is returned.
         """
         total, pages, query = self._construct_query(msg)
-        if self._d['operation'] == 'count':
+        if self._d["operation"] == "count":
             result = total
-        elif isinstance(self._d['operation'], dict):
+        elif isinstance(self._d["operation"], dict):
             expression = self._format_lambda_operation(msg)
             result = single_argument_lambda_factory(
-                expression=expression, argument=query, name='query')
+                expression=expression, argument=query, name="query"
+            )
         else:
-            operation = getattr(query, self._d['operation'])
+            operation = getattr(query, self._d["operation"])
             result = operation()
         return self.condition(result)
```

### Comparing `fedbadges-1.0.2/fedbadges/utils.py` & `fedbadges-2.0.0/fedbadges/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,135 +1,177 @@
 """ Utilities for fedbadges that don't quite fit anywhere else. """
 
-import types
-
-import logging
-log = logging.getLogger("moksha.hub")
-
-import fedmsg
-import fedora.client
-import requests
-
 # These are here just so they're available in globals()
 # for compiling lambda expressions
 import json
+import logging
 import re
-import fedmsg.config
-import fedmsg.encoding
-import fedmsg.meta
+import sys
+import traceback
+import types
+
+import backoff
+from fedora_messaging import api as fm_api
+from fedora_messaging import exceptions as fm_exceptions
+
+
+log = logging.getLogger(__name__)
+
+
+def construct_substitutions(message: fm_api.Message):
+    subs = dict_to_subs({"msg": message.body})
+    subs["topic"] = message.topic
+    return subs
 
 
-def construct_substitutions(msg):
-    """ Convert a fedmsg message into a dict of substitutions. """
+def dict_to_subs(msg: dict):
+    """Convert a fedmsg message into a dict of substitutions."""
     subs = {}
     for key1 in msg:
         if isinstance(msg[key1], dict):
-            subs.update(dict([
-                ('.'.join([key1, key2]), val2)
-                for key2, val2 in construct_substitutions(msg[key1]).items()
-            ]))
+            subs.update(
+                dict(
+                    [
+                        (".".join([key1, key2]), val2)
+                        for key2, val2 in list(dict_to_subs(msg[key1]).items())
+                    ]
+                )
+            )
             subs[key1] = msg[key1]
-        elif isinstance(msg[key1], basestring):
+        elif isinstance(msg[key1], str):
             subs[key1] = msg[key1].lower()
         else:
             subs[key1] = msg[key1]
     return subs
 
 
 def format_args(obj, subs):
-    """ Recursively apply a substitutions dict to a given criteria subtree """
+    """Recursively apply a substitutions dict to a given criteria subtree"""
 
     if isinstance(obj, dict):
         for key in obj:
             obj[key] = format_args(obj[key], subs)
-    elif isinstance(obj, list):
+    elif isinstance(obj, list) or isinstance(obj, tuple):
         return [format_args(item, subs) for item in obj]
-    elif isinstance(obj, basestring) and obj[2:-2] in subs:
+    elif isinstance(obj, str) and obj[2:-2] in subs:
         obj = subs[obj[2:-2]]
     elif isinstance(obj, (int, float)):
         pass
     else:
         obj = obj % subs
 
     return obj
 
 
-def single_argument_lambda_factory(expression, argument, name='value'):
-    """ Compile and execute a lambda expression with a single argument """
+def single_argument_lambda_factory(expression, argument, name="value"):
+    """Compile and execute a lambda expression with a single argument"""
 
-    code = compile("lambda %s: %s" % (name, expression), __file__, "eval")
-    func = types.LambdaType(code, globals())()
+    code = compile(f"lambda {name}: {expression}", __file__, "eval")
+    lambda_globals = {
+        "__builtins__": __builtins__,
+        "json": json,
+        "re": re,
+    }
+    func = types.LambdaType(code, lambda_globals)()
     return func(argument)
 
 
-def recursive_lambda_factory(obj, arg, name='value'):
-    """ Given a dict, find any lambdas, compile, and execute them. """
+def recursive_lambda_factory(obj, arg, name="value"):
+    """Given a dict, find any lambdas, compile, and execute them."""
 
     if isinstance(obj, dict):
         for key in obj:
-            if key == 'lambda':
+            if key == "lambda":
                 # If so, *replace* the parent dict with the result of the expr
                 obj = single_argument_lambda_factory(obj[key], arg, name)
                 break
             else:
                 obj[key] = recursive_lambda_factory(obj[key], arg, name)
     elif isinstance(obj, list):
         return [recursive_lambda_factory(e, arg, name) for e in obj]
     else:
         pass
 
     return obj
 
 
 def graceful(default_return_value):
-    """ A decorator that gracefully handles exceptions. """
+    """A decorator that gracefully handles exceptions."""
 
     def decorate(method):
         def inner(self, *args, **kwargs):
             try:
                 return method(self, *args, **kwargs)
-            except Exception as e:
-                log.exception(e)
-                log.error("From method: %r self: %r args: %r kwargs: %r" % (
-                    method, self, args, kwargs))
+            except Exception:
+                log.exception(
+                    "From method: %r self: %r args: %r kwargs: %r", method, self, args, kwargs
+                )
                 return default_return_value
+
         return inner
+
     return decorate
 
 
-def notification_callback(topic, msg):
-    """ This is a callback called by tahrir_api whenever something
+def _backoff_hdlr(details):
+    log.warning(f"Publishing message failed. Retrying. {traceback.format_tb(sys.exc_info()[2])}")
+
+
+@backoff.on_exception(
+    backoff.expo,
+    (fm_exceptions.ConnectionException, fm_exceptions.PublishException),
+    max_tries=3,
+    on_backoff=_backoff_hdlr,
+)
+def _publish(message):
+    fm_api.publish(message)
+
+
+def notification_callback(message):
+    """This is a callback called by tahrir_api whenever something
     it deems important has happened.
 
     It is just used to publish fedmsg messages.
     """
-    fedmsg.publish(
-        topic=topic,
-        msg=msg,
-    )
+    try:
+        _publish(message)
+    except fm_exceptions.BaseException:
+        log.error(f"Publishing message failed. Giving up. {traceback.format_tb(sys.exc_info()[2])}")
+
 
+def user_exists_in_fas(fasjson, user):
+    """Return true if the user exists in FAS."""
+    return fasjson.get_user(username=user) is not None
 
-def user_exists_in_fas(config, user):
-    """ Return true if the user exists in FAS. """
-    default_url = 'https://admin.fedoraproject.org/accounts/'
-    fas2 = fedora.client.AccountSystem(
-        base_url=config['fas_credentials'].get('base_url', default_url),
-        username=config['fas_credentials']['username'],
-        password=config['fas_credentials']['password'],
-    )
-    return bool(fas2.person_by_username(user))
 
 def get_pagure_authors(authors):
-    """ Extract the name of pagure authors from
+    """Extract the name of pagure authors from
     a dictionary
 
     Args:
     authors (list): A list of dict that contains fullname and name key.
     """
     authors_name = []
     for item in authors:
         if isinstance(item, dict):
             try:
-                authors_name.append(item["name"])
-            except KeyError:
-                raise Exception("Multiple recipients : name not found in the message")
+                if item["name"] is not None:
+                    authors_name.append(item["name"])
+            except KeyError as e:
+                raise ValueError("Multiple recipients: name not found in the message") from e
     return authors_name
+
+
+def nick2fas(nick, fasjson):
+    """Return the user in FAS."""
+    return fasjson.get_user(username=nick)
+
+
+def email2fas(email, fasjson):
+    """Return the user with the specified email in FAS."""
+    if email.endswith("@fedoraproject.org"):
+        return nick2fas(email.rsplit("@", 1)[0], fasjson)
+
+    result = fasjson.search_users(email=email)
+    if not result:
+        return None
+    return result[0]
```

