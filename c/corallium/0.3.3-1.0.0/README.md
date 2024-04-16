# Comparing `tmp/corallium-0.3.3.tar.gz` & `tmp/corallium-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corallium-0.3.3.tar", max compression
+gzip compressed data, was "corallium-1.0.0.tar", max compression
```

## Comparing `corallium-0.3.3.tar` & `corallium-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2023-08-14 01:24:52.139328 corallium-0.3.3/LICENSE
--rw-r--r--   0        0        0     1788 2023-08-14 01:26:34.906733 corallium-0.3.3/corallium/__init__.py
--rw-r--r--   0        0        0     8668 2023-08-13 13:46:16.076509 corallium-0.3.3/corallium/file_helpers.py
--rw-r--r--   0        0        0     3671 2023-02-25 15:48:42.282044 corallium-0.3.3/corallium/log.py
--rw-r--r--   0        0        0        0 2023-02-23 12:18:48.616595 corallium-0.3.3/corallium/loggers/__init__.py
--rw-r--r--   0        0        0      494 2023-06-21 07:55:37.168870 corallium-0.3.3/corallium/loggers/plain_printer.py
--rw-r--r--   0        0        0     2123 2023-08-13 02:56:57.602580 corallium-0.3.3/corallium/loggers/rich_printer.py
--rw-r--r--   0        0        0      274 2023-04-22 04:52:34.549543 corallium-0.3.3/corallium/loggers/structlog_logger/__init__.py
--rw-r--r--   0        0        0      758 2023-04-22 04:57:25.576582 corallium-0.3.3/corallium/loggers/structlog_logger/_structlog_logger.py
--rw-r--r--   0        0        0     2108 2023-08-13 13:16:01.382681 corallium-0.3.3/corallium/loggers/styles.py
--rw-r--r--   0        0        0     4486 2023-06-17 12:19:52.231514 corallium-0.3.3/corallium/pretty_process.py
--rw-r--r--   0        0        0     3798 2023-08-13 03:12:00.101052 corallium-0.3.3/corallium/shell.py
--rw-r--r--   0        0        0      192 2023-02-22 03:38:37.960591 corallium-0.3.3/corallium/tomllib.py
--rw-r--r--   0        0        0     2833 2023-08-14 01:26:39.428419 corallium-0.3.3/docs/README.md
--rw-r--r--   0        0        0     1617 2023-08-14 01:26:34.916151 corallium-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3969 1970-01-01 00:00:00.000000 corallium-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-16 12:38:46.672808 corallium-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1850 2024-04-16 12:55:16.353486 corallium-1.0.0/corallium/__init__.py
+-rw-r--r--   0        0        0     8684 2023-12-10 17:52:22.388535 corallium-1.0.0/corallium/file_helpers.py
+-rw-r--r--   0        0        0     3756 2023-12-10 17:52:47.559820 corallium-1.0.0/corallium/log.py
+-rw-r--r--   0        0        0        0 2023-02-23 12:18:48.616595 corallium-1.0.0/corallium/loggers/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-21 07:55:37.168870 corallium-1.0.0/corallium/loggers/plain_printer.py
+-rw-r--r--   0        0        0     2114 2023-12-10 16:26:52.360419 corallium-1.0.0/corallium/loggers/rich_printer.py
+-rw-r--r--   0        0        0      274 2023-04-22 04:52:34.549543 corallium-1.0.0/corallium/loggers/structlog_logger/__init__.py
+-rw-r--r--   0        0        0      758 2023-04-22 04:57:25.576582 corallium-1.0.0/corallium/loggers/structlog_logger/_structlog_logger.py
+-rw-r--r--   0        0        0     2094 2023-09-12 23:27:54.142142 corallium-1.0.0/corallium/loggers/styles.py
+-rw-r--r--   0        0        0     4234 2023-12-10 17:57:10.741345 corallium-1.0.0/corallium/pretty_process.py
+-rw-r--r--   0        0        0     3749 2024-04-16 12:40:28.343049 corallium-1.0.0/corallium/shell.py
+-rw-r--r--   0        0        0      218 2023-12-10 17:58:03.509787 corallium-1.0.0/corallium/tomllib.py
+-rw-r--r--   0        0        0     2833 2024-04-16 12:55:20.846119 corallium-1.0.0/docs/README.md
+-rw-r--r--   0        0        0     1677 2024-04-16 12:55:16.369150 corallium-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 corallium-1.0.0/PKG-INFO
```

### Comparing `corallium-0.3.3/LICENSE` & `corallium-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corallium-0.3.3/corallium/__init__.py` & `corallium-1.0.0/corallium/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,52 +4,52 @@
 from enum import Enum
 from os import getenv
 from warnings import filterwarnings
 
 from beartype import BeartypeConf
 from beartype.claw import beartype_this_package
 from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
-from typing_extensions import Self  # noqa: UP035
+from typing_extensions import Self
 
-__version__ = '0.3.3'
+__version__ = '1.0.0'
 __pkg_name__ = 'corallium'
 
 
 class _RuntimeTypeCheckingModes(Enum):
     """Supported global runtime type checking modes."""
 
     ERROR = 'ERROR'
     WARNING = 'WARNING'
     OFF = None
 
     @classmethod
-    def from_environment(cls) -> Self:
+    def from_environment(cls) -> Self:  # pragma: no cover
         """Return the configured mode."""
         rtc_mode = getenv('RUNTIME_TYPE_CHECKING_MODE') or None
         try:
             return cls(rtc_mode)
         except ValueError:
             modes = [_e.value for _e in cls]
             msg = f"'RUNTIME_TYPE_CHECKING_MODE={rtc_mode}' is not an allowed mode from {modes}"
             raise ValueError(msg) from None
 
 
-def configure_runtime_type_checking_mode() -> None:
+def configure_runtime_type_checking_mode() -> None:  # pragma: no cover
     """Optionally configure runtime type checking mode globally."""
     rtc_mode = _RuntimeTypeCheckingModes.from_environment()
 
     if rtc_mode is not _RuntimeTypeCheckingModes.OFF:
-        from beartype.roar import BeartypeClawDecorWarning
+        from beartype.roar import BeartypeClawDecorWarning  # noqa: PLC0415
 
         beartype_this_package(conf=BeartypeConf(
             warning_cls_on_decorator_exception=(
                 None if rtc_mode is _RuntimeTypeCheckingModes.ERROR else BeartypeClawDecorWarning
             ),
         ))
 
 
 _PEP585_DATE = 2025
-if datetime.now(tz=timezone.utc).year <= _PEP585_DATE:
+if datetime.now(tz=timezone.utc).year <= _PEP585_DATE:  # pragma: no cover
     filterwarnings('ignore', category=BeartypeDecorHintPep585DeprecationWarning)
 configure_runtime_type_checking_mode()
 
 # ====== Above is the recommended code from calcipy_template and may be updated on new releases ======
```

### Comparing `corallium-0.3.3/corallium/file_helpers.py` & `corallium-1.0.0/corallium/file_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         path_yaml: path to the yaml file
 
     Returns:
         dictionary representation of the source file
 
     """
     try:
-        import yaml  # lazy-load the optional dependency
+        import yaml  # noqa: PLC0415 # lazy-load the optional dependency
     except ImportError as exc:
         raise RuntimeError("The 'calcipy[docs]' extras are missing") from exc
 
     # PLANNED: Refactor so that unsafe_load isn't necessary:
     #   read_text; remove any line containing ': !!python'; then yaml.loag
 
     # Based on: https://github.com/yaml/pyyaml/issues/86#issuecomment-380252434
```

### Comparing `corallium-0.3.3/corallium/log.py` & `corallium-1.0.0/corallium/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,31 +79,31 @@
 
     @beartype
     def text_debug(self, message: str, *, is_header: bool = False, **kwargs: Any) -> None:
         """Variation on text that will appear as a debug log if not supported."""
         self.debug(message, **{'_is_text': True, 'is_header': is_header, **kwargs})
 
     @beartype
-    def debug(self, message: str, **kwargs: Any) -> None:
+    def debug(self, message: str, **kwargs: Any) -> None:  # noqa: PLR6301
         _LOG_SINGLETON.log(message, _this_level=logging.DEBUG, **kwargs)
 
     @beartype
-    def info(self, message: str, **kwargs: Any) -> None:
+    def info(self, message: str, **kwargs: Any) -> None:  # noqa: PLR6301
         _LOG_SINGLETON.log(message, _this_level=logging.INFO, **kwargs)
 
     @beartype
-    def warning(self, message: str, **kwargs: Any) -> None:
+    def warning(self, message: str, **kwargs: Any) -> None:  # noqa: PLR6301
         _LOG_SINGLETON.log(message, _this_level=logging.WARNING, **kwargs)
 
     @beartype
-    def error(self, message: str, **kwargs: Any) -> None:
+    def error(self, message: str, **kwargs: Any) -> None:  # noqa: PLR6301
         _LOG_SINGLETON.log(message, _this_level=logging.ERROR, **kwargs)
 
     @beartype
-    def exception(self, message: str, **kwargs: Any) -> None:
+    def exception(self, message: str, **kwargs: Any) -> None:  # noqa: PLR6301
         _LOG_SINGLETON.log(message, _this_level=logging.CRITICAL, **kwargs)
 
 
 @beartype
 def configure_logger(*, log_level: int = DEF_LEVEL, logger: Optional[LogCallable] = None, **kwargs: Any) -> None:
     """Configure the global log level or replace the logger."""
     _LOG_SINGLETON.set_logger(logger=logger, log_level=log_level, **kwargs)
```

### Comparing `corallium-0.3.3/corallium/loggers/rich_printer.py` & `corallium-1.0.0/corallium/loggers/rich_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from rich.console import Console
 from rich.text import Text
 
 from .styles import Styles, get_name
 
 
 @beartype
-def rich_printer(  # noqa: CAC001,CFQ002
+def rich_printer(  # noqa: CAC001
     message: str,
     *,
     is_header: bool,
     _this_level: int,
     _is_text: bool,
     # Logger-specific parameters that need to be initialized with partial(...)
     _console: Console,
@@ -25,15 +25,15 @@
     _keys_on_own_line: Optional[List[str]] = None,
     **kwargs: Any,
 ) -> None:
     """Generic log writer.."""
     text = Text()
     if _is_text:
         if is_header:
-            print('')  # noqa: T201
+            print()  # noqa: T201
         text.append(f'{message}', style=_styles.message)
     else:
         timestamp = kwargs.pop('timestamp', datetime.now())  # noqa: DTZ005
         text.append(f'{timestamp: <28} ', style=_styles.timestamp)
         text.append('[', style=_styles.timestamp)
         level_style = _styles.get_style(level=_this_level)
         text.append(f'{get_name(level=_this_level): <7}', style=level_style)
```

### Comparing `corallium-0.3.3/corallium/loggers/structlog_logger/_structlog_logger.py` & `corallium-1.0.0/corallium/loggers/structlog_logger/_structlog_logger.py`

 * *Files identical despite different names*

### Comparing `corallium-0.3.3/corallium/loggers/styles.py` & `corallium-1.0.0/corallium/loggers/styles.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     https://rich.readthedocs.io/en/latest/style.html
 
     Inspired by: https://github.com/Delgan/loguru/blob/07f94f3c8373733119f85aa8b9ca05ace3325a4b/loguru/_defaults.py#L31-L73
 
     And: https://github.com/hynek/structlog/blob/bcfc7f9e60640c150bffbdaeed6328e582f93d1e/src/structlog/dev.py#L126-L141
 
-    """  # noqa: E501
+    """
 
     timestamp: str = '#8DAAA1'
     message: str = 'bold'
 
     # Tokyo Night: https://github.com/folke/tokyonight.nvim#-extras
     level_error: str = '#e77d8f'
     level_warn: str = '#d8b172'
```

### Comparing `corallium-0.3.3/corallium/pretty_process.py` & `corallium-1.0.0/corallium/pretty_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,53 +5,53 @@
 """
 
 import math
 import multiprocessing
 from concurrent.futures import ProcessPoolExecutor
 from multiprocessing.managers import DictProxy
 from time import sleep
-from typing import runtime_checkable
 
 from beartype import beartype
-from beartype.typing import Any, List, Protocol, TypeVar, Union
-from rich.progress import BarColumn, Progress, ProgressColumn, TimeElapsedColumn, TimeRemainingColumn
+from beartype.typing import Any, Callable, List, TypeVar, Union
+from rich.progress import BarColumn, Progress, ProgressColumn, TaskID, TimeElapsedColumn, TimeRemainingColumn
 
 _ItemT = TypeVar('_ItemT', bound=Any)
 """Iterated item in the data."""
 
 
-@runtime_checkable
-class _DelegatedTask(Protocol):
-    """Defined the kwargs accepted for a delegated task."""
-
-    def __call__(
-        self,
-        *,
-        task_id: int,
-        shared_progress: DictProxy,  # type: ignore[type-arg]
-        data: List[_ItemT],
-    ) -> Any:
-        ...
+_DelegatedTask = Callable[
+    [
+        TaskID,
+        DictProxy,  # type: ignore[type-arg]
+        list[_ItemT],
+    ],
+    Any,
+]
 
 
 @beartype
 def _chunked(data: List[_ItemT], count: int) -> List[List[_ItemT]]:
     """Chunk the list of data into equally sized lists."""
     # TODO: See below link for other options for chunking
     #   https://realpython.com/how-to-split-a-python-list-into-chunks/
     size = len(data)
-    chunk_size, chunk_rem = size // count, size % count  # noqa: S001
+    chunk_size, chunk_rem = size // count, size % count
     chunk_size += int(math.ceil(chunk_rem / size))
     return [
         data[ix:ix + chunk_size] for ix in range(0, size, chunk_size)
     ]
 
 
 @beartype
-def pretty_process(delegated_task: _DelegatedTask, *, data: List[_ItemT], num_workers: int = 3) -> Any:
+def pretty_process(
+    delegated_task: _DelegatedTask,  # type: ignore[type-arg]
+    *,
+    data: List[_ItemT],
+    num_workers: int = 3,
+) -> Any:
     """Run a task in parallel to process all provided data.
 
     Uses `rich` to display pretty progress bars
 
     Args:
         delegated_task: must call `shared_progress[task_id] += 1` on each item in data
         data: the list of data to distribute
@@ -75,17 +75,15 @@
             task_id_all = progress.add_task('[green]All jobs progress:')
 
             with ProcessPoolExecutor(max_workers=num_workers) as executor:
                 for ix, chunk in enumerate(_chunked(data, count=num_cpus)):
                     task_id = progress.add_task(f'task {ix}')
                     shared_progress[task_id] = 0
                     totals[task_id] = len(chunk)
-                    jobs.append(executor.submit(
-                        delegated_task, task_id=task_id, shared_progress=shared_progress, data=chunk,
-                    ))
+                    jobs.append(executor.submit(delegated_task, task_id, shared_progress, chunk))
 
                 # Update progress bar from shared state
                 remaining = len(jobs)
                 while remaining:
                     n_done = 0
                     for task_id, latest in shared_progress.items():
                         n_done += latest
@@ -94,15 +92,15 @@
                     remaining = len(jobs) - sum(job.done() for job in jobs)
 
                 # Collect results and catch and errors
                 return [job.result() for job in jobs]
 
 
 # Note: can't use beartype on a delegated_task & this function can't be in the if-block below
-def __long_task(*, task_id: int, shared_progress: DictProxy, data: List[_ItemT]) -> Any:  # type: ignore[type-arg]
+def __long_task(task_id: int, shared_progress: DictProxy, data: List[_ItemT]) -> Any:  # type: ignore[type-arg]
     """Example long task."""
     for _val in data:
         sleep(1)  # nosemgrep: python.lang.best-practice.sleep.arbitrary-sleep
         shared_progress[task_id] += 1
     return True
 
 
@@ -110,12 +108,12 @@
     # Run demo with: 'poetry run python -m shoal.pretty_process'
 
     # Resolve number of cores or specified maximum
     num_cpus = 4
     try:
         import psutil  # pyright: ignore[reportMissingModuleSource]
         num_cpus = psutil.cpu_count(logical=False)
-    except Exception as exc:  # noqa: PIE786
+    except Exception as exc:
         print(exc)  # noqa: T201
 
     result = pretty_process(__long_task, data=[*range(23)], num_workers=num_cpus)
     print(result)  # noqa: T201
```

### Comparing `corallium-0.3.3/corallium/shell.py` & `corallium-1.0.0/corallium/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Run shell commands."""
 
 import asyncio
-import subprocess  # noqa: S404  # nosec
+import subprocess  # nosec # noqa: S404
 import sys
 from io import BufferedReader, StringIO, TextIOWrapper
 from pathlib import Path
 from time import time
 
 from beartype import beartype
 from beartype.typing import Callable, Optional, Union
@@ -34,15 +34,15 @@
         CalledProcessError: if return code is non-zero
 
     """
     logger.debug('Running', cmd=cmd, timeout=timeout, cwd=cwd, printer=printer)
 
     start = time()
     lines = []
-    with subprocess.Popen(  # noqa: DUO116  # nosec  # nosemgrep
+    with subprocess.Popen(  # nosec  # nosemgrep
         cmd, cwd=cwd,
         stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True,
         shell=True,  # noqa: S602
     ) as proc:
         stdout: Union[BufferedReader, StringIO, TextIOWrapper] = proc.stdout  # type: ignore[assignment]
         return_code = None
         while return_code is None:
@@ -59,15 +59,15 @@
     output = ''.join(lines)  # type: ignore[arg-type]
     if return_code != 0:
         raise subprocess.CalledProcessError(returncode=return_code or 404, cmd=cmd, output=output)
     return output
 
 
 async def _capture_shell_async(cmd: str, *, cwd: Optional[Path] = None) -> str:
-    proc = await asyncio.create_subprocess_shell(  # noqa: DUO116  # nosec  # nosemgrep
+    proc = await asyncio.create_subprocess_shell(  # nosec  # nosemgrep
         cmd, cwd=cwd,
         stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
         shell=True,  # noqa: S604
     )
 
     stdout, _stderr = await proc.communicate()
     output = stdout.decode().strip()
@@ -110,12 +110,12 @@
 
     Raises:
         CalledProcessError: if return code is non-zero
 
     """
     logger.debug('Running', cmd=cmd, timeout=timeout, cwd=cwd)
 
-    subprocess.run(  # noqa: DUO116  # nosemgrep
+    subprocess.run(  # nosemgrep
         cmd, timeout=timeout or None, cwd=cwd,
         stdout=sys.stdout, stderr=sys.stderr, check=True,
         shell=True,  # noqa: S602,  # nosec
     )
```

### Comparing `corallium-0.3.3/docs/README.md` & `corallium-1.0.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `corallium-0.3.3/pyproject.toml` & `corallium-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "0.3.3"
+version = "1.0.0"
 version_files = ["corallium/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
 ] # https://pypi.org/classifiers/
 description = "Shared functionality for the calcipy-ecosystem"
 documentation = "https://corallium.kyleking.me"
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "corallium"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/corallium"
-version = "0.3.3"
+version = "1.0.0"
 
 [tool.poetry.dependencies]
-python = "^3.8.12"
-beartype = ">=0.15.0"
-pydantic = ">=2.1.1"
-rich = ">=12.6.0"
+python = "^3.9.13"
+beartype = ">=0.18.2"
+pydantic = ">=2.7.0"
+rich = ">=13.7.1"
 tomli = {markers = "python_version < '3.11'", version = ">=2.0.1"}
 
 [tool.poetry.group.dev.dependencies]
-calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=1.6.2"}
-pytest-asyncio = ">=0.21.0"
-pytest-structlog = ">=0.6" # Provides pytest fixture 'log'
-pytest-subprocess = ">=1.4.1"
-structlog = ">=22.3.0"
+calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=2.0.4"}
+pytest-asyncio = ">=0.23.6"
+pytest-structlog = ">=0.8" # Provides pytest fixture 'log'
+pytest-subprocess = ">=1.5.0"
+structlog = ">=24.1.0"
 types-pyyaml = ">=6.0.12.8"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kyleking/corallium/issues"
 "Changelog" = "https://github.com/kyleking/corallium/blob/main/docs/docs/CHANGELOG.md"
 
 [tool.pyright]
 include = ["corallium"]
-pythonVersion = "3.8"
+pythonVersion = "3.9"
+
+[tool.tomlsort]
+all = true
+in_place = true
+sort_first = ["python"]
+trailing_comma_inline_array = true
```

### Comparing `corallium-0.3.3/PKG-INFO` & `corallium-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: corallium
-Version: 0.3.3
+Version: 1.0.0
 Summary: Shared functionality for the calcipy-ecosystem
 Home-page: https://github.com/kyleking/corallium
 License: MIT
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
-Requires-Python: >=3.8.12,<4.0.0
+Requires-Python: >=3.9.13,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: beartype (>=0.15.0)
-Requires-Dist: pydantic (>=2.1.1)
-Requires-Dist: rich (>=12.6.0)
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: beartype (>=0.18.2)
+Requires-Dist: pydantic (>=2.7.0)
+Requires-Dist: rich (>=13.7.1)
 Requires-Dist: tomli (>=2.0.1) ; python_version < "3.11"
 Project-URL: Bug Tracker, https://github.com/kyleking/corallium/issues
 Project-URL: Changelog, https://github.com/kyleking/corallium/blob/main/docs/docs/CHANGELOG.md
 Project-URL: Documentation, https://corallium.kyleking.me
 Project-URL: Repository, https://github.com/kyleking/corallium
 Description-Content-Type: text/markdown
```

