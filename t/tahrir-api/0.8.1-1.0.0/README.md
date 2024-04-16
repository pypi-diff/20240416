# Comparing `tmp/tahrir-api-0.8.1.tar.gz` & `tmp/tahrir_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tahrir-api-0.8.1.tar", last modified: Tue Nov  1 09:34:58 2016, max compression
+gzip compressed data, was "tahrir_api-1.0.0.tar", max compression
```

## Comparing `tahrir-api-0.8.1.tar` & `tahrir_api-1.0.0.tar`

### file list

```diff
@@ -1,70 +1,35 @@
-drwxr-xr-x   0 sachowdh  (1000) sachowdh  (1000)        0 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     2740 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/PKG-INFO
-drwxr-xr-x   0 sachowdh  (1000) sachowdh  (1000)        0 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/tests/
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     6321 2016-09-20 09:16:14.000000 tahrir-api-0.8.1/tests/test_dbai.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     6158 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/tests/test_ranking.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)        0 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/tests/__init__.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1596 2016-11-01 09:34:54.000000 tahrir-api-0.8.1/setup.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      107 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/MANIFEST.in
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)       59 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/setup.cfg
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1777 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/README.rst
-drwxr-xr-x   0 sachowdh  (1000) sachowdh  (1000)        0 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/tahrir_api.egg-info/
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)        1 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/tahrir_api.egg-info/dependency_links.txt
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     2740 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/tahrir_api.egg-info/PKG-INFO
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)        1 2016-07-15 11:37:37.000000 tahrir-api-0.8.1/tahrir_api.egg-info/not-zip-safe
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      173 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/tahrir_api.egg-info/entry_points.txt
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)       80 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/tahrir_api.egg-info/requires.txt
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)       11 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/tahrir_api.egg-info/top_level.txt
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     2406 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/tahrir_api.egg-info/SOURCES.txt
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)       47 2016-09-20 09:15:56.000000 tahrir-api-0.8.1/tahrir_api.egg-info/pbr.json
-drwxr-xr-x   0 sachowdh  (1000) sachowdh  (1000)        0 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/tahrir_api/
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)    10336 2016-09-20 09:16:14.000000 tahrir-api-0.8.1/tahrir_api/model.py
-drwxr-xr-x   0 sachowdh  (1000) sachowdh  (1000)        0 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/tahrir_api/scripts/
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)        0 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/tahrir_api/scripts/__init__.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     2557 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/tahrir_api/scripts/initializedb.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     3695 2016-09-20 09:16:14.000000 tahrir-api-0.8.1/tahrir_api/scripts/populateseries.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)        0 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/tahrir_api/__init__.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      839 2016-09-20 09:16:14.000000 tahrir-api-0.8.1/tahrir_api/utils.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)    31422 2016-09-20 09:16:14.000000 tahrir-api-0.8.1/tahrir_api/dbapi.py
-drwxr-xr-x   0 sachowdh  (1000) sachowdh  (1000)        0 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/alembic/
-drwxr-xr-x   0 sachowdh  (1000) sachowdh  (1000)        0 2016-11-01 09:34:58.000000 tahrir-api-0.8.1/alembic/versions/
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1860 2016-09-02 13:22:32.000000 tahrir-api-0.8.1/alembic/versions/a635705c8f3_create_new_tables_for_quest.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1061 2016-06-27 13:29:59.000000 tahrir-api-0.8.1/alembic/versions/4099fa344171_add_last_login.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      706 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/versions/39583332f4ea_add_profile_fields_t.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1083 2016-06-27 13:29:59.000000 tahrir-api-0.8.1/alembic/versions/16943d9088cf_fix_foreign_key_mism.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1184 2016-06-27 13:29:59.000000 tahrir-api-0.8.1/alembic/versions/39583332f4ea_add_profile_fields_t.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      499 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/versions/5791a2b9fb6a_add_tags_field_to_ba.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1083 2016-06-27 13:29:59.000000 tahrir-api-0.8.1/alembic/versions/420c02357a1b_add_created_on_field.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      627 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/versions/24282792d72a_add_created_by_field.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1038 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/versions/3c7fd5b4e2c2_add_two_new_columns_.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      829 2016-09-02 15:18:25.000000 tahrir-api-0.8.1/alembic/versions/27bf068f5635_.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1061 2016-06-27 13:29:59.000000 tahrir-api-0.8.1/alembic/versions/508367dcbbb5_add_an_stl_column_fo.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1305 2016-09-02 15:15:07.000000 tahrir-api-0.8.1/alembic/versions/ce541796a7_add_authz_table.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1584 2016-06-27 13:29:59.000000 tahrir-api-0.8.1/alembic/versions/3c7fd5b4e2c2_add_two_new_columns_.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1860 2016-09-02 14:29:18.000000 tahrir-api-0.8.1/alembic/versions/3ec523a2bbf_create_new_tables_for_quest.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      431 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/versions/139ec7ed17b7_add_a_rank_column_to.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      509 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/versions/508367dcbbb5_add_an_stl_column_fo.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1159 2016-06-27 13:29:59.000000 tahrir-api-0.8.1/alembic/versions/24282792d72a_add_created_by_field.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     2066 2016-09-02 15:21:14.000000 tahrir-api-0.8.1/alembic/versions/e7040e76728_create_new_tables_for_quest.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1865 2016-09-02 14:29:34.000000 tahrir-api-0.8.1/alembic/versions/322364e7de8b_create_new_tables_for_quest.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      737 2016-09-02 15:14:36.000000 tahrir-api-0.8.1/alembic/versions/ce541796a7_add_authz_table.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1019 2016-06-27 13:29:59.000000 tahrir-api-0.8.1/alembic/versions/2879ed5a6297_issued_for.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      523 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/versions/420c02357a1b_add_created_on_field.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      634 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/versions/4099fa344171_add_last_login.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1976 2016-09-02 15:18:50.000000 tahrir-api-0.8.1/alembic/versions/22cfda208915_.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1044 2016-06-27 13:29:59.000000 tahrir-api-0.8.1/alembic/versions/5791a2b9fb6a_add_tags_field_to_ba.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      489 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/versions/2879ed5a6297_issued_for.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      542 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/versions/fa1d309e8c3_add_created_on_field.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     2360 2016-09-20 09:16:14.000000 tahrir-api-0.8.1/alembic/versions/e7040e76728_create_new_tables_for_quest.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1865 2016-09-02 15:07:27.000000 tahrir-api-0.8.1/alembic/versions/13f1d1938e53_create_new_tables_for_quest.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1088 2016-06-27 13:29:59.000000 tahrir-api-0.8.1/alembic/versions/139ec7ed17b7_add_a_rank_column_to.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1096 2016-06-27 13:29:59.000000 tahrir-api-0.8.1/alembic/versions/fa1d309e8c3_add_created_on_field.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     1865 2016-09-02 13:22:20.000000 tahrir-api-0.8.1/alembic/versions/49165401144f_create_new_tables_for_quest.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      444 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/versions/16943d9088cf_fix_foreign_key_mism.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      412 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/script.py.mako
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      154 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/README
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     2277 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/alembic/env.py
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)     2140 2016-06-27 13:29:51.000000 tahrir-api-0.8.1/alembic/env.pyc
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)    35147 2016-04-21 21:38:50.000000 tahrir-api-0.8.1/LICENSE
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)      955 2016-09-02 15:07:24.000000 tahrir-api-0.8.1/alembic.ini
--rw-r--r--   0 sachowdh  (1000) sachowdh  (1000)    26786 2016-11-01 09:34:54.000000 tahrir-api-0.8.1/CHANGELOG.rst
+-rw-r--r--   0        0        0    35147 2024-03-06 10:08:38.072854 tahrir_api-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2510 2024-03-06 10:08:38.072854 tahrir_api-1.0.0/README.rst
+-rw-r--r--   0        0        0      273 2024-04-12 13:36:07.983534 tahrir_api-1.0.0/examples/awardbadge.py
+-rw-r--r--   0        0        0      519 2024-04-12 13:36:07.983534 tahrir_api-1.0.0/examples/fossboxbadge.py
+-rw-r--r--   0        0        0     2028 2024-04-16 15:15:50.859264 tahrir_api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-06 10:08:38.073854 tahrir_api-1.0.0/tahrir_api/__init__.py
+-rw-r--r--   0        0        0    30886 2024-04-16 12:57:13.118516 tahrir_api-1.0.0/tahrir_api/dbapi.py
+-rw-r--r--   0        0        0      154 2024-03-06 10:08:38.072854 tahrir_api-1.0.0/tahrir_api/migrations/README
+-rw-r--r--   0        0        0      946 2024-03-06 10:08:38.072854 tahrir_api-1.0.0/tahrir_api/migrations/alembic.ini
+-rw-r--r--   0        0        0     2121 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/env.py
+-rw-r--r--   0        0        0      532 2024-04-16 14:33:44.206257 tahrir_api-1.0.0/tahrir_api/migrations/script.py.mako
+-rw-r--r--   0        0        0      432 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/139ec7ed17b7_add_a_rank_column_to.py
+-rw-r--r--   0        0        0      445 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/16943d9088cf_fix_foreign_key_mism.py
+-rw-r--r--   0        0        0      609 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py
+-rw-r--r--   0        0        0      490 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/2879ed5a6297_issued_for.py
+-rw-r--r--   0        0        0      707 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py
+-rw-r--r--   0        0        0     1037 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py
+-rw-r--r--   0        0        0      618 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/4099fa344171_add_last_login.py
+-rw-r--r--   0        0        0      507 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/420c02357a1b_add_created_on_field.py
+-rw-r--r--   0        0        0      510 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/508367dcbbb5_add_an_stl_column_fo.py
+-rw-r--r--   0        0        0      500 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/5791a2b9fb6a_add_tags_field_to_ba.py
+-rw-r--r--   0        0        0      735 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py
+-rw-r--r--   0        0        0     2429 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py
+-rw-r--r--   0        0        0      526 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py
+-rw-r--r--   0        0        0     9931 2024-04-16 12:54:03.656878 tahrir_api-1.0.0/tahrir_api/model.py
+-rw-r--r--   0        0        0        0 2024-03-06 10:08:38.073854 tahrir_api-1.0.0/tahrir_api/scripts/__init__.py
+-rw-r--r--   0        0        0     2705 2024-04-15 17:04:27.316278 tahrir_api-1.0.0/tahrir_api/scripts/populateseries.py
+-rw-r--r--   0        0        0      383 2024-04-16 05:45:07.833267 tahrir_api-1.0.0/tahrir_api/scripts/syncdb.py
+-rw-r--r--   0        0        0     1445 2024-04-16 06:02:37.465169 tahrir_api-1.0.0/tahrir_api/scripts/utils.py
+-rw-r--r--   0        0        0      838 2024-04-15 16:33:53.573885 tahrir_api-1.0.0/tahrir_api/utils.py
+-rw-r--r--   0        0        0        0 2024-03-06 10:08:38.073854 tahrir_api-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      408 2024-04-16 06:24:32.846311 tahrir_api-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     5578 2024-04-16 06:42:32.863046 tahrir_api-1.0.0/tests/test_dbapi.py
+-rw-r--r--   0        0        0     4909 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tests/test_ranking.py
+-rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 tahrir_api-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tahrir-api-0.8.1/tahrir_api/model.py` & `tahrir_api-1.0.0/tahrir_api/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,315 +1,289 @@
-import pygments
-import simplejson
-import hashlib
-import uuid
 import datetime
+import hashlib
 import time
+import uuid
 
 import arrow
-
-from sqlalchemy import (
-    Column,
-    DateTime,
-    Unicode,
-    ForeignKey,
-    UniqueConstraint,
-)
-from sqlalchemy.types import (
-    Integer,
-    Boolean,
-)
-
-from sqlalchemy.ext.declarative import declarative_base
-
-from sqlalchemy.orm import (
-    scoped_session,
-    sessionmaker,
-    relationship,
-)
-
-
-from zope.sqlalchemy import ZopeTransactionExtension
-
-DBSession = scoped_session(sessionmaker(extension=ZopeTransactionExtension()))
-DeclarativeBase = declarative_base()
-DeclarativeBase.query = DBSession.query_property()
+import pygments
+import simplejson
+from sqlalchemy import Column, DateTime, ForeignKey, Unicode, UniqueConstraint
+from sqlalchemy.orm import object_session, relationship, sessionmaker
+from sqlalchemy.types import Boolean, Integer
+from sqlalchemy_helpers import Base as DeclarativeBase
 
 
 class Issuer(DeclarativeBase):
-    __tablename__ = 'issuers'
+    __tablename__ = "issuers"
     id = Column(Integer, unique=True, primary_key=True)
     origin = Column(Unicode(128), nullable=False)
     name = Column(Unicode(128), nullable=False, unique=True)
     org = Column(Unicode(128), nullable=False)
     contact = Column(Unicode(128), nullable=False)
     badges = relationship("Badge", backref="issuer")
-    created_on = Column(DateTime, nullable=False,
-                        default=datetime.datetime.utcnow)
+    created_on = Column(DateTime, nullable=False, default=datetime.datetime.now)
 
-    def __unicode__(self):
-        return self.name
+    def __str__(self):
+        return str(self.name)
 
-    def __json__(self):
+    def as_dict(self):
         return dict(
             origin=self.origin,
             name=self.name,
             org=self.org,
             contact=self.contact,
             created_on=time.mktime(self.created_on.timetuple()),
         )
 
 
 def generate_default_id(context):
-    return context.current_parameters['name'].lower().replace(' ', '-')
+    return context.current_parameters["name"].lower().replace(" ", "-")
 
 
 class Badge(DeclarativeBase):
-    __tablename__ = 'badges'
+    __tablename__ = "badges"
     id = Column(Unicode(128), primary_key=True, default=generate_default_id)
     name = Column(Unicode(128), nullable=False, unique=True)
     image = Column(Unicode(128), nullable=False)
     stl = Column(Unicode(128))
     description = Column(Unicode(128), nullable=False)
     criteria = Column(Unicode(128), nullable=False)
-    issuer_id = Column(Integer, ForeignKey('issuers.id'), nullable=False)
+    issuer_id = Column(Integer, ForeignKey("issuers.id"), nullable=False)
     milestone = relationship("Milestone", backref="badge")
     authorizations = relationship("Authorization", backref="badge")
     assertions = relationship("Assertion", backref="badge")
     invitations = relationship("Invitation", backref="badge")
-    created_on = Column(DateTime, nullable=False,
-                        default=datetime.datetime.utcnow)
+    created_on = Column(DateTime, nullable=False, default=datetime.datetime.now)
     tags = Column(Unicode(128))
 
-    def __unicode__(self):
-        return self.name
+    def __str__(self):
+        return str(self.name)
 
-    def __json__(self):
+    def as_dict(self):
         if self.image.startswith("http"):
             image = self.image
         else:
             image = "/pngs/" + self.image
         return dict(
             version="0.5.0",
             name=self.name,
             image=image,
             description=self.description,
             criteria=self.criteria,
-            issuer=self.issuer.__json__(),
+            issuer=self.issuer.as_dict(),
             created_on=time.mktime(self.created_on.timetuple()),
             tags=self.tags,
         )
 
     def authorized(self, person):
-        """ Return true if a given person is authorized to admin a badge """
+        """Return true if a given person is authorized to admin a badge"""
         for authz in self.authorizations:
             if authz.person == person:
                 return True
 
         return False
 
 
 class Team(DeclarativeBase):
     __tablename__ = "team"
     id = Column(Unicode(128), primary_key=True, default=generate_default_id)
     name = Column(Unicode(128), nullable=False, unique=True)
     series = relationship("Series", backref="team")
-    created_on = Column(DateTime, nullable=False,
-                        default=datetime.datetime.utcnow)
+    created_on = Column(DateTime, nullable=False, default=datetime.datetime.now)
 
-    def __json__(self):
-        return dict(
-            id=self.id,
-            name=self.name,
-            created_on=str(self.created_on),
-        )
+    def as_dict(self):
+        return dict(id=self.id, name=self.name, created_on=str(self.created_on))
 
 
 class Series(DeclarativeBase):
-    __tablename__ = 'series'
+    __tablename__ = "series"
     id = Column(Unicode(128), primary_key=True, default=generate_default_id)
     name = Column(Unicode(128), nullable=False, unique=True)
     description = Column(Unicode(128), nullable=False)
-    created_on = Column(DateTime, nullable=False,
-                        default=datetime.datetime.utcnow)
-    last_updated = Column(DateTime, nullable=False,
-                          default=datetime.datetime.utcnow,
-                          onupdate=datetime.datetime.utcnow)
+    created_on = Column(DateTime, nullable=False, default=datetime.datetime.now)
+    last_updated = Column(
+        DateTime,
+        nullable=False,
+        default=datetime.datetime.now,
+        onupdate=datetime.datetime.now,
+    )
     tags = Column(Unicode(128))
     milestone = relationship("Milestone", backref="series")
-    team_id = Column(Unicode(128), ForeignKey('team.id'), nullable=False)
+    team_id = Column(Unicode(128), ForeignKey("team.id"), nullable=False)
 
-    def __json__(self):
+    def as_dict(self):
         return dict(
             id=self.id,
             name=self.name,
             created_on=str(self.created_on),
             last_updated=str(self.last_updated),
-            team=self.team.__json__(),
+            team=self.team.as_dict(),
         )
 
 
 class Milestone(DeclarativeBase):
-    __tablename__ = 'milestone'
-    __table_args__ = (
-        UniqueConstraint('position', 'badge_id', 'series_id'),
-    )
+    __tablename__ = "milestone"
+    __table_args__ = (UniqueConstraint("position", "badge_id", "series_id"),)
     id = Column(Integer, unique=True, primary_key=True)
     position = Column(Integer, default=None)
-    badge_id = Column(Unicode(128), ForeignKey('badges.id'), nullable=False)
-    series_id = Column(Unicode(128), ForeignKey('series.id'), nullable=False)
+    badge_id = Column(Unicode(128), ForeignKey("badges.id"), nullable=False)
+    series_id = Column(Unicode(128), ForeignKey("series.id"), nullable=False)
 
-    def __json__(self):
+    def as_dict(self):
         return dict(
             position=self.position,
-            badge=self.badge.__json__(),
+            badge=self.badge.as_dict(),
             series_id=self.series.id,
         )
 
 
 class Person(DeclarativeBase):
-    __tablename__ = 'persons'
+    __tablename__ = "persons"
     id = Column(Integer, unique=True, primary_key=True)
     email = Column(Unicode(128), nullable=False, unique=True)
     authorizations = relationship("Authorization", backref="person")
     assertions = relationship("Assertion", backref="person")
     nickname = Column(Unicode(128), unique=True)
     website = Column(Unicode(128))
     bio = Column(Unicode(140))
-    created_on = Column(DateTime, nullable=False,
-                        default=datetime.datetime.utcnow)
+    created_on = Column(DateTime, nullable=False, default=datetime.datetime.now)
     last_login = Column(DateTime, nullable=True, default=None)
     opt_out = Column(Boolean, nullable=False, default=False)
     # An integer that organizes the users by the number of
     # badges they have ever been awarded.  A value of None
     # indicates that they have not been ranked yet at all.
     rank = Column(Integer, default=None)
 
     def __repr__(self):
-        return "<Person: '%s <%s>'" % (self.nickname, self.email)
+        return f"<Person: '{self.nickname} <{self.email}>'"
 
     @property
     def gravatar_link(self):
-        d, s = 'mm', 24
-        hash = hashlib.md5(self.email).hexdigest()
-        url = "http://www.gravatar.com/avatar/%s?s=%i&d=%s" % (hash, s, d)
+        d, s = "mm", 24
+        hash = self.email_md5
+        url = f"http://www.gravatar.com/avatar/{hash}?s={s}&d={d}"
         return url
 
-    def __unicode__(self):
-        return self.email
+    @property
+    def email_md5(self):
+        return hashlib.md5(self.email.encode("utf-8")).hexdigest()
 
-    def __json__(self):
+    @property
+    def email_sha1(self):
+        return hashlib.sha1(self.email.encode("utf-8")).hexdigest()
+
+    def __str__(self):
+        return str(self.email)
+
+    def as_dict(self):
         return dict(
             email=self.email,
             id=self.id,
             nickname=self.nickname,
             website=self.website,
             bio=self.bio,
             rank=self.rank,
         )
 
 
 def invitation_id_default(context):
-    return unicode(hashlib.md5(salt_default(context)).hexdigest())
+    return hashlib.md5(salt_default(context).encode("utf-8")).hexdigest()
 
 
 class Invitation(DeclarativeBase):
-    """ This is a temporary invitation to receive a badge.
+    """This is a temporary invitation to receive a badge.
 
     The idea is that a user can create a "You made my day" badge, and
     then award it to another user.  However, instead of just directly
     associating the righthand user with the badge, we "invite" them
     to accept it.
 
     """
-    __tablename__ = 'invitations'
-    id = Column(
-        Unicode(32), primary_key=True, unique=True,
-        default=invitation_id_default,
-    )
+
+    __tablename__ = "invitations"
+    id = Column(Unicode(32), primary_key=True, unique=True, default=invitation_id_default)
     created_on = Column(DateTime, nullable=False)
     expires_on = Column(DateTime, nullable=False)
-    badge_id = Column(Unicode(128), ForeignKey('badges.id'), nullable=False)
-    created_by = Column(Integer, ForeignKey('persons.id'),
-                        nullable=False)
+    badge_id = Column(Unicode(128), ForeignKey("badges.id"), nullable=False)
+    created_by = Column(Integer, ForeignKey("persons.id"), nullable=False)
 
     @property
     def expired(self):
-        return datetime.datetime.utcnow() > self.expires_on
+        return datetime.datetime.now() > self.expires_on
 
     @property
     def expires_on_relative(self):
         return arrow.get(self.expires_on).humanize()
 
 
 class Authorization(DeclarativeBase):
-    __tablename__ = 'authorizations'
+    __tablename__ = "authorizations"
     id = Column(Integer, primary_key=True)
-    badge_id = Column(Unicode(128), ForeignKey('badges.id'), nullable=False)
-    person_id = Column(Integer, ForeignKey('persons.id'), nullable=False)
+    badge_id = Column(Unicode(128), ForeignKey("badges.id"), nullable=False)
+    person_id = Column(Integer, ForeignKey("persons.id"), nullable=False)
 
 
 def recipient_default(context):
     Session = sessionmaker(context.engine)()
-    person_id = context.current_parameters['person_id']
+    person_id = context.current_parameters["person_id"]
     person = Session.query(Person).filter_by(id=person_id).one()
-    return unicode(hashlib.sha256(
-        person.email + context.current_parameters['salt']).hexdigest())
+
+    return hashlib.sha256(
+        (person.email + context.current_parameters["salt"]).encode("utf-8")
+    ).hexdigest()
 
 
 def salt_default(context):
-    return unicode(uuid.uuid4())
+    return str(uuid.uuid4())
 
 
 def assertion_id_default(context):
-    person_id = context.current_parameters['person_id']
-    badge_id = context.current_parameters['badge_id']
-    return "%s -> %r" % (badge_id, person_id)
+    person_id = context.current_parameters["person_id"]
+    badge_id = context.current_parameters["badge_id"]
+    return f"{badge_id} -> {person_id}"
 
 
 class Assertion(DeclarativeBase):
-    __tablename__ = 'assertions'
-    id = Column(Unicode(128), primary_key=True, unique=True,
-                default=assertion_id_default)
-    badge_id = Column(Unicode(128), ForeignKey('badges.id'), nullable=False)
-    person_id = Column(Integer, ForeignKey('persons.id'), nullable=False)
+    __tablename__ = "assertions"
+    id = Column(Unicode(128), primary_key=True, unique=True, default=assertion_id_default)
+    badge_id = Column(Unicode(128), ForeignKey("badges.id"), nullable=False)
+    person_id = Column(Integer, ForeignKey("persons.id"), nullable=False)
     salt = Column(Unicode(128), nullable=False, default=salt_default)
-    issued_on = Column(DateTime, nullable=False, default=datetime.datetime.utcnow)
+    issued_on = Column(DateTime, nullable=False, default=datetime.datetime.now)
 
     # An optional link back to the event that warranted the award
     issued_for = Column(Unicode(256))
 
     recipient = Column(Unicode(256), nullable=False, default=recipient_default)
 
-    def __unicode__(self):
-        return unicode(self.badge) + "<->" + unicode(self.person)
+    def __str__(self):
+        return str(self.badge) + "<->" + str(self.person)
 
     @property
     def _recipient(self):
-        return "sha256${0}".format(self.recipient)
+        return f"sha256${self.recipient}"
 
-    def __json__(self):
-        result = dict(
-            recipient=self._recipient,
-            salt=self.salt,
-            badge=self.badge.__json__(),)
+    def as_dict(self):
+        result = dict(recipient=self._recipient, salt=self.salt, badge=self.badge.as_dict())
         # Eliminate this check since I made issued_on not nullable?
         if self.issued_on:
-            result['issued_on'] = self.issued_on.strftime("%Y-%m-%d")
+            result["issued_on"] = self.issued_on.strftime("%Y-%m-%d")
         return result
 
     def __getitem__(self, key):
         if key not in ("pygments", "delete"):
             raise KeyError
-        return getattr(self, "__{0}__".format(key))()
+        return getattr(self, f"__{key}__")()
 
     def __delete__(self):
-        return lambda: DBSession.delete(self)
+        session = object_session(self)
+        return lambda: session.delete(self)
 
     def __pygments__(self):
-        html_args = {'full': False}
+        html_args = {"full": False}
         pretty_encoder = simplejson.encoder.JSONEncoder(indent=2)
         html = pygments.highlight(
-            pretty_encoder.encode(self.__json__()),
+            pretty_encoder.encode(self.as_dict()),
             pygments.lexers.JavascriptLexer(),
-            pygments.formatters.HtmlFormatter(**html_args)).strip()
+            pygments.formatters.HtmlFormatter(**html_args),
+        ).strip()
         return html
```

### Comparing `tahrir-api-0.8.1/tahrir_api/scripts/populateseries.py` & `tahrir_api-1.0.0/tahrir_api/scripts/populateseries.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,36 @@
 import os
-import sys
-import transaction
 import re
+import sys
 
-from sqlalchemy import engine_from_config
-from paste.deploy import appconfig
-
-
-from ..model import (
-    DBSession,
-    Badge,
-    Milestone,
-    Series,
-)
+from ..model import Badge, Milestone, Series
+from .utils import get_db_manager_from_paste
 
 
 def usage(argv):
     cmd = os.path.basename(argv[0])
-    print('usage: %s <config_uri>\n'
-          '(example: "%s development.ini")' % (cmd, cmd))
+    print(f"usage: {cmd} <config_uri>\n '(example: \"{cmd} development.ini\"'")
     sys.exit(1)
 
 
-def _getpathsec(config_uri, name):
-    if '#' in config_uri:
-        path, section = config_uri.split('#', 1)
-    else:
-        path, section = config_uri, 'main'
-    if name:
-        section = name
-    return path, section
-
-
-_ROMAN_TO_ARABIC = dict([
-    ('I', 1),
-    ('V', 5),
-    ('X', 10),
-    ('L', 50),
-    ('C', 100),
-    ('D', 500),
-    ('M', 1000),
-])
+_ROMAN_TO_ARABIC = dict(
+    [("I", 1), ("V", 5), ("X", 10), ("L", 50), ("C", 100), ("D", 500), ("M", 1000)]
+)
 _REPLACEMENTS = [
-    ('CM', 'DCCCC'),
-    ('CD', 'CCCC'),
-    ('XC', 'LXXXX'),
-    ('XL', 'XXXX'),
-    ('IX', 'VIIII'),
-    ('IV', 'IIII'),
+    ("CM", "DCCCC"),
+    ("CD", "CCCC"),
+    ("XC", "LXXXX"),
+    ("XL", "XXXX"),
+    ("IX", "VIIII"),
+    ("IV", "IIII"),
 ]
 # A name of a badge in series must end with parenthesised series name and
 # ordinal number, either in arabic or roman numerals. All badges in a given
 # series must share the same series name.
-_SERIES_NAME_RE = re.compile(r'.+ \((?P<name>.+) (?P<ord>[0-9IXVL]+)\)')
+_SERIES_NAME_RE = re.compile(r".+ \((?P<name>.+) (?P<ord>[0-9IXVL]+)\)")
 
 
 def _convert(mapping, x):
     for prefix, replacement in mapping:
         x = x.replace(prefix, replacement)
     return x
 
@@ -74,62 +48,45 @@
     this badge in the series.
 
     If the badge is not in any series, both tuple elements are None.
     """
     m = _SERIES_NAME_RE.match(name)
     if not m:
         return None, None
-    base = m.group('name')
-    idx = m.group('ord')
+    base = m.group("name")
+    idx = m.group("ord")
     try:
         try:
             return base, int(idx)
         except ValueError:
             return base, _to_number(idx)
     except (ValueError, KeyError):
         return None, None
 
 
 def main(argv=sys.argv):
     if len(argv) != 2:
         usage(argv)
 
     config_uri = argv[1]
-    path, section = _getpathsec(config_uri, "pyramid")
-    config_name = 'config:%s' % path
-    here_dir = os.getcwd()
-
-    global_conf = None
-    if 'OPENSHIFT_APP_NAME' in os.environ:
-        if 'OPENSHIFT_MYSQL_DB_URL' in os.environ:
-            template = '{OPENSHIFT_MYSQL_DB_URL}{OPENSHIFT_APP_NAME}'
-        elif 'OPENSHIFT_POSTGRESQL_DB_URL' in os.environ:
-            template = '{OPENSHIFT_POSTGRESQL_DB_URL}{OPENSHIFT_APP_NAME}'
-
-        global_conf = {
-            'sqlalchemy.url': template.format(**os.environ)
-        }
-
-    settings = appconfig(config_name, name=section, relative_to=here_dir,
-                         global_conf=global_conf)
-
-    engine = engine_from_config(settings, 'sqlalchemy.')
-    DBSession.configure(bind=engine)
-
-    with transaction.manager:
-        for badge in DBSession.query(Badge).all():
+    db_mgr = get_db_manager_from_paste(config_uri)
+    with db_mgr.Session() as session:
+        for badge in session.query(Badge).all():
             if badge.milestone:
                 # Skip badges that already are in some series.
                 continue
             series_name, ordering = get_series_name(badge.name)
             if series_name and ordering:
-                series = DBSession.query(Series).filter(Series.name == series_name).first()
+                series = session.query(Series).filter(Series.name == series_name).first()
 
                 if not series:
-                    print('Series <%s> does not exist, skipping '
-                          'processing badge %s' % (series_name, badge.name))
+                    print(
+                        f"Series <{series_name}> does not exist, skipping "
+                        f"processing badge {badge.name}"
+                    )
                     continue
                 milestone = Milestone()
                 milestone.badge_id = badge.id
                 milestone.position = ordering
-                milestone.series_id = series_name.lower().replace(' ', '-')
-                DBSession.add(milestone)
+                milestone.series_id = series_name.lower().replace(" ", "-")
+                session.add(milestone)
+        session.commit()
```

### Comparing `tahrir-api-0.8.1/tahrir_api/utils.py` & `tahrir_api-1.0.0/tahrir_api/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Module to keep random utils. """
 
 
 def autocommit(func):
-    """ A decorator that autocommits after API calls unless
+    """A decorator that autocommits after API calls unless
     configured otherwise.
     """
 
     def _wrapper(self, *args, **kwargs):
         result = func(self, *args, **kwargs)
         if self.autocommit:
             self.session.commit()
@@ -23,13 +23,13 @@
     Convert a badge name into a valid badge ID.
 
     :type name: string
     :param name: The badge name to convert to an ID
     """
 
     badge_id = name.lower().replace(" ", "-")
-    bad = ['"', "'", '(', ')', '*', '&', '?']
-    replacements = dict(zip(bad, [''] * len(bad)))
+    bad = ['"', "'", "(", ")", "*", "&", "?"]
+    replacements = dict(zip(bad, [""] * len(bad)))
     for a, b in replacements.items():
         badge_id = badge_id.replace(a, b)
 
     return badge_id
```

### Comparing `tahrir-api-0.8.1/tahrir_api/dbapi.py` & `tahrir_api-1.0.0/tahrir_api/dbapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,137 +1,154 @@
-# -*- coding: utf-8 -*-
 # Authors: Ross Delinger
 #          Remy D <remyd@civx.us>
 # Description: API For interacting with the Tahrir database
 
-from utils import autocommit, convert_name_to_id
-from model import Badge, Invitation, Issuer, Assertion, Person, Authorization
-from model import Team, Series, Milestone
-from sqlalchemy import create_engine, func, and_, not_
-from sqlalchemy.orm import sessionmaker, scoped_session
-from datetime import (
-    datetime,
-    timedelta,
+import importlib.resources
+from collections import OrderedDict
+from datetime import datetime, timedelta, timezone
+
+from sqlalchemy import and_, func, not_, text
+from sqlalchemy_helpers import DatabaseManager
+from tahrir_messages import BadgeAwardV1, PersonLoginFirstV1, PersonRankAdvanceV1
+
+from .model import (
+    Assertion,
+    Authorization,
+    Badge,
+    Invitation,
+    Issuer,
+    Milestone,
+    Person,
+    Series,
+    Team,
 )
+from .utils import autocommit, convert_name_to_id
 
-try:
-    from collections import OrderedDict
-except ImportError:
-    from ordereddict import OrderedDict
 
-
-class TahrirDatabase(object):
+class TahrirDatabase:
     """
     Class for talking to the Tahrir database
     It handles adding information necessary to issue open badges
 
     Pass one or the other of the two parameters, but not both.
 
     :type dburi: str
     :param dburi: the sqlalchemy database URI
 
     :type session: SQLAlchemy session object
     :param session: an already configured session object.
     """
 
-    def __init__(self, dburi=None, session=None, autocommit=True,
-                 notification_callback=None):
+    def __init__(self, dburi=None, session=None, autocommit=True, notification_callback=None):
         if not dburi and not session:
             raise ValueError("You must provide either 'dburi' or 'session'")
 
         if dburi and session:
             raise ValueError("Provide only one, either 'dburi' or 'session'")
 
         self.autocommit = autocommit
-        self.session = session
 
         if dburi:
-            self.session_maker = sessionmaker(bind=create_engine(dburi))
-            self.session = scoped_session(self.session_maker)
+            with importlib.resources.as_file(
+                importlib.resources.files("tahrir_api").joinpath("migrations")
+            ) as alembic_path:
+                self.db_mgr = DatabaseManager(dburi, alembic_path.as_posix())
+            self.session = self.db_mgr.Session()
+        else:
+            self.session = session
 
         self.notification_callback = notification_callback
 
     def team_exists(self, team_id):
         """
         Check to see if this team already exists in the database
 
         :type team_id: str
         :param team_id: The ID of a Team
         """
 
-        return self.session.query(Team).filter(
-            func.lower(Team.id) == func.lower(team_id)).count() != 0
+        return (
+            self.session.query(Team).filter(func.lower(Team.id) == func.lower(team_id)).count() != 0
+        )
 
     def get_team(self, team_id):
         """
         Return the team with the given ID
 
         :type team_id: str
         :param team_id: The ID of the team to return
         """
 
         if self.team_exists(team_id):
-            return self.session.query(Team).filter(
-                func.lower(Team.id) == func.lower(team_id)).first()
+            return (
+                self.session.query(Team).filter(func.lower(Team.id) == func.lower(team_id)).first()
+            )
         return None
 
     @autocommit
     def create_team(self, name, team_id=None):
         """
         Adds a new team to the database
 
         :type name: str
         :param name: Name of the team
+        :type team_id: int
+        :param team_id: Id of the team
         """
 
         if not team_id:
             team_id = convert_name_to_id(name)
 
         if not self.team_exists(team_id):
-            new_team = Team(id=team_id,
-                            name=name)
+            new_team = Team(id=team_id, name=name)
 
             self.session.add(new_team)
             self.session.flush()
         return team_id
 
     def series_exists(self, series_id):
         """
         Check to see if this series already exists in the database
 
         :type series_id: str
         :param series_id: The ID of a Series
         """
 
-        return self.session.query(Series).filter(
-            func.lower(Series.id) == func.lower(series_id)).count() != 0
+        return (
+            self.session.query(Series)
+            .filter(func.lower(Series.id) == func.lower(series_id))
+            .count()
+            != 0
+        )
 
     def get_series(self, series_id):
         """
         Return the series with the given ID
 
         :type series_id: str
         :param series_id: The ID of the series to return
         """
 
         if self.series_exists(series_id):
-            return self.session.query(Series).filter(
-                func.lower(Series.id) == func.lower(series_id)).one()
+            return (
+                self.session.query(Series)
+                .filter(func.lower(Series.id) == func.lower(series_id))
+                .one()
+            )
         return None
 
     def get_series_from_team(self, team_id):
         """
         Return the series related to a given team ID
 
-        :type series_id: str
-        :param series_id: The ID of the team
+        :type team_id: str
+        :param team_id: The ID of the team
         """
         if self.team_exists(team_id):
-            return self.session.query(Series).filter(
-                Series.team_id == team_id).all()
+            return self.session.query(Series).filter(Series.team_id == team_id).all()
 
     @autocommit
     def create_series(self, name, desc, team_id, tags=None, series_id=None):
         """
         Adds a new series to the database
 
         :type name: str
@@ -150,19 +167,17 @@
         :param series_id: ID of the Series
         """
 
         if not series_id:
             series_id = convert_name_to_id(name)
 
         if not self.series_exists(series_id):
-            new_series = Series(id=series_id,
-                                name=name,
-                                description=desc,
-                                tags=tags,
-                                team_id=team_id)
+            new_series = Series(
+                id=series_id, name=name, description=desc, tags=tags, team_id=team_id
+            )
 
             self.session.add(new_series)
             self.session.flush()
         return series_id
 
     def get_all_series(self):
         """
@@ -174,63 +189,62 @@
     def milestone_exists(self, milestone_id):
         """
         Check to see if this milestone already exists in the database
 
         :type milestone_id: str
         :param milestone_id: The ID of a Milestone
         """
-        return self.session.query(Milestone).filter(
-            Milestone.id == milestone_id).count() != 0
+        return self.session.query(Milestone).filter(Milestone.id == milestone_id).count() != 0
 
     def milestone_exists_for_badge_series(self, badge_id, series_id):
         """
         Check if the milestone with the given series and badge id exists
 
         :type badge_id: str
         :param badge_id: The ID of the badge
 
         :type series_id: str
         :param series_id: The ID of the series
         """
-        return self.get_milestone_from_badge_series(badge_id,
-                                                    series_id).count() != 0
+        return self.get_milestone_from_badge_series(badge_id, series_id).count() != 0
 
     def get_milestone_from_badge_series(self, badge_id, series_id):
         """
         Return the milestone with the given series and badge id
 
         :type badge_id: str
         :param badge_id: The ID of the badge
 
         :type series_id: str
         :param series_id: The ID of the series
         """
         return self.session.query(Milestone).filter(
-            and_(Milestone.series_id == func.lower(series_id),
-                 Milestone.badge_id == func.lower(badge_id)))
+            and_(
+                Milestone.series_id == func.lower(series_id),
+                Milestone.badge_id == func.lower(badge_id),
+            )
+        )
 
     def get_milestone(self, milestone_id):
         """
         Return the matching milestone from the database
 
         :type milestone_id: str
         :param milestone_id: The ID of a Milestone
         """
-        return self.session.query(Milestone).filter(
-            Milestone.id == milestone_id)
+        return self.session.query(Milestone).filter(Milestone.id == milestone_id)
 
     def get_all_milestones(self, series_id):
         """
         Returns all the milestones for the series
 
         :type series_id: str
         :param series_id: The id of the Series
         """
-        return self.session.query(Milestone).filter(
-            Milestone.series_id == series_id).all()
+        return self.session.query(Milestone).filter(Milestone.series_id == series_id).all()
 
     @autocommit
     def create_milestone(self, position, badge_id, series_id):
         """
         Adds a new milestone to the database
 
         :type name: int
@@ -238,36 +252,32 @@
 
         :type badge_id: str
         :param badge_id: Badge ID for the Milestone
 
         :type series_id: str
         :param series_id: ID of the Series
         """
-        milestone = self.get_milestone_from_badge_series(badge_id,
-                                                         series_id).first()
+        milestone = self.get_milestone_from_badge_series(badge_id, series_id).first()
         if not milestone:
-            milestone = Milestone(position=position,
-                                  badge_id=badge_id,
-                                  series_id=series_id)
+            milestone = Milestone(position=position, badge_id=badge_id, series_id=series_id)
 
             self.session.add(milestone)
             self.session.flush()
         milestone_id = milestone.id
 
         return milestone_id
 
     def get_milestone_from_series_ids(self, series_ids):
         """
         Return list of milestones for the list of series ids
 
         :type series: list
         :param series: list of series ids
         """
-        milestones = self.session.query(Milestone).filter(
-            Milestone.series_id.in_(series_ids)).all()
+        milestones = self.session.query(Milestone).filter(Milestone.series_id.in_(series_ids)).all()
 
         seen = set()
         unique_milestones = []
 
         for milestone in milestones:
             milestone_meta = (milestone.series_id, milestone.id)
             if milestone_meta not in seen:
@@ -284,54 +294,55 @@
         :param team_id: id of the team
         """
         if self.team_exists(team_id):
             series = self.get_series_from_team(team_id)
             series_ids = [elem.id for elem in series]
 
             milestones = self.get_milestone_from_series_ids(series_ids)
-            badge_ids = list(set([milestone.badge_id
-                                  for milestone in milestones]))
+            badge_ids = list(set([milestone.badge_id for milestone in milestones]))
 
             badges = self.get_badges(badge_ids)
             return badges
         return None
 
     def badge_exists(self, badge_id):
         """
         Check to see if this badge already exists in the database
 
         :type badge_id: str
         :param badge_id: The ID of a Badge
         """
 
-        return self.session.query(Badge).filter(
-            func.lower(Badge.id) == func.lower(badge_id)).count() != 0
+        return (
+            self.session.query(Badge).filter(func.lower(Badge.id) == func.lower(badge_id)).count()
+            != 0
+        )
 
     def get_badge(self, badge_id):
         """
         Return the badge with the given ID
 
         :type badge_id: str
         :param badge_id: The ID of the badge to return
         """
 
         if self.badge_exists(badge_id):
-            return self.session.query(Badge).filter(
-                func.lower(Badge.id) == func.lower(badge_id)).one()
+            return (
+                self.session.query(Badge).filter(func.lower(Badge.id) == func.lower(badge_id)).one()
+            )
         return None
 
     def get_badges(self, badge_ids):
         """
         Return the badges with the given IDs
 
         :type badge_ids: list
         :param badge_ids: The list of badge IDs
         """
-        badges = self.session.query(Badge).filter(
-            Badge.id.in_(badge_ids)).all()
+        badges = self.session.query(Badge).filter(Badge.id.in_(badge_ids)).all()
 
         return badges
 
     def get_badges_from_tags(self, tags, match_all=False):
         """
         Return badges matching tags.
 
@@ -343,23 +354,27 @@
         """
 
         badges = list()
 
         if match_all:
             # Return badges matching all tags
             # ... by doing argument-expansion on a list comprehension
-            badges.extend(self.session.query(Badge).filter(and_(*[
-                func.lower(Badge.tags).contains(str(tag + ',').lower())
-                for tag in tags])))
+            badges.extend(
+                self.session.query(Badge).filter(
+                    and_(*[func.lower(Badge.tags).contains(str(tag + ",").lower()) for tag in tags])
+                )
+            )
         else:
             # Return badges matching any of the tags
             for tag in tags:
-                badges.extend(self.session.query(Badge).filter(
-                    func.lower(Badge.tags).contains(
-                        str(tag + ',').lower())).all())
+                badges.extend(
+                    self.session.query(Badge)
+                    .filter(func.lower(Badge.tags).contains(str(tag + ",").lower()))
+                    .all()
+                )
 
         # Eliminate any duplicates.
         unique_badges = list()
         for badge in badges:
             if badge not in unique_badges:
                 unique_badges.append(badge)
 
@@ -385,16 +400,15 @@
             to_delete = self.session.query(Badge).filter_by(id=badge_id).one()
             self.session.delete(to_delete)
             self.session.flush()
             return badge_id
         return False
 
     @autocommit
-    def add_badge(self, name, image, desc, criteria, issuer_id,
-                  tags=None, badge_id=None):
+    def add_badge(self, name, image, desc, criteria, issuer_id, tags=None, badge_id=None):
         """
         Add a new badge to the database
 
         :type name: str
         :param name: Name of the Badge
 
         :type image: str
@@ -414,25 +428,27 @@
             badge_id = convert_name_to_id(name)
 
         if not self.badge_exists(badge_id):
             # Make sure the tags string has a trailing
             # comma at the end. The tags view in Tahrir
             # depends on that comma when matching all
             # tags.
-            if tags and not tags.endswith(','):
-                tags = tags + ','
+            if tags and not tags.endswith(","):
+                tags = tags + ","
 
             # Actually add the badge.
-            new_badge = Badge(id=badge_id,
-                              name=name,
-                              image=image,
-                              description=desc,
-                              criteria=criteria,
-                              issuer_id=issuer_id,
-                              tags=tags)
+            new_badge = Badge(
+                id=badge_id,
+                name=name,
+                image=image,
+                description=desc,
+                criteria=criteria,
+                issuer_id=issuer_id,
+                tags=tags,
+            )
             self.session.add(new_badge)
             self.session.flush()
         return badge_id
 
     def person_exists(self, email=None, id=None, nickname=None):
         """
         Check if a Person with this email is stored in the database
@@ -445,42 +461,43 @@
 
         :type nickname: str
         :param nickname: A nickname to search for.
         """
 
         query = self.session.query(Person)
         if email:
-            return query.filter(
-                func.lower(Person.email) == func.lower(email)).count() != 0
+            return query.filter(func.lower(Person.email) == func.lower(email)).count() != 0
         elif id:
             return query.filter_by(id=id).count() != 0
         elif nickname:
-            return query.filter(func.lower(Person.nickname) == func.lower(
-                nickname)).count() != 0
+            return query.filter(func.lower(Person.nickname) == func.lower(nickname)).count() != 0
         else:
             return False
 
     def person_opted_out(self, email=None, id=None, nickname=None):
-        """ Returns true if a given person has opted out of tahrir. """
+        """Returns true if a given person has opted out of tahrir."""
 
         person = self.get_person(email, id, nickname)
 
         # If they don't exist, then they haven't opted out.
         if not person:
             return False
 
         # Otherwise, return whatever value they have in the DB.
         return person.opt_out
 
-    def get_all_persons(self):
+    def get_all_persons(self, include_opted_out=False):
         """
         Gets all the persons in the db.
         """
 
-        return self.session.query(Person)
+        query = self.session.query(Person)
+        if not include_opted_out:
+            query = query.filter(not_(Person.opt_out))
+        return query
 
     def get_person_email(self, person_id):
         """
         Convience function to retrieve a person email from an id.
 
         I am so sorry that I had to write this.
         It is easier than rewriting all of the get_person and
@@ -493,16 +510,20 @@
         get_x_by_email or get_x and get_x_by_id).
 
         :type person_id: str
         :param person_id: The email of a Person in the database.
         """
 
         if self.person_exists(id=person_id):
-            return self.session.query(Person).filter(
-                func.lower(Person.id) == func.lower(person_id)).one().email
+            return (
+                self.session.query(Person)
+                .filter(func.lower(Person.id) == func.lower(person_id))
+                .one()
+                .email
+            )
         return None
 
     def get_person(self, person_email=None, id=None, nickname=None):
         """
         Convenience function to retrieve a person object from an email,
         id, or nickname.
 
@@ -515,21 +536,19 @@
         :type nickname: str
         :param nickname: The nickname of a Person in the database
         """
 
         query = self.session.query(Person)
 
         if person_email and self.person_exists(email=person_email):
-            return query.filter(
-                func.lower(Person.email) == func.lower(person_email)).one()
+            return query.filter(func.lower(Person.email) == func.lower(person_email)).one()
         elif id and self.person_exists(id=id):
             return query.filter_by(id=id).one()
         elif nickname and self.person_exists(nickname=nickname):
-            return query.filter(
-                func.lower(Person.nickname) == func.lower(nickname)).one()
+            return query.filter(func.lower(Person.nickname) == func.lower(nickname)).one()
         else:
             return None
 
     @autocommit
     def delete_person(self, person_email):
         """
         Delete a person with the given email
@@ -541,16 +560,15 @@
         if self.person_exists(email=person_email):
             self.session.delete(self.get_person(person_email))
             self.session.flush()
             return person_email
         return False
 
     @autocommit
-    def add_person(self, email, nickname=None,
-                   website=None, bio=None):
+    def add_person(self, email, nickname=None, website=None, bio=None):
         """
         Add a new Person to the database
 
         :type email: str
         :param email: This Person's email address
 
         :type nickname: str
@@ -560,64 +578,53 @@
         :param website: This Person's website
 
         :type website: str
         :param bio: This Person's bio
         """
 
         if not self.person_exists(email=email):
-
             # If no nickname is specified, just use the first bit of their
             # email as a convenient default.
             if not nickname:
-                nickname = email.split('@')[0]
+                nickname = email.split("@")[0]
 
-            new_person = Person(email=email, nickname=nickname,
-                                website=website, bio=bio)
+            new_person = Person(email=email, nickname=nickname, website=website, bio=bio)
             self.session.add(new_person)
             self.session.flush()
 
             return email
         return False
 
     @autocommit
     def note_login(self, person_email=None, id=None, nickname=None):
-        """ Make a note that a person has logged in. """
+        """Make a note that a person has logged in."""
 
         person = self.get_person(person_email, id, nickname)
 
         # If this is the first time they have ever logged in, optionally
         # publish a notification about the event.
         if not person.last_login and self.notification_callback:
-            self.notification_callback(
-                topic='person.login.first',
-                msg=dict(
-                    user=dict(
-                        username=person.nickname,
-                        badges_user_id=person.id,
-                    )
-                )
-            )
+            body = dict(user=dict(username=person.nickname, badges_user_id=person.id))
+            self.notification_callback(PersonLoginFirstV1(body=body))
 
         # Finally, update the field.
-        person.last_login = datetime.utcnow()
+        person.last_login = datetime.now(timezone.utc)
 
     def issuer_exists(self, origin, name):
         """
         Check to see if an issuer with this ID is in the database
 
         :type issuer_id: int
         :param issuer_id: The unique ID of this issuer
         """
 
-        return self.session.query(Issuer).filter_by(
-            origin=origin, name=name).count() != 0
+        return self.session.query(Issuer).filter_by(origin=origin, name=name).count() != 0
 
     @autocommit
-    def add_invitation(self, badge_id, created_on=None, expires_on=None,
-                       created_by_email=None):
+    def add_invitation(self, badge_id, created_on=None, expires_on=None, created_by_email=None):
         """
         Add a new invitation to the database
 
         :type badge_id: str
         :param badge_id: A badge ID
 
         :type created_on: datetime.datetime
@@ -630,20 +637,20 @@
         :param created_by_email: User email of creator
 
         """
 
         if not self.badge_exists(badge_id):
             raise ValueError("No such badge %r" % badge_id)
 
-        created_on = created_on or datetime.utcnow()
+        created_on = created_on or datetime.now(timezone.utc)
         expires_on = expires_on or (created_on + timedelta(hours=1))
         if self.person_exists(email=created_by_email):
             created_by = self.get_person(created_by_email).id
         else:
-            created_by = "1"
+            created_by = self.session.query(Person).first().id
 
         invitation = Invitation(
             created_on=created_on,
             expires_on=expires_on,
             badge_id=badge_id,
             created_by=created_by,
         )
@@ -655,16 +662,15 @@
         """
         Check to see if an invitation exists with this ID.
 
         :type invitation_id: str
         :param invitation_id: The unique ID of this invitation
         """
 
-        return self.session.query(Invitation).filter_by(
-            id=invitation_id).count() != 0
+        return self.session.query(Invitation).filter_by(id=invitation_id).count() != 0
 
     def get_all_invitations(self):
         """
         Get all invitations in the db.
         """
 
         return self.session.query(Invitation)
@@ -674,30 +680,28 @@
         Get invitation by an invitation id.
 
         :type invitation_id: str
         :param invitation_id: The unique ID of this invitation
         """
 
         if self.invitation_exists(invitation_id):
-            return self.session.query(Invitation).filter_by(
-                id=invitation_id).one()
+            return self.session.query(Invitation).filter_by(id=invitation_id).one()
         else:
             return False
 
     def get_invitations(self, person_id):
         """
         Get invitations created by a particular person.
 
         :type issuer_id: str
         :param issuer_id: The person ID for which inviations
                           will be retrieved.
         """
 
-        return self.session.query(Invitation).filter_by(
-            created_by=person_id).all()
+        return self.session.query(Invitation).filter_by(created_by=person_id).all()
 
     def get_issuer(self, issuer_id):
         """
         Return the issuer with the given ID
 
         :type issuer_id: int
         :param issuer_id: ID of the issuer to return
@@ -739,26 +743,20 @@
         :param org: The org of this issuer
 
         :type contact: str
         :param contact: The Contact email for this issuer
         """
 
         if not self.issuer_exists(origin, name):
-            new_issuer = Issuer(
-                origin=origin,
-                name=name,
-                org=org,
-                contact=contact,
-            )
+            new_issuer = Issuer(origin=origin, name=name, org=org, contact=contact)
             self.session.add(new_issuer)
             self.session.flush()
             return new_issuer.id
 
-        return self.session.query(Issuer)\
-            .filter_by(name=name, origin=origin).one().id
+        return self.session.query(Issuer).filter_by(name=name, origin=origin).one().id
 
     def get_all_issuers(self):
         """
         Get all issuers in the db.
         """
 
         return self.session.query(Issuer)
@@ -775,32 +773,33 @@
         Get all assertions attached to the given email
 
         :type person_email: str
         :param person_email: Email of the person to get assertions for
         """
 
         if self.person_exists(email=person_email):
-            person_id = self.session.query(Person).filter_by(
-                email=person_email).one().id
-            return self.session.query(Assertion).filter_by(
-                person_id=person_id).all()
+            person_id = self.session.query(Person).filter_by(email=person_email).one().id
+            return self.session.query(Assertion).filter_by(person_id=person_id).all()
         else:
             return False
 
     def get_assertions_by_badge(self, badge_id):
         """
         Get all assertions of a particular badge.
 
         :type badge_id: str
         :param badge_id: Badge id to get assertions for.
         """
 
         if self.badge_exists(badge_id):
-            return self.session.query(Assertion).filter(
-                func.lower(Assertion.badge_id) == func.lower(badge_id)).all()
+            return (
+                self.session.query(Assertion)
+                .filter(func.lower(Assertion.badge_id) == func.lower(badge_id))
+                .all()
+            )
         else:
             return False
 
     def assertion_exists(self, badge_id, email):
         """
         Check if an assertion exists in the database
 
@@ -812,16 +811,18 @@
         """
 
         person = self.get_person(email)
 
         if not person:
             return False
 
-        return self.session.query(Assertion).filter_by(
-            person_id=person.id, badge_id=badge_id).count() != 0
+        return (
+            self.session.query(Assertion).filter_by(person_id=person.id, badge_id=badge_id).count()
+            != 0
+        )
 
     def authorization_exists(self, badge_id, email):
         """
         Check if an authorization exists in the database
 
         :type badge_id: str
         :param badge_id: ID of the badge
@@ -831,49 +832,46 @@
         """
 
         person = self.get_person(email)
 
         if not person:
             return False
 
-        return self.session.query(Authorization).filter_by(
-            person_id=person.id, badge_id=badge_id).count() != 0
+        return (
+            self.session.query(Authorization)
+            .filter_by(person_id=person.id, badge_id=badge_id)
+            .count()
+            != 0
+        )
 
     @autocommit
     def add_authorization(self, badge_id, person_email):
         """
         Add an authorization (allow someone to admin a certain badge)
 
         :type badge_id: str
         :param badge_id: ID of the badge
 
         :type person_email: str
         :param person_email: Email of the Person grant rights to
         """
 
-        if self.person_exists(email=person_email) and \
-           self.badge_exists(badge_id):
-
+        if self.person_exists(email=person_email) and self.badge_exists(badge_id):
             person = self.get_person(person_email)
 
-            new_authz = Authorization(badge_id=badge_id,
-                                      person_id=person.id)
+            new_authz = Authorization(badge_id=badge_id, person_id=person.id)
             self.session.add(new_authz)
             self.session.flush()
 
             return (person_email, badge_id)
 
         return False
 
     @autocommit
-    def add_assertion(self,
-                      badge_id,
-                      person_email,
-                      issued_on,
-                      issued_for=None):
+    def add_assertion(self, badge_id, person_email, issued_on, issued_for=None):
         """
         Add an assertion (award a badge) to the database
 
         :type badge_id: str
         :param badge_id: ID of the badge to be issued
 
         :type person_email: str
@@ -884,55 +882,50 @@
         on
 
         :type issued_for: str
         :param issued_for: An optional link back to the warranting event
         """
 
         if issued_on is None:
-            issued_on = datetime.utcnow()
-
-        if self.person_exists(email=person_email) and \
-           self.badge_exists(badge_id):
+            issued_on = datetime.now(timezone.utc)
 
+        if self.person_exists(email=person_email) and self.badge_exists(badge_id):
             badge = self.get_badge(badge_id)
             person = self.get_person(person_email)
             old_rank = person.rank
 
-            new_assertion = Assertion(badge_id=badge_id,
-                                      person_id=person.id,
-                                      issued_on=issued_on,
-                                      issued_for=issued_for)
+            new_assertion = Assertion(
+                badge_id=badge_id,
+                person_id=person.id,
+                issued_on=issued_on,
+                issued_for=issued_for,
+            )
             self.session.add(new_assertion)
             self.session.flush()
 
             if self.notification_callback:
-                self.notification_callback(
-                    topic='badge.award',
-                    msg=dict(
-                        badge=dict(
-                            name=badge.name,
-                            description=badge.description,
-                            image_url=badge.image,
-                            badge_id=badge_id,
-                        ),
-                        user=dict(
-                            username=person.nickname,
-                            badges_user_id=person.id,
-                        )
-                    )
+                body = dict(
+                    badge=dict(
+                        name=badge.name,
+                        description=badge.description,
+                        image_url=badge.image,
+                        badge_id=badge_id,
+                    ),
+                    user=dict(username=person.nickname, badges_user_id=person.id),
                 )
+                self.notification_callback(BadgeAwardV1(body=body))
 
             self._adjust_ranks(person, old_rank)
 
-            return (person_email, badge_id)
+            return person_email, badge_id
 
         return False
 
     def _adjust_ranks(self, person, old_rank):
-        """ Given a person model object and the 'old' rank of that person,
+        """Given a person model object and the 'old' rank of that person,
         adjust the ranks of all persons between the 'old' rank and the present
         rank of the given person.
 
         This is a utility function typically called when a person is awarded a
         new badge, and their rank advances.  Since we cache rank in the
         database, we want to also decrement the rank of all persons that the
         given person is "passing" on the all-time leaderboard.
@@ -943,29 +936,24 @@
 
         # Recalculate rank in all cases, otherwise "overtaking" won't work
         # anymore (with rank being shared, a new badge won't change a person's
         # own position, but needs to demote the rest).
 
         # Otherwise, take our calculations and commit them to the db.
         for _person, data in leaderboard.items():
-            _person.rank = data['rank']
+            _person.rank = data["rank"]
 
         self.session.flush()
 
+        body = dict(person=person.as_dict(), old_rank=old_rank)
         if self.notification_callback:
-            self.notification_callback(
-                topic='person.rank.advance',
-                msg=dict(
-                    person=person,
-                    old_rank=old_rank,
-                )
-            )
+            self.notification_callback(PersonRankAdvanceV1(body=body))
 
     def _make_leaderboard(self, start=None, stop=None):
-        """ Produce a dict mapping persons to information about
+        """Produce a dict mapping persons to information about
         the number of badges they have been awarded and their
         rank, freshly calculated.  This is relatively expensive.
 
         The 'start' and 'stop' parameters are optional datetime objects.
         If specified, the leaderboard will be calculated from badges that were
         awarded only in the time period between 'start' and 'stop'.  Passing
         only one of 'start' or 'stop' is meaningless -- the other value will be
@@ -976,28 +964,29 @@
         null/None rank.  They will be absent from the returned leaderboard
         dict.
 
         Ricky Elrod originally contributed this to tahrir.
         Moved here by Ralph Bean.
         """
 
-        leaderboard = self.session\
-            .query(Person, func.count(Person.assertions).label('count_1'))\
-            .join(Assertion)
+        leaderboard = self.session.query(
+            Person, func.count(Person.assertions).label("count_1")
+        ).join(Assertion)
 
         if start and stop:
-            leaderboard = leaderboard\
-                .filter(Assertion.issued_on >= start)\
-                .filter(Assertion.issued_on <= stop)
-
-        leaderboard = leaderboard\
-            .order_by('count_1 desc')\
-            .filter(not_(Person.opt_out))\
-            .group_by(Person)\
+            leaderboard = leaderboard.filter(Assertion.issued_on >= start).filter(
+                Assertion.issued_on <= stop
+            )
+
+        leaderboard = (
+            leaderboard.order_by(text("count_1 desc"))
+            .filter(not_(Person.opt_out))
+            .group_by(Person)
             .all()
+        )
 
         # Hackishly, but relatively cheaply get the rank of all users.
         # This is:
         # { <person object>:
         #   {
         #     'badges': <number of badges they have>,
         #     'rank': <their global rank>
@@ -1014,12 +1003,10 @@
             user, badges = data[0:2]
             if badges == prev_badges:
                 # same amount of badges -> same rank
                 rank = prev_rank
             else:
                 prev_rank = rank = idx + 1
                 prev_badges = badges
-            user_to_rank[user] = {
-                'badges': badges,
-                'rank': rank}
+            user_to_rank[user] = {"badges": badges, "rank": rank}
 
         return user_to_rank
```

### Comparing `tahrir-api-0.8.1/alembic/versions/24282792d72a_add_created_by_field.py` & `tahrir_api-1.0.0/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 Revision ID: 24282792d72a
 Revises: 5791a2b9fb6a
 Create Date: 2013-06-10 15:51:02.288685
 
 """
 
-# revision identifiers, used by Alembic.
-revision = '24282792d72a'
-down_revision = '5791a2b9fb6a'
-
-from alembic import op
 import sqlalchemy as sa
+from alembic import op
+
+
+# revision identifiers, used by Alembic.
+revision = "24282792d72a"
+down_revision = "5791a2b9fb6a"
 
 
 def upgrade():
     op.add_column(
-        'invitations',
-        sa.Column(
-            'created_by', sa.Unicode(128),
-            sa.ForeignKey('persons.id'), nullable=False))
+        "invitations",
+        sa.Column("created_by", sa.Unicode(128), sa.ForeignKey("persons.id"), nullable=False),
+    )
 
 
 def downgrade():
     # Downgrade will fail if using SQLite. The transaction will
     # be rolled back as per env.py.
-    op.drop_column('invitations', 'created_by')
+    op.drop_column("invitations", "created_by")
```

### Comparing `tahrir-api-0.8.1/alembic/versions/3c7fd5b4e2c2_add_two_new_columns_.py` & `tahrir_api-1.0.0/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 
 Revision ID: 3c7fd5b4e2c2
 Revises: 24282792d72a
 Create Date: 2013-06-26 14:46:28.361709
 
 """
 
-# revision identifiers, used by Alembic.
-revision = '3c7fd5b4e2c2'
-down_revision = '16943d9088cf'
+import datetime
 
-import tahrir_api
-from alembic import op
 import sqlalchemy as sa
-import datetime
+from alembic import op
+
+import tahrir_api
+
+
+# revision identifiers, used by Alembic.
+revision = "3c7fd5b4e2c2"
+down_revision = "16943d9088cf"
 
 
 def upgrade():
-    op.add_column(u'persons', sa.Column('created_on', sa.DateTime()))
-    op.add_column(u'persons', sa.Column('opt_out', sa.Boolean()))
+    op.add_column("persons", sa.Column("created_on", sa.DateTime()))
+    op.add_column("persons", sa.Column("opt_out", sa.Boolean()))
 
     # We have to do this manually because I can't figure out how to make
     # alembic apply defaults to sqlite.
     engine = op.get_bind().engine
     session_maker = sa.orm.sessionmaker(bind=engine)
     session = sa.orm.scoped_session(session_maker)
     persons = session.query(tahrir_api.model.Person).all()
@@ -30,9 +33,9 @@
         # Set our defaults
         person.created_on = datetime.datetime.now()
         person.opt_out = False
     session.commit()
 
 
 def downgrade():
-    op.drop_column(u'persons', 'opt_out')
-    op.drop_column(u'persons', 'created_on')
+    op.drop_column("persons", "opt_out")
+    op.drop_column("persons", "created_on")
```

### Comparing `tahrir-api-0.8.1/alembic/versions/ce541796a7_add_authz_table.py` & `tahrir_api-1.0.0/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 
 Revision ID: ce541796a7
 Revises: 4099fa344171
 Create Date: 2013-12-13 15:30:16.576871
 
 """
 
-# revision identifiers, used by Alembic.
-revision = 'ce541796a7'
-down_revision = '4099fa344171'
-
-from alembic import op
 import sqlalchemy as sa
+from alembic import op
+
+
+# revision identifiers, used by Alembic.
+revision = "ce541796a7"
+down_revision = "4099fa344171"
 
 
 def upgrade():
     op.create_table(
-        'authorizations',
-        sa.Column('id', sa.Integer(), nullable=False),
-        sa.Column('badge_id', sa.Unicode(length=128), nullable=False),
-        sa.Column('person_id', sa.Integer(), nullable=False),
-        sa.ForeignKeyConstraint(['badge_id'], ['badges.id'], ),
-        sa.ForeignKeyConstraint(['person_id'], ['persons.id'], ),
-        sa.PrimaryKeyConstraint('id')
+        "authorizations",
+        sa.Column("id", sa.Integer(), nullable=False),
+        sa.Column("badge_id", sa.Unicode(length=128), nullable=False),
+        sa.Column("person_id", sa.Integer(), nullable=False),
+        sa.ForeignKeyConstraint(["badge_id"], ["badges.id"]),
+        sa.ForeignKeyConstraint(["person_id"], ["persons.id"]),
+        sa.PrimaryKeyConstraint("id"),
     )
 
 
 def downgrade():
-    op.drop_table('authorizations')
+    op.drop_table("authorizations")
```

### Comparing `tahrir-api-0.8.1/alembic/versions/4099fa344171_add_last_login.py` & `tahrir_api-1.0.0/tahrir_api/migrations/versions/4099fa344171_add_last_login.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 
 Revision ID: 4099fa344171
 Revises: 139ec7ed17b7
 Create Date: 2013-10-24 10:13:45.104902
 
 """
 
-# revision identifiers, used by Alembic.
-revision = '4099fa344171'
-down_revision = '139ec7ed17b7'
-
-from alembic import op
 import sqlalchemy as sa
+from alembic import op
+
+
+# revision identifiers, used by Alembic.
+revision = "4099fa344171"
+down_revision = "139ec7ed17b7"
 
 
 def upgrade():
     ### commands auto generated by Alembic - please adjust! ###
-    op.add_column(
-        'persons',
-        sa.Column('last_login', sa.DateTime(), nullable=True))
+    op.add_column("persons", sa.Column("last_login", sa.DateTime(), nullable=True))
     ### end Alembic commands ###
 
 
 def downgrade():
     ### commands auto generated by Alembic - please adjust! ###
-    op.drop_column('persons', 'last_login')
+    op.drop_column("persons", "last_login")
     ### end Alembic commands ###
```

### Comparing `tahrir-api-0.8.1/alembic/versions/fa1d309e8c3_add_created_on_field.py` & `tahrir_api-1.0.0/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 Revision ID: fa1d309e8c3
 Revises: 420c02357a1b
 Create Date: 2013-06-10 12:30:31.850641
 
 """
 
-# revision identifiers, used by Alembic.
-revision = 'fa1d309e8c3'
-down_revision = '420c02357a1b'
-
-from alembic import op
 import sqlalchemy as sa
+from alembic import op
+
+
+# revision identifiers, used by Alembic.
+revision = "fa1d309e8c3"
+down_revision = "420c02357a1b"
 
 
 def upgrade():
-    op.add_column(
-        'issuers',
-        sa.Column('created_on', sa.DateTime, nullable=False))
+    op.add_column("issuers", sa.Column("created_on", sa.DateTime, nullable=False))
 
 
 def downgrade():
     # This will fail if using SQLite. The transaction will
     # be rolled back.
-    op.drop_column('issuers', 'created_on')
+    op.drop_column("issuers", "created_on")
```

### Comparing `tahrir-api-0.8.1/alembic/versions/e7040e76728_create_new_tables_for_quest.py` & `tahrir_api-1.0.0/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,67 +2,80 @@
 
 Revision ID: e7040e76728
 Revises: 508367dcbbb5
 Create Date: 2016-09-02 20:51:14.951460
 
 """
 
-# revision identifiers, used by Alembic.
-revision = 'e7040e76728'
-down_revision = '508367dcbbb5'
-
 import datetime
 
-from alembic import op
 import sqlalchemy as sa
+from alembic import op
+
+
+# revision identifiers, used by Alembic.
+revision = "e7040e76728"
+down_revision = "508367dcbbb5"
+
 
 def generate_default_id(context):
-    return context.current_parameters['name'].lower().replace(' ', '-')
+    return context.current_parameters["name"].lower().replace(" ", "-")
+
 
 def upgrade():
 
     op.create_table(
-        'team',
-        sa.Column('id', sa.Unicode(length=128), nullable=False,
-                  default=generate_default_id),
-        sa.Column('name', sa.Unicode(length=128), nullable=False),
-        sa.Column('created_on', sa.DateTime(), nullable=False,
-                  default=datetime.datetime.utcnow),
-        sa.PrimaryKeyConstraint('id'),
-        sa.UniqueConstraint('name')
+        "team",
+        sa.Column("id", sa.Unicode(length=128), nullable=False, default=generate_default_id),
+        sa.Column("name", sa.Unicode(length=128), nullable=False),
+        sa.Column(
+            "created_on",
+            sa.DateTime(),
+            nullable=False,
+            default=datetime.datetime.now,
+        ),
+        sa.PrimaryKeyConstraint("id"),
+        sa.UniqueConstraint("name"),
     )
     op.create_table(
-        'series',
-        sa.Column('id', sa.Unicode(length=128), nullable=False,
-                  default=generate_default_id),
-        sa.Column('name', sa.Unicode(length=128), nullable=False),
-        sa.Column('description', sa.Unicode(length=128), nullable=False),
-        sa.Column('created_on', sa.DateTime(), nullable=False,
-                  default=datetime.datetime.utcnow),
-        sa.Column('last_updated', sa.DateTime(), nullable=False,
-                  default=datetime.datetime.utcnow,
-                  onupdate=datetime.datetime.utcnow),
-        sa.Column('tags', sa.Unicode(length=128), nullable=True),
-        sa.Column('team_id', sa.Unicode(length=128), nullable=False),
-        sa.ForeignKeyConstraint(['team_id'], ['team.id'], ),
-        sa.PrimaryKeyConstraint('id'),
-        sa.UniqueConstraint('name')
+        "series",
+        sa.Column("id", sa.Unicode(length=128), nullable=False, default=generate_default_id),
+        sa.Column("name", sa.Unicode(length=128), nullable=False),
+        sa.Column("description", sa.Unicode(length=128), nullable=False),
+        sa.Column(
+            "created_on",
+            sa.DateTime(),
+            nullable=False,
+            default=datetime.datetime.now,
+        ),
+        sa.Column(
+            "last_updated",
+            sa.DateTime(),
+            nullable=False,
+            default=datetime.datetime.now,
+            onupdate=datetime.datetime.now,
+        ),
+        sa.Column("tags", sa.Unicode(length=128), nullable=True),
+        sa.Column("team_id", sa.Unicode(length=128), nullable=False),
+        sa.ForeignKeyConstraint(["team_id"], ["team.id"]),
+        sa.PrimaryKeyConstraint("id"),
+        sa.UniqueConstraint("name"),
     )
     op.create_table(
-        'milestone',
-        sa.Column('id', sa.Integer(), nullable=False),
-        sa.Column('position', sa.Integer(), nullable=True),
-        sa.Column('badge_id', sa.Unicode(length=128), nullable=False),
-        sa.Column('series_id', sa.Unicode(length=128), nullable=False),
-        sa.ForeignKeyConstraint(['badge_id'], ['badges.id'], ),
-        sa.ForeignKeyConstraint(['series_id'], ['series.id'], ),
-        sa.PrimaryKeyConstraint('id'),
-        sa.UniqueConstraint('id'),
-        sa.UniqueConstraint('position', 'badge_id', 'series_id')
+        "milestone",
+        sa.Column("id", sa.Integer(), nullable=False),
+        sa.Column("position", sa.Integer(), nullable=True),
+        sa.Column("badge_id", sa.Unicode(length=128), nullable=False),
+        sa.Column("series_id", sa.Unicode(length=128), nullable=False),
+        sa.ForeignKeyConstraint(["badge_id"], ["badges.id"]),
+        sa.ForeignKeyConstraint(["series_id"], ["series.id"]),
+        sa.PrimaryKeyConstraint("id"),
+        sa.UniqueConstraint("id"),
+        sa.UniqueConstraint("position", "badge_id", "series_id"),
     )
 
 
 def downgrade():
 
-    op.drop_table('milestone')
-    op.drop_table('series')
-    op.drop_table('team')
+    op.drop_table("milestone")
+    op.drop_table("series")
+    op.drop_table("team")
```

### Comparing `tahrir-api-0.8.1/alembic/env.py` & `tahrir_api-1.0.0/tahrir_api/migrations/env.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,81 +1,77 @@
-from __future__ import with_statement
+# from logging.config import fileConfig
+
 from alembic import context
 from sqlalchemy import engine_from_config, pool
-from logging.config import fileConfig
-
-import sqlalchemy as sa
-
-# this is the Alembic Config object, which provides
-# access to the values within the .ini file in use.
-config = context.config
-
-# Interpret the config file for Python logging.
-# This line sets up loggers basically.
-fileConfig(config.config_file_name)
 
 # add your model's MetaData object here
 # for 'autogenerate' support
 # from myapp import mymodel
 # target_metadata = mymodel.Base.metadata
 from tahrir_api import model
+
+
 target_metadata = model.DeclarativeBase.metadata
 
+# this is the Alembic Config object, which provides
+# access to the values within the .ini file in use.
+config = context.config
+
+# Interpret the config file for Python logging.
+# This line sets up loggers basically.
+# if config.config_file_name is not None:
+#     fileConfig(config.config_file_name)
 
 # other values from the config, defined by the needs of env.py,
 # can be acquired:
 # my_important_option = config.get_main_option("my_important_option")
 # ... etc.
 
-def run_migrations_offline():
+
+def run_migrations_offline() -> None:
     """Run migrations in 'offline' mode.
 
     This configures the context with just a URL
     and not an Engine, though an Engine is acceptable
     here as well.  By skipping the Engine creation
     we don't even need a DBAPI to be available.
 
     Calls to context.execute() here emit the given string to the
     script output.
 
     """
     url = config.get_main_option("sqlalchemy.url")
-    context.configure(url=url)
+    context.configure(
+        url=url,
+        target_metadata=target_metadata,
+        literal_binds=True,
+        dialect_opts={"paramstyle": "named"},
+    )
 
     with context.begin_transaction():
         context.run_migrations()
 
 
-def run_migrations_online():
+def run_migrations_online() -> None:
     """Run migrations in 'online' mode.
 
     In this scenario we need to create an Engine
     and associate a connection with the context.
 
     """
-    engine = engine_from_config(
-        config.get_section(config.config_ini_section),
-        prefix='sqlalchemy.',
-        poolclass=pool.NullPool)
+    connectable = engine_from_config(
+        config.get_section(config.config_ini_section, {}),
+        prefix="sqlalchemy.",
+        poolclass=pool.NullPool,
+    )
 
-    connection = engine.connect()
-    context.configure(
-        connection=connection,
-        target_metadata=target_metadata)
+    with connectable.connect() as connection:
+        context.configure(connection=connection, target_metadata=target_metadata)
 
-    trans = connection.begin()
-    try:
         with context.begin_transaction():
             context.run_migrations()
-            trans.commit()
-    except sa.exc.OperationalError as e:
-        print "SQLite does not allow one of these operations. Rolling back."
-        print "The exception was:"
-        print repr(e)
-        trans.rollback()
-    finally:
-        connection.close()
+
 
 if context.is_offline_mode():
     run_migrations_offline()
 else:
     run_migrations_online()
```

### Comparing `tahrir-api-0.8.1/LICENSE` & `tahrir_api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tahrir-api-0.8.1/alembic.ini` & `tahrir_api-1.0.0/tahrir_api/migrations/alembic.ini`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # file_template = %%(rev)s_%%(slug)s
 
 # set to 'true' to run the environment during
 # the 'revision' command, regardless of autogenerate
 # revision_environment = false
 
 # I guess we'll just assume that tahrir is in the same parent directory?
-sqlalchemy.url = sqlite:///%(here)s/../tahrir/tahrir.db
+sqlalchemy.url = sqlite:////%(here)s/tahrir.db
 
 
 # Logging configuration
 [loggers]
 keys = root,sqlalchemy,alembic
 
 [handlers]
```

