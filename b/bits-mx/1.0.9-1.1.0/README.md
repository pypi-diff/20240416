# Comparing `tmp/bits-mx-1.0.9.tar.gz` & `tmp/bits_mx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bits-mx-1.0.9.tar", last modified: Thu Aug  3 18:08:22 2023, max compression
+gzip compressed data, was "bits_mx-1.1.0.tar", max compression
```

## Comparing `bits-mx-1.0.9.tar` & `bits_mx-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:08:22.656836 bits-mx-1.0.9/
--rw-r--r--   0 root         (0) root         (0)      166 2023-08-03 18:08:22.658361 bits-mx-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-28 19:15:07.000000 bits-mx-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:08:22.483310 bits-mx-1.0.9/bits/
--rw-r--r--   0 root         (0) root         (0)       89 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:08:22.577608 bits-mx-1.0.9/bits/mx/
--rw-r--r--   0 root         (0) root         (0)      712 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/mx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/mx/gnarwl.py
--rw-r--r--   0 root         (0) root         (0)     3046 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/mx/google.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/mx/groups.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-03-28 19:15:07.000000 bits-mx-1.0.9/bits/mx/localmail.py
--rw-r--r--   0 root         (0) root         (0)     2602 2023-05-08 19:04:51.000000 bits-mx-1.0.9/bits/mx/nicknames.py
--rw-r--r--   0 root         (0) root         (0)     3940 2023-05-08 15:26:23.000000 bits-mx-1.0.9/bits/mx/rt.py
--rw-r--r--   0 root         (0) root         (0)     8959 2023-05-08 19:07:02.000000 bits-mx-1.0.9/bits/mx/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 18:08:22.649244 bits-mx-1.0.9/bits_mx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      166 2023-08-03 18:08:22.000000 bits-mx-1.0.9/bits_mx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      377 2023-08-03 18:08:22.000000 bits-mx-1.0.9/bits_mx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 18:08:22.000000 bits-mx-1.0.9/bits_mx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 17:20:55.000000 bits-mx-1.0.9/bits_mx.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-03 18:08:22.000000 bits-mx-1.0.9/bits_mx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-03 18:08:22.000000 bits-mx-1.0.9/bits_mx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-08-03 18:08:22.664063 bits-mx-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-08 19:10:28.000000 bits-mx-1.0.9/setup.py
+-rw-r--r--   0        0        0       26 2024-04-16 19:06:36.332754 bits_mx-1.1.0/README.md
+-rw-r--r--   0        0        0       89 2024-04-16 19:06:36.332754 bits_mx-1.1.0/bits/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-16 19:06:36.332754 bits_mx-1.1.0/bits/mx/__init__.py
+-rw-r--r--   0        0        0     2506 2024-04-16 19:06:36.332754 bits_mx-1.1.0/bits/mx/gnarwl.py
+-rw-r--r--   0        0        0     3218 2024-04-16 19:06:36.332754 bits_mx-1.1.0/bits/mx/google.py
+-rw-r--r--   0        0        0     2524 2024-04-16 19:06:36.332754 bits_mx-1.1.0/bits/mx/groups.py
+-rw-r--r--   0        0        0     1954 2024-04-16 19:06:36.332754 bits_mx-1.1.0/bits/mx/localmail.py
+-rw-r--r--   0        0        0     2602 2024-04-16 19:06:36.332754 bits_mx-1.1.0/bits/mx/nicknames.py
+-rw-r--r--   0        0        0     8128 2024-04-16 19:06:36.332754 bits_mx-1.1.0/bits/mx/update.py
+-rw-r--r--   0        0        0      763 2024-04-16 19:06:36.332754 bits_mx-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 bits_mx-1.1.0/PKG-INFO
```

### Comparing `bits-mx-1.0.9/bits/mx/__init__.py` & `bits_mx-1.1.0/bits/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `bits-mx-1.0.9/bits/mx/gnarwl.py` & `bits_mx-1.1.0/bits/mx/gnarwl.py`

 * *Files identical despite different names*

### Comparing `bits-mx-1.0.9/bits/mx/google.py` & `bits_mx-1.1.0/bits/mx/google.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,17 @@
     def get_people_transports(self):
         """Return People transports."""
         transports = []
         for username in sorted(self.update.people):
             # skip terminated people
             if self.update.people[username]['terminated']:
                 continue
+            # skip future hires
+            if "future_hire" in self.update.people[username] and self.update.people[username]['future_hire'] == 1:
+                continue
             # add broadinstitute.org transport
             transports.append('%s@broadinstitute.org\tsmtp:[%s]' % (
                 username,
                 self.transportdest,
             ))
             # add broadintitute.com transport
             transports.append('%s@broadinstitute.com\tsmtp:[%s]' % (
```

### Comparing `bits-mx-1.0.9/bits/mx/groups.py` & `bits_mx-1.1.0/bits/mx/groups.py`

 * *Files identical despite different names*

### Comparing `bits-mx-1.0.9/bits/mx/localmail.py` & `bits_mx-1.1.0/bits/mx/localmail.py`

 * *Files identical despite different names*

### Comparing `bits-mx-1.0.9/bits/mx/nicknames.py` & `bits_mx-1.1.0/bits/mx/nicknames.py`

 * *Files identical despite different names*

### Comparing `bits-mx-1.0.9/bits/mx/update.py` & `bits_mx-1.1.0/bits/mx/update.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """MX Update class file."""
 
 from bits.mx.gnarwl import Gnarwl
 from bits.mx.google import Google
 from bits.mx.groups import Groups
 from bits.mx.localmail import Localmail
 from bits.mx.nicknames import Nicknames
-from bits.mx.rt import RT
 
 
 class Update(object):
     """Update class."""
 
     def __init__(self, mx):
         """Initialize a class instance."""
@@ -33,47 +32,36 @@
         """Update everything."""
         self.gnarwl_aliases()
         self.gnarwl_ldap()
         self.google_transport()
         self.groups_transport()
         self.localmail_aliases()
         self.nickname_aliases()
-        self.rt_aliases()
 
     def get_gnarwl(self):
         """Get Gnarwl data from MongoDB."""
         if self.gnarwl:
             return self.gnarwl
         if self.verbose:
             print('Getting gnarwl from MongoDB...')
-        m = self.auth.mongo()
-        self.gnarwl = m.get_collection_dict('gnarwl')
+        mongoh = self.auth.mongo_bitsdb()
+        self.gnarwl = mongoh.get_collection_dict('gnarwl')
         return self.gnarwl
 
     def get_groups(self):
         """Get Groups data from Google."""
         if self.groups:
             return self.groups
         if self.verbose:
             print('Getting groups from Google...')
         g = self.auth.google()
         g.auth_service_account(g.scopes, g.subject)
         self.groups = g.directory().get_groups_dict()
         return self.groups
 
-    def get_help_queues(self):
-        """Get RT queues from help."""
-        if self.help_queues:
-            return self.help_queues
-        if self.verbose:
-            print('Getting help queues from RT...')
-        h = self.auth.help()
-        self.help_queues = h.getQueues()
-        return self.help_queues
-
     def get_localmail(self):
         """Get Localmail from LDAP."""
         lm = self.auth.localmail()
         if self.localmail:
             return self.localmail
         if self.verbose:
             print('Getting localmail from MongoDB...')
@@ -86,46 +74,46 @@
 
     def get_nicknames(self):
         """Get Nicknames data from MongoDB."""
         if self.nicknames:
             return self.nicknames
         if self.verbose:
             print('Getting nicknames from MongoDB...')
-        m = self.auth.mongo()
-        self.nicknames = m.get_collection_dict('nicknames')
+        mongoh = self.auth.mongo_bitsdb()
+        self.nicknames = mongoh.get_collection_dict('nicknames')
         return self.nicknames
 
     def get_all_other_accounts(self):
         """Get All Other Accounts from MongoDB."""
         if self.all_other_accounts:
             return self.all_other_accounts
         if self.verbose:
             print('Getting other_accounts from MongoDB...')
-        m = self.auth.mongo()
-        self.all_other_accounts = m.get_collection_dict('other_accounts')
+        mongoh = self.auth.mongo_bitsdb()
+        self.all_other_accounts = mongoh.get_collection_dict('other_accounts')
         return self.all_other_accounts
 
     def get_google_other_accounts(self):
         """Get Other Accounts from MongoDB."""
         if self.google_other_accounts:
             return self.google_other_accounts
         if self.verbose:
             print('Getting other_accounts from MongoDB...')
-        m = self.auth.mongo()
-        self.google_other_accounts = m.get_collection_dict('other_accounts', key='google_username')
+        mongoh = self.auth.mongo_bitsdb()
+        self.google_other_accounts = mongoh.get_collection_dict('other_accounts', key='google_username')
         return self.google_other_accounts
 
     def get_people(self):
-        """Get People from PeopleDB."""
+        """Get People from MongoDB."""
         if self.people:
             return self.people
         if self.verbose:
-            print('Getting people from PeopleDB...')
-        p = self.auth.people()
-        self.people = p.getPeople('username')
+            print('Getting people from MongoDB...')
+        mongoh = self.auth.mongo_bitsdb()
+        self.people = mongoh.get_collection_dict('people', key='username')
         return self.people
 
     def gnarwl_aliases(self):
         """Update Gnarwl aliases."""
         g = Gnarwl(self)
         if self.verbose:
             print('Updating gnarwl aliases...')
@@ -237,31 +225,14 @@
             ))
         output = n.generate()
         # write file
         self.write_file(n.puppetfile, output)
         if self.verbose:
             print('Wrote nickname aliases to: %s\n' % (n.puppetfile))
 
-    def rt_aliases(self):
-        """Update RT aliases."""
-        rt = RT(self)
-        if self.verbose:
-            print('Updating rt aliases...')
-        help_queues = self.get_help_queues()
-        # check help_queues data
-        if len(help_queues) < 10:
-            print('ERROR: Not enough help entries (%s), exiting.' % (
-                len(help_queues)
-            ))
-        output = rt.generate()
-        # write file
-        self.write_file(rt.puppetfile, output)
-        if self.verbose:
-            print('Wrote rt aliases to: %s\n' % (rt.puppetfile))
-
     def write_file(self, filename, output):
         """Write out a single file to disk."""
         # open puppetfile
         outputfile = open(filename, 'w')
         # write output
         outputfile.write('%s\n' % (output))
         # close puppetfile
```

