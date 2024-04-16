# Comparing `tmp/linktools-0.8.3rc1.tar.gz` & `tmp/linktools-0.8.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktools-0.8.3rc1.tar", last modified: Fri Apr  5 13:46:49 2024, max compression
+gzip compressed data, was "linktools-0.8.4rc0.tar", last modified: Tue Apr 16 08:50:18 2024, max compression
```

## Comparing `linktools-0.8.3rc1.tar` & `linktools-0.8.4rc0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.452102 linktools-0.8.3rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    35093 2024-04-05 13:46:49.448102 linktools-0.8.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33179 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:46:49.452102 linktools-0.8.3rc1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.424102 linktools-0.8.3rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.432102 linktools-0.8.3rc1/src/linktools/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.432102 linktools-0.8.3rc1/src/linktools/android/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/android/adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/android/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-04-05 13:46:39.000000 linktools-0.8.3rc1/src/linktools/assets/android-tools.apk
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-05 13:46:39.000000 linktools-0.8.3rc1/src/linktools/assets/android-tools.json
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/chrome-driver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.428102 linktools-0.8.3rc1/src/linktools/assets/containers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/dnsapi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/http.conf
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/https.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/assets/containers/110-portainer/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/110-portainer/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/110-portainer/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/110-portainer/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/fake_useragent.json
--rw-r--r--   0 runner    (1001) docker     (127)    51432 2024-04-05 13:44:38.000000 linktools-0.8.3rc1/src/linktools/assets/frida.js
--rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-05 13:44:38.000000 linktools-0.8.3rc1/src/linktools/assets/frida.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.428102 linktools-0.8.3rc1/src/linktools/assets/objection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/assets/objection/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/objection/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools/assets/tools.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    30240 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.440102 linktools-0.8.3rc1/src/linktools/cli/commands/android/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/adb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15337 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/debug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/objection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/pidcat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/top.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.440102 linktools-0.8.3rc1/src/linktools/cli/commands/common/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/cntr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/grep.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4118 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.440102 linktools-0.8.3rc1/src/linktools/cli/commands/ios/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/objection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/container/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16099 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/container/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/container/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/container/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/frida/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/android.py
--rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/ida/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ida/ida.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/ios/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/reactor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/references/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/references/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.448102 linktools-0.8.3rc1/src/linktools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/utils/_lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/utils/_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/utils/_subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18061 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.448102 linktools-0.8.3rc1/src/linktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35093 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.993133 linktools-0.8.4rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-16 08:50:18.993133 linktools-0.8.4rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32997 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:50:18.993133 linktools-0.8.4rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.969134 linktools-0.8.4rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.973134 linktools-0.8.4rc0/src/linktools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/android/adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/android/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-04-16 08:50:09.000000 linktools-0.8.4rc0/src/linktools/assets/android-tools.apk
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-16 08:50:09.000000 linktools-0.8.4rc0/src/linktools/assets/android-tools.json
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/chrome-driver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.969134 linktools-0.8.4rc0/src/linktools/assets/containers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/http.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/https.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/fake_useragent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-04-16 08:48:13.000000 linktools-0.8.4rc0/src/linktools/assets/frida.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-16 08:48:13.000000 linktools-0.8.4rc0/src/linktools/assets/frida.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.969134 linktools-0.8.4rc0/src/linktools/assets/objection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/assets/objection/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/objection/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools/assets/tools.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31589 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/commands/android/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/adb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15337 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/debug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/objection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/pidcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/top.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/commands/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15194 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/cntr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/grep.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4134 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/cli/commands/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/objection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/frida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ida/ida.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/reactor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.989133 linktools-0.8.4rc0/src/linktools/references/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.989133 linktools-0.8.4rc0/src/linktools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19460 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.989133 linktools-0.8.4rc0/src/linktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/top_level.txt
```

### Comparing `linktools-0.8.3rc1/LICENSE` & `linktools-0.8.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/PKG-INFO` & `linktools-0.8.4rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.3rc1
+Version: 0.8.4rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -27,62 +27,60 @@
 Requires-Dist: scp; extra == "ssh"
 Provides-Extra: ssl
 Requires-Dist: pyOpenSSL; extra == "ssl"
 Provides-Extra: container
 Requires-Dist: GitPython; extra == "container"
 Requires-Dist: jinja2; extra == "container"
 Requires-Dist: pyyaml; extra == "container"
+Provides-Extra: argcomplete
+Requires-Dist: argcomplete>=2.0.0; extra == "argcomplete"
 Provides-Extra: all
 Requires-Dist: requests[socks]; extra == "all"
 Requires-Dist: frida>=15.0.0; extra == "all"
 Requires-Dist: objection; extra == "all"
 Requires-Dist: lief>0.10.1; extra == "all"
 Requires-Dist: python-magic; platform_system == "Linux" and extra == "all"
 Requires-Dist: python-magic; platform_system == "Darwin" and extra == "all"
 Requires-Dist: python-magic-bin; platform_system == "Windows" and extra == "all"
 Requires-Dist: paramiko; extra == "all"
 Requires-Dist: scp; extra == "all"
 Requires-Dist: pyOpenSSL; extra == "all"
 Requires-Dist: GitPython; extra == "all"
 Requires-Dist: jinja2; extra == "all"
 Requires-Dist: pyyaml; extra == "all"
+Requires-Dist: argcomplete>=2.0.0; extra == "all"
 
 # Linktools Toolkit
 
 ## 开始使用
 
 ### 依赖项
 
 python & pip (3.6及以上): <https://www.python.org/downloads/>
 
 ### 安装
 
 使用pip安装linktools
 
 ```bash
-# 可以pip直接安装linktools，也可以用以下命令安装github上的最新版本:
-# python3 -m pip install "linktools@ git+https://github.com/ice-black-tea/Zelda.git"
-python3 -m pip install -U "linktools[all]" # 按需添加依赖项，推荐使用all添加所有依赖项
+# pip直接安装linktools，按需添加依赖项，推荐使用all添加所有依赖项
+python3 -m pip install -U "linktools[all]"
+# 也可以用以下命令安装github上的最新版本:
+# python3 -m pip install --ignore-installed "linktools@ git+https://github.com/ice-black-tea/linktools.git@master"
 ```
 
-额外的依赖项以及相应功能如下：
-```
-linktools[requests]：下载时使用requests包，并且支持socks5代理
-linktools[lief]：为grep提供服务，可解析apk、elf等文件格式（注意：对于mac系统，需要额外安装brew install libmagic）
-linktools[frida]：集成frida hook框架，支持android、ios hook
-linktooks[objection]：集成objection框架
-linktools[ssh]：使用ssh连接越狱后的iphone
-linktools[ssl]：解析证书时使用
-```
+额外的依赖项以及相应功能可通过[requirements.yml](https://raw.githubusercontent.com/ice-black-tea/linktools/master/requirements.yml)查看
 
 ### 配置alias（推荐）
 
 对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置alias，简化调用方式：
 
 ```bash
+eval "$(ct-env --silent complete --shell bash)" # 给命令添加自动补全功能
+
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
 alias apktool="ct-tools apktool"
 alias burpsuite="ct-tools --set version=2023.10 burpsuite"
 alias jadx="JAVA_OPTS=-Xmx8g ct-tools --set version=1.4.7 jadx-gui" # 指定jadx版本号，配置jvm最大内存
@@ -205,15 +203,15 @@
 </details>
 
 #### 👉 ct-tools
 
 <details>
 <summary>读取配置文件，即可下载使用对应工具，声明了adb、jadx、apktool、baksmali等常用工具</summary>
 
-所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/src/linktools/assets/tools.yml)查看
+所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/assets/tools.yml)查看
 
 ```
 $ usage: ct-tools [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-c | --download | --clear | -d] ...
 
 Tools downloaded from the web
 
     ___       __   __              __
@@ -483,15 +481,15 @@
   -c IP[:PORT], --connect IP[:PORT]
                         use device with TCP/IP
   -l, --last            use last device
 ```
 
 **输出效果**
 
-![apps](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/images/apps.png)
+![apps](https://raw.githubusercontent.com/ice-black-tea/linktools/master/images/apps.png)
 
 </details>
 
 #### 👉 at-frida
 
 <details>
 <summary>该功能旨在方便使用frida，可自动下载server，支持加载远程脚本，并内置了常用功能</summary>
@@ -546,29 +544,29 @@
   --emulator            use TCP/IP device (adb -e option)
   --connect IP[:PORT]   use device with TCP/IP
   --last                use last device
 ```
 
 **1) 以命令行方式运行**
 
-比如要加载 [https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js) 脚本：
+比如要加载 [https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js](https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js) 脚本：
 
 在终端中运行
 ```bash
-$ at-frida -c https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js
+$ at-frida -c https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js
 ```
 
 输出如下：
 ```
-[15:24:09]  I  Download ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js)
+[15:24:09]  I  Download ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js)
 [15:24:11]  W  java.js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1,704/513 bytes ? 100% eta 0:00:00
-[15:24:13]  I  Load trusted ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js)
+[15:24:13]  I  Load trusted ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js)
 [15:24:14]  I  Start frida server ...
 [15:24:15]  I  Frida server is running ...
-[15:24:18]  I  Load ScriptFile(filename=/Users/huji/Projects/Zelda/src/linktools/assets/frida.min.js)
+[15:24:18]  I  Load ScriptFile(filename=/Users/huji/Projects/linktools/src/linktools/assets/frida.min.js)
 [15:24:19]  I  Session(pid=32087, name=马赛克) attached
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.access$300()
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.access$600()
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.decode(java.lang.String)
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.encode(java.lang.String)
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.encode(java.lang.String, java.lang.String)
 [15:24:19]  I  Hook method: android.net.Uri android.net.Uri.fromFile(java.io.File)
@@ -673,15 +671,15 @@
                    "java.lang.Thread.run(Thread.java:923)"
                  ]
                }
 ```
 
 **2) 当然也可以使用python方式调用**
 
-执行如下python脚本即可自动开启frida-server，并将js代码注入到指定进程中，若需要同时注入子进程，按[src/linktools/cli/scripts/android/frida.py](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/src/linktools/cli/scripts/android/frida.py) 重写 FridaApplication 的 on_spawn_added 方法即可
+执行如下python脚本即可自动开启frida-server，并将js代码注入到指定进程中，若需要同时注入子进程，按[src/linktools/cli/scripts/android/frida.py](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/cli/scripts/android/frida.py) 重写 FridaApplication 的 on_spawn_added 方法即可
 
 ```python
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import logging
 from linktools.frida import FridaApplication, FridaEvalCode
 from linktools.frida.android import AndroidFridaServer
```

### Comparing `linktools-0.8.3rc1/README.md` & `linktools-0.8.4rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,29 @@
 python & pip (3.6及以上): <https://www.python.org/downloads/>
 
 ### 安装
 
 使用pip安装linktools
 
 ```bash
-# 可以pip直接安装linktools，也可以用以下命令安装github上的最新版本:
-# python3 -m pip install "linktools@ git+https://github.com/ice-black-tea/Zelda.git"
-python3 -m pip install -U "linktools[all]" # 按需添加依赖项，推荐使用all添加所有依赖项
+# pip直接安装linktools，按需添加依赖项，推荐使用all添加所有依赖项
+python3 -m pip install -U "linktools[all]"
+# 也可以用以下命令安装github上的最新版本:
+# python3 -m pip install --ignore-installed "linktools@ git+https://github.com/ice-black-tea/linktools.git@master"
 ```
 
-额外的依赖项以及相应功能如下：
-```
-linktools[requests]：下载时使用requests包，并且支持socks5代理
-linktools[lief]：为grep提供服务，可解析apk、elf等文件格式（注意：对于mac系统，需要额外安装brew install libmagic）
-linktools[frida]：集成frida hook框架，支持android、ios hook
-linktooks[objection]：集成objection框架
-linktools[ssh]：使用ssh连接越狱后的iphone
-linktools[ssl]：解析证书时使用
-```
+额外的依赖项以及相应功能可通过[requirements.yml](https://raw.githubusercontent.com/ice-black-tea/linktools/master/requirements.yml)查看
 
 ### 配置alias（推荐）
 
 对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置alias，简化调用方式：
 
 ```bash
+eval "$(ct-env --silent complete --shell bash)" # 给命令添加自动补全功能
+
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
 alias apktool="ct-tools apktool"
 alias burpsuite="ct-tools --set version=2023.10 burpsuite"
 alias jadx="JAVA_OPTS=-Xmx8g ct-tools --set version=1.4.7 jadx-gui" # 指定jadx版本号，配置jvm最大内存
@@ -157,15 +152,15 @@
 </details>
 
 #### 👉 ct-tools
 
 <details>
 <summary>读取配置文件，即可下载使用对应工具，声明了adb、jadx、apktool、baksmali等常用工具</summary>
 
-所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/src/linktools/assets/tools.yml)查看
+所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/assets/tools.yml)查看
 
 ```
 $ usage: ct-tools [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-c | --download | --clear | -d] ...
 
 Tools downloaded from the web
 
     ___       __   __              __
@@ -435,15 +430,15 @@
   -c IP[:PORT], --connect IP[:PORT]
                         use device with TCP/IP
   -l, --last            use last device
 ```
 
 **输出效果**
 
-![apps](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/images/apps.png)
+![apps](https://raw.githubusercontent.com/ice-black-tea/linktools/master/images/apps.png)
 
 </details>
 
 #### 👉 at-frida
 
 <details>
 <summary>该功能旨在方便使用frida，可自动下载server，支持加载远程脚本，并内置了常用功能</summary>
@@ -498,29 +493,29 @@
   --emulator            use TCP/IP device (adb -e option)
   --connect IP[:PORT]   use device with TCP/IP
   --last                use last device
 ```
 
 **1) 以命令行方式运行**
 
-比如要加载 [https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js) 脚本：
+比如要加载 [https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js](https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js) 脚本：
 
 在终端中运行
 ```bash
-$ at-frida -c https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js
+$ at-frida -c https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js
 ```
 
 输出如下：
 ```
-[15:24:09]  I  Download ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js)
+[15:24:09]  I  Download ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js)
 [15:24:11]  W  java.js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1,704/513 bytes ? 100% eta 0:00:00
-[15:24:13]  I  Load trusted ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js)
+[15:24:13]  I  Load trusted ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js)
 [15:24:14]  I  Start frida server ...
 [15:24:15]  I  Frida server is running ...
-[15:24:18]  I  Load ScriptFile(filename=/Users/huji/Projects/Zelda/src/linktools/assets/frida.min.js)
+[15:24:18]  I  Load ScriptFile(filename=/Users/huji/Projects/linktools/src/linktools/assets/frida.min.js)
 [15:24:19]  I  Session(pid=32087, name=马赛克) attached
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.access$300()
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.access$600()
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.decode(java.lang.String)
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.encode(java.lang.String)
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.encode(java.lang.String, java.lang.String)
 [15:24:19]  I  Hook method: android.net.Uri android.net.Uri.fromFile(java.io.File)
@@ -625,15 +620,15 @@
                    "java.lang.Thread.run(Thread.java:923)"
                  ]
                }
 ```
 
 **2) 当然也可以使用python方式调用**
 
-执行如下python脚本即可自动开启frida-server，并将js代码注入到指定进程中，若需要同时注入子进程，按[src/linktools/cli/scripts/android/frida.py](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/src/linktools/cli/scripts/android/frida.py) 重写 FridaApplication 的 on_spawn_added 方法即可
+执行如下python脚本即可自动开启frida-server，并将js代码注入到指定进程中，若需要同时注入子进程，按[src/linktools/cli/scripts/android/frida.py](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/cli/scripts/android/frida.py) 重写 FridaApplication 的 on_spawn_added 方法即可
 
 ```python
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import logging
 from linktools.frida import FridaApplication, FridaEvalCode
 from linktools.frida.android import AndroidFridaServer
```

### Comparing `linktools-0.8.3rc1/pyproject.toml` & `linktools-0.8.4rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/setup.py` & `linktools-0.8.4rc0/setup.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/__init__.py` & `linktools-0.8.4rc0/src/linktools/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/__main__.py` & `linktools-0.8.4rc0/src/linktools/__main__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/_config.py` & `linktools-0.8.4rc0/src/linktools/_config.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/_environ.py` & `linktools-0.8.4rc0/src/linktools/_environ.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/_tools.py` & `linktools-0.8.4rc0/src/linktools/_tools.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/_url.py` & `linktools-0.8.4rc0/src/linktools/_url.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/android/__init__.py` & `linktools-0.8.4rc0/src/linktools/android/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/android/adb.py` & `linktools-0.8.4rc0/src/linktools/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/android/struct.py` & `linktools-0.8.4rc0/src/linktools/android/struct.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/assets/android-tools.apk` & `linktools-0.8.4rc0/src/linktools/assets/android-tools.apk`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/assets/android-tools.json` & `linktools-0.8.4rc0/src/linktools/assets/android-tools.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'ANDROID_TOOL_BRIDGE_APK'": "{'time': '2024-04-16 16:50:09'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "ANDROID_TOOL_BRIDGE_APK": {
         "main": "android.tools.Main",
         "md5": "3097e19b66070036181860877768b952",
         "name": "android-tools.apk",
         "size": 82987,
-        "time": "2024-04-05 21:46:39"
+        "time": "2024-04-16 16:50:09"
     },
     "ANDROID_TOOL_FRIDA_SERVER": [
         {
             "min_version": "15.1.8",
             "name": "strong-frida-server-{version}-android-{abi}",
             "url": "https://github.com/hzzheyang/strongR-frida-android/releases/download/{version}/hluda-server-{version}-android-{abi}.xz"
         },
```

### Comparing `linktools-0.8.3rc1/src/linktools/assets/chrome-driver.json` & `linktools-0.8.4rc0/src/linktools/assets/chrome-driver.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/Dockerfile` & `linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/Dockerfile`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM nginx:alpine
+FROM nginx:{{ NGINX_TAG }}
 
 RUN apk --no-cache add openssl socat
 RUN curl https://get.acme.sh | sh -s email=acme@google.com && \
     ln -s ~/.acme.sh/acme.sh /usr/bin/acme.sh && \
     acme.sh --set-default-ca --server letsencrypt
 
 RUN echo "#!/bin/sh" > /docker-entrypoint.d/99-start-crond.sh \
@@ -15,19 +15,14 @@
     {% with value = config.get(key, default=None) -%}
         {% if value %}
 ENV {{ key }} {{ value }}
         {% endif %}
     {%- endwith %}
 {%- endfor %}
 
-{% if DEBUG %}
-RUN acme.sh --issue  --debug --domain {{ ROOT_DOMAIN }} --domain *.{{ ROOT_DOMAIN }} --dns {{ ACME_DNS_API }}
-{% else %}
-RUN acme.sh --issue --domain {{ ROOT_DOMAIN }} --domain *.{{ ROOT_DOMAIN }} --dns {{ ACME_DNS_API }}
-{% endif %}
+RUN acme.sh --issue --domain {{ ROOT_DOMAIN }} --domain *.{{ ROOT_DOMAIN }} --dns {{ ACME_DNS_API }} --debug 2
 
 RUN acme.sh --install-cert --domain {{ ROOT_DOMAIN }} --domain *.{{ ROOT_DOMAIN }} \
     --cert-file /etc/certs/{{ ROOT_DOMAIN }}_cert.pem \
     --key-file /etc/certs/{{ ROOT_DOMAIN }}_key.pem \
     --fullchain-file /etc/certs/{{ ROOT_DOMAIN }}_fullchain.pem \
     --reloadcmd "nginx -s reload 2>/dev/null || true"
-
```

### Comparing `linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/container.py` & `linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         data = utils.read_file(path, text=True)
         pattern = re.compile(r'export +(\w+)="?')
         return sorted(list(set(pattern.findall(data))))
 
     @cached_property
     def configs(self):
         return dict(
+            NGINX_TAG="alpine",
             ROOT_DOMAIN=Config.Prompt(cached=True),
             WILDCARD_DOMAIN=Config.Confirm(default=False, cached=True),
             HTTP_PORT=Config.Prompt(default=80, type=int, cached=True),
             HTTPS_PORT=Config.Prompt(default=443, type=int, cached=True),
             ACME_DNS_API=Config.Error(textwrap.dedent(
                 """
                 Ensure ACME_DNS_API config matches --dns parameter in acme command is set.
@@ -60,22 +61,14 @@
                 · For details, see: https://github.com/acmesh-official/acme.sh/wiki/dnsapi.
                 · Example command:
                   $ ct-cntr config set ACME_DNS_API=dns_ali Ali_Key=xxx Ali_Secret=yyy
                 """
             ))
         )
 
-    @cached_property
-    def enable(self):
-        return self.manager.config.get(
-            "NGINX_ENABLE",
-            type=bool,
-            default=Config.Confirm(default=True, cached=True)
-        )
-
     def on_starting(self):
         path = self.get_app_path("conf.d")
         if not os.path.exists(path):
             return
         for name in os.listdir(path):
             target_path = os.path.join(path, name)
             if os.path.isdir(target_path):
```

### Comparing `linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/dnsapi.txt` & `linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/assets/containers/110-portainer/container.py` & `linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,21 +29,18 @@
 
 from linktools.container import BaseContainer, ExposeLink
 from linktools.decorator import cached_property
 
 
 class Container(BaseContainer):
 
-    @property
-    def dependencies(self) -> [str]:
-        return ["nginx"]
-
     @cached_property
     def configs(self):
         return dict(
+            PORTAINER_TAG="alpine",
             PORTAINER_DOMAIN=self.get_nginx_domain(),
             PORTAINER_EXPOSE_PORT=None,
         )
 
     @cached_property
     def exposes(self) -> [ExposeLink]:
         return [
```

### Comparing `linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/compose.yml` & `linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/compose.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 services:
   flare:
-    image: soulteary/flare
+    image: soulteary/flare:{{ FLARE_TAG }}
     user: '{{ DOCKER_UID }}:{{ DOCKER_GID }}'
 #   {% if int(FLARE_EXPOSE_PORT, 0) > 0 %}
     ports:
       - '{{ FLARE_EXPOSE_PORT }}:5005'
 #   {% endif %}
 #   {% if bool(FLARE_DISABLE_LOGIN) %}
     command: flare --disable_login=1 --visibility=private
```

### Comparing `linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/container.py` & `linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,20 @@
 from linktools.container import BaseContainer
 from linktools.container.container import ExposeMixin, ExposeLink, ExposeCategory
 from linktools.decorator import cached_property
 
 
 class Container(BaseContainer):
 
-    @property
-    def dependencies(self) -> [str]:
-        return ["nginx"]
-
     @cached_property
     def configs(self):
         return dict(
             WILDCARD_DOMAIN=True,
 
+            FLARE_TAG="latest",
             FLARE_DISABLE_LOGIN=Config.Confirm(default=True, cached=True),
             FLARE_DOAMIN=self.get_nginx_domain(""),
             FLARE_EXPOSE_PORT=None,
             FLARE_USER=Config.Prompt(default="admin", cached=True),
             FLARE_PASSWORD=Config.Prompt(cached=True),
         )
```

### Comparing `linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/nginx.conf` & `linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/nginx.conf`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/assets/fake_useragent.json` & `linktools-0.8.4rc0/src/linktools/assets/fake_useragent.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/assets/frida.js` & `linktools-0.8.4rc0/src/linktools/assets/frida.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -944,8 +944,8 @@
             }, t;
         }();
 
         exports.ObjCHelper = t;
 
     }, {}]
 }, {}, [1])
-//# sourceMappingURL=data:application/json;charset=utf-8;base64,eyJ2ZXJzaW9uIjozLCJzb3VyY2VzIjpbIm5vZGVfbW9kdWxlcy9icm93c2VyLXBhY2svX3ByZWx1ZGUuanMiLCJpbmRleC50cyIsImxpYi9hbmRyb2lkLnRzIiwibGliL2MudHMiLCJsaWIvaW9zLnRzIiwibGliL2phdmEudHMiLCJsaWIvb2JqYy50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiQUFBQTs7Ozs7OztBQ0tBLElBQUEsSUFBQTtFQUFBLFNBQUE7SUFBQSxJQUFBLElBQUE7SUFFWSxLQUFBLGdCQUF1QixJQUN2QixLQUFBLGFBQWtCLE1Bd0JsQixLQUFBLFFBQVE7TUFNWixJQUx3QixTQUFwQixFQUFLLGVBQ0wsYUFBYSxFQUFLLGFBQ2xCLEVBQUssYUFBYTtNQUdZLE1BQTlCLEVBQUssY0FBYyxRQUF2QjtRQUlBLElBQU0sSUFBUyxFQUFLO1FBQ3BCLEVBQUssZ0JBQWdCLElBRXJCLEtBQUs7VUFBRSxTQUFTOzs7QUFDcEI7QUFDSjtFQUFBLE9BckNJLEVBQUEsVUFBQSxPQUFBLFNBQUssR0FBYyxHQUFjO0lBQzdCLElBQU0sSUFBUTtJQUNkLEVBQU0sS0FBUSxHQUVGLFFBQVIsS0FFQSxLQUFLLGNBQWMsS0FBSyxJQUNwQixLQUFLLGNBQWMsVUFBVSxLQUc3QixLQUFLLFVBQ3NCLFNBQXBCLEtBQUssZUFDWixLQUFLLGFBQWEsV0FBVyxLQUFLLE9BQU8sU0FLN0MsS0FBSztJQUNMLEtBQUs7TUFBRSxTQUFTLEVBQUM7T0FBVTtBQUVuQyxLQWlCSjtBQUFBLENBMUNBLElBNkNBLElBQUE7RUFBQSxTQUFBLEtBS0E7RUFBQSxPQUhJLEVBQUEsVUFBQSxPQUFBLFNBQUssR0FBYztJQUNmLEVBQWMsS0FBSyxPQUFPLEdBQVM7QUFDdkMsS0FDSjtBQUFBLENBTEEsSUFZQSxJQUFBO0VBUUksU0FBQTtJQU5BLEtBQUEsUUFBUSxHQUNSLEtBQUEsT0FBTyxHQUNQLEtBQUEsVUFBVSxHQUNWLEtBQUEsUUFBUSxHQUNBLEtBQUEsU0FBUyxLQUFLO0lBR2xCLElBQU0sSUFBVyxTQUFXO01BQ3hC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QUFRO01BSXBCLFlBSHFDLE1BQWpDLEVBQXdCLE9BQ3hCLEVBQXdCLEtBQU8sWUFBWSxZQUFZLEtBRXBELEVBQXdCO0FBQ25DOzs7OztBQ3pUUjtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTs7Ozs7Ozs7QUM1SUEsSUFBQSxJQUFBO0VBQUEsU0FBQTtJQUVJLEtBQUEsY0FBYztBQXdO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
+//# sourceMappingURL=data:application/json;charset=utf-8;base64,eyJ2ZXJzaW9uIjozLCJzb3VyY2VzIjpbIm5vZGVfbW9kdWxlcy9icm93c2VyLXBhY2svX3ByZWx1ZGUuanMiLCJpbmRleC50cyIsImxpYi9hbmRyb2lkLnRzIiwibGliL2MudHMiLCJsaWIvaW9zLnRzIiwibGliL2phdmEudHMiLCJsaWIvb2JqYy50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiQUFBQTs7Ozs7OztBQ0tBLElBQUEsSUFBQTtFQUFBLFNBQUE7SUFBQSxJQUFBLElBQUE7SUFFWSxLQUFBLGdCQUF1QixJQUN2QixLQUFBLGFBQWtCLE1Bd0JsQixLQUFBLFFBQVE7TUFNWixJQUx3QixTQUFwQixFQUFLLGVBQ0wsYUFBYSxFQUFLLGFBQ2xCLEVBQUssYUFBYTtNQUdZLE1BQTlCLEVBQUssY0FBYyxRQUF2QjtRQUlBLElBQU0sSUFBUyxFQUFLO1FBQ3BCLEVBQUssZ0JBQWdCLElBRXJCLEtBQUs7VUFBRSxTQUFTOzs7QUFDcEI7QUFDSjtFQUFBLE9BckNJLEVBQUEsVUFBQSxPQUFBLFNBQUssR0FBYyxHQUFjO0lBQzdCLElBQU0sSUFBUTtJQUNkLEVBQU0sS0FBUSxHQUVGLFFBQVIsS0FFQSxLQUFLLGNBQWMsS0FBSyxJQUNwQixLQUFLLGNBQWMsVUFBVSxLQUc3QixLQUFLLFVBQ3NCLFNBQXBCLEtBQUssZUFDWixLQUFLLGFBQWEsV0FBVyxLQUFLLE9BQU8sU0FLN0MsS0FBSztJQUNMLEtBQUs7TUFBRSxTQUFTLEVBQUM7T0FBVTtBQUVuQyxLQWlCSjtBQUFBLENBMUNBLElBNkNBLElBQUE7RUFBQSxTQUFBLEtBS0E7RUFBQSxPQUhJLEVBQUEsVUFBQSxPQUFBLFNBQUssR0FBYztJQUNmLEVBQWMsS0FBSyxPQUFPLEdBQVM7QUFDdkMsS0FDSjtBQUFBLENBTEEsSUFZQSxJQUFBO0VBUUksU0FBQTtJQU5BLEtBQUEsUUFBUSxHQUNSLEtBQUEsT0FBTyxHQUNQLEtBQUEsVUFBVSxHQUNWLEtBQUEsUUFBUSxHQUNBLEtBQUEsU0FBUyxLQUFLO0lBR2xCLElBQU0sSUFBVyxTQUFXO01BQ3hCLE9BQU87UUFFSCxLQURBLElBQUksSUFBVSxJQUNMLElBQUksR0FBRyxJQUFJLFVBQVUsUUFBUSxLQUM5QixJQUFJLE1BQ0osS0FBVyxNQUVmLEtBQVcsY0FBYyxVQUFVO1FBRXZDLEVBQUc7QUFDUDtBQUNIO0lBRUQsUUFBUSxRQUFRLEVBQVMsS0FBSyxFQUFFLEtBQUssUUFDckMsUUFBUSxPQUFPLEVBQVMsS0FBSyxFQUFFLEtBQUssUUFDcEMsUUFBUSxPQUFPLEVBQVMsS0FBSyxFQUFFLEtBQUs7SUFDcEMsUUFBUSxRQUFRLEVBQVMsS0FBSyxFQUFFLEtBQUssUUFDckMsUUFBUSxNQUFNLEVBQVMsS0FBSyxFQUFFLEtBQUs7QUFDdkM7RUFrQ0osT0FoQ0ksT0FBQSxlQUFJLEVBQUEsV0FBQSxTQUFLO1NBQVQ7TUFDSSxPQUFPLEtBQUs7QUFDaEI7OztNQUVBLEVBQUEsVUFBQSxXQUFBLFNBQVM7SUFDTCxLQUFLLFNBQVMsR0FDZCxLQUFLLEVBQUUsb0JBQW9CO0FBQy9CLEtBRUEsRUFBQSxVQUFBLElBQUEsU0FBRSxHQUFjO0lBQ1IsS0FBSyxVQUFVLEtBQUssU0FDcEIsRUFBYyxLQUFLLE9BQU87TUFBRSxPQUFPO01BQVMsU0FBUztPQUFXO0FBRXhFLEtBRUEsRUFBQSxVQUFBLElBQUEsU0FBRSxHQUFjO0lBQ1IsS0FBSyxVQUFVLEtBQUssUUFDcEIsRUFBYyxLQUFLLE9BQU87TUFBRSxPQUFPO01BQVEsU0FBUztPQUFXO0FBRXZFLEtBRUEsRUFBQSxVQUFBLElBQUEsU0FBRSxHQUFjO0lBQ1IsS0FBSyxVQUFVLEtBQUssV0FDcEIsRUFBYyxLQUFLLE9BQU87TUFBRSxPQUFPO01BQVcsU0FBUztPQUFXO0FBRTFFLEtBRUEsRUFBQSxVQUFBLElBQUEsU0FBRSxHQUFjO0lBQ1IsS0FBSyxVQUFVLEtBQUssU0FDcEIsRUFBYyxLQUFLLE9BQU87TUFBRSxPQUFPO01BQVMsU0FBUztPQUFXO0FBRXhFLEtBQ0o7QUFBQSxDQTdEQSxJQTZFQSxJQUFBO0VBQUEsU0FBQSxLQW9CQTtFQUFBLE9BbEJJLEVBQUEsVUFBQSxPQUFBLFNBQUssR0FBbUI7SUFDcEIsS0FBcUIsSUFBQSxJQUFBLEdBQUEsSUFBQSxHQUFBLElBQUEsRUFBQSxRQUFBLEtBQVM7TUFBekIsSUFBTSxJQUFNLEVBQUE7TUFDYjtRQUNJLElBQUksSUFBTyxFQUFPO1FBRWxCLEtBREEsSUFBTyxFQUFLLFFBQVEsV0FBVyxNQUNuQixRQUFRLG9CQUFvQixNQUN4QyxJQUFPLE1BQUEsT0FBTSxHQUFPLFVBQVUsR0FBRztTQUNwQixHQUFJLE1BQ2IsYUFBQSxPQUFhLEdBQUksa0JBQUEsT0FBaUIsRUFBTyxRQUFNLFlBQy9DLGlCQUFBLE9BQWlCLEVBQU8sVUFFNUIsQ0FBSztRQUNQLE9BQU87UUFDTCxJQUFJLElBQVUsRUFBRSxlQUFlLFdBQVcsRUFBRSxRQUFRO1FBQ3BELE1BQU0sSUFBSSxNQUFNLGtCQUFBLE9BQWtCLEVBQU8sVUFBUSxNQUFBLE9BQUs7OztBQUdsRSxLQUNKO0FBQUEsQ0FwQkE7O0FBQWEsUUFBQTs7QUFzQmIsSUFBTSxJQUFlLElBQUk7O0FBRXpCLElBQUksVUFBVTtFQUNWLGFBQWEsRUFBYSxLQUFLLEtBQUs7OztBQU94QyxJQUFNLElBQWdCLElBQUksR0FDcEIsSUFBMkQsSUFNakUsSUFBQSxRQUFBLFlBQ0EsSUFBQSxRQUFBLGVBQ0EsSUFBQSxRQUFBLGtCQUNBLElBQUEsUUFBQSxlQUNBLElBQUEsUUFBQSxjQUVNLElBQVUsSUFBSSxHQUNkLElBQU0sSUFBSSxHQUNWLElBQVUsSUFBSSxFQUFBLFNBQ2QsSUFBYSxJQUFJLEVBQUEsWUFDakIsSUFBZ0IsSUFBSSxFQUFBLGVBQ3BCLElBQWEsSUFBSSxFQUFBLFlBQ2pCLElBQVksSUFBSSxFQUFBOztBQXNCdEIsT0FBTyxpQkFBaUIsWUFBWTtFQUNoQyxTQUFTO0lBQ0wsYUFBWTtJQUNaLE9BQU87O0VBRVgsS0FBSztJQUNELGFBQVk7SUFDWixPQUFPOztFQUVYLFNBQVM7SUFDTCxhQUFZO0lBQ1osT0FBTzs7RUFFWCxZQUFZO0lBQ1IsYUFBWTtJQUNaLE9BQU87O0VBRVgsZUFBZTtJQUNYLGFBQVk7SUFDWixPQUFPOztFQUVYLFlBQVk7SUFDUixhQUFZO0lBQ1osT0FBTzs7RUFFWCxXQUFXO0lBQ1AsYUFBWTtJQUNaLE9BQU87O0VBRVgsWUFBWTtJQUNSLGFBQVk7SUFDWixPQUFPLFNBQVU7TUFDYixPQUErQyx3QkFBeEMsT0FBTyxVQUFVLFNBQVMsS0FBSztBQUMxQzs7RUFFSixhQUFhO0lBQ1QsYUFBWTtJQUNaLE9BQU8sU0FBYSxHQUFhO1dBQUEsTUFBQSxlQUFBO01BQzdCO1FBQ0ksT0FBTztRQUNULE9BQU87UUFFTCxPQURBLEVBQUksRUFBRSwwQkFBMEIsSUFDekI7O0FBRWY7O0VBRUosY0FBYztJQUNWLGFBQVk7SUFDWixPQUFPLFNBQVUsR0FBeUI7TUFDdEMsU0FEc0MsTUFBQSxlQUFBLElBQ2Ysb0JBQVosR0FDUCxPQUFPO01BRVgsSUFBdUIsbUJBQVosR0FBc0I7UUFDN0IsSUFBTSxJQUFRLEVBQU07UUFDcEIsSUFBYyxXQUFWLEdBQ0EsUUFBTztRQUNKLElBQWMsWUFBVixHQUNQLFFBQU87O01BR2YsT0FBTztBQUNYOztFQUVKLGVBQWU7SUFDWCxhQUFZO0lBQ1osT0FBTyxTQUFVO01BSWIsT0FIbUIsbUJBQVIsTUFDUCxJQUFNLFlBQVksS0FFZixLQUFLLFVBQVU7QUFDMUI7O0VBRUosYUFBYTtJQUNULGFBQVk7SUFDWixPQUFPLFNBQVU7TUFDYixNQUFNLGFBQWUsU0FDakIsT0FBTztNQUVYLElBQUksTUFBTSxRQUFRLElBQU07UUFFcEIsS0FEQSxJQUFJLElBQVMsSUFDSixJQUFJLEdBQUcsSUFBSSxFQUFJLFFBQVEsS0FDNUIsRUFBTyxLQUFLLFlBQVksRUFBSTtRQUVoQyxPQUFPOztNQUVYLE9BQUksS0FBSyxhQUNELEVBQVcsYUFBYSxLQUNqQixFQUFXLFlBQVksU0FBUyxNQUFNLEtBRzlDLGFBQVk7UUFBTSxPQUFBLEVBQUk7QUFBSjtBQUM3Qjs7RUFFSiwyQkFBMkI7SUFDdkIsYUFBWTtJQUNaLE9BQU8sU0FBVTtNQUNiLElBQU0sSUFBTSxFQUFRO01BSXBCLFlBSHFDLE1BQWpDLEVBQXdCLE9BQ3hCLEVBQXdCLEtBQU8sWUFBWSxZQUFZLEtBRXBELEVBQXdCO0FBQ25DOzs7OztBQ3pUUjtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTs7Ozs7Ozs7QUM1SUEsSUFBQSxJQUFBO0VBQUEsU0FBQTtJQUVJLEtBQUEsY0FBYztBQXdO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SztBQUNqQixPQUVPO0FBQ1gsS0FFSjtBQUFBLENBMU5BOztBQUFhLFFBQUE7OztBQ2JiO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTs7QUNuQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTs7QUM1UUE7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0EiLCJmaWxlIjoiZ2VuZXJhdGVkLmpzIiwic291cmNlUm9vdCI6IiJ9
```

### Comparing `linktools-0.8.3rc1/src/linktools/assets/frida.min.js` & `linktools-0.8.4rc0/src/linktools/assets/frida.min.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/assets/objection/plugins/__init__.py` & `linktools-0.8.4rc0/src/linktools/assets/objection/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/assets/tools.json` & `linktools-0.8.4rc0/src/linktools/assets/tools.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987492108585858%*

 * *Differences: {"'TOOL_AAPT'": "{'target_path': {'case': {1: {'then': '{version_name}\\\\{name}.exe'}}}}",*

 * * "'TOOL_ADB'": "{'target_path': {'case': {1: {'then': 'platform-tools\\\\\\\\{name}.exe'}}}}",*

 * * "'TOOL_APKSIGNER'": "{'target_path': {'case': {1: {'then': '{version_name}\\\\{name}.bat'}}}}",*

 * * "'TOOL_DEX2JAR'": "{'target_path': {'case': {1: {'then': "*

 * *                   "'dex-tools-{version}\\\\\\\\d2j-{name}.bat'}}}}",*

 * * "'TOOL_FASTBOOT'": "{'target_path': {'case': {1: {'then': 'platform-tools\\\\\\\\{name}.exe'}}}}" […]*

```diff
@@ -33,15 +33,15 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "{version_name}/{name}.exe",
+                    "then": "{version_name}\\{name}.exe",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -61,15 +61,15 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "platform-tools/{name}.exe",
+                    "then": "platform-tools\\\\{name}.exe",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -111,15 +111,15 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "{version_name}/{name}.exe",
+                    "then": "{version_name}\\{name}.bat",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -287,15 +287,15 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "dex-tools-{version}/d2j-{name}.bat",
+                    "then": "dex-tools-{version}\\\\d2j-{name}.bat",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -315,15 +315,15 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "platform-tools/{name}.exe",
+                    "then": "platform-tools\\\\{name}.exe",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -387,15 +387,15 @@
                     "then": "bin/ipatool-{version}-linux-amd64",
                     "when": {
                         "machine": "x86_64",
                         "system": "linux"
                     }
                 },
                 {
-                    "then": "bin/ipatool-{version}-windows-amd64.exe",
+                    "then": "bin\\\\ipatool-{version}-windows-amd64.exe",
                     "when": {
                         "machine": "amd64",
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
@@ -415,15 +415,15 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "bin/{name}.bat",
+                    "then": "bin\\\\{name}.bat",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -443,15 +443,15 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "bin/{name}.bat",
+                    "then": "bin\\\\{name}.bat",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -470,15 +470,15 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "dex-tools-{version}/d2j-{name}.bat",
+                    "then": "dex-tools-{version}\\\\d2j-{name}.bat",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -535,15 +535,15 @@
                 {
                     "then": "sapmachine-jdk-{version}/bin/{name}",
                     "when": {
                         "system": "linux"
                     }
                 },
                 {
-                    "then": "sapmachine-jdk-{version}/bin/{name}.exe",
+                    "then": "sapmachine-jdk-{version}\\\\bin\\\\{name}.exe",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -599,15 +599,15 @@
                 {
                     "then": "sapmachine-jdk-{version}/bin/{name}",
                     "when": {
                         "system": "linux"
                     }
                 },
                 {
-                    "then": "sapmachine-jdk-{version}/bin/{name}.exe",
+                    "then": "sapmachine-jdk-{version}\\\\bin\\\\{name}.exe",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -740,15 +740,15 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "{version_name}/{name}.exe",
+                    "then": "{version_name}\\{name}.exe",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
```

### Comparing `linktools-0.8.3rc1/src/linktools/cli/__init__.py` & `linktools-0.8.4rc0/src/linktools/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,12 +28,13 @@
 """
 
 from . import argparse
 
 from .command import \
     BaseCommand, BaseCommandGroup, CommandError, \
     SubCommand, SubCommandGroup, SubCommandWrapper, \
-    subcommand, subcommand_argument, SubCommandError
+    subcommand, subcommand_argument, SubCommandError, \
+    iter_command_modules
 
 from .device import \
     DeviceCommandMixin, AndroidCommandMixin, IOSCommandMixin, \
     AndroidCommand, IOSCommand
```

### Comparing `linktools-0.8.3rc1/src/linktools/cli/command.py` & `linktools-0.8.4rc0/src/linktools/cli/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,43 +31,87 @@
 import inspect
 import logging
 import os
 import textwrap
 import traceback
 from argparse import ArgumentParser, Action, Namespace
 from argparse import RawDescriptionHelpFormatter, SUPPRESS, FileType, HelpFormatter
-from importlib.util import module_from_spec
 from pkgutil import walk_packages
 from types import ModuleType, GeneratorType
 from typing import TYPE_CHECKING, Optional, Callable, List, Type, Tuple, Generator, Any, Iterable, Union, Set, Dict
 
 from rich import get_console
 from rich.tree import Tree
 
-from .argparse import BooleanOptionalAction
+from .argparse import BooleanOptionalAction, auto_complete
+from .. import utils
 from .._environ import environ
 from ..decorator import cached_property
 from ..metadata import __missing__
 from ..rich import LogHandler, is_terminal
 
 if TYPE_CHECKING:
-    from typing import TypeVar
+    from typing import TypeVar, Union, Literal
     from .._environ import BaseEnviron
 
     T = TypeVar("T")
+    ERROR_HANDLER = Union[Literal["error", "ignore", "warn"], Callable[[str, Exception], None]]
 
 
 class CommandError(Exception):
     pass
 
 
 class SubCommandError(CommandError):
     pass
 
 
+class _CommandModuleInfo:
+    name: str
+    parent_name: str
+    module: ModuleType
+    module_name: str
+    command: "Optional[BaseCommand]"
+    command_name: str
+    command_description: str
+
+
+def iter_command_modules(root: ModuleType, *, onerror: "ERROR_HANDLER" = "error"):
+    prefix = root.__name__ + "."
+    for finder, name, is_package in walk_packages(path=root.__path__, prefix=prefix):
+        try:
+            info = _CommandModuleInfo()
+            info.name = name[len(prefix):]
+            info.parent_name = name[len(prefix):name.rfind(".")]
+            info.module = module = utils.import_module(name, spec=finder.find_spec(name))
+            info.module_name = module.__name__
+            if is_package:
+                info.command = None
+                info.command_name = getattr(module, "__command__", None) or info.name[info.name.rfind(".") + 1:]
+                info.command_description = getattr(module, "__description__", None) or ""
+                yield info
+            elif hasattr(info.module, "command") and isinstance(info.module.command, BaseCommand):
+                info.command = info.module.command
+                info.command_name = info.command.name
+                info.command_description = info.command.description
+                yield info
+        except Exception as e:
+            if callable(onerror):
+                onerror(name, e)
+            elif onerror == "error":
+                raise e
+            elif onerror == "warn":
+                environ.logger.warning(
+                    f"Ignore {name}, caused by {e.__class__.__name__}: {e}",
+                    exc_info=e if environ.debug else None
+                )
+            elif onerror == "ignore":
+                pass
+
+
 def _filter_kwargs(kwargs):
     return {k: v for k, v in kwargs.items() if v != __missing__}
 
 
 _subcommand_index: int = 0
 _subcommand_map: Dict[str, Set[str]] = {}
 
@@ -222,23 +266,27 @@
 class _SubCommandInfo:
 
     def __init__(self, subcommand: "Union[SubCommand, _SubCommandInfo]"):
         self.node: SubCommand = subcommand.node if isinstance(subcommand, _SubCommandInfo) else subcommand
         self.children: List[_SubCommandInfo] = []
 
 
+def _join_id(*ids: str):
+    return "#".join([id for id in ids if id])
+
+
 class SubCommand(metaclass=abc.ABCMeta):
     """
     子命令接口
     """
 
-    ROOT_ID = ""
+    ROOT_ID = _join_id()
 
     def __init__(self, name: str, description: str, id: str = None, parent_id: str = None):
-        self.id = id or name
+        self.id = id or _join_id(parent_id, name)
         self.parent_id = parent_id or self.ROOT_ID
         self.name = name
         self.description = description
 
     @property
     def has_parent(self):
         """
@@ -402,67 +450,56 @@
 
     def run(self, args: Namespace):
         return self.command(args)
 
 
 class SubCommandMixin:
 
-    def walk_subcommands(self: "BaseCommand", target: Any) -> Generator[SubCommand, None, None]:
+    def walk_subcommands(self: "BaseCommand", target: Any, parent_id: str = None) -> Generator[SubCommand, None, None]:
         """
         根据target对象，遍历所有的子命令，规则如下：
         1. 如果target是SubCommand类型，则直接返回
         2. 如果target是list、tuple、set、generator类型，则递归遍历
         3. 如果target是模块类型，则遍历模块下的所有子命令
         4. 如果target是其他类型，则遍历target下的所有包含@subcommand注解的方法
         """
         if isinstance(target, SubCommand):
             yield target
 
         elif isinstance(target, (list, tuple, set, GeneratorType)):
             for item in target:
-                yield from self.walk_subcommands(item)
+                yield from self.walk_subcommands(item, parent_id=parent_id)
 
         elif isinstance(target, ModuleType):
-            prefix = target.__name__ + "."  # prefix: aaa.
-            for finder, name, is_package in walk_packages(path=target.__path__, prefix=prefix):  # name: aaa.bbb.ccc
-                module_name = name[len(prefix):]  # bbb.ccc
-                parent_module_name = name[len(prefix):name.rfind(".")]  # bbb
-
-                try:
-                    spec = finder.find_spec(name)
-                    module = module_from_spec(spec)
-                    spec.loader.exec_module(module)
-                except Exception as e:
-                    self.logger.warning(
-                        f"Ignore {module_name}, caused by {e.__class__.__name__}: {e}",
-                        exc_info=e if environ.debug else None
+            for m in iter_command_modules(target, onerror="warn"):
+                if m.command:
+                    yield SubCommandWrapper(
+                        m.command,
+                        id=_join_id(parent_id, m.name), parent_id=_join_id(parent_id, m.parent_name)
+                    )
+                else:
+                    yield SubCommandGroup(
+                        m.command_name, m.command_description,
+                        id=_join_id(parent_id, m.name), parent_id=_join_id(parent_id, m.parent_name)
                     )
-                    continue
-
-                if is_package:
-                    _name = getattr(module, "__command__", None) or name[name.rfind(".") + 1:]  # ccc
-                    _description = getattr(module, "__description__", None) or ""
-                    yield SubCommandGroup(_name, _description, id=module_name, parent_id=parent_module_name)
-                elif hasattr(module, "command") and isinstance(module.command, BaseCommand):
-                    yield SubCommandWrapper(module.command, id=module_name, parent_id=parent_module_name)
 
         else:
             subcommand_map: Dict[str, List[_SubCommandMethod]] = {}
             for clazz in target.__class__.mro():
                 class_name = f"{clazz.__module__}.{clazz.__qualname__}"
                 if class_name not in _subcommand_map:
                     continue
                 for func_name in _subcommand_map[class_name]:
                     if not hasattr(clazz, func_name):
                         continue
                     func = getattr(clazz, func_name)
                     if not hasattr(func, "__subcommand_info__"):
                         continue
                     info: _SubCommandMethodInfo = func.__subcommand_info__
-                    subcommand = _SubCommandMethod(info, target)
+                    subcommand = _SubCommandMethod(info, target, parent_id=parent_id)
                     subcommand_map.setdefault(subcommand.name, list())
                     subcommand_map[info.name].append(subcommand)
 
             command_infos: List[Tuple[int, _SubCommandMethod]] = []
             for name, subcommands in subcommand_map.items():
                 command_infos.append((min([c.info.index for c in subcommands]), subcommands[0]))
             for _, subcommand in sorted(command_infos, key=lambda o: o[0]):
@@ -708,21 +745,26 @@
         pass
 
     def init_common_arguments(self, parser: ArgumentParser) -> None:
         """
         初始化公共参数，会在命令本身和所有子命令中调用
         """
         environ = self.environ
-        prefix = parser.prefix_chars
+        prefix = parser.prefix_chars[0] if parser.prefix_chars else "-"
 
         class VerboseAction(Action):
 
             def __call__(self, parser, namespace, values, option_string=None):
                 logging.root.setLevel(logging.DEBUG)
 
+        class SilentAction(Action):
+
+            def __call__(self, parser, namespace, values, option_string=None):
+                logging.disable(logging.CRITICAL)
+
         class DebugAction(Action):
 
             def __call__(self, parser, namespace, values, option_string=None):
                 environ.debug = True
                 environ.logger.setLevel(logging.DEBUG)
 
         class LogTimeAction(BooleanOptionalAction):
@@ -741,34 +783,36 @@
                 if option_string in self.option_strings:
                     value = not option_string.startswith("--no-")
                     handler = LogHandler.get_instance()
                     if handler:
                         handler.show_level = value
                     environ.set_config("SHOW_LOG_LEVEL", value)
 
-        group = parser.add_argument_group(title="log options")
+        group = parser.add_argument_group(title="log options").add_mutually_exclusive_group()
         group.add_argument(f"{prefix}{prefix}verbose", action=VerboseAction, nargs=0, const=True, dest=SUPPRESS,
                            help="increase log verbosity")
+        group.add_argument(f"{prefix}{prefix}silent", action=SilentAction, nargs=0, const=True, dest=SUPPRESS,
+                           help="disable all log output")
         group.add_argument(f"{prefix}{prefix}debug", action=DebugAction, nargs=0, const=True, dest=SUPPRESS,
                            help=f"increase {self.environ.name}'s log verbosity, and enable debug mode")
 
         if LogHandler.get_instance():
             group.add_argument(f"{prefix}{prefix}time", action=LogTimeAction, dest=SUPPRESS,
                                help="show log time")
             group.add_argument(f"{prefix}{prefix}level", action=LogLevelAction, dest=SUPPRESS,
                                help="show log level")
 
         if self.environ.version != NotImplemented:
             parser.add_argument(
                 f"{prefix}{prefix}version", action="version", version=self.environ.version
             )
 
-    def main(self, *args, **kwargs) -> None:
+    def init_logging(self):
         """
-        main命令入口
+        初始化log
         """
         if is_terminal():
             logging.basicConfig(
                 level=logging.INFO,
                 format="%(message)s",
                 datefmt="[%X]",
                 handlers=[LogHandler(self.environ)]
@@ -776,48 +820,41 @@
         else:
             logging.basicConfig(
                 level=logging.INFO,
                 format="[%(asctime)s] %(levelname)s %(module)s %(funcName)s %(message)s",
                 datefmt="%H:%M:%S"
             )
 
+    def main(self, *args, **kwargs) -> None:
+        """
+        main命令入口
+        """
+        self.init_logging()
+
         try:
             result = self(*args, **kwargs)
         except SystemExit as e:
             result = e.code
-
-        except (KeyboardInterrupt, EOFError) as e:
-            result = 1
-            error_type, error_message = e.__class__.__name__, str(e).strip()
-            self.logger.error(
-                f"{error_type}: {error_message}" if error_message else error_type,
-            )
-
         except:
+            get_console().print_exception(show_locals=True) \
+                if environ.debug \
+                else self.logger.error(traceback.format_exc())
             result = 1
-            if environ.debug:
-                console = get_console()
-                console.print_exception(show_locals=True)
-            else:
-                self.logger.error(traceback.format_exc())
 
         exit(result)
 
     def __call__(self, args: Union[List[str], Namespace] = None) -> int:
         """
         内部调用命令入口
         """
         try:
             if not isinstance(args, Namespace):
                 parser = self._argument_parser
-                try:
-                    import argcomplete
-                    argcomplete.autocomplete(parser)
-                except ModuleNotFoundError:
-                    pass
+                if auto_complete:
+                    auto_complete.autocomplete(parser)
                 args = parser.parse_args(args)
 
             exit_code = self.run(args) or 0
 
         except (KeyboardInterrupt, EOFError, *self.known_errors) as e:
             exit_code = 1
             error_type, error_message = e.__class__.__name__, str(e).strip()
```

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/android/adb.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/android/agent.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/agent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/android/app.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/android/debug.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/debug.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/android/frida.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/android/info.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/info.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/android/intent.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/intent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/android/objection.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/objection.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/android/pidcat.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/pidcat.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/android/top.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/top.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/common/cert.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/common/cert.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/common/env.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/ssh.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 @author  : Hu Ji
-@file    : container.py
-@time    : 2024/3/21
-@site    : https://github.com/ice-black-tea
-@software: PyCharm
+@file    : ssh.py 
+@time    : 2022/11/27
+@site    :  
+@software: PyCharm 
 
               ,----------------,              ,---------,
          ,-----------------------,          ,"        ,"|
        ,"                      ,"|        ,"        ,"  |
       +-----------------------+  |      ,"        ,"    |
       |  .-----------------.  |  |     +---------+      |
       |  |                 |  |  |     | -==----'|      |
@@ -22,80 +22,57 @@
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
-from typing import Any
+from argparse import ArgumentParser, Namespace
+from typing import Optional, Type, List
+
+import paramiko
+from paramiko.ssh_exception import SSHException
 
 from linktools import utils
-from linktools.cli import subcommand, subcommand_argument, SubCommandWrapper, BaseCommandGroup
+from linktools.cli import IOSCommand
+from linktools.ssh import SSHClient
 
 
-class InitCommand(BaseCommandGroup):
+class Command(IOSCommand):
     """
-    initialize environment
+    OpenSSH remote login client (require iOS device jailbreak)
     """
 
-    @property
-    def name(self) -> str:
-        return "init"
-
-    @subcommand("android", help="initialize android environment")
-    def on_init_android(self):
-        try:
-            self.logger.info("initialize adb ...")
-            self.environ.tools["adb"].prepare()
-        except Exception as e:
-            self.logger.warning(f"initialize adb failed: {e}")
-
-        try:
-            from linktools.frida.android import AndroidFridaServer
-            self.logger.info("initialize android frida server ...")
-            AndroidFridaServer.setup(abis=["arm", "arm64"])
-        except Exception as e:
-            self.logger.warning(f"initialize android frida server failed: {e}")
-
-    @subcommand("ios", help="initialize ios environment")
-    def on_init_ios(self):
-        try:
-            self.logger.info("initialize sib ...")
-            self.environ.tools["sib"].prepare()
-        except Exception as e:
-            self.logger.warning(f"initialize sib failed: {e}")
+    def main(self, *args, **kwargs) -> None:
+        self.environ.config.set_default("SHOW_LOG_LEVEL", False)
+        self.environ.config.set_default("SHOW_LOG_TIME", False)
+        return super().main(*args, **kwargs)
 
+    @property
+    def known_errors(self) -> List[Type[BaseException]]:
+        return super().known_errors + [SSHException]
 
-class Command(BaseCommandGroup):
-    """
-    Linktools environment commands
-    """
+    def init_arguments(self, parser: ArgumentParser) -> None:
+        parser.add_argument("-u", "--username", action="store", default="root",
+                            help="iOS ssh username (default: root)")
+        parser.add_argument("-p", "--port", action="store", type=int, default=22,
+                            help="iOS ssh port (default: 22)")
+        parser.add_argument("--password", action="store",
+                            help="iOS ssh password")
+        parser.add_argument('ssh_args', nargs='...', help="ssh args")
+
+    def run(self, args: Namespace) -> Optional[int]:
+        device = args.device_picker.pick()
+
+        local_port = utils.pick_unused_port()
+        with device.forward(local_port, args.port):
+            with SSHClient() as client:
+                client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+                client.connect_with_pwd("localhost", port=local_port, username=args.username, password=args.password)
+                client.open_shell(*args.ssh_args)
 
-    def init_subcommands(self) -> Any:
-        return [
-            SubCommandWrapper(InitCommand()),
-            self
-        ]
-
-    @subcommand("shell", help="run shell command")
-    @subcommand_argument("-c", "--command", help="shell command")
-    def on_shell(self, command: str = None):
-        shell = self.environ.tools["shell"]
-        if not shell.exists:
-            raise NotImplementedError(f"Not found shell path")
-
-        if command:
-            process = utils.Process(command, shell=True)
-            return process.call()
-
-        process = shell.popen()
-        return process.call()
-
-    @subcommand("clean", help="clean temporary files")
-    @subcommand_argument("days", metavar="DAYS", nargs="?", help="expire days")
-    def on_clean_temp(self, days: int = 7):
-        self.environ.clean_temp_files(days)
+        return 0
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/common/grep.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/common/grep.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/common/tools.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/common/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         group.add_argument("-d", "--daemon", action="store_true", default=False,
                            help="execute tools as a daemon")
 
         tool_names = sorted([tool.name for tool in iter(self.environ.tools)])
         subparsers = parser.add_subparsers(metavar="TOOL", help=f"{{{','.join(tool_names)}}}")
         subparsers.required = True
         for tool_name in tool_names:
-            tool_parser = subparsers.add_parser(tool_name, prefix_chars=chr(0))
+            tool_parser = subparsers.add_parser(tool_name, prefix_chars=chr(0), add_help=False)
             tool_parser.add_argument("tool_args", metavar="args", nargs="...")
             tool_parser.set_defaults(tool_name=tool_name)
 
     def run(self, args: Namespace) -> Optional[int]:
 
         tool_name, tool_args = args.tool_name, args.tool_args
         tool = self.environ.get_tool(tool_name, **(args.configs or {}))
```

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/ios/frida.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/ios/ipa.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/ios/objection.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/objection.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/ios/scp.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/scp.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/commands/ios/sib.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/cli/device.py` & `linktools-0.8.4rc0/src/linktools/cli/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
 
 class DeviceCommandMixin:
 
     def add_device_options(self: "BaseCommand", parser: ArgumentParser):
 
         parser = parser or self._argument_parser
-        prefix = parser.prefix_chars
+        prefix = parser.prefix_chars[0] if parser.prefix_chars else "-"
 
         cache = DeviceCache(
             self.environ.get_temp_path(
                 "cache", "device", "mobile",
                 create_parent=True
             )
         )
@@ -199,15 +199,15 @@
 
 
 class AndroidCommandMixin:
 
     def add_android_options(self: BaseCommand, parser: ArgumentParser) -> None:
 
         parser = parser or self._argument_parser
-        prefix = parser.prefix_chars
+        prefix = parser.prefix_chars[0] if parser.prefix_chars else "-"
 
         cache = DeviceCache(
             self.environ.get_temp_path(
                 "cache", "device", "android",
                 create_parent=True
             )
         )
@@ -336,15 +336,15 @@
 
 
 class IOSCommandMixin:
 
     def add_ios_options(self: BaseCommand, parser: ArgumentParser):
 
         parser = parser or self._argument_parser
-        prefix = parser.prefix_chars
+        prefix = parser.prefix_chars[0] if parser.prefix_chars else "-"
 
         cache = DeviceCache(
             self.environ.get_temp_path(
                 "cache", "device", "ios",
                 create_parent=True
             )
         )
```

### Comparing `linktools-0.8.3rc1/src/linktools/container/__init__.py` & `linktools-0.8.4rc0/src/linktools/container/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/container/container.py` & `linktools-0.8.4rc0/src/linktools/container/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         match = re.match(r"^(\d{1,3})-(.*)$", name, re.M | re.I)
         if match:
             self._order = int(match.group(1))
             self._name = match.group(2)
         else:
             self._order = 900
             self._name = name
+        self._enable = False
         self.manager = manager
         self.logger = manager.logger
         self.root_path = root_path
 
     @property
     def name(self) -> str:
         return self._name
@@ -164,16 +165,20 @@
         return textwrap.dedent((self.__doc__ or "").strip())
 
     @property
     def order(self) -> int:
         return self._order
 
     @property
-    def enable(self):
-        return self.manager.config.get(f"{self.name.upper()}_ENABLE", type=bool, default=True)
+    def enable(self) -> bool:
+        return self._enable
+
+    @enable.setter
+    def enable(self, value: bool):
+        self._enable = value
 
     @property
     def dependencies(self) -> [str]:
         return []
 
     @property
     def configs(self) -> Dict[str, Any]:
@@ -261,31 +266,30 @@
         options = []
         if privileged:
             options.append("--privileged")
         if user:
             options.append("--user")
             options.append(user)
 
-        shell_args = []
-        if command:
-            shell_args = ["-c", command]
-
-        commands = []
-        for shell in ["/bin/zsh", "/bin/fish", "/bin/bash", "/bin/ash", "/bin/sh"]:
-            shell_command = [
-                "if" if len(commands) == 0 else "elif", "[", "-f", shell, "]", ";",
-                "then", shell, *shell_args, ";",
-            ]
-            commands.extend(shell_command)
-        commands.extend(["else", "sh", *shell_args, ";"])
-        commands.append("fi")
+        if not command:
+            commands = []
+            for shell in ["/bin/zsh", "/bin/fish", "/bin/bash", "/bin/ash", "/bin/sh"]:
+                shell_command = [
+                    "if" if len(commands) == 0 else "elif", "[", "-f", shell, "]", ";",
+                    "then", shell, ";",
+                ]
+                commands.extend(shell_command)
+            commands.extend(["else", "sh", ";"])
+            commands.append("fi")
+            commands = ("sh", "-c", utils.list2cmdline(commands))
+        else:
+            commands = utils.cmdline2list(command)
 
         return self.manager.create_docker_process(
-            "exec", "-it", *options, service.get("container_name"),
-            "sh", "-c", utils.list2cmdline(commands)
+            "exec", "-it", *options, service.get("container_name"), *commands
         ).call()
 
     @subcommand("logs", help="fetch the logs of container")
     @subcommand_argument("-f", "--follow",
                          help="follow log output")
     @subcommand_argument("-t", "--timestamps",
                          help="show timestamps")
```

### Comparing `linktools-0.8.3rc1/src/linktools/container/manager.py` & `linktools-0.8.4rc0/src/linktools/container/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,37 +27,38 @@
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import functools
 import json
 import os
 import os.path
 import shutil
-from typing import TYPE_CHECKING, Dict, Any, List, Union, Callable, Tuple, Set
+from typing import TYPE_CHECKING, Dict, Any, List, Union, Callable, Tuple, Set, TypeVar
 
 from filelock import FileLock
 
 from .container import BaseContainer, SimpleContainer, ContainerError
 from .repository import Repository
 from .. import utils, Config
 from .._environ import environ
 from ..decorator import cached_property
 
 if TYPE_CHECKING:
     from .._environ import BaseEnviron
 
+    T = TypeVar("T")
+
 
 class ContainerManager:
 
     def __init__(self, environ: "BaseEnviron", name: str = "aio"):  # all_in_one
         self.user = utils.get_user()
         self.uid = utils.get_uid()
         self.gid = utils.get_gid()
-
-        self.system = environ.system
-        self.machine = environ.machine
+        self.system = utils.get_system()
+        self.machine = utils.get_machine()
 
         self.environ = environ
         self.logger = environ.get_logger("container")
 
         self.config = self.environ.wrap_config(namespace="container", prefix="")
         self.config.update_defaults(
             COMPOSE_PROJECT_NAME=name or self.environ.name,
@@ -65,14 +66,16 @@
             DOCKER_UID=Config.Lazy(lambda cfg: utils.get_uid(cfg.get("DOCKER_USER", type=str))),
             DOCKER_GID=Config.Lazy(lambda cfg: utils.get_gid(cfg.get("DOCKER_USER", type=str))),
         )
 
         self.docker_container_name = "container.py"
         self.docker_compose_names = ("compose.yaml", "compose.yml", "docker-compose.yaml", "docker-compose.yml")
 
+        self._config_caches = {}
+
     @property
     def debug(self) -> bool:
         return os.environ.get("DEBUG", self.environ.debug)
 
     @cached_property
     def container_type(self) -> str:
         choices = ["docker", "docker-rootless", "podman"] \
@@ -178,107 +181,94 @@
         containers: List[BaseContainer] = []
 
         self.logger.debug(f"Load containers from assets")
         asset_path = environ.get_asset_path("containers")
         for container in self._walk_containers(asset_path, max_level=1):
             containers.append(container)
 
-        for url, repo in self.get_all_repos().items():
+        for url, meta in self.get_all_repos().items():
             self.logger.debug(f"Load containers from repository `{url}`")
-            repo_path = repo.get("repo_path")
+            repo_path = meta.get("repo_path")
             if not repo_path or not os.path.exists(repo_path) or not os.path.isdir(repo_path):
                 self.logger.warning(f"Repository `{url}` not found, skip.")
                 continue
-            for container in self._walk_containers(repo_path, max_level=2):
+            for container in self._walk_containers(repo_path, max_level=1):
                 containers.append(container)
 
         return containers
 
     def _walk_containers(self, path: str, max_level: int):
+        if not os.path.isdir(path):
+            return
         yield from self._load_container(path)
         if max_level <= 0:
             return
         for name in os.listdir(path):
-            root_path = os.path.join(path, name)
-            if os.path.isdir(root_path):
-                yield from self._walk_containers(root_path, max_level - 1)
+            yield from self._walk_containers(
+                os.path.join(path, name),
+                max_level - 1
+            )
 
     def _load_container(self, path: str):
-        if not os.path.isdir(path):
-            return
-
         container_path = os.path.join(path, self.docker_container_name)
         if os.path.exists(container_path):
             try:
                 name = path.replace(os.sep, ".")
-                module = utils.lazy_import_file(name, container_path)
+                module = utils.import_module_file(name, container_path)
                 for key, value in module.__dict__.items():
                     if isinstance(value, type) and issubclass(value, BaseContainer):
                         if not value.__abstract__:
                             container = value(self, path)
                             self.logger.debug(f"Load container {container.name} in {path}")
                             yield container
                             return
             except Exception as e:
                 self.logger.warning(f"Failed to load container from `{path}`: {e}")
+                return
 
         for compose_name in self.docker_compose_names:
             compose_path = os.path.join(path, compose_name)
             if os.path.exists(compose_path):
                 container = SimpleContainer(self, path)
                 self.logger.debug(f"Load container {container.name} in {path}")
                 yield container
                 return
 
-    def get_installed_containers(self) -> List[BaseContainer]:
+    def get_installed_containers(self, resolve: bool = True) -> List[BaseContainer]:
         with self._config_lock:
-            return self._load_installed_containers()
-
-    def check_installed_containers(self):
-        with self._config_lock:
-            for name in self._load_config(self._config_path):
-                if name not in self.containers:
-                    self.logger.warning(f"Not found container {name}, skip.")
-
-    def iter_installed_container_names(self):
-        containers = self.get_installed_containers()
-        containers = self.resolve_depend_containers(containers)
-        for container in containers:
-            yield container.name
+            containers = self._load_installed_containers()
+        if resolve:
+            containers = self.resolve_depend_containers(containers)
+        return containers
 
     def resolve_depend_containers(self, containers: List[BaseContainer]) -> List[BaseContainer]:
         order = lambda o: o() if callable(o) else o
         result: Dict[BaseContainer, Union[int, Callable[[], int]]] = dict()
         container_queue: Set[BaseContainer] = set(containers)
         while container_queue:
             container = container_queue.pop()
-            if not container.enable:
-                self.logger.debug(f"Skip disabled container {container.name}")
-                continue
             result.setdefault(container, container.order)
             for dependency in container.dependencies:
                 if dependency not in self.containers:
                     raise ContainerError(f"Dependency container {dependency} not found")
                 depend_container = self.containers[dependency]
-                if not depend_container.enable:
-                    continue
                 if depend_container not in result:
                     result.setdefault(depend_container, depend_container.order)
                     container_queue.add(depend_container)
                 if order(result[depend_container]) >= order(result[container]):
                     result[depend_container] = functools.partial(lambda o: order(result[o]) - 1, container)
-
         return sorted(result, key=lambda o: (order(result[o]), o.order, o.name))
 
     def prepare_installed_containers(self) -> List[BaseContainer]:
         self.logger.debug(f"Load container type: {self.container_type}")  # 加载容器类型
-        containers = self.get_installed_containers()
-        containers = self.resolve_depend_containers(containers)
+        containers = self.get_installed_containers(resolve=True)
         if not containers:
             raise ContainerError("No container installed")
+        for container in self.containers.values():
+            container.enable = container in containers
         for container in reversed(containers):
             self.config.update_defaults(**container.configs)
         for container in containers:
             container.on_init()
         for container in containers:
             if container.docker_file and self.debug:  # 加载每个容器的dockerfile
                 self.logger.debug(f"Generate Dockerfile for {container.name}")
@@ -289,21 +279,22 @@
     def add_installed_containers(self, *names: str) -> List[BaseContainer]:
         with self._config_lock:
             result = set()
             for name in names:
                 container = self.containers.get(name, None)
                 if container:
                     result.add(container)
-            installed_containers = self._load_installed_containers() + list(result)
-            self._dump_installed_containers(installed_containers)
+            containers = self._load_installed_containers(reload=True)
+            containers.extend(result)
+            self._dump_installed_containers(containers)
             return list(result)
 
     def remove_installed_containers(self, *names: str, force: bool = False) -> List[BaseContainer]:
         with self._config_lock:
-            containers = self._load_installed_containers()
+            containers = self._load_installed_containers(reload=True)
 
             result = set()
             remove_names = set(names)
             for name in set(names):
                 if name not in self.containers:
                     continue
                 for container in containers:
@@ -325,25 +316,25 @@
                     result.add(container)
                     containers.remove(container)
 
             self._dump_installed_containers(containers)
 
             return list(result)
 
-    def _load_installed_containers(self) -> List[BaseContainer]:
+    def _load_installed_containers(self, reload: bool = False) -> List[BaseContainer]:
         result = set()
-        for name in self._load_config(self._config_path):
+        for name in self._load_config(self._config_path, reload=reload, default=()):
             if name in self.containers:
                 result.add(self.containers[name])
         return list(result)
 
     def _dump_installed_containers(self, containers: List[BaseContainer]) -> None:
         self._dump_config(
             self._config_path,
-            list(set([container.name for container in containers]))
+            list(set([container.name for container in containers])),
         )
 
     def create_process(
             self,
             *args,
             privilege: bool = None,
             **kwargs
@@ -386,20 +377,19 @@
             commands.extend(["podman", "compose"])
         else:
             raise ContainerError(f"Invalid container type: {self.container_type}")
 
         options = []
         for container in containers:
             path = container.get_docker_compose_file()
-            if path:
-                options.extend(["-f", path])
-        append_env = kwargs.get("append_env", dict())
-        append_env.setdefault("COMPOSE_PROJECT_NAME", self.config.get("COMPOSE_PROJECT_NAME"))
+            if path and os.path.exists(path):
+                options.extend(["--file", path])
+        options.extend(["--project-name", self.config.get("COMPOSE_PROJECT_NAME")])
 
-        return self.create_process(*commands, *options, *args, append_env=append_env, privilege=privilege, **kwargs)
+        return self.create_process(*commands, *options, *args, privilege=privilege, **kwargs)
 
     def change_owner(self, path: str, user: str):
         if hasattr(os, "chown") and os.path.exists(path):
             info = os.stat(path)
             self.create_process(
                 "chown", "-R", user, path,
                 privilege=self.uid != info.st_uid or self.uid != utils.get_uid(user)
@@ -409,25 +399,26 @@
         with self._repo_lock:
             repos = self._load_config(self._repo_config_path)
         return repos
 
     def add_repo(self, url: str, branch: str = None, force: bool = False):
 
         with self._repo_lock:
-            repos = self._load_config(self._repo_config_path)
+            repos = self._load_config(self._repo_config_path, reload=True)
 
             def ensure_repo_not_exist(key):
                 if key not in repos:
                     return
                 if not force:
                     raise ContainerError(f"Repository `{key}` already exists.")
                 self._remove_repo_file(repos.pop(key))
                 self._dump_config(self._repo_config_path, repos)
 
-            if url.startswith("http://") or url.startswith("https://") or url.startswith("ssh://") or url.startswith("git@"):
+            if url.startswith("http://") or url.startswith("https://") or \
+                    url.startswith("ssh://") or url.startswith("git@"):
                 ensure_repo_not_exist(url)
                 self.logger.info(f"Add git repository: {url}")
                 repo_name = utils.guess_file_name(url)
                 repo_path = self._choose_repo_path(repo_name)
                 Repository.clone_with_progress(url, repo_path, branch)
                 repos[url] = dict(type="git", repo_path=repo_path, repo_name=repo_name)
 
@@ -460,15 +451,15 @@
                         raise ContainerError(f"Repository `{repo_path}` is dirty")
                     self.logger.warning(f"Repository `{repo_path}` is dirty, reset to HEAD")
                     repo.git.reset(hard=True)
                 repo.update_with_progress()
 
     def remove_repo(self, url: str):
         with self._repo_lock:
-            repos = self._load_config(self._repo_config_path)
+            repos = self._load_config(self._repo_config_path, reload=True)
             if url not in repos:
                 raise ContainerError(f"Repository `{url}` not found.")
             self._remove_repo_file(repos.pop(url))
             self._dump_config(self._repo_config_path, repos)
 
     def _choose_repo_path(self, name: str):
         index = 0
@@ -504,25 +495,26 @@
     def _repo_path(self):
         return self.environ.get_data_path("container", "repo", create_parent=True)
 
     @cached_property
     def _repo_config_path(self):
         return self.environ.get_data_path("container", "repo", "repo.json", create_parent=True)
 
-    def _load_config(self, path: str) -> Union[Dict, List, Tuple]:
+    def _load_config(self, path: str, reload: bool = False, default: Any = None) -> Union[Dict, List, Tuple]:
+        if reload:
+            self._config_caches.pop(path, None)
+        elif path in self._config_caches:
+            return self._config_caches[path]
         if os.path.exists(path):
             try:
-                return json.loads(
-                    utils.read_file(path, text=True)
-                )
+                self._config_caches[path] = json.loads(utils.read_file(path, text=True))
+                return self._config_caches[path]
             except Exception as e:
                 self.logger.warning(f"Failed to load config file {path}: {e}")
-        return {}
+        return default if default is not None else {}
 
     def _dump_config(self, path: str, config: Union[Dict, List, Tuple]):
         try:
-            utils.write_file(
-                path,
-                json.dumps(config, indent=2, ensure_ascii=False)
-            )
+            self._config_caches.pop(path, None)
+            utils.write_file(path, json.dumps(config, indent=2, ensure_ascii=False))
         except Exception as e:
             self.logger.warning(f"Failed to dump config file {path}: {e}")
```

### Comparing `linktools-0.8.3rc1/src/linktools/container/repository.py` & `linktools-0.8.4rc0/src/linktools/container/repository.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/decorator.py` & `linktools-0.8.4rc0/src/linktools/decorator.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/device.py` & `linktools-0.8.4rc0/src/linktools/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/frida/__init__.py` & `linktools-0.8.4rc0/src/linktools/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/frida/android.py` & `linktools-0.8.4rc0/src/linktools/frida/android.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/frida/app.py` & `linktools-0.8.4rc0/src/linktools/frida/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/frida/ios.py` & `linktools-0.8.4rc0/src/linktools/frida/ios.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/frida/script.py` & `linktools-0.8.4rc0/src/linktools/frida/script.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/frida/server.py` & `linktools-0.8.4rc0/src/linktools/frida/server.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/ida/__init__.py` & `linktools-0.8.4rc0/src/linktools/ida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/ida/ida.py` & `linktools-0.8.4rc0/src/linktools/ida/ida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/ios/ipa.py` & `linktools-0.8.4rc0/src/linktools/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/ios/sib.py` & `linktools-0.8.4rc0/src/linktools/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/metadata.py` & `linktools-0.8.4rc0/src/linktools/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 class __MissingType:
     __eq__ = lambda l, r: \
         l is r or type(l) is type(r)
 
 
 __name__ = "linktools"
 __release__ = True
-__version__ = "0.8.3rc1"
+__version__ = "0.8.4rc0"
 __missing__ = __MissingType()
 __description__ = f"""\
     ___       __   __              __
    / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.3rc1)
+  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.4rc0)
  / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
 /_/_/_/ /_/_/|_|\\__/\\____/\\____/_/____/
 """
```

### Comparing `linktools-0.8.3rc1/src/linktools/reactor.py` & `linktools-0.8.4rc0/src/linktools/reactor.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/references/fake_useragent/fake.py` & `linktools-0.8.4rc0/src/linktools/references/fake_useragent/fake.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/references/fake_useragent/utils.py` & `linktools-0.8.4rc0/src/linktools/references/fake_useragent/utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/rich.py` & `linktools-0.8.4rc0/src/linktools/rich.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,24 +186,23 @@
     def __init__(self):
         super().__init__(table_column=Column(no_wrap=True))
 
     def render(self, task: Task = None) -> Union[str, Text]:
         result = Text()
 
         handler = LogHandler.get_instance()
-        if handler:
-            if handler.show_time:
-                if len(result) > 0:
-                    result.append(" ")
-                result.append(handler.make_time_text())
-
-            if handler.show_level:
-                if len(result) > 0:
-                    result.append(" ")
-                result.append(handler.make_level_text(logging.INFO))
+        if handler and handler.show_time:
+            if len(result) > 0:
+                result.append(" ")
+            result.append(handler.make_time_text())
+
+        if handler and handler.show_level:
+            if len(result) > 0:
+                result.append(" ")
+            result.append(handler.make_level_text(logging.INFO))
 
         return result
 
 
 def create_simple_progress(*fields: str):
     columns = []
 
@@ -270,19 +269,19 @@
                 stream: Optional[TextIO] = None,
         ) -> str:
 
             prefix = []
             prefix_len = 0
 
             handler = LogHandler.get_instance()
-            if handler.show_time:
+            if handler and handler.show_time:
                 time = handler.make_time_text()
                 prefix.append(time)
                 prefix_len += time.cell_len + 1
-            if handler.show_level:
+            if handler and handler.show_level:
                 level = handler.make_level_text(logging.WARNING, "↳")
                 prefix.append(level)
                 prefix_len += level.cell_len + 1
 
             lines = prompt.split(include_separator=True, allow_blank=True)
             console.print(*(*prefix, lines[0]), sep=" ", end="")
             for i in range(1, len(lines)):
@@ -290,17 +289,17 @@
                 console.print(lines[i], new_line_start=True, end="")
 
             return console.input(password=password, stream=stream)
 
         def on_validate_error(self, value: str, error: InvalidResponse) -> None:
             prefix = Text("")
             handler = LogHandler.get_instance()
-            if handler.show_time:
+            if handler and handler.show_time:
                 prefix = prefix + handler.make_time_text() + " "
-            if handler.show_level:
+            if handler and handler.show_level:
                 prefix = prefix + handler.make_level_text(logging.ERROR, "↳") + " "
             self.console.print(prefix, error, sep="")
 
         def process_response(self, value: str) -> "PromptType":
             value = value.strip()
             if not allow_empty and not value:
                 raise InvalidResponse(self.validate_error_message)
```

### Comparing `linktools-0.8.3rc1/src/linktools/ssh.py` & `linktools-0.8.4rc0/src/linktools/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/utils/__init__.py` & `linktools-0.8.4rc0/src/linktools/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,23 +35,24 @@
     get_item, pop_item, get_list_item,
     get_md5, get_sha1, get_sha256, make_uuid, gzip_compress,
     get_path, read_file, write_file,
     get_lan_ip, get_wan_ip,
     parse_version, get_char_width,
     make_url, parse_header, parser_cookie, guess_file_name, user_agent,
     get_system, get_machine, get_user, get_uid, get_gid, get_shell_path,
+    import_module, import_module_file
 )
 
-from ._lazy import (
-    get_derived_type, lazy_load, lazy_iter, lazy_raise, lazy_import, lazy_import_file
+from ._proxy import (
+    get_derived_type, lazy_load, lazy_iter, lazy_raise
 )
 
 from ._subprocess import (
     Process,
-    list2cmdline,
+    list2cmdline, cmdline2list,
 )
 
 from ._port import (
     is_port_free,
     pick_unused_port,
     NoFreePortFoundError,
 )
```

### Comparing `linktools-0.8.3rc1/src/linktools/utils/_lazy.py` & `linktools-0.8.4rc0/src/linktools/utils/_proxy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 # Datetime  : 2022/11/4 下午1:18
 # Author    : HuJi <jihu.hj@alibaba-inc.com>
 
 import functools
-import os
-import sys
-from importlib.util import find_spec, LazyLoader, module_from_spec, spec_from_file_location
 from typing import TYPE_CHECKING, TypeVar, Type, Callable, Iterable
 
 if TYPE_CHECKING:
     from typing import ParamSpec
 
     T = TypeVar("T")
     P = ParamSpec("P")
@@ -303,60 +300,27 @@
 
 def lazy_iter(fn: "Callable[P, Iterable[T]]", *args: "P.args", **kwargs: "P.kwargs") -> "Iterable[T]":
     """
     延迟迭代
     :param fn: 延迟迭代的方法
     :return: proxy
     """
+
     class IterProxy(Iterable):
 
-        def __iter__(self):  # 用于 for 循环语句
-            return fn(*args, **kwargs)
+        def __init__(self):
+            self._data: Iterable[T] = _PROXY_MISSING
+
+        def __iter__(self):
+            if self._data == _PROXY_MISSING:
+                self._data = fn(*args, **kwargs)
+            return iter(self._data)
 
     return IterProxy()
 
 
 def raise_error(e: BaseException):
     raise e
 
 
 def lazy_raise(e: BaseException) -> "T":
     return lazy_load(raise_error, e)
-
-
-def lazy_import(name: str) -> "T":
-    """
-    延迟导入模块
-    :param name: 模块名
-    :return: module
-    """
-    spec = find_spec(name)
-    if not spec:
-        raise ModuleNotFoundError(f"No module named '{name}'")
-    loader = LazyLoader(spec.loader)
-    spec.loader = loader
-    module = module_from_spec(spec)
-    sys.modules[name] = module
-    loader.exec_module(module)
-    return module
-
-
-def lazy_import_file(name: str, path: str) -> "T":
-    """
-    延迟导入模块
-    :param name: 模块名
-    :param path: 模块路径
-    :return: module
-    """
-    if os.path.isdir(path):
-        path = os.path.join(path, "__init__.py")
-    if not os.path.exists(path):
-        raise ModuleNotFoundError(f"No such file or directory: '{path}'")
-    spec = spec_from_file_location(name, path)
-    if not spec:
-        raise ModuleNotFoundError(f"No module named '{name}'")
-    loader = LazyLoader(spec.loader)
-    spec.loader = loader
-    module = module_from_spec(spec)
-    sys.modules[name] = module
-    spec.loader.exec_module(module)
-    return module
```

### Comparing `linktools-0.8.3rc1/src/linktools/utils/_port.py` & `linktools-0.8.4rc0/src/linktools/utils/_port.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools/utils/_subprocess.py` & `linktools-0.8.4rc0/src/linktools/utils/_subprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 import errno
 import os
 import queue
+import shlex
 import subprocess
 import threading
-from typing import AnyStr, Tuple, Optional, IO, Callable, Any, Dict, Union
+from typing import AnyStr, Tuple, Optional, IO, Callable, Any, Dict, Union, List
 
 from . import Timeout, timeoutable
 from .._environ import environ
 from ..decorator import cached_property
 
-list2cmdline = subprocess.list2cmdline
+
+def list2cmdline(args: List[str]) -> str:
+    return subprocess.list2cmdline(args)
+
+
+def cmdline2list(cmdline: str) -> List[str]:
+    return shlex.split(cmdline)
 
 
 class Output:
     STDOUT = 1
     STDERR = 2
 
     def __init__(self, stdout: IO[AnyStr], stderr: IO[AnyStr]):
```

### Comparing `linktools-0.8.3rc1/src/linktools/utils/_utils.py` & `linktools-0.8.4rc0/src/linktools/utils/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,21 @@
 import inspect
 import os
 import platform
 import random
 import re
 import shutil
 import socket
+import sys
 import threading
 import time
 import uuid
 from collections.abc import Iterable, Sized
+from importlib.machinery import ModuleSpec
+from importlib.util import find_spec, LazyLoader, module_from_spec, spec_from_file_location
 from typing import TYPE_CHECKING, Union, Callable, Optional, Type, Any, List, TypeVar, Tuple, Set, Dict
 from urllib import parse
 from urllib.request import urlopen
 
 from .._environ import environ
 from ..decorator import singleton
 from ..metadata import __missing__
@@ -717,7 +720,51 @@
         if "ComSpec" in os.environ:
             shell_path = os.environ["ComSpec"]
             if shell_path and os.path.exists(shell_path):
                 return shell_path
         return shutil.which("powershell") or shutil.which("cmd")
 
     return ""
+
+
+def import_module(name: str, spec: ModuleSpec = None) -> "T":
+    """
+    延迟导入模块
+    :param name: 模块名
+    :param spec: 模块spec
+    :return: module
+    """
+    if name in sys.modules:
+        return sys.modules[name]
+    spec = spec or find_spec(name)
+    if not spec:
+        raise ModuleNotFoundError(f"No module named '{name}'")
+    loader = LazyLoader(spec.loader)
+    spec.loader = loader
+    module = module_from_spec(spec)
+    sys.modules[name] = module
+    loader.exec_module(module)
+    return module
+
+
+def import_module_file(name: str, path: str) -> "T":
+    """
+    延迟导入模块
+    :param name: 模块名
+    :param path: 模块路径
+    :return: module
+    """
+    if name in sys.modules:
+        return sys.modules[name]
+    if os.path.isdir(path):
+        path = os.path.join(path, "__init__.py")
+    if not os.path.exists(path):
+        raise ModuleNotFoundError(f"No such file or directory: '{path}'")
+    spec = spec_from_file_location(name, path)
+    if not spec:
+        raise ModuleNotFoundError(f"No module named '{name}'")
+    loader = LazyLoader(spec.loader)
+    spec.loader = loader
+    module = module_from_spec(spec)
+    sys.modules[name] = module
+    loader.exec_module(module)
+    return module
```

### Comparing `linktools-0.8.3rc1/src/linktools.egg-info/PKG-INFO` & `linktools-0.8.4rc0/src/linktools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.3rc1
+Version: 0.8.4rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -27,62 +27,60 @@
 Requires-Dist: scp; extra == "ssh"
 Provides-Extra: ssl
 Requires-Dist: pyOpenSSL; extra == "ssl"
 Provides-Extra: container
 Requires-Dist: GitPython; extra == "container"
 Requires-Dist: jinja2; extra == "container"
 Requires-Dist: pyyaml; extra == "container"
+Provides-Extra: argcomplete
+Requires-Dist: argcomplete>=2.0.0; extra == "argcomplete"
 Provides-Extra: all
 Requires-Dist: requests[socks]; extra == "all"
 Requires-Dist: frida>=15.0.0; extra == "all"
 Requires-Dist: objection; extra == "all"
 Requires-Dist: lief>0.10.1; extra == "all"
 Requires-Dist: python-magic; platform_system == "Linux" and extra == "all"
 Requires-Dist: python-magic; platform_system == "Darwin" and extra == "all"
 Requires-Dist: python-magic-bin; platform_system == "Windows" and extra == "all"
 Requires-Dist: paramiko; extra == "all"
 Requires-Dist: scp; extra == "all"
 Requires-Dist: pyOpenSSL; extra == "all"
 Requires-Dist: GitPython; extra == "all"
 Requires-Dist: jinja2; extra == "all"
 Requires-Dist: pyyaml; extra == "all"
+Requires-Dist: argcomplete>=2.0.0; extra == "all"
 
 # Linktools Toolkit
 
 ## 开始使用
 
 ### 依赖项
 
 python & pip (3.6及以上): <https://www.python.org/downloads/>
 
 ### 安装
 
 使用pip安装linktools
 
 ```bash
-# 可以pip直接安装linktools，也可以用以下命令安装github上的最新版本:
-# python3 -m pip install "linktools@ git+https://github.com/ice-black-tea/Zelda.git"
-python3 -m pip install -U "linktools[all]" # 按需添加依赖项，推荐使用all添加所有依赖项
+# pip直接安装linktools，按需添加依赖项，推荐使用all添加所有依赖项
+python3 -m pip install -U "linktools[all]"
+# 也可以用以下命令安装github上的最新版本:
+# python3 -m pip install --ignore-installed "linktools@ git+https://github.com/ice-black-tea/linktools.git@master"
 ```
 
-额外的依赖项以及相应功能如下：
-```
-linktools[requests]：下载时使用requests包，并且支持socks5代理
-linktools[lief]：为grep提供服务，可解析apk、elf等文件格式（注意：对于mac系统，需要额外安装brew install libmagic）
-linktools[frida]：集成frida hook框架，支持android、ios hook
-linktooks[objection]：集成objection框架
-linktools[ssh]：使用ssh连接越狱后的iphone
-linktools[ssl]：解析证书时使用
-```
+额外的依赖项以及相应功能可通过[requirements.yml](https://raw.githubusercontent.com/ice-black-tea/linktools/master/requirements.yml)查看
 
 ### 配置alias（推荐）
 
 对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置alias，简化调用方式：
 
 ```bash
+eval "$(ct-env --silent complete --shell bash)" # 给命令添加自动补全功能
+
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
 alias apktool="ct-tools apktool"
 alias burpsuite="ct-tools --set version=2023.10 burpsuite"
 alias jadx="JAVA_OPTS=-Xmx8g ct-tools --set version=1.4.7 jadx-gui" # 指定jadx版本号，配置jvm最大内存
@@ -205,15 +203,15 @@
 </details>
 
 #### 👉 ct-tools
 
 <details>
 <summary>读取配置文件，即可下载使用对应工具，声明了adb、jadx、apktool、baksmali等常用工具</summary>
 
-所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/src/linktools/assets/tools.yml)查看
+所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/assets/tools.yml)查看
 
 ```
 $ usage: ct-tools [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-c | --download | --clear | -d] ...
 
 Tools downloaded from the web
 
     ___       __   __              __
@@ -483,15 +481,15 @@
   -c IP[:PORT], --connect IP[:PORT]
                         use device with TCP/IP
   -l, --last            use last device
 ```
 
 **输出效果**
 
-![apps](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/images/apps.png)
+![apps](https://raw.githubusercontent.com/ice-black-tea/linktools/master/images/apps.png)
 
 </details>
 
 #### 👉 at-frida
 
 <details>
 <summary>该功能旨在方便使用frida，可自动下载server，支持加载远程脚本，并内置了常用功能</summary>
@@ -546,29 +544,29 @@
   --emulator            use TCP/IP device (adb -e option)
   --connect IP[:PORT]   use device with TCP/IP
   --last                use last device
 ```
 
 **1) 以命令行方式运行**
 
-比如要加载 [https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js) 脚本：
+比如要加载 [https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js](https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js) 脚本：
 
 在终端中运行
 ```bash
-$ at-frida -c https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js
+$ at-frida -c https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js
 ```
 
 输出如下：
 ```
-[15:24:09]  I  Download ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js)
+[15:24:09]  I  Download ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js)
 [15:24:11]  W  java.js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1,704/513 bytes ? 100% eta 0:00:00
-[15:24:13]  I  Load trusted ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/Zelda/master/agent/frida/test/java.js)
+[15:24:13]  I  Load trusted ShareScript(filename=https://raw.githubusercontent.com/ice-black-tea/linktools/master/agent/frida/test/java.js)
 [15:24:14]  I  Start frida server ...
 [15:24:15]  I  Frida server is running ...
-[15:24:18]  I  Load ScriptFile(filename=/Users/huji/Projects/Zelda/src/linktools/assets/frida.min.js)
+[15:24:18]  I  Load ScriptFile(filename=/Users/huji/Projects/linktools/src/linktools/assets/frida.min.js)
 [15:24:19]  I  Session(pid=32087, name=马赛克) attached
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.access$300()
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.access$600()
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.decode(java.lang.String)
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.encode(java.lang.String)
 [15:24:19]  I  Hook method: java.lang.String android.net.Uri.encode(java.lang.String, java.lang.String)
 [15:24:19]  I  Hook method: android.net.Uri android.net.Uri.fromFile(java.io.File)
@@ -673,15 +671,15 @@
                    "java.lang.Thread.run(Thread.java:923)"
                  ]
                }
 ```
 
 **2) 当然也可以使用python方式调用**
 
-执行如下python脚本即可自动开启frida-server，并将js代码注入到指定进程中，若需要同时注入子进程，按[src/linktools/cli/scripts/android/frida.py](https://raw.githubusercontent.com/ice-black-tea/Zelda/master/src/linktools/cli/scripts/android/frida.py) 重写 FridaApplication 的 on_spawn_added 方法即可
+执行如下python脚本即可自动开启frida-server，并将js代码注入到指定进程中，若需要同时注入子进程，按[src/linktools/cli/scripts/android/frida.py](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/cli/scripts/android/frida.py) 重写 FridaApplication 的 on_spawn_added 方法即可
 
 ```python
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import logging
 from linktools.frida import FridaApplication, FridaEvalCode
 from linktools.frida.android import AndroidFridaServer
```

### Comparing `linktools-0.8.3rc1/src/linktools.egg-info/SOURCES.txt` & `linktools-0.8.4rc0/src/linktools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -92,11 +92,11 @@
 src/linktools/references/fake_useragent/__init__.py
 src/linktools/references/fake_useragent/errors.py
 src/linktools/references/fake_useragent/fake.py
 src/linktools/references/fake_useragent/log.py
 src/linktools/references/fake_useragent/settings.py
 src/linktools/references/fake_useragent/utils.py
 src/linktools/utils/__init__.py
-src/linktools/utils/_lazy.py
 src/linktools/utils/_port.py
+src/linktools/utils/_proxy.py
 src/linktools/utils/_subprocess.py
 src/linktools/utils/_utils.py
```

### Comparing `linktools-0.8.3rc1/src/linktools.egg-info/entry_points.txt` & `linktools-0.8.4rc0/src/linktools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc1/src/linktools.egg-info/requires.txt` & `linktools-0.8.4rc0/src/linktools.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 lief>0.10.1
 paramiko
 scp
 pyOpenSSL
 GitPython
 jinja2
 pyyaml
+argcomplete>=2.0.0
 
 [all:platform_system == "Darwin"]
 python-magic
 
 [all:platform_system == "Linux"]
 python-magic
 
 [all:platform_system == "Windows"]
 python-magic-bin
 
+[argcomplete]
+argcomplete>=2.0.0
+
 [container]
 GitPython
 jinja2
 pyyaml
 
 [frida]
 frida>=15.0.0
```

