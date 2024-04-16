# Comparing `tmp/tableau_migration-2.1.0.tar.gz` & `tmp/tableau_migration-2.1.1.tar.gz`

## Comparing `tableau_migration-2.1.0.tar` & `tableau_migration-2.1.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/requirements.txt
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/__init__.py
--rw-r--r--   0        0        0     8648 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration.py
--rw-r--r--   0        0        0    18376 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_filters.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_mappings.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_transformers.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_migrators.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_options.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_logger.py
--rw-r--r--   0        0        0    19104 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll
--rw-r--r--   0        0        0    32432 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll
--rw-r--r--   0        0        0    34848 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll
--rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll
--rw-r--r--   0        0        0    29448 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll
--rw-r--r--   0        0        0    44808 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll
--rw-r--r--   0        0        0    23312 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
--rw-r--r--   0        0        0    45328 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll
--rw-r--r--   0        0        0    63264 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll
--rw-r--r--   0        0        0    34224 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll
--rw-r--r--   0        0        0    93984 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll
--rw-r--r--   0        0        0    41376 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll
--rw-r--r--   0        0        0    32008 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll
--rw-r--r--   0        0        0    31152 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll
--rw-r--r--   0        0        0    37144 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll
--rw-r--r--   0        0        0    23728 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll
--rw-r--r--   0        0        0    53000 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll
--rw-r--r--   0        0        0   115248 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll
--rw-r--r--   0        0        0   129056 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll
--rw-r--r--   0        0        0    89368 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.dll
--rw-r--r--   0        0        0    21680 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll
--rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll
--rw-r--r--   0        0        0    66336 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll
--rw-r--r--   0        0        0    29968 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll
--rw-r--r--   0        0        0    52496 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll
--rw-r--r--   0        0        0    25264 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll
--rw-r--r--   0        0        0    24336 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll
--rw-r--r--   0        0        0    66312 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Options.dll
--rw-r--r--   0        0        0    45336 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll
--rw-r--r--   0        0        0    37936 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll
--rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll
--rw-r--r--   0        0        0   116768 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll
--rw-r--r--   0        0        0    65568 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll
--rw-r--r--   0        0        0   242976 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Polly.Core.dll
--rw-r--r--   0        0        0    56736 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Polly.Extensions.dll
--rw-r--r--   0        0        0    29600 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Polly.RateLimiting.dll
--rw-r--r--   0        0        0   247584 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.Collections.Immutable.dll
--rw-r--r--   0        0        0   164616 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll
--rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.IO.Abstractions.dll
--rw-r--r--   0        0        0    71440 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.Text.Encodings.Web.dll
--rw-r--r--   0        0        0   579848 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.Text.Json.dll
--rw-r--r--   0        0        0    70416 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.Threading.RateLimiting.dll
--rw-r--r--   0        0        0    37426 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.deps.json
--rw-r--r--   0        0        0   985600 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.dll
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.runtimeconfig.json
--rw-r--r--   0        0        0  1074636 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.xml
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll
--rw-r--r--   0        0        0    29184 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll
--rw-r--r--   0        0        0    71448 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/.gitignore
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/README.md
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/requirements.txt
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/__init__.py
+-rw-r--r--   0        0        0     8648 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration.py
+-rw-r--r--   0        0        0    18376 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine.py
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_filters.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_mappings.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_transformers.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_migrators.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_options.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_logger.py
+-rw-r--r--   0        0        0    19104 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll
+-rw-r--r--   0        0        0    32432 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll
+-rw-r--r--   0        0        0    34848 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll
+-rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll
+-rw-r--r--   0        0        0    29448 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll
+-rw-r--r--   0        0        0    44808 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll
+-rw-r--r--   0        0        0    23312 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
+-rw-r--r--   0        0        0    45328 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll
+-rw-r--r--   0        0        0    63264 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll
+-rw-r--r--   0        0        0    34224 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll
+-rw-r--r--   0        0        0    93984 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll
+-rw-r--r--   0        0        0    41376 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll
+-rw-r--r--   0        0        0    32008 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll
+-rw-r--r--   0        0        0    31152 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll
+-rw-r--r--   0        0        0    37144 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll
+-rw-r--r--   0        0        0    23728 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll
+-rw-r--r--   0        0        0    53000 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll
+-rw-r--r--   0        0        0   115248 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll
+-rw-r--r--   0        0        0   129056 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll
+-rw-r--r--   0        0        0    89368 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.dll
+-rw-r--r--   0        0        0    21680 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll
+-rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll
+-rw-r--r--   0        0        0    66336 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll
+-rw-r--r--   0        0        0    29968 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll
+-rw-r--r--   0        0        0    52496 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll
+-rw-r--r--   0        0        0    25264 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll
+-rw-r--r--   0        0        0    24336 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll
+-rw-r--r--   0        0        0    66312 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Options.dll
+-rw-r--r--   0        0        0    45336 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll
+-rw-r--r--   0        0        0    37936 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll
+-rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll
+-rw-r--r--   0        0        0   116768 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll
+-rw-r--r--   0        0        0    65568 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll
+-rw-r--r--   0        0        0   242976 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Polly.Core.dll
+-rw-r--r--   0        0        0    56736 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Polly.Extensions.dll
+-rw-r--r--   0        0        0    29600 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Polly.RateLimiting.dll
+-rw-r--r--   0        0        0   247584 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.Collections.Immutable.dll
+-rw-r--r--   0        0        0   164616 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll
+-rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.IO.Abstractions.dll
+-rw-r--r--   0        0        0    71440 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.Text.Encodings.Web.dll
+-rw-r--r--   0        0        0   579848 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.Text.Json.dll
+-rw-r--r--   0        0        0    70416 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.Threading.RateLimiting.dll
+-rw-r--r--   0        0        0    37426 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.deps.json
+-rw-r--r--   0        0        0   985600 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.dll
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.runtimeconfig.json
+-rw-r--r--   0        0        0  1074636 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.xml
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll
+-rw-r--r--   0        0        0    29184 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll
+-rw-r--r--   0        0        0    71448 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/.gitignore
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/README.md
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/PKG-INFO
```

### Comparing `tableau_migration-2.1.0/src/tableau_migration/__init__.py` & `tableau_migration-2.1.1/src/tableau_migration/__init__.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/migration.py` & `tableau_migration-2.1.1/src/tableau_migration/migration.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/migration_engine.py` & `tableau_migration-2.1.1/src/tableau_migration/migration_engine.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks.py` & `tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_filters.py` & `tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_filters.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_mappings.py` & `tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_mappings.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_transformers.py` & `tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_transformers.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/migration_engine_migrators.py` & `tableau_migration-2.1.1/src/tableau_migration/migration_engine_migrators.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/migration_engine_options.py` & `tableau_migration-2.1.1/src/tableau_migration/migration_engine_options.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/migration_logger.py` & `tableau_migration-2.1.1/src/tableau_migration/migration_logger.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Options.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Options.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Polly.Core.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Polly.Core.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Polly.Extensions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Polly.Extensions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Polly.RateLimiting.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Polly.RateLimiting.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/System.Collections.Immutable.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/System.Collections.Immutable.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/System.IO.Abstractions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/System.IO.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/System.Text.Encodings.Web.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/System.Text.Encodings.Web.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/System.Text.Json.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/System.Text.Json.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/System.Threading.RateLimiting.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/System.Threading.RateLimiting.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.deps.json` & `tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.deps.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'libraries'": "{'Tableau.Migration/2.1.1': OrderedDict([('type', 'project'), ('serviceable', "*

 * *                "False), ('sha512', '')]), delete: ['Tableau.Migration/2.1.0']}",*

 * * "'targets'": "{'.NETCoreApp,Version=v6.0': {'Tableau.Migration/2.1.1': "*

 * *              "OrderedDict([('dependencies', "*

 * *              "OrderedDict([('Microsoft.Extensions.Configuration.EnvironmentVariables', '8.0.0'), "*

 * *              "('Microsoft.Extensions.Http', '8.0.0'), ('Microsoft.Extensions.Http.Resilience', "*

 * *               […]*

```diff
@@ -305,15 +305,15 @@
         "System.Threading.RateLimiting/8.0.0": {
             "hashPath": "system.threading.ratelimiting.8.0.0.nupkg.sha512",
             "path": "system.threading.ratelimiting/8.0.0",
             "serviceable": true,
             "sha512": "sha512-7mu9v0QDv66ar3DpGSZHg9NuNcxDaaAcnMULuZlaTpP9+hwXhrxNGsF5GmLkSHxFdb5bBc1TzeujsRgTrPWi+Q==",
             "type": "package"
         },
-        "Tableau.Migration/2.1.0": {
+        "Tableau.Migration/2.1.1": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         },
         "TestableIO.System.IO.Abstractions.Wrappers/20.0.15": {
             "hashPath": "testableio.system.io.abstractions.wrappers.20.0.15.nupkg.sha512",
             "path": "testableio.system.io.abstractions.wrappers/20.0.15",
@@ -859,15 +859,15 @@
                 "runtime": {
                     "lib/net6.0/System.Threading.RateLimiting.dll": {
                         "assemblyVersion": "8.0.0.0",
                         "fileVersion": "8.0.23.53103"
                     }
                 }
             },
-            "Tableau.Migration/2.1.0": {
+            "Tableau.Migration/2.1.1": {
                 "dependencies": {
                     "Microsoft.Extensions.Configuration.EnvironmentVariables": "8.0.0",
                     "Microsoft.Extensions.Http": "8.0.0",
                     "Microsoft.Extensions.Http.Resilience": "8.2.0",
                     "Microsoft.Extensions.Localization": "8.0.2",
                     "Microsoft.Extensions.Options.ConfigurationExtensions": "8.0.0",
                     "Microsoft.IO.RecyclableMemoryStream": "3.0.0",
```

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.dll`

 * *Files 0% similar despite different names*

#### pedump {}

```diff
@@ -1,12 +1,12 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0x8ce8f25f
+	             Time stamp: 0xe89acb94
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
```

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.xml` & `tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.xml`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll` & `tableau_migration-2.1.1/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/.gitignore` & `tableau_migration-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/pyproject.toml` & `tableau_migration-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.0/PKG-INFO` & `tableau_migration-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tableau_migration
-Version: 2.1.0
+Version: 2.1.1
 Summary: Tableau Migration SDK
 Project-URL: Homepage, http://www.tableau.com
 Project-URL: Bug Tracker, http://www.tableau.com
 Project-URL: Repository, https://github.com/tableau/tableau-migration-sdk
 Author: Tableau a Salesforce Product
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

