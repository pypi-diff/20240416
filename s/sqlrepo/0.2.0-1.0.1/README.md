# Comparing `tmp/sqlrepo-0.2.0.tar.gz` & `tmp/sqlrepo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlrepo-0.2.0.tar", last modified: Sun Apr 14 13:14:49 2024, max compression
+gzip compressed data, was "sqlrepo-1.0.1.tar", last modified: Mon Apr 15 11:41:28 2024, max compression
```

## Comparing `sqlrepo-0.2.0.tar` & `sqlrepo-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
--rw-r--r--   0        0        0       42 2024-04-14 11:04:24.825878 sqlrepo-0.2.0/README.md
--rw-r--r--   0        0        0     3013 2024-04-14 13:14:49.595104 sqlrepo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-23 13:08:38.602420 sqlrepo-0.2.0/sqlrepo/__init__.py
--rw-r--r--   0        0        0      452 2024-04-14 11:04:24.825878 sqlrepo-0.2.0/sqlrepo/exc.py
--rw-r--r--   0        0        0      748 2024-04-14 11:18:40.730497 sqlrepo-0.2.0/sqlrepo/logging.py
--rw-r--r--   0        0        0    26229 2024-04-14 13:11:15.769849 sqlrepo-0.2.0/sqlrepo/queries.py
--rw-r--r--   0        0        0    15641 2024-04-14 13:11:24.489836 sqlrepo-0.2.0/sqlrepo/repositories.py
--rw-r--r--   0        0        0     2565 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/sqlrepo/uow.py
--rw-r--r--   0        0        0        0 2024-02-23 13:08:38.602420 sqlrepo-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     6707 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0    15461 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/tests/test_base_queries.py
--rw-r--r--   0        0        0     9417 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/tests/test_sync_queries.py
--rw-r--r--   0        0        0        0 2024-02-23 13:08:38.602420 sqlrepo-0.2.0/tests/test_uow.py
--rw-r--r--   0        0        0      804 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/tests/types.py
--rw-r--r--   0        0        0     7107 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/tests/utils.py
--rw-r--r--   0        0        0      395 1970-01-01 00:00:00.000000 sqlrepo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7537 2024-04-15 11:38:30.385830 sqlrepo-1.0.1/README.md
+-rw-r--r--   0        0        0     3013 2024-04-15 11:41:28.464993 sqlrepo-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-1.0.1/sqlrepo/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-1.0.1/sqlrepo/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-1.0.1/sqlrepo/.pytest_cache/README.md
+-rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-1.0.1/sqlrepo/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-1.0.1/sqlrepo/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-1.0.1/sqlrepo/__init__.py
+-rw-r--r--   0        0        0      491 2024-04-15 09:17:35.411159 sqlrepo-1.0.1/sqlrepo/exc.py
+-rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-1.0.1/sqlrepo/logging.py
+-rw-r--r--   0        0        0    27442 2024-04-15 09:18:27.514734 sqlrepo-1.0.1/sqlrepo/queries.py
+-rw-r--r--   0        0        0    22014 2024-04-15 10:24:33.503572 sqlrepo-1.0.1/sqlrepo/repositories.py
+-rw-r--r--   0        0        0     3556 2024-04-15 11:35:37.037570 sqlrepo-1.0.1/sqlrepo/uow.py
+-rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     6707 2024-04-15 06:16:49.990950 sqlrepo-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0    15461 2024-04-15 06:16:49.990950 sqlrepo-1.0.1/tests/test_base_queries.py
+-rw-r--r--   0        0        0     9417 2024-04-15 06:16:49.990950 sqlrepo-1.0.1/tests/test_sync_queries.py
+-rw-r--r--   0        0        0        0 2024-04-05 11:56:33.229687 sqlrepo-1.0.1/tests/test_uow.py
+-rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-1.0.1/tests/types.py
+-rw-r--r--   0        0        0     7107 2024-04-15 06:16:49.991950 sqlrepo-1.0.1/tests/utils.py
+-rw-r--r--   0        0        0     7890 1970-01-01 00:00:00.000000 sqlrepo-1.0.1/PKG-INFO
```

### Comparing `sqlrepo-0.2.0/pyproject.toml` & `sqlrepo-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -170,24 +170,24 @@
     "httpx>=0.27.0",
     "pyment>=0.3.3",
     "ipython>=8.19.0",
 ]
 
 [project]
 name = "sqlrepo"
-version = "0.2.0"
+version = "1.0.1"
 description = "sqlalchemy repositories with crud operations and other utils for it."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = [
     "sqlalchemy>=2.0.29",
-    "python-dev-utils[sqlalchemy_filters]>=1.0.6",
+    "python-dev-utils[sqlalchemy_filters]>=1.1.0",
 ]
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
```

### Comparing `sqlrepo-0.2.0/sqlrepo/logging.py` & `sqlrepo-1.0.1/sqlrepo/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Logging configuration for sqlrepo project."""
+
 import logging
 import logging.config
 
 LOGGER_CONFIG = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
```

### Comparing `sqlrepo-0.2.0/sqlrepo/queries.py` & `sqlrepo-1.0.1/sqlrepo/queries.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+"""Queries classes with executable statements and methods with them."""
+
 import datetime
 import re
 from collections.abc import Callable
 from typing import TYPE_CHECKING, Any, Literal, NotRequired, TypedDict, TypeVar
 
 from dev_utils.sqlalchemy.filters.converters import BaseFilterConverter  # type: ignore
 from dev_utils.sqlalchemy.utils import (  # type: ignore
     apply_joins,
     apply_loads,
     get_sqlalchemy_attribute,
     get_utc_now,
 )
-from sqlalchemy import CursorResult, and_, delete
+from sqlalchemy import CursorResult, and_, delete, func, or_, select, text, update
 from sqlalchemy import exc as sqlalchemy_exc
-from sqlalchemy import func, or_, select, text, update
 from sqlalchemy.orm import joinedload
 
 from sqlrepo.logging import logger as default_logger
 
 
 class JoinKwargs(TypedDict):
     """Kwargs for join statement."""
@@ -325,14 +326,15 @@
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         filters: "Filter | None" = None,
         joins: "Sequence[Join] | None" = None,
         loads: "Sequence[Load] | None" = None,
     ) -> "BaseSQLAlchemyModel | None":
+        """Get one instance of model by given filters."""
         stmt = self._get_item_stmt(
             model=model,
             filters=filters,
             joins=joins,
             loads=loads,
         )
         result = self.session.scalars(stmt)
@@ -341,14 +343,15 @@
     def get_items_count(
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         joins: "Sequence[Join] | None" = None,
         filters: "Filter | None" = None,
     ) -> int:
+        """Get count of instances of model by given filters."""
         stmt = self._get_items_count_stmt(
             model=model,
             joins=joins,
             filters=filters,
         )
         count = self.session.scalar(stmt)
         # NOTE: code block for sure.
@@ -366,14 +369,15 @@
         search: str | None = None,
         search_by: "Sequence[SearchParam] | None" = None,
         order_by: "Sequence[OrderByParam] | None" = None,
         limit: int | None = None,
         offset: int | None = None,
         unique_items: bool = False,
     ) -> "Sequence[BaseSQLAlchemyModel]":
+        """Get list of instances of model."""
         stmt = self._get_item_list_stmt(
             model=model,
             joins=joins,
             loads=loads,
             filters=filters,
             search=search,
             search_by=search_by,
@@ -390,14 +394,15 @@
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         # TODO: add sequence of data to make more than one object at the same time.
         data: "DataDict | None" = None,
         use_flush: bool = False,
     ) -> "BaseSQLAlchemyModel":
+        """Create model instance from given data."""
         item = model() if data is None else model(**data)
         self.session.add(item)
         if use_flush:
             self.session.flush()
         else:
             self.session.commit()
 
@@ -412,14 +417,15 @@
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         data: "DataDict",
         filters: "Filter | None" = None,
         use_flush: bool = False,
     ) -> "Sequence[BaseSQLAlchemyModel]":
+        """Update model from given data."""
         stmt = self._db_update_stmt(
             model=model,
             data=data,
             filters=filters,
         )
         result = self.session.scalars(stmt)
         if use_flush:
@@ -434,14 +440,18 @@
         data: "DataDict",
         # TODO: add sequence items to make more than one object update at the same time.
         item: "BaseSQLAlchemyModel",
         set_none: bool = False,
         allowed_none_fields: 'Literal["*"] | set[str]' = "*",
         use_flush: bool = False,
     ) -> "tuple[Updated, BaseSQLAlchemyModel]":
+        """Update model instance from given data.
+
+        Returns tuple with boolean (was instance updated or not) and updated instance.
+        """
         is_updated = False
         if not set_none:
             data = {key: value for key, value in data.items() if value is not None}
         for field, value in data.items():
             if (
                 set_none
                 and value is None
@@ -465,14 +475,15 @@
     def db_delete(
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         filters: "Filter | None" = None,
         use_flush: bool = False,
     ) -> "Count":
+        """Delete model in db by given filters."""
         stmt = self._db_delete_stmt(
             model=model,
             filters=filters,
         )
         result = self.session.execute(stmt)
         if use_flush:
             self.session.flush()
@@ -484,14 +495,15 @@
 
     def delete_item(
         self,
         *,
         item: "Base",
         use_flush: bool = False,
     ) -> "Deleted":
+        """Delete model_class instance."""
         item_repr = repr(item)
         try:
             self.session.delete(item)
             if use_flush:
                 self.session.flush()
             else:
                 self.session.commit()
@@ -512,14 +524,15 @@
         id_field: "InstrumentedAttribute[Any]",
         disable_field: "InstrumentedAttribute[Any]",
         field_type: type[datetime.datetime] | type[bool] = datetime.datetime,
         allow_filter_by_value: bool = True,
         extra_filters: "Filter | None" = None,
         use_flush: bool = False,
     ) -> "Count":
+        """Disable model instances with given ids and extra_filters."""
         stmt = self._disable_items_stmt(
             model=model,
             ids_to_disable=ids_to_disable,
             id_field=id_field,
             disable_field=disable_field,
             field_type=field_type,
             allow_filter_by_value=allow_filter_by_value,
@@ -555,14 +568,15 @@
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         filters: "Filter | None" = None,
         joins: "Sequence[Join] | None" = None,
         loads: "Sequence[Load] | None" = None,
     ) -> "BaseSQLAlchemyModel | None":
+        """Get one instance of model by given filters."""
         stmt = self._get_item_stmt(
             model=model,
             filters=filters,
             joins=joins,
             loads=loads,
         )
         result = await self.session.scalars(stmt)
@@ -571,14 +585,15 @@
     async def get_items_count(
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         joins: "Sequence[Join] | None" = None,
         filters: "Filter | None" = None,
     ) -> int:
+        """Get count of instances of model by given filters."""
         stmt = self._get_items_count_stmt(
             model=model,
             joins=joins,
             filters=filters,
         )
         count = await self.session.scalar(stmt)
         # NOTE: code block for sure.
@@ -596,14 +611,15 @@
         search: str | None = None,
         search_by: "Sequence[SearchParam] | None" = None,
         order_by: "Sequence[OrderByParam] | None" = None,
         limit: int | None = None,
         offset: int | None = None,
         unique_items: bool = False,
     ) -> "Sequence[BaseSQLAlchemyModel]":
+        """Get list of instances of model."""
         stmt = self._get_item_list_stmt(
             model=model,
             joins=joins,
             loads=loads,
             filters=filters,
             search=search,
             search_by=search_by,
@@ -619,14 +635,15 @@
     async def create_item(
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         data: "DataDict | None" = None,
         use_flush: bool = False,
     ) -> "BaseSQLAlchemyModel":
+        """Create model instance from given data."""
         item = model() if data is None else model(**data)
         self.session.add(item)
         if use_flush:
             await self.session.flush()
         else:
             await self.session.commit()
 
@@ -641,14 +658,15 @@
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         data: "DataDict",
         filters: "Filter | None" = None,
         use_flush: bool = False,
     ) -> "Sequence[BaseSQLAlchemyModel] | None":
+        """Update model from given data."""
         stmt = self._db_update_stmt(
             model=model,
             data=data,
             filters=filters,
         )
         result = await self.session.scalars(stmt)
         if use_flush:
@@ -662,14 +680,18 @@
         *,
         data: "DataDict",
         item: "BaseSQLAlchemyModel",
         set_none: bool = False,
         allowed_none_fields: 'Literal["*"] | set[str]' = "*",
         use_flush: bool = False,
     ) -> "tuple[bool, BaseSQLAlchemyModel]":
+        """Update model instance from given data.
+
+        Returns tuple with boolean (was instance updated or not) and updated instance.
+        """
         is_updated = False
         if not set_none:
             data = {key: value for key, value in data.items() if value is not None}
         for field, value in data.items():
             if (
                 set_none
                 and value is None
@@ -693,14 +715,15 @@
     async def db_delete(
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         filters: "Filter | None" = None,
         use_flush: bool = False,
     ) -> "Count":
+        """Delete model in db by given filters."""
         stmt = self._db_delete_stmt(
             model=model,
             filters=filters,
         )
         result = await self.session.execute(stmt)
         if use_flush:
             await self.session.flush()
@@ -712,14 +735,15 @@
 
     async def delete_item(
         self,
         *,
         item: "Base",
         use_flush: bool = False,
     ) -> "Deleted":
+        """Delete model_class instance."""
         item_repr = repr(item)
         try:
             await self.session.delete(item)
             if use_flush:
                 await self.session.flush()
             else:
                 await self.session.commit()
@@ -740,14 +764,15 @@
         id_field: "InstrumentedAttribute[Any]",
         disable_field: "InstrumentedAttribute[Any]",
         field_type: type[datetime.datetime] | type[bool] = datetime.datetime,
         allow_filter_by_value: bool = True,
         extra_filters: "Filter | None" = None,
         use_flush: bool = False,
     ) -> "Count":
+        """Disable model instances with given ids and extra_filters."""
         stmt = self._disable_items_stmt(
             model=model,
             ids_to_disable=ids_to_disable,
             id_field=id_field,
             disable_field=disable_field,
             field_type=field_type,
             allow_filter_by_value=allow_filter_by_value,
```

### Comparing `sqlrepo-0.2.0/sqlrepo/repositories.py` & `sqlrepo-1.0.1/sqlrepo/repositories.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Main implementations for sqlrepo project."""
+
 import datetime
 import warnings
 from collections.abc import Callable
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
@@ -19,15 +21,15 @@
     AdvancedOperatorFilterConverter,
     BaseFilterConverter,
     DjangoLikeFilterConverter,
     SimpleFilterConverter,
 )
 from dev_utils.sqlalchemy.filters.types import FilterConverterStrategiesLiteral  # type: ignore
 from sqlalchemy.orm import DeclarativeBase as Base
-from sqlalchemy.orm import joinedload
+from sqlalchemy.orm import selectinload
 
 from sqlrepo import exc as sqlrepo_exc
 from sqlrepo.logging import logger as default_logger
 from sqlrepo.queries import BaseAsyncQuery, BaseSyncQuery
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
@@ -43,14 +45,15 @@
     class JoinKwargs(TypedDict):
         """Kwargs for join."""
 
         isouter: NotRequired[bool]
         full: NotRequired[bool]
 
     Count = int
+    Deleted = bool
     Model = type[Base]
     JoinClause = ColumnElement[bool]
     ModelWithOnclause = tuple[Model, JoinClause]
     CompleteModel = tuple[Model, JoinClause, JoinKwargs]
     Join = str | Model | ModelWithOnclause | CompleteModel
     Filter = dict[str, Any] | Sequence[dict[str, Any] | ColumnElement[bool]] | ColumnElement[bool]
     Load = str | _AbstractLoad
@@ -67,19 +70,45 @@
     """Base repository class.
 
     Don't Use it directly. Use BaseAsyncRepository and BaseSyncRepository, or pass query_class
     directly (not recommended.)
     """
 
     __inheritance_check_model_class__: bool = True
-    _model_class: type["BaseSQLAlchemyModel"]
+    """
+    Private custom magic property.
+
+    Use it, if you want to inherit Repository without checking model_class attribute.
+    """
+
+    model_class: type["BaseSQLAlchemyModel"]
+    """
+    Model class for repository.
+
+    You can set this option manually, but it is not recommended. Repository will automatically
+    add model_class attribute by extracting it from Generic type.
 
-    # TODO: добавить specific_column_mapping в фильтры, joins и loads.
+    Use case:
+
+    ```
+    from my_package.models import Admin
+
+    class AdminRepository(BaseSyncRepository[Admin]):
+        pass
+
+    # So, when you will use AdminRepository, model_class attribute will be set with Admin
+    # automatically.
+    ```
+    """
+
+    # TODO: add specific_column_mapping to filters, joins and loads.
     specific_column_mapping: ClassVar["dict[str, ColumnElement[Any]]"] = {}
     """
+    Warning! Current version of sqlrepo doesn't support this mapping for filters, joins and loads.
+
     Uses as mapping for some attributes, that you need to alias or need to specify column
     from other models.
 
     Warning: if you specify column from other model, it may cause errors. For example, update
     doesn't use it for filters, because joins are not presents in update.
     """
     use_flush: ClassVar[bool] = True
@@ -89,48 +118,139 @@
     By default, True, because repository has (mostly) multiple methods evaluate use. For example,
     generally, you want to create some model instances, create some other (for example, log table)
     and then receive other model instance in one use (for example, in Unit of work pattern).
 
     If you will work with repositories as single methods uses, switch to use_flush=False. It will
     make queries commit any changes.
     """
+    update_set_none: ClassVar[bool] = False
+    """
+    Uses as flag of set None option in ``update_instance`` method.
+
+    If True, allow to force ``update_instance`` instance columns with None value. Works together
+    with ``update_allowed_none_fields``.
+
+    By default False, because it's not safe to set column to None - current version if sqlrepo
+    not able to check optional type. Will be added in next versions, and ``then update_set_none``
+    will be not necessary.
+    """
+    update_allowed_none_fields: ClassVar['Literal["*"] | set[StrField]'] = "*"
+    """
+    Set of strings, which represents columns of model.
+
+    Uses as include or exclude for given data in ``update_instance`` method.
+
+    By default allow any fields. Not dangerous, because ``update_set_none`` by default set to False,
+    and there will be no affect on ``update_instance`` method
+    """
     allow_disable_filter_by_value: ClassVar[bool] = True
     """
     Uses as flag of filtering in disable method.
 
     If True, make additional filter, which will exclude items, which already disabled.
     Logic of disable depends on type of disable column. See ``disable_field`` docstring for more
     information.
 
     By default True, because it will make more efficient query to not override disable column. In
     some cases (like datetime disable field) it may be better to turn off this flag to save disable
     with new context (repeat disable, if your domain supports repeat disable and it make sense).
     """
-    update_set_none: ClassVar[bool] = False
-    update_allowed_none_fields: ClassVar['Literal["*"] | set[StrField]'] = "*"
-    disable_field_type: ClassVar[type[datetime.datetime] | type[bool]] = datetime.datetime
-    unique_list_items: ClassVar[bool] = False
-    filter_convert_strategy: ClassVar[FilterConverterStrategiesLiteral] = "simple"
-    load_strategy: ClassVar[Callable[..., "_AbstractLoad"]] = joinedload
-    id_field: ClassVar["InstrumentedAttribute[Any] | None"] = None
+    disable_field_type: ClassVar[type[datetime.datetime] | type[bool] | None] = None
+    """
+    Uses as choice of type of disable field.
+
+    By default, None. Needs to be set manually, because this option depends on user custom
+    implementation of disable_field. If None and ``disable`` method was evaluated, there will be
+    RepositoryAttributeError exception raised by Repository class.
+    """
     disable_field: ClassVar["InstrumentedAttribute[Any] | None"] = None
+    """
+    Uses as choice of used defined disable field.
+
+    By default, None. Needs to be set manually, because this option depends on user custom
+    implementation of disable_field. If None and ``disable`` method was evaluated, there will be
+    RepositoryAttributeError exception raised by Repository class.
+    """
+    disable_id_field: ClassVar["InstrumentedAttribute[Any] | None"] = None
+    """
+    Uses as choice of used defined id field in model, which supports disable.
+
+    By default, None. Needs to be set manually, because this option depends on user custom
+    implementation of disable_field. If None and ``disable`` method was evaluated, there will be
+    RepositoryAttributeError exception raised by Repository class.
+    """
+    unique_list_items: ClassVar[bool] = True
+    """
+    Warning! Ambiguous option!
+    ==========================
+
+    Current version of ``sqlrepo`` works with load strategies with user configured option
+    ``load_strategy``. In order to make ``list`` method works stable, this option is used.
+    If you don't work with relationships in your model or you don't need unique (for example,
+    if you use selectinload), set this option to False. Otherwise keep it in True state.
+    """
+    filter_convert_strategy: ClassVar[FilterConverterStrategiesLiteral] = "simple"
+    """
+    Uses as choice of filter convert.
+
+    By default "simple", so you able to pass filters with ``key-value`` structure. You still can
+    pass raw filters (just list of SQLAlchemy filters), but if you pass dict, it will be converted
+    to SQLAlchemy filters with passed strategy.
+
+    Currently, supported converters:
+
+        ``simple`` - ``key-value`` dict.
+
+        ``advanced`` - dict with ``field``, ``value`` and ``operator`` keys.
+        List of operators:
+
+            ``=, >, <, >=, <=, is, is_not, between, contains``
+
+        ``django-like`` - ``key-value`` dict with django-like lookups system. See django docs for
+        more info.
+    """
+    load_strategy: ClassVar[Callable[..., "_AbstractLoad"]] = selectinload
+    """
+    Uses as choice of SQLAlchemy load strategies.
+
+    By default selectinload, because it makes less errors.
+    """
 
     _filter_convert_classes: Final[
         dict[FilterConverterStrategiesLiteral, type[BaseFilterConverter]]
     ] = {
         "simple": SimpleFilterConverter,
         "advanced": AdvancedOperatorFilterConverter,
         "django": DjangoLikeFilterConverter,
     }
+    """
+    Final convert class filters mapping.
+
+    Don't override it, because it can makes unexpected errors.
+    """
+
+    @classmethod
+    def _validate_disable_attributes(cls) -> None:
+        if (
+            cls.disable_id_field is None
+            or cls.disable_field is None
+            or cls.disable_field_type is None
+        ):
+            msg = (
+                'Attribute "disable_id_field" or "disable_field" or "disable_field_type" not '
+                "set in your repository class. Can't disable entities."
+            )
+            raise sqlrepo_exc.RepositoryAttributeError(msg)
 
     def __init_subclass__(cls) -> None:  # noqa: D105
-        if hasattr(cls, "_model_class"):
+        if hasattr(cls, "model_class"):
             msg = (
-                "Don't change _model_class attribute to class. Use generic syntax instead. "
-                "See PEP 646 (https://peps.python.org/pep-0646/)"
+                "Don't change model_class attribute to class. Use generic syntax instead. "
+                "See PEP 646 (https://peps.python.org/pep-0646/). Repository will automatically "
+                "add model_class attribute by extracting it from Generic type."
             )
             warnings.warn(msg, stacklevel=2)
             return
         if cls.__inheritance_check_model_class__ is False:
             cls.__inheritance_check_model_class__ = True
             return
         try:
@@ -156,15 +276,15 @@
             msg = "GenericType was not passed for SQLAlchemy model declarative class."
             warnings.warn(msg, stacklevel=2)
             return
         if not issubclass(model, Base):
             msg = "Passed GenericType is not SQLAlchemy model declarative class."
             warnings.warn(msg, stacklevel=2)
             return
-        cls._model_class = model  # type: ignore
+        cls.model_class = model  # type: ignore
 
     def get_filter_convert_class(self) -> type[BaseFilterConverter]:
         """Get filter convert class from passed strategy."""
         return self._filter_convert_classes[self.filter_convert_strategy]
 
 
 class BaseAsyncRepository(BaseRepository[BaseSQLAlchemyModel]):
@@ -189,126 +309,156 @@
             self.get_filter_convert_class(),
             self.specific_column_mapping,
             self.load_strategy,
         )
 
     async def get(
         self,
+        filters: "Filter",
         *,
-        filters: "Filter | None" = None,
         joins: "Sequence[Join] | None" = None,
         loads: "Sequence[Load] | None" = None,
     ) -> "BaseSQLAlchemyModel | None":
+        """Get one instance of model_class by given filters."""
         result = await self.queries.get_item(
-            model=self._model_class,
+            model=self.model_class,
             joins=joins,
             loads=loads,
             filters=filters,
         )
         return result
 
     async def count(
         self,
         *,
-        joins: "Sequence[Join] | None" = None,
         filters: "Filter | None" = None,
+        joins: "Sequence[Join] | None" = None,
     ) -> int:
+        """Get count of instances of model_class by given filters."""
         result = await self.queries.get_items_count(
-            model=self._model_class,
+            model=self.model_class,
             joins=joins,
             filters=filters,
         )
         return result
 
     async def list(  # noqa: A003
         self,
         *,
         # TODO: улучшить интерфейс, чтобы можно было принимать как 1 элемент, так и несколько
+        filters: "Filter | None" = None,
         joins: "Sequence[Join] | None" = None,
         loads: "Sequence[Load] | None" = None,
-        filters: "Filter | None" = None,
         search: str | None = None,
         search_by: "Sequence[SearchParam] | None" = None,
         order_by: "Sequence[OrderByParam] | None" = None,
         limit: int | None = None,
         offset: int | None = None,
     ) -> "Sequence[BaseSQLAlchemyModel]":
+        """Get list of instances of model_class."""
         result = await self.queries.get_item_list(
-            model=self._model_class,
+            model=self.model_class,
             joins=joins,
             loads=loads,
             filters=filters,
             search=search,
             search_by=search_by,
             order_by=order_by,
             limit=limit,
             offset=offset,
             unique_items=self.unique_list_items,
         )
         return result
 
+    # TODO: def create - insert stmt execute
+
     async def create_instance(
         self,
-        *,
         data: "DataDict | None" = None,
     ) -> "BaseSQLAlchemyModel":
+        """Create model_class instance from given data."""
         result = await self.queries.create_item(
-            model=self._model_class,
+            model=self.model_class,
             data=data,
             use_flush=self.use_flush,
         )
         return result
 
     async def update(
         self,
         *,
         data: "DataDict",
         filters: "Filter | None" = None,
     ) -> "Sequence[BaseSQLAlchemyModel] | None":
+        """Update model_class from given data."""
         result = await self.queries.db_update(
-            model=self._model_class,
+            model=self.model_class,
             data=data,
             filters=filters,
             use_flush=self.use_flush,
         )
         return result
 
     async def update_instance(
         self,
         *,
         instance: "BaseSQLAlchemyModel",
         data: "DataDict",
     ) -> "tuple[bool, BaseSQLAlchemyModel]":
+        """Update model_class instance from given data.
+
+        Returns tuple with boolean (was instance updated or not) and updated instance.
+        """
         result = await self.queries.change_item(
             data=data,
             item=instance,
             set_none=self.update_set_none,
             allowed_none_fields=self.update_allowed_none_fields,
             use_flush=self.use_flush,
         )
         return result
 
+    async def delete(
+        self,
+        filters: "Filter | None" = None,
+    ) -> "Count":
+        """Delete model_class in db by given filters."""
+        result = await self.queries.db_delete(
+            model=self.model_class,
+            filters=filters,
+            use_flush=self.use_flush,
+        )
+        return result
+
+    async def delete_item(
+        self,
+        *,
+        instance: "BaseSQLAlchemyModel",
+    ) -> "Deleted":
+        """Delete model_class instance."""
+        result = await self.queries.delete_item(
+            item=instance,
+            use_flush=self.use_flush,
+        )
+        return result
+
     async def disable(
         self,
         *,
         ids_to_disable: set[Any],
         extra_filters: "Filter | None" = None,
     ) -> "Count":
-        if self.id_field is None or self.disable_field is None:
-            msg = (
-                'Attribute "id_field" or "disable_field" not set in your repository class. '
-                "Can't disable entities."
-            )
-            raise sqlrepo_exc.RepositoryAttributeError(msg)
+        """Disable model_class instances with given ids and extra_filters."""
+        self._validate_disable_attributes()
         result = await self.queries.disable_items(
-            model=self._model_class,
+            model=self.model_class,
             ids_to_disable=ids_to_disable,
-            id_field=self.id_field,
-            disable_field=self.disable_field,
-            field_type=self.disable_field_type,
+            id_field=self.disable_id_field,  # type: ignore
+            disable_field=self.disable_field,  # type: ignore
+            field_type=self.disable_field_type,  # type: ignore
             allow_filter_by_value=self.allow_disable_filter_by_value,
             extra_filters=extra_filters,
             use_flush=self.use_flush,
         )
         return result
 
 
@@ -332,35 +482,37 @@
             self.get_filter_convert_class(),
             self.specific_column_mapping,
             self.load_strategy,
         )
 
     def get(
         self,
+        filters: "Filter",
         *,
-        filters: "Filter | None" = None,
         joins: "Sequence[Join] | None" = None,
         loads: "Sequence[Load] | None" = None,
     ) -> "BaseSQLAlchemyModel | None":
+        """Get one instance of model_class by given filters."""
         result = self.queries.get_item(
-            model=self._model_class,
+            model=self.model_class,
             joins=joins,
             loads=loads,
             filters=filters,
         )
         return result
 
     def count(
         self,
         *,
         joins: "Sequence[Join] | None" = None,
         filters: "Filter | None" = None,
     ) -> int:
+        """Get count of instances of model_class by given filters."""
         result = self.queries.get_items_count(
-            model=self._model_class,
+            model=self.model_class,
             joins=joins,
             filters=filters,
         )
         return result
 
     async def list(  # noqa: A003
         self,
@@ -371,85 +523,113 @@
         filters: "Filter | None" = None,
         search: str | None = None,
         search_by: "Sequence[SearchParam] | None" = None,
         order_by: "Sequence[OrderByParam] | None" = None,
         limit: int | None = None,
         offset: int | None = None,
     ) -> "Sequence[BaseSQLAlchemyModel]":
+        """Get list of instances of model_class."""
         result = self.queries.get_item_list(
-            model=self._model_class,
+            model=self.model_class,
             joins=joins,
             loads=loads,
             filters=filters,
             search=search,
             search_by=search_by,
             order_by=order_by,
             limit=limit,
             offset=offset,
             unique_items=self.unique_list_items,
         )
         return result
 
+    # TODO: async def create - insert stmt execute
+
     async def create_instance(
         self,
         *,
         data: "DataDict | None" = None,
     ) -> "BaseSQLAlchemyModel":
+        """Create model_class instance from given data."""
         result = self.queries.create_item(
-            model=self._model_class,
+            model=self.model_class,
             data=data,
             use_flush=self.use_flush,
         )
         return result
 
     async def update(
         self,
         *,
         data: "DataDict",
         filters: "Filter | None" = None,
     ) -> "Sequence[BaseSQLAlchemyModel] | None":
+        """Update model_class from given data."""
         result = self.queries.db_update(
-            model=self._model_class,
+            model=self.model_class,
             data=data,
             filters=filters,
             use_flush=self.use_flush,
         )
         return result
 
     def update_instance(
         self,
         *,
         instance: "BaseSQLAlchemyModel",
         data: "DataDict",
     ) -> "tuple[bool, BaseSQLAlchemyModel]":
+        """Update model_class instance from given data.
+
+        Returns tuple with boolean (was instance updated or not) and updated instance.
+        """
         result = self.queries.change_item(
             data=data,
             item=instance,
             set_none=self.update_set_none,
             allowed_none_fields=self.update_allowed_none_fields,
             use_flush=self.use_flush,
         )
         return result
 
+    def delete(
+        self,
+        filters: "Filter | None" = None,
+    ) -> "Count":
+        """Delete model_class in db by given filters."""
+        result = self.queries.db_delete(
+            model=self.model_class,
+            filters=filters,
+            use_flush=self.use_flush,
+        )
+        return result
+
+    def delete_item(
+        self,
+        *,
+        instance: "BaseSQLAlchemyModel",
+    ) -> "Deleted":
+        """Delete model_class instance."""
+        result = self.queries.delete_item(
+            item=instance,
+            use_flush=self.use_flush,
+        )
+        return result
+
     def disable(
         self,
         *,
         ids_to_disable: set[Any],
         extra_filters: "Filter | None" = None,
     ) -> "Count":
-        if self.id_field is None or self.disable_field is None:
-            msg = (
-                'Attribute "id_field" or "disable_field" not set in your repository class. '
-                "Can't disable entities."
-            )
-            raise sqlrepo_exc.RepositoryAttributeError(msg)
+        """Disable model_class instances with given ids and extra_filters."""
         result = self.queries.disable_items(
-            model=self._model_class,
+            model=self.model_class,
             ids_to_disable=ids_to_disable,
-            id_field=self.id_field,
-            disable_field=self.disable_field,
-            field_type=self.disable_field_type,
+            id_field=self.disable_id_field,  # type: ignore
+            disable_field=self.disable_field,  # type: ignore
+            field_type=self.disable_field_type,  # type: ignore
             allow_filter_by_value=self.allow_disable_filter_by_value,
             extra_filters=extra_filters,
             use_flush=self.use_flush,
         )
         return result
```

### Comparing `sqlrepo-0.2.0/tests/conftest.py` & `sqlrepo-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-0.2.0/tests/test_base_queries.py` & `sqlrepo-1.0.1/tests/test_base_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-0.2.0/tests/test_sync_queries.py` & `sqlrepo-1.0.1/tests/test_sync_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-0.2.0/tests/types.py` & `sqlrepo-1.0.1/tests/types.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-0.2.0/tests/utils.py` & `sqlrepo-1.0.1/tests/utils.py`

 * *Files identical despite different names*

