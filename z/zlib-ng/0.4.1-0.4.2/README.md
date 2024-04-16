# Comparing `tmp/zlib-ng-0.4.1.tar.gz` & `tmp/zlib-ng-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlib-ng-0.4.1.tar", last modified: Mon Mar 11 13:35:03 2024, max compression
+gzip compressed data, was "zlib-ng-0.4.2.tar", last modified: Wed Apr 10 11:51:22 2024, max compression
```

## Comparing `zlib-ng-0.4.1.tar` & `zlib-ng-0.4.2.tar`

### file list

```diff
@@ -1,400 +1,400 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.671692 zlib-ng-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-03-11 13:35:03.671692 zlib-ng-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 13:35:03.671692 zlib-ng-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.591693 zlib-ng-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.599693 zlib-ng-0.4.1/src/zlib_ng/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/src/zlib_ng/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/src/zlib_ng/gzip_ng.py
--rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/src/zlib_ng/gzip_ng_threaded.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/src/zlib_ng/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.615693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-11 13:30:57.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.git
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.615693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.615693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/analyze.yml
--rw-r--r--   0 runner    (1001) docker     (127)    27791 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/cmake.yml
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/configure.yml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/fuzz.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/libpng.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/link.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/nmake.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/pigz.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/pkgcheck.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.shellcheckrc
--rw-r--r--   0 runner    (1001) docker     (127)    49865 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/FAQ.zlib
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/INDEX.md
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/PORTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/adler32.c
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/adler32_fold.c
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/adler32_fold.h
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/adler32_p.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.615693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.619693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/acle_intrins.h
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/adler32_neon.c
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/arm_features.c
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/arm_features.h
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/chunkset_neon.c
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/compare256_neon.c
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/crc32_acle.c
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/insert_string_acle.c
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/neon_intrins.h
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/slide_hash_armv6.c
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/slide_hash_neon.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.619693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/generic/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/generic/chunk_permute_table.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.619693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/adler32_power8.c
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/adler32_vmx.c
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/chunkset_power8.c
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/compare256_power9.c
--rw-r--r--   0 runner    (1001) docker     (127)    59493 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/crc32_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)    24160 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/crc32_power8.c
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/fallback_builtins.h
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/power_features.c
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/power_features.h
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/slide_hash_power8.c
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/slide_hash_vmx.c
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/slide_ppc_tpl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.623693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/adler32_rvv.c
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/chunkset_rvv.c
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/compare256_rvv.c
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/riscv_features.c
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/riscv_features.h
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/slide_hash_rvv.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.623693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)    12034 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/crc32-vx.c
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_common.c
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_common.h
--rw-r--r--   0 runner    (1001) docker     (127)    15284 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_deflate.c
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_deflate.h
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_detail.h
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_inflate.c
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_inflate.h
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/s390_features.c
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/s390_features.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.623693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/actions-runner.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/actions-runner.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.591693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.591693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.623693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      991 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner
--rwxr-xr-x   0 runner    (1001) docker     (127)      740 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/qemu-user-static.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.631693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx2.c
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx2_p.h
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx2_tpl.h
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512.c
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_p.h
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_tpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_vnni.c
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_sse42.c
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_ssse3.c
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_ssse3_p.h
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/chunkset_avx2.c
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/chunkset_sse2.c
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/chunkset_ssse3.c
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/compare256_avx2.c
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/compare256_sse2.c
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/crc32_fold_pclmulqdq_tpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/crc32_fold_vpclmulqdq_tpl.h
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/crc32_pclmulqdq.c
--rw-r--r--   0 runner    (1001) docker     (127)    13728 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/crc32_pclmulqdq_tpl.h
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/crc32_vpclmulqdq.c
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/insert_string_sse42.c
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/slide_hash_avx2.c
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/slide_hash_sse2.c
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/x86_features.c
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/x86_features.h
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/x86_intrins.h
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/chunkset.c
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/chunkset_tpl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.635693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-arch.c
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-arch.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-coverage.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-install-dirs.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    18385 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-intrinsics.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-sanitizer.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/fallback-macros.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-aarch64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-arm.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-armhf.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-aarch64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-armv7.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-i686.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-x86_64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-mingw-i686.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-mingw-x86_64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-mips.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-mips64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64-clang.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64-power9.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le-clang.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le-power9.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-riscv.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-s390x.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-sparc64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/compare256.c
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/compare256_rle.h
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/compress.c
--rwxr-xr-x   0 runner    (1001) docker     (127)    74420 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/configure
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cpu_features.c
--rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_braid.c
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_braid_comb.c
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_braid_comb_p.h
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_braid_p.h
--rw-r--r--   0 runner    (1001) docker     (127)   591911 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_braid_tbl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_fold.c
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_fold.h
--rw-r--r--   0 runner    (1001) docker     (127)    54204 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate.c
--rw-r--r--   0 runner    (1001) docker     (127)    16264 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate.h
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_fast.c
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_huff.c
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_medium.c
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_p.h
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_quick.c
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_rle.c
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_slow.c
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_stored.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.639693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/algorithm.txt
--rw-r--r--   0 runner    (1001) docker     (127)   776142 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/crc-doc.1.0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   384202 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/crc-pclmulqdq.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    20502 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/rfc1950.txt
--rw-r--r--   0 runner    (1001) docker     (127)    36944 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/rfc1951.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25040 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/rfc1952.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/txtvsbin.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/fallback_builtins.h
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/functable.c
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/functable.h
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/gzguts.h
--rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/gzlib.c
--rw-r--r--   0 runner    (1001) docker     (127)    20491 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/gzread.c.in
--rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/gzwrite.c
--rw-r--r--   0 runner    (1001) docker     (127)    18978 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/infback.c
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inffast_tpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inffixed_tbl.h
--rw-r--r--   0 runner    (1001) docker     (127)    50619 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inflate.c
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inflate.h
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inflate_p.h
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inftrees.c
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inftrees.h
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/insert_string.c
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/insert_string_roll.c
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/insert_string_tpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/match_tpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/slide_hash.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.647693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9500 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.647693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2002-0059/
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2002-0059/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.647693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2004-0797/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2004-0797/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.647693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2005-1849/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2005-1849/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.647693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2005-2096/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2005-2096/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.647693 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2018-25032/
--rw-r--r--   0 runner    (1001) docker     (127)    48192 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2018-25032/default.txt
--rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2018-25032/fixed.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.651692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-1600/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-1600/packobj.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.651692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-361/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-361/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.651692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-364/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-364/test.bin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.651692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-382/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-382/defneg3.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.651692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-751/
--rw-r--r--   0 runner    (1001) docker     (127)   180001 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-751/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.651692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-979/
--rw-r--r--   0 runner    (1001) docker     (127)   106840 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-979/pigz-2.6.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.659692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/ignore
--rw-r--r--   0 runner    (1001) docker     (127)   107877 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-aarch64-unknown-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)   107447 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-arm-unknown-linux-gnueabi.abi
--rw-r--r--   0 runner    (1001) docker     (127)   107505 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-arm-unknown-linux-gnueabihf.abi
--rw-r--r--   0 runner    (1001) docker     (127)    91835 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-mips-unknown-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)    91644 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-mips64-unknown-linux-gnuabi64.abi
--rw-r--r--   0 runner    (1001) docker     (127)   107817 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc-unknown-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)   106939 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc64-unknown-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)   106989 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc64le-unknown-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)   106242 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-x86_64-pc-linux-gnu-m32.abi
--rw-r--r--   0 runner    (1001) docker     (127)   107129 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-x86_64-pc-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)   168992 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-aarch64-unknown-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)   167531 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-arm-unknown-linux-gnueabi.abi
--rw-r--r--   0 runner    (1001) docker     (127)   167122 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-arm-unknown-linux-gnueabihf.abi
--rw-r--r--   0 runner    (1001) docker     (127)   123460 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-mips-unknown-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)   124655 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-mips64-unknown-linux-gnuabi64.abi
--rw-r--r--   0 runner    (1001) docker     (127)   168065 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc-unknown-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)   168877 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc64-unknown-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)   168459 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc64le-unknown-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)   175926 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-x86_64-pc-linux-gnu-m32.abi
--rw-r--r--   0 runner    (1001) docker     (127)   178588 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-x86_64-pc-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abicheck.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     4349 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abicheck.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.659692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/add-subdirectory-project/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/add-subdirectory-project/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/add-subdirectory-project/main.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.659692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_adler32.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_adler32_copy.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_compare256.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_compare256_rle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_crc32.cc
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_main.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_decode.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_encode.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_shared.h
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_slidehash.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.663692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/compress-and-verify.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/run-and-compare.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/run-and-redirect.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/test-cves.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/test-data.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/test-issues.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/test-tools.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.663692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)   123093 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/data/fireworks.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   419233 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/data/lcet10.txt
--rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/data/paper-100k.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    33920 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/example.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.663692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_checksum.c
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_dict.c
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_flush.c
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_large.c
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_small.c
--rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_minigzip.c
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/standalone_fuzz_target_runner.c
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/gh1235.c
--rw-r--r--   0 runner    (1001) docker     (127)    26228 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/infcover.c
--rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/minideflate.c
--rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/minigzip.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.667692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/pigz/
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/pigz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/pkgcheck.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/switchlevels.c
--rw-r--r--   0 runner    (1001) docker     (127)    34864 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_adler32.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_aligned_alloc.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_compare256.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_compare256_rle.cc
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_compress.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_compress_bound.cc
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_compress_dual.cc
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_crc32.cc
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_cve-2003-0107.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_bound.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_concurrency.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_copy.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_dict.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_hash_head_0.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_header.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_params.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_pending.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_prime.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_quick_bi_valid.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_quick_block_open.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_tune.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_dict.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_gzio.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_inflate_adler32.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_inflate_sync.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_large_buffers.cc
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_main.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_raw.cc
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_shared.h
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_shared_ng.h
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_small_buffers.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_small_window.cc
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_version.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.667692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)      678 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/tools/config.sub
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/tools/makecrct.c
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/tools/makefixed.c
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/tools/maketrees.c
--rw-r--r--   0 runner    (1001) docker     (127)    31525 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/trees.c
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/trees.h
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/trees_emit.h
--rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/trees_tbl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/uncompr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.667692 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/
--rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/Makefile.a64
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/Makefile.arm
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/Makefile.msc
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/replace.vbs
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/zlib-ng.def.in
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/zlib-ng1.rc
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/zlib.def.in
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/zlib1.rc
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/zlibcompat.def.in
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zbuild.h
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zconf-ng.h.in
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zconf.h.in
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zendian.h
--rw-r--r--   0 runner    (1001) docker     (127)    92770 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib-ng.h.in
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib-ng.map
--rw-r--r--   0 runner    (1001) docker     (127)    95414 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib.h.in
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib.map
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib.pc.cmakein
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib_name_mangling-ng.h.in
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib_name_mangling.h.empty
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib_name_mangling.h.in
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zutil.c
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zutil.h
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-11 13:30:59.000000 zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zutil_p.h
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/src/zlib_ng/zlib_ng.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    96568 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/src/zlib_ng/zlib_ngmodule.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.667692 zlib-ng-0.4.1/src/zlib_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-03-11 13:35:03.000000 zlib-ng-0.4.1/src/zlib_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-03-11 13:35:03.000000 zlib-ng-0.4.1/src/zlib_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 13:35:03.000000 zlib-ng-0.4.1/src/zlib_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 13:35:03.000000 zlib-ng-0.4.1/src/zlib_ng.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 13:35:03.000000 zlib-ng-0.4.1/src/zlib_ng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:35:03.667692 zlib-ng-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    33505 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/tests/test_gzip_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/tests/test_gzip_ng.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/tests/test_gzip_ng_threaded.py
--rw-r--r--   0 runner    (1001) docker     (127)    44789 2024-03-11 13:30:56.000000 zlib-ng-0.4.1/tests/test_zlib_compliance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.742758 zlib-ng-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-10 11:51:22.738757 zlib-ng-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:51:22.742758 zlib-ng-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.670757 zlib-ng-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.674758 zlib-ng-0.4.2/src/zlib_ng/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/src/zlib_ng/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/src/zlib_ng/gzip_ng.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/src/zlib_ng/gzip_ng_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/src/zlib_ng/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.690758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.git
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.690758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.694758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/analyze.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    27791 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/cmake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/configure.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/fuzz.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/libpng.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/link.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/nmake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/pigz.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/pkgcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.shellcheckrc
+-rw-r--r--   0 runner    (1001) docker     (127)    49865 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/FAQ.zlib
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/INDEX.md
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/PORTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/adler32_fold.c
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/adler32_fold.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/adler32_p.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.694758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.694758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/acle_intrins.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/adler32_neon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/arm_features.c
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/arm_features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/chunkset_neon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/compare256_neon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/crc32_acle.c
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/insert_string_acle.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/neon_intrins.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/slide_hash_armv6.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/slide_hash_neon.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.694758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/generic/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/generic/chunk_permute_table.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.698758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/adler32_power8.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/adler32_vmx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/chunkset_power8.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/compare256_power9.c
+-rw-r--r--   0 runner    (1001) docker     (127)    59493 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/crc32_constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24160 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/crc32_power8.c
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/fallback_builtins.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/power_features.c
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/power_features.h
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/slide_hash_power8.c
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/slide_hash_vmx.c
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/slide_ppc_tpl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.698758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/adler32_rvv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/chunkset_rvv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/compare256_rvv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/riscv_features.c
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/riscv_features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/slide_hash_rvv.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.702757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12034 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/crc32-vx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15284 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_deflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_deflate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_detail.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_inflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_inflate.h
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/s390_features.c
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/s390_features.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.702757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/actions-runner.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/actions-runner.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.670757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.670757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.702757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      991 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner
+-rwxr-xr-x   0 runner    (1001) docker     (127)      740 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/qemu-user-static.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.706757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx2_p.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx2_tpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_p.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_tpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_vnni.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_sse42.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_ssse3.c
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_ssse3_p.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/chunkset_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/chunkset_sse2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/chunkset_ssse3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/compare256_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/compare256_sse2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/crc32_fold_pclmulqdq_tpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/crc32_fold_vpclmulqdq_tpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/crc32_pclmulqdq.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13728 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/crc32_pclmulqdq_tpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/crc32_vpclmulqdq.c
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/insert_string_sse42.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/slide_hash_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/slide_hash_sse2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/x86_features.c
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/x86_features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/x86_intrins.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/chunkset.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/chunkset_tpl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.710758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-arch.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-arch.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-coverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-install-dirs.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    18385 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-intrinsics.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-sanitizer.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/fallback-macros.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-aarch64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-arm.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-armhf.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-aarch64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-armv7.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-i686.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-x86_64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-mingw-i686.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-mingw-x86_64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-mips.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-mips64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64-clang.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64-power9.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le-clang.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le-power9.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-riscv.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-s390x.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-sparc64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/compare256.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/compare256_rle.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/compress.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)    74420 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/configure
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cpu_features.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cpu_features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_braid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_braid_comb.c
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_braid_comb_p.h
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_braid_p.h
+-rw-r--r--   0 runner    (1001) docker     (127)   591911 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_braid_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_fold.c
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_fold.h
+-rw-r--r--   0 runner    (1001) docker     (127)    54204 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16264 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_fast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_huff.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_medium.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_p.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_quick.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_rle.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_slow.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_stored.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.714758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/algorithm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   776142 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/crc-doc.1.0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   384202 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/crc-pclmulqdq.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    20502 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/rfc1950.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36944 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/rfc1951.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25040 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/rfc1952.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/txtvsbin.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/fallback_builtins.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/functable.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/functable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/gzguts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/gzlib.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20491 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/gzread.c.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/gzwrite.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18978 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/infback.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inffast_tpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inffixed_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    50619 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inflate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inflate_p.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inftrees.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inftrees.h
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/insert_string.c
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/insert_string_roll.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/insert_string_tpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/match_tpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/slide_hash.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9500 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2002-0059/
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2002-0059/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2004-0797/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2004-0797/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2005-1849/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2005-1849/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2005-2096/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2005-2096/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2018-25032/
+-rw-r--r--   0 runner    (1001) docker     (127)    48192 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2018-25032/default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2018-25032/fixed.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-1600/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-1600/packobj.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-361/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-361/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-364/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-364/test.bin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-382/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-382/defneg3.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-751/
+-rw-r--r--   0 runner    (1001) docker     (127)   180001 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-751/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.722757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-979/
+-rw-r--r--   0 runner    (1001) docker     (127)   106840 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-979/pigz-2.6.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.730758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/ignore
+-rw-r--r--   0 runner    (1001) docker     (127)   107877 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-aarch64-unknown-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   107447 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-arm-unknown-linux-gnueabi.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   107505 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-arm-unknown-linux-gnueabihf.abi
+-rw-r--r--   0 runner    (1001) docker     (127)    91835 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-mips-unknown-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)    91644 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-mips64-unknown-linux-gnuabi64.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   107817 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc-unknown-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   106939 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc64-unknown-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   106989 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc64le-unknown-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   106242 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-x86_64-pc-linux-gnu-m32.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   107129 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-x86_64-pc-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   168992 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-aarch64-unknown-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   167531 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-arm-unknown-linux-gnueabi.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   167122 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-arm-unknown-linux-gnueabihf.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   123460 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-mips-unknown-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   124655 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-mips64-unknown-linux-gnuabi64.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   168065 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc-unknown-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   168877 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc64-unknown-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   168459 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc64le-unknown-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   175926 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-x86_64-pc-linux-gnu-m32.abi
+-rw-r--r--   0 runner    (1001) docker     (127)   178588 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-x86_64-pc-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abicheck.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4349 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abicheck.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.730758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/add-subdirectory-project/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/add-subdirectory-project/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/add-subdirectory-project/main.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.734758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_adler32.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_adler32_copy.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_compare256.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_compare256_rle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_crc32.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_decode.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_encode.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_shared.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_slidehash.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.734758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/compress-and-verify.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/run-and-compare.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/run-and-redirect.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/test-cves.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/test-data.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/test-issues.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/test-tools.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.734758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   123093 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/data/fireworks.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   419233 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/data/lcet10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/data/paper-100k.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    33920 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/example.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.734758 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_checksum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_dict.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_flush.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_large.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_small.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_minigzip.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/standalone_fuzz_target_runner.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/gh1235.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26228 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/infcover.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/minideflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/minigzip.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.738757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/pigz/
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/pigz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/pkgcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/switchlevels.c
+-rw-r--r--   0 runner    (1001) docker     (127)    34864 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_adler32.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_aligned_alloc.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_compare256.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_compare256_rle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_compress.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_compress_bound.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_compress_dual.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_cpu_features.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_crc32.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_cve-2003-0107.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_bound.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_concurrency.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_copy.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_dict.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_hash_head_0.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_header.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_params.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_pending.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_prime.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_quick_bi_valid.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_quick_block_open.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_tune.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_dict.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_gzio.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_inflate_adler32.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_inflate_sync.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_large_buffers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_raw.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_shared.h
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_shared_ng.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_small_buffers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_small_window.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_version.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.738757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      678 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/tools/config.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/tools/makecrct.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/tools/makefixed.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/tools/maketrees.c
+-rw-r--r--   0 runner    (1001) docker     (127)    31525 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/trees.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/trees.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/trees_emit.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/trees_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/uncompr.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.738757 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/Makefile.a64
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/Makefile.arm
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/Makefile.msc
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/replace.vbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/zlib-ng.def.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/zlib-ng1.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/zlib.def.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/zlib1.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/zlibcompat.def.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zbuild.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zconf-ng.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zconf.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zendian.h
+-rw-r--r--   0 runner    (1001) docker     (127)    92770 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib-ng.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib-ng.map
+-rw-r--r--   0 runner    (1001) docker     (127)    95414 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib.map
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib.pc.cmakein
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib_name_mangling-ng.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib_name_mangling.h.empty
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib_name_mangling.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zutil.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zutil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-10 11:47:25.000000 zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zutil_p.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/src/zlib_ng/zlib_ng.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    96592 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/src/zlib_ng/zlib_ngmodule.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.738757 zlib-ng-0.4.2/src/zlib_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-10 11:51:22.000000 zlib-ng-0.4.2/src/zlib_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-04-10 11:51:22.000000 zlib-ng-0.4.2/src/zlib_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:51:22.000000 zlib-ng-0.4.2/src/zlib_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:51:22.000000 zlib-ng-0.4.2/src/zlib_ng.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 11:51:22.000000 zlib-ng-0.4.2/src/zlib_ng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:51:22.738757 zlib-ng-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33505 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/tests/test_gzip_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/tests/test_gzip_ng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/tests/test_gzip_ng_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44789 2024-04-10 11:47:24.000000 zlib-ng-0.4.2/tests/test_zlib_compliance.py
```

### Comparing `zlib-ng-0.4.1/LICENSE` & `zlib-ng-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/PKG-INFO` & `zlib-ng-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlib-ng
-Version: 0.4.1
+Version: 0.4.2
 Summary: Drop-in replacement for zlib and gzip modules using zlib-ng
 Home-page: https://github.com/pycompression/python-zlib-ng
 Author: Leiden University Medical Center
 Author-email: r.h.p.vorderman@lumc.nl
 License: PSF-2.0
 Keywords: zlib-ng zlib compression deflate gzip
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `zlib-ng-0.4.1/README.rst` & `zlib-ng-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/setup.py` & `zlib-ng-0.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,16 @@
     # it.
     build_env = os.environ.copy()
     build_env["CFLAGS"] = build_env.get("CFLAGS", "") + " -fPIC"
     # Add -fPIC flag to allow static compilation
     run_args = dict(cwd=build_dir, env=build_env)
     if sys.platform == "darwin":  # Cmake does not work properly
         subprocess.run([os.path.join(build_dir, "configure")], **run_args)
-        subprocess.run(["gmake", "libz-ng.a"], **run_args)
+        make_program = "gmake" if shutil.which("gmake") else "make"
+        subprocess.run([make_program, "libz-ng.a"], **run_args)
     elif sys.platform == "linux":
         subprocess.run([os.path.join(build_dir, "configure")], **run_args)
         subprocess.run(["make", "libz-ng.a", "-j", str(cpu_count)], **run_args)
     else:
         subprocess.run(["cmake", build_dir], **run_args)
         # Do not create test suite and do not perform tests to shorten build times.
         # There is no need when stable releases of zlib-ng are used.
@@ -119,15 +120,15 @@
     if BUILD_CACHE:
         BUILD_CACHE_FILE.write_text(build_dir)
     return build_dir
 
 
 setup(
     name="zlib-ng",
-    version="0.4.1",
+    version="0.4.2",
     description="Drop-in replacement for zlib and gzip modules using zlib-ng",
     author="Leiden University Medical Center",
     author_email="r.h.p.vorderman@lumc.nl",  # A placeholder for now
     long_description=Path("README.rst").read_text(),
     long_description_content_type="text/x-rst",
     cmdclass={"build_ext": BuildZlibNGExt},
     license="PSF-2.0",
```

### Comparing `zlib-ng-0.4.1/src/zlib_ng/gzip_ng.py` & `zlib-ng-0.4.2/src/zlib_ng/gzip_ng.py`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/gzip_ng_threaded.py` & `zlib-ng-0.4.2/src/zlib_ng/gzip_ng_threaded.py`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/analyze.yml` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/analyze.yml`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/cmake.yml` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/cmake.yml`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/codeql.yml` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/configure.yml` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/fuzz.yml` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/libpng.yml` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/libpng.yml`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/link.yml` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/link.yml`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/nmake.yml` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/nmake.yml`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/pigz.yml` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/pigz.yml`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/pkgcheck.yml` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/pkgcheck.yml`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.github/workflows/release.yml` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.gitignore` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.gitignore`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/.shellcheckrc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/.shellcheckrc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/CMakeLists.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/FAQ.zlib` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/FAQ.zlib`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/INDEX.md` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/INDEX.md`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/LICENSE.md` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/Makefile.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/Makefile.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/PORTING.md` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/PORTING.md`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/README.md` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/README.md`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/adler32.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/adler32.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/adler32_p.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/adler32_p.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/Makefile.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/Makefile.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/acle_intrins.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/acle_intrins.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/adler32_neon.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/adler32_neon.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/arm_features.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/arm_features.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/chunkset_neon.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/chunkset_neon.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/compare256_neon.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/compare256_neon.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/crc32_acle.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/crc32_acle.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/insert_string_acle.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/insert_string_acle.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/neon_intrins.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/neon_intrins.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/slide_hash_armv6.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/slide_hash_armv6.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/arm/slide_hash_neon.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/arm/slide_hash_neon.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/generic/chunk_permute_table.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/generic/chunk_permute_table.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/Makefile.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/Makefile.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/adler32_power8.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/adler32_power8.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/adler32_vmx.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/adler32_vmx.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/chunkset_power8.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/chunkset_power8.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/compare256_power9.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/compare256_power9.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/crc32_constants.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/crc32_constants.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/crc32_power8.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/crc32_power8.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/fallback_builtins.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/fallback_builtins.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/power_features.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/power_features.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/power/slide_ppc_tpl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/power/slide_ppc_tpl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/README.md` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/README.md`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/adler32_rvv.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/adler32_rvv.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/chunkset_rvv.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/chunkset_rvv.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/compare256_rvv.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/compare256_rvv.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/riscv_features.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/riscv_features.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/riscv/slide_hash_rvv.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/riscv/slide_hash_rvv.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/Makefile.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/Makefile.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/README.md` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/README.md`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/crc32-vx.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/crc32-vx.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_common.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_common.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_common.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_common.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_deflate.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_deflate.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_deflate.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_deflate.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_detail.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_detail.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_inflate.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_inflate.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/dfltcc_inflate.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/dfltcc_inflate.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/actions-runner.Dockerfile` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/actions-runner.Dockerfile`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/actions-runner.service` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/actions-runner.service`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/Makefile.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/Makefile.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx2_p.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx2_p.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx2_tpl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx2_tpl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_p.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_p.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_tpl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_tpl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_vnni.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_avx512_vnni.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_sse42.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_sse42.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_ssse3.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_ssse3.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/adler32_ssse3_p.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/adler32_ssse3_p.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/chunkset_avx2.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/chunkset_avx2.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/chunkset_sse2.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/chunkset_sse2.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/chunkset_ssse3.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/chunkset_ssse3.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/compare256_avx2.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/compare256_avx2.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/compare256_sse2.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/compare256_sse2.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/crc32_fold_pclmulqdq_tpl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/crc32_fold_pclmulqdq_tpl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/crc32_fold_vpclmulqdq_tpl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/crc32_fold_vpclmulqdq_tpl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/crc32_pclmulqdq.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/crc32_pclmulqdq.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/crc32_pclmulqdq_tpl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/crc32_pclmulqdq_tpl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/crc32_vpclmulqdq.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/crc32_vpclmulqdq.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/insert_string_sse42.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/insert_string_sse42.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/slide_hash_avx2.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/slide_hash_avx2.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/slide_hash_sse2.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/slide_hash_sse2.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/x86_features.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/x86_features.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/x86_features.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/x86_features.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/arch/x86/x86_intrins.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/arch/x86/x86_intrins.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/chunkset.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/chunkset.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/chunkset_tpl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/chunkset_tpl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-arch.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-arch.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-arch.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-arch.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-coverage.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-coverage.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-install-dirs.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-install-dirs.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-intrinsics.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-intrinsics.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/detect-sanitizer.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/detect-sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/fallback-macros.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/fallback-macros.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-aarch64.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-aarch64.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-arm.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-arm.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-armhf.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-armhf.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-aarch64.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-aarch64.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-armv7.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-armv7.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-i686.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-i686.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-x86_64.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-llvm-mingw-x86_64.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-mingw-i686.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-mingw-i686.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-mingw-x86_64.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-mingw-x86_64.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-mips.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-mips.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-mips64.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-mips64.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64-clang.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64-clang.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64-power9.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64-power9.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le-clang.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le-clang.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le-power9.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le-power9.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-powerpc64le.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-riscv.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-riscv.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-s390x.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-s390x.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cmake/toolchain-sparc64.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cmake/toolchain-sparc64.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/compare256.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/compare256.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/compare256_rle.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/compare256_rle.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/compress.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/compress.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/configure` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/configure`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cpu_features.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cpu_features.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/cpu_features.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/cpu_features.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_braid.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_braid.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_braid_comb.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_braid_comb.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_braid_comb_p.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_braid_comb_p.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_braid_p.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_braid_p.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_braid_tbl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_braid_tbl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_fold.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_fold.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/crc32_fold.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/crc32_fold.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_fast.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_fast.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_huff.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_huff.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_medium.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_medium.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_p.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_p.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_quick.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_quick.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_rle.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_rle.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_slow.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_slow.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/deflate_stored.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/deflate_stored.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/algorithm.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/algorithm.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/crc-doc.1.0.pdf` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/crc-doc.1.0.pdf`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/crc-pclmulqdq.pdf` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/crc-pclmulqdq.pdf`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/rfc1950.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/rfc1950.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/rfc1951.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/rfc1951.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/rfc1952.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/rfc1952.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/doc/txtvsbin.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/doc/txtvsbin.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/fallback_builtins.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/fallback_builtins.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/functable.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/functable.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/functable.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/functable.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/gzguts.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/gzguts.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/gzlib.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/gzlib.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/gzread.c.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/gzread.c.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/gzwrite.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/gzwrite.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/infback.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/infback.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inffast_tpl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inffast_tpl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inffixed_tbl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inffixed_tbl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inflate.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inflate.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inflate.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inflate.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inflate_p.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inflate_p.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inftrees.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inftrees.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/inftrees.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/inftrees.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/insert_string.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/insert_string.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/insert_string_roll.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/insert_string_roll.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/insert_string_tpl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/insert_string_tpl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/match_tpl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/match_tpl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/slide_hash.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/slide_hash.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CMakeLists.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2002-0059/test.gz` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2002-0059/test.gz`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2018-25032/default.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2018-25032/default.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/CVE-2018-25032/fixed.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/CVE-2018-25032/fixed.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/GH-979/pigz-2.6.tar.gz` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/GH-979/pigz-2.6.tar.gz`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/Makefile.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/Makefile.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/README.md` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/README.md`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-aarch64-unknown-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-aarch64-unknown-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-arm-unknown-linux-gnueabi.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-arm-unknown-linux-gnueabi.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-arm-unknown-linux-gnueabihf.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-arm-unknown-linux-gnueabihf.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-mips-unknown-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-mips-unknown-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-mips64-unknown-linux-gnuabi64.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-mips64-unknown-linux-gnuabi64.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc-unknown-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc-unknown-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc64-unknown-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc64-unknown-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc64le-unknown-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-powerpc64le-unknown-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-x86_64-pc-linux-gnu-m32.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-x86_64-pc-linux-gnu-m32.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-x86_64-pc-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-04f42ceca40f73e2978b50e93806c2a18c1281fc-x86_64-pc-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-aarch64-unknown-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-aarch64-unknown-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-arm-unknown-linux-gnueabi.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-arm-unknown-linux-gnueabi.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-arm-unknown-linux-gnueabihf.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-arm-unknown-linux-gnueabihf.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-mips-unknown-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-mips-unknown-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-mips64-unknown-linux-gnuabi64.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-mips64-unknown-linux-gnuabi64.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc-unknown-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc-unknown-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc64-unknown-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc64-unknown-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc64le-unknown-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-powerpc64le-unknown-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-x86_64-pc-linux-gnu-m32.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-x86_64-pc-linux-gnu-m32.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-x86_64-pc-linux-gnu.abi` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abi/zlib-ng-e4614ebcb9b3e5b108dc983c155e4baf80882311-x86_64-pc-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abicheck.md` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abicheck.md`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/abicheck.sh` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/abicheck.sh`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/CMakeLists.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/README.md` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_adler32.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_adler32.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_adler32_copy.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_adler32_copy.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_compare256.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_compare256.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_compare256_rle.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_compare256_rle.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_crc32.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_crc32.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_main.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_main.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_decode.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_decode.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_encode.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_encode.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_shared.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_png_shared.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_slidehash.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/benchmarks/benchmark_slidehash.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/compress-and-verify.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/compress-and-verify.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/run-and-compare.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/run-and-compare.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/run-and-redirect.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/run-and-redirect.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/test-cves.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/test-cves.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/test-data.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/test-data.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/test-issues.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/test-issues.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/cmake/test-tools.cmake` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/cmake/test-tools.cmake`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/data/fireworks.jpg` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/data/fireworks.jpg`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/data/lcet10.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/data/lcet10.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/data/paper-100k.pdf` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/data/paper-100k.pdf`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/example.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/example.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/CMakeLists.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_checksum.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_checksum.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_compress.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_compress.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_dict.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_dict.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_flush.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_flush.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_large.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_large.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_small.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_example_small.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_minigzip.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/fuzzer_minigzip.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/fuzz/standalone_fuzz_target_runner.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/fuzz/standalone_fuzz_target_runner.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/gh1235.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/gh1235.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/infcover.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/infcover.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/minideflate.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/minideflate.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/minigzip.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/minigzip.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/pigz/CMakeLists.txt` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/pigz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/pkgcheck.sh` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/pkgcheck.sh`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/switchlevels.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/switchlevels.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_adler32.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_adler32.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_aligned_alloc.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_aligned_alloc.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_compare256.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_compare256.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_compare256_rle.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_compare256_rle.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_compress.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_compress.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_compress_bound.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_compress_bound.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_compress_dual.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_compress_dual.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_crc32.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_crc32.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_cve-2003-0107.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_cve-2003-0107.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_bound.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_bound.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_concurrency.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_concurrency.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_copy.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_copy.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_dict.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_dict.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_hash_head_0.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_hash_head_0.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_header.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_header.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_params.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_params.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_pending.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_pending.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_prime.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_prime.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_quick_bi_valid.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_quick_bi_valid.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_quick_block_open.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_quick_block_open.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_deflate_tune.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_deflate_tune.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_dict.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_dict.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_gzio.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_gzio.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_inflate_adler32.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_inflate_adler32.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_inflate_sync.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_inflate_sync.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_large_buffers.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_large_buffers.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_raw.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_raw.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_shared.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_shared.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_shared_ng.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_shared_ng.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_small_buffers.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_small_buffers.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_small_window.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_small_window.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/test/test_version.cc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/test/test_version.cc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/tools/config.sub` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/tools/config.sub`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/tools/makecrct.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/tools/makecrct.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/tools/makefixed.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/tools/makefixed.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/tools/maketrees.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/tools/maketrees.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/trees.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/trees.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/trees.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/trees.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/trees_emit.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/trees_emit.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/trees_tbl.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/trees_tbl.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/uncompr.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/uncompr.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/Makefile.a64` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/Makefile.a64`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/Makefile.arm` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/Makefile.arm`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/Makefile.msc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/Makefile.msc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/zlib-ng.def.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/zlib-ng.def.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/zlib-ng1.rc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/zlib-ng1.rc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/zlib.def.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/zlib.def.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/zlib1.rc` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/zlib1.rc`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/win32/zlibcompat.def.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/win32/zlibcompat.def.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zbuild.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zbuild.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zconf-ng.h.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zconf-ng.h.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zconf.h.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zconf.h.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zendian.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zendian.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib-ng.h.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib-ng.h.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib-ng.map` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib-ng.map`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib.h.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib.h.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib.map` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib.map`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib_name_mangling-ng.h.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib_name_mangling-ng.h.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zlib_name_mangling.h.in` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zlib_name_mangling.h.in`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zutil.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zutil.c`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zutil.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zutil.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib-ng/zutil_p.h` & `zlib-ng-0.4.2/src/zlib_ng/zlib-ng/zutil_p.h`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib_ng.pyi` & `zlib-ng-0.4.2/src/zlib_ng/zlib_ng.pyi`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/src/zlib_ng/zlib_ngmodule.c` & `zlib-ng-0.4.2/src/zlib_ng/zlib_ngmodule.c`

 * *Files 0% similar despite different names*

```diff
@@ -3057,14 +3057,15 @@
     if (ver != NULL)
         PyModule_AddObject(m, "ZLIBNG_RUNTIME_VERSION", ver);
 
     /* Add latest compatible zlib version */
     ver = PyUnicode_FromString("1.2.12");
     if (ver!= NULL) {
         PyModule_AddObject(m, "ZLIB_VERSION", ver);
+        Py_INCREF(ver);
         PyModule_AddObject(m, "ZLIB_RUNTIME_VERSION", ver);
     }
 
     PyModule_AddStringConstant(m, "__version__", "1.0");
 
     return m;
 }
```

### Comparing `zlib-ng-0.4.1/src/zlib_ng.egg-info/PKG-INFO` & `zlib-ng-0.4.2/src/zlib_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlib-ng
-Version: 0.4.1
+Version: 0.4.2
 Summary: Drop-in replacement for zlib and gzip modules using zlib-ng
 Home-page: https://github.com/pycompression/python-zlib-ng
 Author: Leiden University Medical Center
 Author-email: r.h.p.vorderman@lumc.nl
 License: PSF-2.0
 Keywords: zlib-ng zlib compression deflate gzip
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `zlib-ng-0.4.1/src/zlib_ng.egg-info/SOURCES.txt` & `zlib-ng-0.4.2/src/zlib_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/tests/test_compat.py` & `zlib-ng-0.4.2/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/tests/test_gzip_compliance.py` & `zlib-ng-0.4.2/tests/test_gzip_compliance.py`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/tests/test_gzip_ng.py` & `zlib-ng-0.4.2/tests/test_gzip_ng.py`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/tests/test_gzip_ng_threaded.py` & `zlib-ng-0.4.2/tests/test_gzip_ng_threaded.py`

 * *Files identical despite different names*

### Comparing `zlib-ng-0.4.1/tests/test_zlib_compliance.py` & `zlib-ng-0.4.2/tests/test_zlib_compliance.py`

 * *Files identical despite different names*

