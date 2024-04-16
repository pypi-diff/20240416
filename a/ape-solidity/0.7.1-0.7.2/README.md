# Comparing `tmp/ape-solidity-0.7.1.tar.gz` & `tmp/ape-solidity-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-solidity-0.7.1.tar", last modified: Fri Jan  5 23:00:54 2024, max compression
+gzip compressed data, was "ape-solidity-0.7.2.tar", last modified: Tue Apr 16 17:47:10 2024, max compression
```

## Comparing `ape-solidity-0.7.1.tar` & `ape-solidity-0.7.2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.787128 ape-solidity-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.771128 ape-solidity-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.771128 ape-solidity-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.771128 ape-solidity-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-01-05 23:00:54.787128 ape-solidity-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.771128 ape-solidity-0.7.1/ape_solidity/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/ape_solidity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/ape_solidity/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    45022 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/ape_solidity/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/ape_solidity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/ape_solidity/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-05 23:00:54.000000 ape-solidity-0.7.1/ape_solidity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/ape_solidity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-01-05 23:00:54.000000 ape-solidity-0.7.1/ape_solidity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-01-05 23:00:54.000000 ape-solidity-0.7.1/ape_solidity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 23:00:54.000000 ape-solidity-0.7.1/ape_solidity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 23:00:54.000000 ape-solidity-0.7.1/ape_solidity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-05 23:00:54.000000 ape-solidity-0.7.1/ape_solidity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-05 23:00:54.000000 ape-solidity-0.7.1/ape_solidity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-05 23:00:54.787128 ape-solidity-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/BrownieProject/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/BrownieProject/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/BrownieProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/BrownieProject/contracts/BrownieContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/BrownieStyleDependency/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/BrownieStyleDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/BrownieStyleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/BrownieStyleDependency/contracts/FailingContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/Dependency/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/Dependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/Dependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/Dependency/contracts/Dependency.sol
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/Dependency/contracts/OlderDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/Dependency/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/Dependency/contracts/subfolder_with_imports/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/DependencyOfDependency/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/DependencyOfDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/DependencyOfDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.775128 ape-solidity-0.7.1/tests/ProjectWithinProject/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/ProjectWithinProject/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.779128 ape-solidity-0.7.1/tests/ProjectWithinProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/ProjectWithinProject/contracts/Contract.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.779128 ape-solidity-0.7.1/tests/VersionSpecifiedInConfig/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/VersionSpecifiedInConfig/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.779128 ape-solidity-0.7.1/tests/VersionSpecifiedInConfig/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.783128 ape-solidity-0.7.1/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/BuiltinErrorChecker.sol
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/CircularImport1.sol
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/CircularImport2.sol
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/CompilesOnce.sol
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/DifferentNameThanFile.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.783128 ape-solidity-0.7.1/tests/contracts/DirectoryWithExtension.sol/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/DirectoryWithExtension.sol/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/ExperimentalABIEncoderV2.sol
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/ImportOlderDependency.sol
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/ImportSourceWithEqualSignVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/ImportSourceWithNoPrefixVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/ImportingLessConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/Imports.sol
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/JustAStruct.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/LibraryFun.sol
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/MissingPragma.sol
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/MultipleDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/NumerousDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/OlderVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/RandomVyperFile.vy
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/RangedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/SpacesInPragma.sol
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/SpecificVersionNoPrefix.sol
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/SpecificVersionNoPrefix2.sol
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/SpecificVersionRange.sol
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/SpecificVersionWithEqualSign.sol
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/UseYearn.sol
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/VagueVersion.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.783128 ape-solidity-0.7.1/tests/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/subfolder/Relativecontract.sol
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.783128 ape-solidity-0.7.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/data/ImportingLessConstrainedVersionFlat.sol
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/data/ImportsFlattened.sol.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.767128 ape-solidity-0.7.1/tests/data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.767128 ape-solidity-0.7.1/tests/data/packages/OpenZeppelin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.783128 ape-solidity-0.7.1/tests/data/packages/OpenZeppelin/v4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)   698486 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.783128 ape-solidity-0.7.1/tests/data/packages/OpenZeppelin/v4.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)   879002 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.767128 ape-solidity-0.7.1/tests/data/packages/vault/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.787128 ape-solidity-0.7.1/tests/data/packages/vault/master/
--rw-r--r--   0 runner    (1001) docker     (127)   167518 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/data/packages/vault/master/vault_main.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.787128 ape-solidity-0.7.1/tests/data/packages/vault/v0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)   167551 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/data/packages/vault/v0.4.5/vault.json
--rw-r--r--   0 runner    (1001) docker     (127)    32767 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:00:54.787128 ape-solidity-0.7.1/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/scripts/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    23200 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-01-05 23:00:01.000000 ape-solidity-0.7.1/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.359098 ape-solidity-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.359098 ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.359098 ape-solidity-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.359098 ape-solidity-0.7.2/ape_solidity/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/ape_solidity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/ape_solidity/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45726 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/ape_solidity/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/ape_solidity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/ape_solidity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 17:47:09.000000 ape-solidity-0.7.2/ape_solidity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/ape_solidity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/BrownieProject/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/BrownieProject/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/BrownieProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/BrownieProject/contracts/BrownieContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/BrownieStyleDependency/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/BrownieStyleDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/BrownieStyleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/BrownieStyleDependency/contracts/FailingContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/Dependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/Dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/Dependency/contracts/Dependency.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/Dependency/contracts/OlderDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/Dependency/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/Dependency/contracts/subfolder_with_imports/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/DependencyOfDependency/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/DependencyOfDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/DependencyOfDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/ProjectWithinProject/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/ProjectWithinProject/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/ProjectWithinProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/ProjectWithinProject/contracts/Contract.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/VersionSpecifiedInConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/VersionSpecifiedInConfig/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.367098 ape-solidity-0.7.2/tests/VersionSpecifiedInConfig/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/BuiltinErrorChecker.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/CircularImport1.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/CircularImport2.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/CompilesOnce.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/DifferentNameThanFile.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/contracts/DirectoryWithExtension.sol/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/DirectoryWithExtension.sol/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/ExperimentalABIEncoderV2.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/ImportOlderDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/ImportSourceWithEqualSignVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/ImportSourceWithNoPrefixVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/ImportingLessConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/Imports.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/JustAStruct.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/LibraryFun.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/MissingPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/MultipleDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/NumerousDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/OlderVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/RandomVyperFile.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/RangedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/SpacesInPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/SpecificVersionNoPrefix.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/SpecificVersionNoPrefix2.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/SpecificVersionRange.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/SpecificVersionWithEqualSign.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/UseYearn.sol
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/VagueVersion.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/subfolder/Relativecontract.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/ImportingLessConstrainedVersionFlat.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/ImportsFlattened.sol.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.355098 ape-solidity-0.7.2/tests/data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.355098 ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)   698486 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)   879002 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.355098 ape-solidity-0.7.2/tests/data/packages/vault/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/tests/data/packages/vault/master/
+-rw-r--r--   0 runner    (1001) docker     (127)   167518 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/packages/vault/master/vault_main.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/tests/data/packages/vault/v0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)   167551 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/packages/vault/v0.4.5/vault.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32767 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/scripts/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/test_integration.py
```

### Comparing `ape-solidity-0.7.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/.github/release-drafter.yml` & `ape-solidity-0.7.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/.github/workflows/codeql.yml` & `ape-solidity-0.7.2/.github/workflows/codeql.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       security-events: write
 
     strategy:
       fail-fast: false
 
     steps:
     - name: Checkout repository
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: Initialize CodeQL
       uses: github/codeql-action/init@v2
       with:
         languages: python
 
     - name: Autobuild
```

### Comparing `ape-solidity-0.7.1/.github/workflows/prtitle.yaml` & `ape-solidity-0.7.2/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
```

### Comparing `ape-solidity-0.7.1/.github/workflows/publish.yaml` & `ape-solidity-0.7.2/.github/workflows/publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
```

### Comparing `ape-solidity-0.7.1/.github/workflows/stale-prs.yml` & `ape-solidity-0.7.2/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/.github/workflows/test.yaml` & `ape-solidity-0.7.2/.github/workflows/test.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
   cancel-in-progress: true
 
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
@@ -38,18 +38,18 @@
         - name: Run mdformat
           run: mdformat . --check
 
     type-check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
@@ -65,18 +65,18 @@
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
                 python-version: [3.8, 3.9, '3.10', '3.11']
 
         env:
           GITHUB_ACCESS_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip uninstall eth-ape --yes
@@ -91,18 +91,18 @@
     # fuzzing:
     #     runs-on: ubuntu-latest
 
     #     strategy:
     #         fail-fast: true
 
     #     steps:
-    #     - uses: actions/checkout@v3
+    #     - uses: actions/checkout@v4
 
     #     - name: Setup Python
-    #       uses: actions/setup-python@v4
+    #       uses: actions/setup-python@v5
     #       with:
     #           python-version: "3.10"
 
     #     - name: Install Dependencies
     #       run: pip install .[test]
 
     #     - name: Run Tests
```

### Comparing `ape-solidity-0.7.1/.gitignore` & `ape-solidity-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/.pre-commit-config.yaml` & `ape-solidity-0.7.2/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-yaml
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 23.12.0
+    rev: 24.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.1
+    rev: v1.9.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-requests, types-setuptools, pydantic, types-pkg-resources]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
```

### Comparing `ape-solidity-0.7.1/CONTRIBUTING.md` & `ape-solidity-0.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/LICENSE` & `ape-solidity-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/PKG-INFO` & `ape-solidity-0.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.7.1
+Version: 0.7.2
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -170,7 +170,22 @@
 
 You can enable `solc`'s `--via-IR` flag by adding the following values to your `ape-config.yaml`
 
 ```yaml
 solidity:
   via_ir: True
 ```
+
+### Contract Flattening
+
+`ape-solidity` has contract-flattening capabilities.
+If you are publishing contracts using Ape, Ape automatically detects and uses the flattened-contract approach if needed.
+
+To manually flatten a contract for your own benefit, use the following code:
+
+```python
+from ape import compilers, project
+
+source_path = project.source_paths[0]  # Replace with your path.
+flattened_src = compilers.flatten_contract(source_path)
+print(str(flattened_src))
+```
```

### Comparing `ape-solidity-0.7.1/README.md` & `ape-solidity-0.7.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -141,7 +141,22 @@
 
 You can enable `solc`'s `--via-IR` flag by adding the following values to your `ape-config.yaml`
 
 ```yaml
 solidity:
   via_ir: True
 ```
+
+### Contract Flattening
+
+`ape-solidity` has contract-flattening capabilities.
+If you are publishing contracts using Ape, Ape automatically detects and uses the flattened-contract approach if needed.
+
+To manually flatten a contract for your own benefit, use the following code:
+
+```python
+from ape import compilers, project
+
+source_path = project.source_paths[0]  # Replace with your path.
+flattened_src = compilers.flatten_contract(source_path)
+print(str(flattened_src))
+```
```

### Comparing `ape-solidity-0.7.1/ape_solidity/_utils.py` & `ape-solidity-0.7.2/ape_solidity/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,30 +91,29 @@
 
         return suffix
 
 
 class ImportRemappingBuilder:
     def __init__(self, contracts_cache: Path):
         # import_map maps import keys like `@openzeppelin/contracts`
-        # to str paths in the contracts' .cache folder.
+        # to str paths in the compiler cache folder.
         self.import_map: Dict[str, str] = {}
         self.dependencies_added: Set[Path] = set()
         self.contracts_cache = contracts_cache
 
     def add_entry(self, remapping: ImportRemapping):
         path = remapping.package_id
-        if not str(path).startswith(f".cache{os.path.sep}"):
-            path = Path(".cache") / path
+        if self.contracts_cache not in path.parents:
+            path = self.contracts_cache / path
 
         self.import_map[remapping.key] = str(path)
 
 
 def get_import_lines(source_paths: Set[Path]) -> Dict[Path, List[str]]:
     imports_dict: Dict[Path, List[str]] = {}
-
     for filepath in source_paths:
         import_set = set()
         if not filepath.is_file():
             continue
 
         source_lines = filepath.read_text().splitlines()
         num_lines = len(source_lines)
```

### Comparing `ape-solidity-0.7.1/ape_solidity/compiler.py` & `ape-solidity-0.7.2/ape_solidity/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,27 +217,28 @@
         if not (remappings := self.settings.import_remapping):
             return {}
 
         elif not isinstance(remappings, (list, tuple)) or not isinstance(remappings[0], str):
             raise IncorrectMappingFormatError()
 
         # We use these helpers to transform the values configured
-        # to values matching files in the `contracts/.cache` folder.
-        contracts_cache = base_path / ".cache"
-        builder = ImportRemappingBuilder(contracts_cache)
+        # to values matching files in the compiler cache folder.
+        builder = ImportRemappingBuilder(
+            get_relative_path(self.project_manager.compiler_cache_folder, base_path)
+        )
         packages_cache = self.config_manager.packages_folder
 
         # Here we hash and validate if there were changes to remappings.
         # If there were, we continue, else return the cached value for
         # performance reasons.
         remappings_tuple = tuple(remappings)
         if (
             self._import_remapping_hash
             and self._import_remapping_hash == hash(remappings_tuple)
-            and contracts_cache.is_dir()
+            and self.project_manager.compiler_cache_folder.is_dir()
         ):
             return self._cached_import_map
 
         # NOTE: Dependencies are only extracted if calling for the first.
         # Likely, this was done already before this point, unless
         # calling python methods manually. However, dependencies MUST be
         # fully loaded to properly evaluate remapping paths.
@@ -261,15 +262,15 @@
                 version_id = next(iter(dependencies[package_id.name]))
                 logger.debug(f"for {package_id.name} version ID missing, using {version_id}")
                 package_id = package_id / version_id
 
             data_folder_cache = packages_cache / package_id
 
             # Re-build a downloaded dependency manifest into the .cache directory for imports.
-            sub_contracts_cache = contracts_cache / package_id
+            sub_contracts_cache = self.project_manager.compiler_cache_folder / package_id
             if not sub_contracts_cache.is_dir() or not list(sub_contracts_cache.iterdir()):
                 cached_manifest_file = data_folder_cache / f"{remapping_obj.name}.json"
                 if not cached_manifest_file.is_file():
                     logger.debug(f"Unable to find dependency '{package_id}'.")
 
                 else:
                     manifest = PackageManifest.model_validate_json(cached_manifest_file.read_text())
@@ -424,22 +425,24 @@
     ) -> Dict[str, str]:
         base_path = base_path or self.project_manager.contracts_folder
         remappings = remappings or self.get_import_remapping(base_path=base_path)
         if not remappings:
             # No remappings used at all.
             return {}
 
+        relative_cache = get_relative_path(self.project_manager.compiler_cache_folder, base_path)
+
         # Filter out unused import remapping.
         return {
             k: v
             for source in (
                 x
-                for sources in self.get_imports(list(sources), base_path=base_path).values()
-                for x in sources
-                if x.startswith(".cache")
+                for sourceset in self.get_imports(list(sources), base_path=base_path).values()
+                for x in sourceset
+                if str(relative_cache) in x
             )
             for parent_key in (
                 os.path.sep.join(source.split(os.path.sep)[:3]) for source in [source]
             )
             for k, v in [(k, v) for k, v in remappings.items() if parent_key in v]
         }
 
@@ -467,14 +470,15 @@
                 missing_src_str = ", ".join(missing_sources)
                 raise CompilerError(f"Missing sources: '{missing_src_str}'.")
 
             sources = {
                 x: {"content": (base_path / x).read_text()}
                 for x in vers_settings["outputSelection"]
             }
+
             input_jsons[solc_version] = {
                 "sources": sources,
                 "settings": vers_settings,
                 "language": "Solidity",
             }
 
         return input_jsons
@@ -492,14 +496,17 @@
             cleaned_version = Version(solc_version.base_version)
             solc_binary = get_executable(version=cleaned_version)
             arguments: Dict = {"solc_binary": solc_binary, "solc_version": cleaned_version}
 
             if solc_version >= Version("0.6.9"):
                 arguments["base_path"] = base_path
 
+            if self.project_manager.compiler_cache_folder.is_dir():
+                arguments["allow_paths"] = self.project_manager.compiler_cache_folder
+
             # Allow empty contracts, like Vyper does.
             arguments["allow_empty"] = True
 
             try:
                 output = compile_standard(input_json, **arguments)
             except SolcError as err:
                 raise SolcCompileError(err) from err
@@ -1000,17 +1007,16 @@
 def get_first_version_pragma(source: str) -> str:
     match = VERSION_PRAGMA_PATTERN.search(source)
     if match:
         return match.group(0)
     return ""
 
 
-def get_licenses(source: str) -> List[Tuple[str, str]]:
-    matches = LICENSES_PATTERN.findall(source)
-    return matches
+def get_licenses(src: str) -> List[Tuple[str, str]]:
+    return LICENSES_PATTERN.findall(src)
 
 
 def process_licenses(contract: str) -> str:
     """
     Process the licenses in a contract.
     Ensure that all licenses are identical, and if not, raise an error.
     The contract is returned with a single license identifier line at its top.
@@ -1019,30 +1025,38 @@
     # Extract SPDX license identifiers from the contract.
     extracted_licenses = get_licenses(contract)
 
     # Return early if no licenses are present in the contract.
     if not extracted_licenses:
         return contract
 
-    # Get the unique license identifiers. We expect that all licenses in a contract are the same.
+    # The "root" license is most-likely last because import statements are
+    # replaced with their sources typically at the top of the file
+    license_line, root_license = extracted_licenses[-1]
+
+    # Get the unique license identifiers. All licenses in a contract _should_ be the same.
     unique_license_identifiers = {
         license_identifier for _, license_identifier in extracted_licenses
     }
 
-    # If we have more than one unique license identifier, raise an error.
+    # If we have more than one unique license identifier, warn the user and use the root.
     if len(unique_license_identifiers) > 1:
-        raise CompilerError(f"Conflicting licenses found: {unique_license_identifiers}")
-
-    # Get the first license line and identifier.
-    license_line, _ = extracted_licenses[0]
+        licenses_str = ", ".join(sorted(unique_license_identifiers))
+        logger.warning(
+            f"Conflicting licenses found: '{licenses_str}'. "
+            f"Using the root file's license '{root_license}'."
+        )
 
     # Remove all of the license lines from the contract.
-    contract_without_licenses = contract.replace(license_line, "")
+    contract_without_licenses = contract
+    for license_tuple in extracted_licenses:
+        line = license_tuple[0]
+        contract_without_licenses = contract_without_licenses.replace(line, "")
 
-    # Prepend the contract with only one license line.
+    # Prepend the contract with only the root license line.
     contract_with_single_license = f"{license_line}\n{contract_without_licenses}"
 
     return contract_with_single_license
 
 
 def _get_sol_panic(revert_message: str) -> Optional[Type[RuntimeErrorUnion]]:
     if revert_message.startswith(RUNTIME_ERROR_CODE_PREFIX):
```

### Comparing `ape-solidity-0.7.1/ape_solidity/exceptions.py` & `ape-solidity-0.7.2/ape_solidity/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/ape_solidity.egg-info/PKG-INFO` & `ape-solidity-0.7.2/ape_solidity.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.7.1
+Version: 0.7.2
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -170,7 +170,22 @@
 
 You can enable `solc`'s `--via-IR` flag by adding the following values to your `ape-config.yaml`
 
 ```yaml
 solidity:
   via_ir: True
 ```
+
+### Contract Flattening
+
+`ape-solidity` has contract-flattening capabilities.
+If you are publishing contracts using Ape, Ape automatically detects and uses the flattened-contract approach if needed.
+
+To manually flatten a contract for your own benefit, use the following code:
+
+```python
+from ape import compilers, project
+
+source_path = project.source_paths[0]  # Replace with your path.
+flattened_src = compilers.flatten_contract(source_path)
+print(str(flattened_src))
+```
```

### Comparing `ape-solidity-0.7.1/ape_solidity.egg-info/SOURCES.txt` & `ape-solidity-0.7.2/ape_solidity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/ape_solidity.egg-info/requires.txt` & `ape-solidity-0.7.2/ape_solidity.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 py-solc-x<3,>=2.0.2
-eth-ape<0.8,>=0.7.0
+eth-ape<0.8,>=0.7.10
 ethpm-types
 eth-pydantic-types
 packaging
 requests
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 pytest-mock
 hypothesis<7.0,>=6.2.0
 pytest-benchmark
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.3.0
+mypy<2,>=1.9.0
 types-requests
 types-setuptools
 types-pkg-resources
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 isort<6,>=5.10.1
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
@@ -37,20 +37,20 @@
 
 [doc]
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
 
 [lint]
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.3.0
+mypy<2,>=1.9.0
 types-requests
 types-setuptools
 types-pkg-resources
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 isort<6,>=5.10.1
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 
 [release]
```

### Comparing `ape-solidity-0.7.1/pyproject.toml` & `ape-solidity-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/setup.py` & `ape-solidity-0.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating and using mocks
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "pytest-benchmark",  # For performance tests
     ],
     "lint": [
-        "black>=23.12.0,<24",  # Auto-formatter and linter
-        "mypy>=1.7.1,<2",  # Static type analyzer
+        "black>=24.3.0,<25",  # Auto-formatter and linter
+        "mypy>=1.9.0,<2",  # Static type analyzer
         "types-requests",  # Needed for mypy type shed
         "types-setuptools",  # Needed for mypy type shed
         "types-pkg-resources",  # Needed for type checking tests
-        "flake8>=6.1.0,<7",  # Style linter
+        "flake8>=7.0.0,<8",  # Style linter
         "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "doc": [
@@ -65,15 +65,15 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-solidity",
     include_package_data=True,
     install_requires=[
         "py-solc-x>=2.0.2,<3",
-        "eth-ape>=0.7.0,<0.8",
+        "eth-ape>=0.7.10,<0.8",
         "ethpm-types",  # Use the version ape requires
         "eth-pydantic-types",  # Use the version ape requires
         "packaging",  # Use the version ape requires
         "requests",
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
```

### Comparing `ape-solidity-0.7.1/tests/ape-config.yaml` & `ape-solidity-0.7.2/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/conftest.py` & `ape-solidity-0.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/contracts/Imports.sol` & `ape-solidity-0.7.2/tests/contracts/Imports.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/contracts/LibraryFun.sol` & `ape-solidity-0.7.2/tests/contracts/LibraryFun.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/data/ImportingLessConstrainedVersionFlat.sol` & `ape-solidity-0.7.2/tests/data/ImportingLessConstrainedVersionFlat.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/data/ImportsFlattened.sol.txt` & `ape-solidity-0.7.2/tests/data/ImportsFlattened.sol.txt`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json` & `ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json` & `ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/data/packages/vault/master/vault_main.json` & `ape-solidity-0.7.2/tests/data/packages/vault/master/vault_main.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/data/packages/vault/v0.4.5/vault.json` & `ape-solidity-0.7.2/tests/data/packages/vault/v0.4.5/vault.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/package-lock.json` & `ape-solidity-0.7.2/tests/package-lock.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/scripts/clean.py` & `ape-solidity-0.7.2/tests/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/test_compiler.py` & `ape-solidity-0.7.2/tests/test_compiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 
 import pytest
 import solcx
 from ape import reverts
 from ape.contracts import ContractContainer
 from ape.exceptions import CompilerError
+from ape.logging import LogLevel
 from packaging.version import Version
 from pkg_resources import get_distribution
 from requests.exceptions import ConnectionError
 
 from ape_solidity import Extension
 from ape_solidity._utils import OUTPUT_SELECTION
 from ape_solidity.exceptions import IndexOutOfBoundsError
@@ -137,15 +138,20 @@
     The fix involved using nicer access to "contracts" in the standard output JSON.
     """
     contract_types = compiler.compile([project.contracts_folder / "JustAStruct.sol"])
     assert len(contract_types) == 0
 
 
 def test_get_imports(project, compiler):
-    import_dict = compiler.get_imports(TEST_CONTRACT_PATHS, BASE_PATH)
+    test_contract_paths = [
+        p
+        for p in project.contracts_folder.iterdir()
+        if ".cache" not in str(p) and not p.is_dir() and p.suffix == Extension.SOL.value
+    ]
+    import_dict = compiler.get_imports(test_contract_paths, project.contracts_folder)
     contract_imports = import_dict["Imports.sol"]
     # NOTE: make sure there aren't duplicates
     assert len([x for x in contract_imports if contract_imports.count(x) > 1]) == 0
     # NOTE: returning a list
     assert isinstance(contract_imports, list)
     # NOTE: in case order changes
     expected = {
@@ -157,14 +163,50 @@
         "MissingPragma.sol",
         "NumerousDefinitions.sol",
         "subfolder/Relativecontract.sol",
     }
     assert set(contract_imports) == expected
 
 
+def test_get_imports_cache_folder(project, compiler):
+    """Test imports when cache folder is configured"""
+    compile_config = project.config_manager.get_config("compile")
+    og_cache_colder = compile_config.cache_folder
+    compile_config.cache_folder = project.path / ".cash"
+    # assert False
+    test_contract_paths = [
+        p
+        for p in project.contracts_folder.iterdir()
+        if ".cache" not in str(p) and not p.is_dir() and p.suffix == Extension.SOL.value
+    ]
+    # Using a different base path here because the cache folder is in the project root
+    import_dict = compiler.get_imports(test_contract_paths, project.path)
+    contract_imports = import_dict["contracts/Imports.sol"]
+    # NOTE: make sure there aren't duplicates
+    assert len([x for x in contract_imports if contract_imports.count(x) > 1]) == 0
+    # NOTE: returning a list
+    assert isinstance(contract_imports, list)
+    # NOTE: in case order changes
+    expected = {
+        ".cash/BrownieDependency/local/BrownieContract.sol",
+        ".cash/BrownieStyleDependency/local/BrownieStyleDependency.sol",
+        ".cash/TestDependency/local/Dependency.sol",
+        ".cash/gnosis/v1.3.0/common/Enum.sol",
+        "contracts/CompilesOnce.sol",
+        "contracts/MissingPragma.sol",
+        "contracts/NumerousDefinitions.sol",
+        "contracts/subfolder/Relativecontract.sol",
+    }
+    assert set(contract_imports) == expected
+
+    # Reset because this config is stateful across tests
+    compile_config.cache_folder = og_cache_colder
+    shutil.rmtree(og_cache_colder)
+
+
 def test_get_imports_raises_when_non_solidity_files(compiler, vyper_source_path):
     with raises_because_not_sol:
         compiler.get_imports([vyper_source_path])
 
 
 def test_get_import_remapping(compiler, project, config):
     import_remapping = compiler.get_import_remapping()
@@ -555,23 +597,31 @@
     # delete source code file
     source_path.unlink()
 
     # flip the via_ir flag back to False
     compiler.config.via_ir = False
 
 
-def test_flatten(project, compiler, data_folder):
+def test_flatten(project, compiler, data_folder, caplog):
     source_path = project.contracts_folder / "Imports.sol"
-    with pytest.raises(CompilerError):
+    with caplog.at_level(LogLevel.WARNING):
         compiler.flatten_contract(source_path)
+        actual = caplog.messages[-1]
+        expected = (
+            "Conflicting licenses found: 'LGPL-3.0-only, MIT'. "
+            "Using the root file's license 'MIT'."
+        )
+        assert actual == expected
 
     source_path = project.contracts_folder / "ImportingLessConstrainedVersion.sol"
     flattened_source = compiler.flatten_contract(source_path)
     flattened_source_path = data_folder / "ImportingLessConstrainedVersionFlat.sol"
-    assert str(flattened_source) == str(flattened_source_path.read_text())
+    actual = str(flattened_source)
+    expected = str(flattened_source_path.read_text())
+    assert actual == expected
 
 
 def test_compile_code(compiler):
     code = """
 contract Contract {
     function snakes() pure public returns(bool) {
         return true;
```

### Comparing `ape-solidity-0.7.1/tests/test_exceptions.py` & `ape-solidity-0.7.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.1/tests/test_integration.py` & `ape-solidity-0.7.2/tests/test_integration.py`

 * *Files identical despite different names*

