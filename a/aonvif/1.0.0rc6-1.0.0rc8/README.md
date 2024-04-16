# Comparing `tmp/aonvif-1.0.0rc6.tar.gz` & `tmp/aonvif-1.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aonvif-1.0.0rc6.tar", last modified: Thu Dec 15 13:39:18 2022, max compression
+gzip compressed data, was "aonvif-1.0.0rc8.tar", last modified: Tue Apr 16 06:31:20 2024, max compression
```

## Comparing `aonvif-1.0.0rc6.tar` & `aonvif-1.0.0rc8.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.081811 aonvif-1.0.0rc6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.049811 aonvif-1.0.0rc6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.061811 aonvif-1.0.0rc6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2022-12-15 13:39:18.081811 aonvif-1.0.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.061811 aonvif-1.0.0rc6/aonvif/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15781 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.065811 aonvif-1.0.0rc6/aonvif/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23286 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/b-2.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/bf-2.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      511 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/include
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/soap-envelope
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/t-1.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.065811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/accesscontrol/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.065811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/accesscontrol/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/accesscontrol/wsdl/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/accessrules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.065811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/accessrules/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)    30010 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/accessrules/wsdl/accessrules.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/accessrules/wsdl/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55762 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/actionengine.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/advancedsecurity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.065811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/advancedsecurity/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)   160937 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/advancedsecurity/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/advancedsecurity/wsdl/index.html
--rw-r--r--   0 runner    (1001) docker     (123)   157969 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/advancedsecurity/wsdl/security.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)    30999 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/analyticsdevice.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/appmgmt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.069811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/appmgmt/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)    24676 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/appmgmt/wsdl/appmgmt.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/appmgmt/wsdl/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/authenticationbehavior/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.069811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/authenticationbehavior/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)    58250 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/authenticationbehavior/wsdl/authenticationbehavior.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/authenticationbehavior/wsdl/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/credential/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.069811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/credential/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)    85719 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/credential/wsdl/credential.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/credential/wsdl/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/device/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.069811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/device/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)   182151 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/device/wsdl/devicemgmt.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)    64785 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/deviceio.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.069811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/display/
--rw-r--r--   0 runner    (1001) docker     (123)    20747 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/display/display.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.069811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/display/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)    20747 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/display/wsdl/index.htm
--rw-r--r--   0 runner    (1001) docker     (123)    23864 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/display.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/doorcontrol/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.069811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/doorcontrol/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/doorcontrol/wsdl/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.069811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/events/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)    20274 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/events/wsdl/bw-2-vs-mod.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)    47663 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/events/wsdl/event-vs.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)    47632 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/events/wsdl/event.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/events/wsdl/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/federatedsearch.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/media/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.069811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/media/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)   171458 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/media/wsdl/media.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.073811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/pacs/
--rw-r--r--   0 runner    (1001) docker     (123)    78387 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/pacs/accesscontrol.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)    69658 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/pacs/doorcontrol.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/pacs/types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/provisioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.073811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/provisioning/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)    24588 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/provisioning/wsdl/provisioning.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)    16593 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/receiver.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)    48265 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/recording.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/replay.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.053811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/schedule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.073811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/schedule/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/schedule/wsdl/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    56036 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/schedule/wsdl/schedule.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.073811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    16879 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/schema/common.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    21132 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/schema/metadatastream.xsd
--rwxr-xr-x   0 runner    (1001) docker     (123)   384657 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/schema/onvif.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    42041 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/search.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.057811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/thermal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.073811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/thermal/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/thermal/wsdl/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    33353 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/thermal/wsdl/thermal.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.073811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/topics/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/topics/topicns.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.057811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/uplink/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.073811 aonvif-1.0.0rc6/aonvif/wsdl/ver10/uplink/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/uplink/wsdl/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver10/uplink/wsdl/uplink.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.057811 aonvif-1.0.0rc6/aonvif/wsdl/ver20/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.077811 aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)    18232 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/humanbody.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    20772 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/humanface.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    17909 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/radiometry.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/rules.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.077811 aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)    33245 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/wsdl/analytics.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/wsdl/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.057811 aonvif-1.0.0rc6/aonvif/wsdl/ver20/imaging/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.077811 aonvif-1.0.0rc6/aonvif/wsdl/ver20/imaging/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)    26153 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/imaging/wsdl/imaging.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.057811 aonvif-1.0.0rc6/aonvif/wsdl/ver20/media/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.077811 aonvif-1.0.0rc6/aonvif/wsdl/ver20/media/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/media/wsdl/index.html
--rw-r--r--   0 runner    (1001) docker     (123)   108963 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/media/wsdl/media.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.057811 aonvif-1.0.0rc6/aonvif/wsdl/ver20/ptz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.077811 aonvif-1.0.0rc6/aonvif/wsdl/ver20/ptz/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)    60601 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/ptz/wsdl/ptz.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.081811 aonvif-1.0.0rc6/aonvif/wsdl/ver20/util/
--rw-r--r--   0 runner    (1001) docker     (123)    86523 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/util/federated_search_documentation.html
--rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/util/fedsearch-docu-viewer.xsl
--rw-r--r--   0 runner    (1001) docker     (123)    94525 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/util/onvif-wsdl-viewer.xsl
--rw-r--r--   0 runner    (1001) docker     (123)    39290 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ver20/util/operationIndex.html
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/ws-addr.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/xml.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/aonvif/wsdl/xmlmime
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.061811 aonvif-1.0.0rc6/aonvif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2022-12-15 13:39:17.000000 aonvif-1.0.0rc6/aonvif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2022-12-15 13:39:18.000000 aonvif-1.0.0rc6/aonvif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 13:39:17.000000 aonvif-1.0.0rc6/aonvif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-15 13:39:17.000000 aonvif-1.0.0rc6/aonvif.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 13:39:16.000000 aonvif-1.0.0rc6/aonvif.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-15 13:39:17.000000 aonvif-1.0.0rc6/aonvif.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-15 13:39:17.000000 aonvif-1.0.0rc6/aonvif.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.081811 aonvif-1.0.0rc6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/examples/continuous_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/examples/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/examples/rotate_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/examples/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-15 13:39:18.081811 aonvif-1.0.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:39:18.081811 aonvif-1.0.0rc6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2022-12-15 13:38:48.000000 aonvif-1.0.0rc6/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.231448 aonvif-1.0.0rc8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.207448 aonvif-1.0.0rc8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.215448 aonvif-1.0.0rc8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-16 06:31:20.231448 aonvif-1.0.0rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.215448 aonvif-1.0.0rc8/aonvif/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17829 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.219448 aonvif-1.0.0rc8/aonvif/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/b-2.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/bf-2.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/include
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/soap-envelope
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/t-1.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.219448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.207448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/accesscontrol/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.219448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/accesscontrol/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/accesscontrol/wsdl/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.207448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/accessrules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.219448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/accessrules/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)    30010 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/accessrules/wsdl/accessrules.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/accessrules/wsdl/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    55762 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/actionengine.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.207448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/advancedsecurity/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.223448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/advancedsecurity/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)   160937 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/advancedsecurity/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/advancedsecurity/wsdl/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)   157969 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/advancedsecurity/wsdl/security.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)    30999 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/analyticsdevice.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/appmgmt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.223448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/appmgmt/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/appmgmt/wsdl/appmgmt.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/appmgmt/wsdl/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/authenticationbehavior/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.223448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/authenticationbehavior/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)    58250 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/authenticationbehavior/wsdl/authenticationbehavior.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/authenticationbehavior/wsdl/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/credential/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.223448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/credential/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)    85719 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/credential/wsdl/credential.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/credential/wsdl/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/device/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.223448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/device/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)   182151 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/device/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)    64785 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/deviceio.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.223448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/display/
+-rw-r--r--   0 runner    (1001) docker     (127)    20747 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/display/display.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.223448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/display/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)    20747 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/display/wsdl/index.htm
+-rw-r--r--   0 runner    (1001) docker     (127)    23864 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/display.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/doorcontrol/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.223448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/doorcontrol/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/doorcontrol/wsdl/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.223448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/events/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/events/wsdl/bw-2-vs-mod.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)    47663 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/events/wsdl/event-vs.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)    47632 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/events/wsdl/event.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/events/wsdl/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/federatedsearch.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/media/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.223448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/media/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)   171458 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/media/wsdl/media.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.227448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/pacs/
+-rw-r--r--   0 runner    (1001) docker     (127)    78387 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/pacs/accesscontrol.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)    69658 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/pacs/doorcontrol.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/pacs/types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/provisioning/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.227448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/provisioning/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)    24588 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/provisioning/wsdl/provisioning.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)    16593 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/receiver.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)    48265 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/recording.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/replay.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/schedule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.227448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/schedule/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/schedule/wsdl/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    56036 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/schedule/wsdl/schedule.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.227448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    16879 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/schema/common.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/schema/metadatastream.xsd
+-rwxr-xr-x   0 runner    (1001) docker     (127)   384657 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/schema/onvif.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    42041 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/search.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/thermal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.227448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/thermal/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/thermal/wsdl/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    33353 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/thermal/wsdl/thermal.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.227448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/topics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/topics/topicns.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/uplink/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.227448 aonvif-1.0.0rc8/aonvif/wsdl/ver10/uplink/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/uplink/wsdl/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver10/uplink/wsdl/uplink.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.215448 aonvif-1.0.0rc8/aonvif/wsdl/ver20/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.227448 aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/humanbody.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    20772 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/humanface.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/radiometry.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/rules.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.231448 aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)    33245 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/wsdl/analytics.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/wsdl/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.211448 aonvif-1.0.0rc8/aonvif/wsdl/ver20/imaging/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.231448 aonvif-1.0.0rc8/aonvif/wsdl/ver20/imaging/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)    26153 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/imaging/wsdl/imaging.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.215448 aonvif-1.0.0rc8/aonvif/wsdl/ver20/media/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.231448 aonvif-1.0.0rc8/aonvif/wsdl/ver20/media/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/media/wsdl/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)   108963 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/media/wsdl/media.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.215448 aonvif-1.0.0rc8/aonvif/wsdl/ver20/ptz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.231448 aonvif-1.0.0rc8/aonvif/wsdl/ver20/ptz/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)    60601 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/ptz/wsdl/ptz.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.231448 aonvif-1.0.0rc8/aonvif/wsdl/ver20/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    86523 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/util/federated_search_documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/util/fedsearch-docu-viewer.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    94525 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/util/onvif-wsdl-viewer.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    39290 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ver20/util/operationIndex.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/xml.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/aonvif/wsdl/xmlmime
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.219448 aonvif-1.0.0rc8/aonvif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-16 06:31:20.000000 aonvif-1.0.0rc8/aonvif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-16 06:31:20.000000 aonvif-1.0.0rc8/aonvif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 06:31:20.000000 aonvif-1.0.0rc8/aonvif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 06:31:20.000000 aonvif-1.0.0rc8/aonvif.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 06:31:19.000000 aonvif-1.0.0rc8/aonvif.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-16 06:31:20.000000 aonvif-1.0.0rc8/aonvif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 06:31:20.000000 aonvif-1.0.0rc8/aonvif.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.231448 aonvif-1.0.0rc8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/examples/continuous_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/examples/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/examples/rotate_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/examples/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-16 06:31:20.231448 aonvif-1.0.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:31:20.231448 aonvif-1.0.0rc8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-16 06:31:00.000000 aonvif-1.0.0rc8/tests/test_client.py
```

### Comparing `aonvif-1.0.0rc6/.github/workflows/ci.yml` & `aonvif-1.0.0rc8/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   lint:
     name: Run lint
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python_version: ['3.8', '3.9', '3.10', '3.11']
+        python_version: ['3.9', '3.10', '3.11']
     steps:
     - name: Checkout source repository for Python ${{ matrix.python_version }}
       uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python_version }}
       uses: actions/setup-python@v1
       with:
@@ -26,15 +26,15 @@
   test:
     name: Run tests
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python_version: ['3.8', '3.9', '3.10', '3.11']
+        python_version: ['3.9', '3.10', '3.11']
     steps:
     - name: Checkout source repository for Python ${{ matrix.python_version }}
       uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python_version }}
       uses: actions/setup-python@v1
       with:
```

### Comparing `aonvif-1.0.0rc6/LICENSE` & `aonvif-1.0.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/Makefile` & `aonvif-1.0.0rc8/Makefile`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/PKG-INFO` & `aonvif-1.0.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: aonvif
-Version: 1.0.0rc6
+Version: 1.0.0rc8
 Summary: ONVIF asynchronous client implementation in Python
 Home-page: https://github.com/martyanov/aonvif
 Author: Andrey Martyanov
 Author-email: andrey@martyanov.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/martyanov/aonvif/issues
 Project-URL: Repository, https://github.com/martyanov/aonvif
 Keywords: onvif,client,asyncio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8.1,<4
+Requires-Python: >=3.9.1,<4
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 aonvif
 ======
```

### Comparing `aonvif-1.0.0rc6/README.rst` & `aonvif-1.0.0rc8/README.rst`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/cli.py` & `aonvif-1.0.0rc8/aonvif/cli.py`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/client.py` & `aonvif-1.0.0rc8/aonvif/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import datetime
+import functools
 import logging
 import os
 import typing
 
 import zeep.cache
 import zeep.client
 import zeep.exceptions
 import zeep.helpers
 import zeep.proxy
 import zeep.transports
+import zeep.wsdl
 import zeep.wsse.username
 
 from . import exceptions
 from . import wsdl
 
 
 logger = logging.getLogger('aonvif')
@@ -28,14 +30,26 @@
             return func(*args, **kwargs)
         except Exception as e:
             raise exceptions.ONVIFError(e)
 
     return wrapped
 
 
+@functools.cache
+def _get_wsdl_document(path: str):
+    return zeep.wsdl.Document(
+        location=path,
+        transport=zeep.transports.AsyncTransport(cache=MemoryCache()),
+        settings=zeep.client.Settings(
+            strict=False,
+            xml_huge_tree=True,
+        ),
+    )
+
+
 class UsernameToken(zeep.wsse.username.UsernameToken):
     """UsernameDigestToken class, with a time drift parameter that can be adjusted.
 
     This allows authentication on cameras without being time synchronized.
     Please note that using NTP on both end is the recommended solution,
     this should only be used in 'safe' environments.
     """
@@ -136,14 +150,17 @@
         username: str,
         password: str,
         url: str,
         binding_name: str,
         use_token_digest: bool = True,
         device_time_drift: typing.Optional[datetime.timedelta] = None,
     ):
+        if not isinstance(url, str) or not os.path.exists(url):
+            raise RuntimeError('ONVIFService url must be valid path')
+
         self.url = url
         self.xaddr = xaddr
 
         # Create security token
         wsse = UsernameToken(
             username,
             password,
@@ -152,17 +169,20 @@
         )
 
         # Client settings
         settings = zeep.client.Settings()
         settings.strict = False
         settings.xml_huge_tree = True
 
+        # Parse wsdl document
+        wsdl = _get_wsdl_document(url)
+
         # Create client
         self._client = zeep.client.AsyncClient(
-            wsdl=url,
+            wsdl=wsdl,
             wsse=wsse,
             settings=settings,
             transport=zeep.transports.AsyncTransport(cache=MemoryCache()),
         )
 
         # Create service proxy, it's a workaround as zeep still
         # doesn't support AsyncServiceProxy for AsyncClient
@@ -270,17 +290,55 @@
         self._device_time_drift = None
 
         # Known xaddrs
         self._xaddrs = {}
 
         # Currently initialized services
         self._services = {}
+        self._capabilities = None
 
         self.to_dict = ONVIFService.to_dict
 
+    def set_capabilities(self, capabilities: dict):
+        """Set custom capabilities.
+
+        :param capabilities: Dictionary of camera capabilities.
+                             It must have the following format:
+                             {
+                                "Media": {
+                                    "XAddr": "http://{host}/{xaddr_path_1},
+                                },
+                                "PTZ": {
+                                    "XAddr": "http://{host}/{xaddr_path_2},
+                                },
+                             }
+        """
+
+        self._validate_capabilities(capabilities)
+        self._capabilities = capabilities
+
+    def _validate_capabilities(self, capabilities: dict):
+        if not isinstance(capabilities, dict):
+            raise RuntimeError('Capabilities type must be dictionary')
+
+        for key, capability in capabilities.items():
+            if not isinstance(key, str):
+                raise RuntimeError('Capabilities key type must be string')
+
+            if not isinstance(capability, dict):
+                raise RuntimeError('Capability type must be dictionary')
+
+            xaddr = capability.get('XAddr')
+
+            if xaddr is None:
+                raise RuntimeError('Capability XAddr is missing')
+
+            if not isinstance(xaddr, str):
+                raise RuntimeError('Capability XAddr type must be string')
+
     async def update_xaddrs(self):
         """Update xaddrs for services."""
 
         # Create devicemgmt service
         devicemgmt = self.create_devicemgmt_service()
 
         # If time adjusting needed, calculate drift
@@ -294,17 +352,20 @@
                 device_time.Time.Minute,
                 device_time.Time.Second,
             )
             self._device_time_drift = device_dt - datetime.datetime.utcnow()
 
         # Get XAddr of services on the device
         self._xaddrs = {}
-        capabilities = await devicemgmt.GetCapabilities({'Category': 'All'})
-        for name in capabilities:
-            capability = capabilities[name]
+
+        if not self._capabilities:
+            self._capabilities = await devicemgmt.GetCapabilities({'Category': 'All'})
+
+        for name in self._capabilities:
+            capability = self._capabilities[name]
             try:
                 if name.lower() in wsdl.SERVICES and capability is not None:
                     namespace = wsdl.SERVICES[name.lower()]['ns']
                     self._xaddrs[namespace] = capability['XAddr']
             except Exception:
                 logger.exception(f'Unexpected service type: {name!r}')
```

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/__init__.py` & `aonvif-1.0.0rc8/aonvif/wsdl/__init__.py`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/b-2.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/bf-2.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/soap-envelope` & `aonvif-1.0.0rc8/aonvif/wsdl/soap-envelope`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/t-1.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/accessrules/wsdl/accessrules.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/accessrules/wsdl/accessrules.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/actionengine.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/advancedsecurity/wsdl/advancedsecurity.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/advancedsecurity/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/advancedsecurity/wsdl/security.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/advancedsecurity/wsdl/security.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/analyticsdevice.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/appmgmt/wsdl/appmgmt.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/appmgmt/wsdl/appmgmt.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/authenticationbehavior/wsdl/authenticationbehavior.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/authenticationbehavior/wsdl/authenticationbehavior.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/credential/wsdl/credential.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/credential/wsdl/credential.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/device/wsdl/devicemgmt.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/device/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/deviceio.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/display/display.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/display/display.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/display/wsdl/index.htm` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/display/wsdl/index.htm`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/display.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/display.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/events/wsdl/bw-2-vs-mod.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/events/wsdl/bw-2-vs-mod.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/events/wsdl/event-vs.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/events/wsdl/event-vs.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/events/wsdl/event.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/events/wsdl/event.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/federatedsearch.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/federatedsearch.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/media/wsdl/media.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/media/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/pacs/accesscontrol.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/pacs/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/pacs/doorcontrol.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/pacs/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/pacs/types.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/pacs/types.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/provisioning/wsdl/provisioning.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/provisioning/wsdl/provisioning.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/receiver.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/recording.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/recording.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/replay.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/replay.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/schedule/wsdl/schedule.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/schedule/wsdl/schedule.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/schema/common.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/schema/common.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/schema/metadatastream.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/schema/metadatastream.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/schema/onvif.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/schema/onvif.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/search.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/search.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/thermal/wsdl/thermal.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/thermal/wsdl/thermal.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/topics/topicns.xml` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/topics/topicns.xml`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver10/uplink/wsdl/uplink.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver10/uplink/wsdl/uplink.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/humanbody.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/humanbody.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/humanface.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/humanface.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/radiometry.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/radiometry.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/rules.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/rules.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver20/analytics/wsdl/analytics.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver20/analytics/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver20/imaging/wsdl/imaging.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver20/imaging/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver20/media/wsdl/media.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver20/media/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver20/ptz/wsdl/ptz.wsdl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver20/ptz/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver20/util/federated_search_documentation.html` & `aonvif-1.0.0rc8/aonvif/wsdl/ver20/util/federated_search_documentation.html`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver20/util/onvif-wsdl-viewer.xsl` & `aonvif-1.0.0rc8/aonvif/wsdl/ver20/util/onvif-wsdl-viewer.xsl`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ver20/util/operationIndex.html` & `aonvif-1.0.0rc8/aonvif/wsdl/ver20/util/operationIndex.html`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/ws-addr.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/xml.xsd` & `aonvif-1.0.0rc8/aonvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif/wsdl/xmlmime` & `aonvif-1.0.0rc8/aonvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/aonvif.egg-info/PKG-INFO` & `aonvif-1.0.0rc8/aonvif.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: aonvif
-Version: 1.0.0rc6
+Version: 1.0.0rc8
 Summary: ONVIF asynchronous client implementation in Python
 Home-page: https://github.com/martyanov/aonvif
 Author: Andrey Martyanov
 Author-email: andrey@martyanov.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/martyanov/aonvif/issues
 Project-URL: Repository, https://github.com/martyanov/aonvif
 Keywords: onvif,client,asyncio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8.1,<4
+Requires-Python: >=3.9.1,<4
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 aonvif
 ======
```

### Comparing `aonvif-1.0.0rc6/aonvif.egg-info/SOURCES.txt` & `aonvif-1.0.0rc8/aonvif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/examples/continuous_move.py` & `aonvif-1.0.0rc8/examples/continuous_move.py`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/examples/events.py` & `aonvif-1.0.0rc8/examples/events.py`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/examples/rotate_image.py` & `aonvif-1.0.0rc8/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/examples/streaming.py` & `aonvif-1.0.0rc8/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `aonvif-1.0.0rc6/setup.py` & `aonvif-1.0.0rc8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     license='MIT',
     keywords=['onvif', 'client', 'asyncio'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     zip_safe=False,
     project_urls={
         'Bug Reports': 'https://github.com/martyanov/aonvif/issues',
@@ -41,15 +40,15 @@
         '': [
             '*.rst',
         ],
         'aonvif.wsdl': [
             '**/*',
         ],
     },
-    python_requires='>=3.8.1,<4',
+    python_requires='>=3.9.1,<4',
     setup_requires=[
         'setuptools_scm==6.3.2',
     ],
     install_requires=[
         'zeep[async]>=4,<5',
     ],
     extras_require={
@@ -62,14 +61,15 @@
             'pep8-naming==0.13.2',
             'twine==4.0.2',
         ],
         'test': [
             'pytest-asyncio==0.20.2',
             'pytest-cov==4.0.0',
             'pytest==7.2.0',
+            'pytest-mock==3.14.0',
         ],
     },
     entry_points={
         'console_scripts': [
             'aonvif-cli=aonvif.cli:main',
         ],
     },
```

### Comparing `aonvif-1.0.0rc6/tests/test.py` & `aonvif-1.0.0rc8/tests/test.py`

 * *Files identical despite different names*

