# Comparing `tmp/falcon_toolkit-3.3.1.tar.gz` & `tmp/falcon_toolkit-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_toolkit-3.3.1.tar", max compression
+gzip compressed data, was "falcon_toolkit-3.4.0.tar", max compression
```

## Comparing `falcon_toolkit-3.3.1.tar` & `falcon_toolkit-3.4.0.tar`

### file list

```diff
@@ -1,38 +1,44 @@
--rw-r--r--   0        0        0     1070 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/LICENSE.md
--rw-r--r--   0        0        0    20636 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/README.md
--rw-r--r--   0        0        0      188 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/__init__.py
--rw-r--r--   0        0        0      174 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/__init__.py
--rw-r--r--   0        0        0     1847 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/auth.py
--rw-r--r--   0        0        0      191 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/auth_backends/__init__.py
--rw-r--r--   0        0        0      449 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/auth_backends/default.py
--rw-r--r--   0        0        0     6254 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/auth_backends/public_mssp.py
--rw-r--r--   0        0        0     4087 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/auth_backends/public_single_cid.py
--rw-r--r--   0        0        0     2709 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/auth_backends/utils.py
--rw-r--r--   0        0        0     1846 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/cli.py
--rw-r--r--   0        0        0     7974 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/config.py
--rw-r--r--   0        0        0      962 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/console_utils.py
--rw-r--r--   0        0        0      550 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/constants.py
--rw-r--r--   0        0        0     2767 2023-09-15 13:26:45.642351 falcon_toolkit-3.3.1/falcon_toolkit/common/logging_config.py
--rw-r--r--   0        0        0      340 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/common/meta.py
--rw-r--r--   0        0        0     1599 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/common/namespace.py
--rw-r--r--   0        0        0     1950 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/common/utils.py
--rwxr-xr-x   0        0        0     9953 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/falcon.py
--rw-r--r--   0        0        0      116 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/hosts/__init__.py
--rw-r--r--   0        0        0     2390 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/hosts/cli.py
--rw-r--r--   0        0        0     5651 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/hosts/host_search.py
--rw-r--r--   0        0        0      120 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/policies/__init__.py
--rw-r--r--   0        0        0     5058 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/policies/cli.py
--rw-r--r--   0        0        0     1049 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/policies/constants.py
--rw-r--r--   0        0        0     3354 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/policies/container.py
--rw-r--r--   0        0        0     3659 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/policies/describe.py
--rw-r--r--   0        0        0      160 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/shell/__init__.py
--rw-r--r--   0        0        0     6989 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/shell/cli.py
--rw-r--r--   0        0        0      219 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/shell/cmd_generators/__init__.py
--rw-r--r--   0        0        0      335 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/shell/cmd_generators/common.py
--rw-r--r--   0        0        0     2583 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/shell/cmd_generators/reg.py
--rw-r--r--   0        0        0    18855 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/shell/parsers.py
--rw-r--r--   0        0        0    40348 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/shell/prompt.py
--rw-r--r--   0        0        0     1880 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/shell/refresh.py
--rw-r--r--   0        0        0      681 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/falcon_toolkit/shell/utils.py
--rw-r--r--   0        0        0     2150 2023-09-15 13:26:45.646352 falcon_toolkit-3.3.1/pyproject.toml
--rw-r--r--   0        0        0    22108 1970-01-01 00:00:00.000000 falcon_toolkit-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/LICENSE.md
+-rw-r--r--   0        0        0    22980 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/README.md
+-rw-r--r--   0        0        0      188 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/__init__.py
+-rw-r--r--   0        0        0      174 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/__init__.py
+-rw-r--r--   0        0        0     1847 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/auth.py
+-rw-r--r--   0        0        0      191 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/auth_backends/__init__.py
+-rw-r--r--   0        0        0      449 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/auth_backends/default.py
+-rw-r--r--   0        0        0     5898 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/auth_backends/public_mssp.py
+-rw-r--r--   0        0        0     4087 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/auth_backends/public_single_cid.py
+-rw-r--r--   0        0        0     2855 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/auth_backends/utils.py
+-rw-r--r--   0        0        0     1846 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/cli.py
+-rw-r--r--   0        0        0     7974 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/config.py
+-rw-r--r--   0        0        0      962 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/console_utils.py
+-rw-r--r--   0        0        0      550 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/constants.py
+-rw-r--r--   0        0        0     2767 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/logging_config.py
+-rw-r--r--   0        0        0      340 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/meta.py
+-rw-r--r--   0        0        0     1599 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/namespace.py
+-rw-r--r--   0        0        0     3683 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/common/utils.py
+-rw-r--r--   0        0        0      122 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/containment/__init__.py
+-rw-r--r--   0        0        0     6114 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/containment/cli.py
+-rw-r--r--   0        0        0     3329 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/containment/perform_containment.py
+-rwxr-xr-x   0        0        0    10190 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/falcon.py
+-rw-r--r--   0        0        0      116 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/hosts/__init__.py
+-rw-r--r--   0        0        0     2390 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/hosts/cli.py
+-rw-r--r--   0        0        0     5651 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/hosts/host_search.py
+-rw-r--r--   0        0        0      133 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/maintenance_token/__init__.py
+-rw-r--r--   0        0        0     5400 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/maintenance_token/cli.py
+-rw-r--r--   0        0        0     1375 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/maintenance_token/device_tokens.py
+-rw-r--r--   0        0        0      120 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/policies/__init__.py
+-rw-r--r--   0        0        0     5196 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/policies/cli.py
+-rw-r--r--   0        0        0     1049 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/policies/constants.py
+-rw-r--r--   0        0        0     3354 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/policies/container.py
+-rw-r--r--   0        0        0     3659 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/policies/describe.py
+-rw-r--r--   0        0        0      160 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/shell/__init__.py
+-rw-r--r--   0        0        0     6989 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/shell/cli.py
+-rw-r--r--   0        0        0      219 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/shell/cmd_generators/__init__.py
+-rw-r--r--   0        0        0      335 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/shell/cmd_generators/common.py
+-rw-r--r--   0        0        0     2583 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/shell/cmd_generators/reg.py
+-rw-r--r--   0        0        0    18855 2024-04-16 13:22:23.622979 falcon_toolkit-3.4.0/falcon_toolkit/shell/parsers.py
+-rw-r--r--   0        0        0    40524 2024-04-16 13:22:23.626979 falcon_toolkit-3.4.0/falcon_toolkit/shell/prompt.py
+-rw-r--r--   0        0        0     1880 2024-04-16 13:22:23.626979 falcon_toolkit-3.4.0/falcon_toolkit/shell/refresh.py
+-rw-r--r--   0        0        0      681 2024-04-16 13:22:23.626979 falcon_toolkit-3.4.0/falcon_toolkit/shell/utils.py
+-rw-r--r--   0        0        0     2204 2024-04-16 13:22:23.626979 falcon_toolkit-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0    24555 1970-01-01 00:00:00.000000 falcon_toolkit-3.4.0/PKG-INFO
```

### Comparing `falcon_toolkit-3.3.1/LICENSE.md` & `falcon_toolkit-3.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/README.md` & `falcon_toolkit-3.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 
 The toolkit provides:
 
 - Host searching, with filter support.
 - Multiple profile support, including support for MSSP / Falcon Flight Control configurations.
 - A shell allowing you to interface with many hosts via RTR at once, and get the output via CSV.
 - Scriptability! You can program the shell by providing pre-written routines via a file on disk, and a full Python extensibility API is provided.
-- Prevention policy import and export
-- Response policy import and export
+- Prevention policy import and export.
+- Response policy import and export.
+- Contain and uncontain systems in bulk, according to filters or a list of device IDs.
 - More functionality is coming soon! Want more functionality? Open an [Issue](https://github.com/CrowdStrike/Falcon-Toolkit/issues/new)!
 
 Since this is built on top of Caracara, you get a bunch of great functionality and flexibility free, including the ability to filter hosts using dynamically generated FQL queries, full debug logging where desired, Falcon Flight Control integration, and more! Plus, the tool is lightning quick as it leverages Caracara's parallelisation tricks to pull more information quickly.
 
 ## Getting Started
 
 There are two supported methods to install Falcon Toolkit.
@@ -178,25 +179,27 @@
 - The name you specify will be the one you use to start a shell, so if you put a space in it remember that you'll need to wrap it in quotes later. Therefore, we do not recommend using a space here.
 - The client ID and secret you specify must have full RTR admin and host querying permissions enabled; otherwise, this tool will not be able to execute any commands.
 
 Two types of configuration backends are provided out of the box: the default, which is for an API keypair associated with a standard Falcon tenant, and a Falcon Flight Control backend. Use the Flight Control backend when authenticating to a Parent CID, as you will be able to specify the desired child CID on execution.
 
 Your API keys should have the following scopes enabled in the Falcon dashboard:
 
-| &darr; API Scopes // Commands &rarr; | `host_search` | `shell` | `policies`<br>(Prevention) | `policies`<br>(Response)  |
-|--------------------------------------|:-------------:|:-------:|:--------------------------:|:-------------------------:|
-| **Falcon Flight Control: Read**      | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* |
-| **Hosts: Read**                      |       X       |    X    |                            |                           |
-| **Prevention Policies: Read**        |               |         | X<br>`describe` / `export` sub-commands |              |
-| **Prevention Policies: Write**       |               |         | X<br>`import` sub-command  |                           |
-| **Real Time Response: Read**         |               |    X    |                            |                           |
-| **Real Time Response: Write**        |               |    X    |                            |                           |
-| **Real Time Response: Admin**        |               |    X<br>*for admin commands*    |    |                           |
-| **Response Policies: Read**          |               |         |                            | X<br>`describe` / `export` sub-commands |
-| **Response Policies: Write**         |               |         |                            | X<br>`import` sub-command |
+| &darr; API Scopes // Commands &rarr; | `host_search` | `shell` | `policies`<br>(Prevention) | `policies`<br>(Response)  | `containment`<br>Host Containment | `maintenance_token`<br>Maintenance Tokens |
+|--------------------------------------|:-------------:|:-------:|:--------------------------:|:-------------------------:|:---------------------------------:|:-----------------------------------------:|
+| **Falcon Flight Control: Read**      | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | | |
+| **Hosts: Read**                      |       X       |    X    |                            |                           | X | X |
+| **Hosts: Write**                     |               |         |                            |                           | X | |
+| **Prevention Policies: Read**        |               |         | X<br>`describe` / `export` sub-commands |              |   | |
+| **Prevention Policies: Write**       |               |         | X<br>`import` sub-command  |                           |   | |
+| **Real Time Response: Read**         |               |    X    |                            |                           |   | |
+| **Real Time Response: Write**        |               |    X    |                            |                           |   | |
+| **Real Time Response: Admin**        |               |    X<br>*for admin commands*    |    |                           |   | |
+| **Response Policies: Read**          |               |         |                            | X<br>`describe` / `export` sub-commands |   | |
+| **Response Policies: Write**         |               |         |                            | X<br>`import` sub-command |   | |
+| **Sensor Update Policies: Write**    |               |         |                            |                           |   | X |
 
 ### Showing Your Profiles
 
 The command `falcon profiles list` will show you all configurations (if any) you have created using the `new` command above, listed by the name you specified.
 
 Example output:
 
@@ -351,14 +354,81 @@
 
 - Execute a batch `get` command and then cache the contents of `self.last_batch_get_successful_requests` to find out how many systems had the file on disk. Then, the script could wait `x` seconds in a loop up to a maximum amount of time, running `get_status` each time. On each iteration, the script may query `self.last_batch_get_completed_uploads` to determine whether a minimum threshold of systems have uploaded the requested file, and then once complete execute `download -e /some/output/folder` to pull those completed uploads down to a folder of choice (then extract them automatically).
 - Execute a series of commands that differ by target OS, using the contents of `self.connected_devices` to make decisions dynamically.
 - Execute `self.send_generic_command` directly, then use the returned `(stdout, stderr)` tuple to make decisions about which command to execute next (best suited to single system connections).
 
 </details>
 
+## Maintenance Tokens
+
+You can fetch maintenance tokens for systems within your Falcon tenant, or retrieve the bulk maintenance token.
+
+### Examples
+
+Show the bulk maintenance token:
+
+```shell
+$ falcon -p MyCompany maintenance_token -b
+Getting the bulk maintenance token
+Bulk maintenance token: redactedexample12345
+WARNING: this token must be kept safe, as it can uninstall all Falcon sensors!
+```
+
+Show a token for a specific system located by hostname:
+
+```shell
+$ falcon -p MyCompany maintenance_token -f Hostname=MY-TEST-BOX-1
+```
+
+Show maintenance tokens for a list of device IDs provided on the command line:
+
+```shell
+$ falcon -p MyCompany maintenance_token -d aid1,aid2,...
+```
+
+## Network Containment
+
+You can `contain` and `uncontain` systems through Falcon Toolkit. Network containment restricts the network connectivity of matching systems to just the Falcon Platform.
+
+The containment functionality accepts the same command line parameters as `host_search` and `shell` (`-d`, `-df`, or multiple instances of `-f` to apply Falcon filters).
+
+### Examples
+
+Network contain all systems that match the FQL hostname pattern `DEVTEST*`:
+
+```shell
+$ falcon -p MyCompany containment -f Hostname=DEVTEST\* contain
+...
+```
+
+Lift the containment status on the same machines:
+
+```shell
+$ falcon -p MyCompany containment -f Hostname=DEVTEST\* uncontain
+...
+```
+
+Network contain specific systems by AID:
+
+```shell
+$ falcon -p MyCompany containment -d aid1,aid2,aid3 contain
+...
+```
+
+Network contain all systems in a CID:
+
+```shell
+$ falcon -p MyCompany containment contain
+You did not specify any parameters. This command will manage the containment status of ALL devices in the Falcon tenant!
+You must enter the string "I AM SURE!" to proceed.
+Are you sure? I AM SURE!
+...
+```
+
+
 ## Policy Manipulation
 
 You can `describe`, `import` and `export` two types of policies: Prevention and Response. The three verbs are applied to the `falcon policies` command to specify what you would like to do with policies, and a command line switch is used to specify the policy type to work with. Exported policies are written to disk as JSON with some Falcon Toolkit-specific data needed to import a policy back again.
 
 ### Examples
 
 Show all Prevention policies within the `MyCompany` Falcon profile:
```

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/common/auth.py` & `falcon_toolkit-3.4.0/falcon_toolkit/common/auth.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/common/auth_backends/public_mssp.py` & `falcon_toolkit-3.4.0/falcon_toolkit/common/auth_backends/public_mssp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Falcon Toolkit: Public Cloud Flight Control (Multi-CID) Parent CID.
 
 This authentication backend can take public cloud API keys (US-1, US-2, EU-1), and will ask the
 user which child CID to authenticate against.
 """
 import os
 
-from typing import Dict, List, Optional
+from typing import Dict, Optional
 
 import keyring
-import pick
 
 from caracara import Client
 
 from falcon_toolkit.common.auth import AuthBackend
 from falcon_toolkit.common.auth_backends.utils import advanced_options_wizard
 from falcon_toolkit.common.constants import KEYRING_SERVICE_NAME
-from falcon_toolkit.common.utils import fancy_input
+from falcon_toolkit.common.utils import fancy_input, choose_cid
 
 
 class PublicCloudFlightControlParentCIDBackend(AuthBackend):
     """Falcon Flight Control (Public Cloud) Authentication Backend.
 
     Authentication backend that uses a Client ID / Client Secret pair to access a Flight Control
     Parent CID. Once connected, a user can select a child CID to interface with.
@@ -114,24 +113,18 @@
         chosen_cid_str = os.environ.get("FALCON_MSSP_CHILD_CID")
         if chosen_cid_str and chosen_cid_str.lower() in child_cids:
             chosen_cid = parent_client.flight_control.get_child_cid_data(
                 cids=[chosen_cid_str]
             )[chosen_cid_str]
         else:
             child_cids_data = parent_client.flight_control.get_child_cid_data(cids=child_cids)
-
-            options: List[pick.Option] = []
-            for child_cid_str, child_cid_data in child_cids_data.items():
-                child_cid_name = child_cid_data['name']
-                option_text = f"{child_cid_str}: {child_cid_name}"
-                option = pick.Option(label=option_text, value=child_cid_str)
-                options.append(option)
-
-            chosen_option, _ = pick.pick(options, "Please select a CID to connect to")
-            chosen_cid_str = chosen_option.value
+            chosen_cid_str = choose_cid(
+                cids=child_cids_data,
+                prompt_text="MSSP Child CID Search"
+            )
             chosen_cid = child_cids_data[chosen_cid_str]
 
         chosen_cid_name = chosen_cid['name']
         print(f"Connecting to {chosen_cid_name}")
 
         client = Client(
             client_id=self.client_id,
```

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/common/auth_backends/public_single_cid.py` & `falcon_toolkit-3.4.0/falcon_toolkit/common/auth_backends/public_single_cid.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/common/auth_backends/utils.py` & `falcon_toolkit-3.4.0/falcon_toolkit/common/auth_backends/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 """Falcon Toolkit: Authentication Backends.
 
 This file contains functions to be shared between all the authentication backends we
 provide out of the box, as well as any that developers may write in the future. It is
 designed to avoid excessive code-reuse between similar implementations of auth backend.
 This file provides:
 - A list of all public CrowdStrike clouds
-- A cloud selection function to allow a user to choose a cloud via pick
+- A cloud selection function to allow a user to choose a cloud via Prompt Toolkit
 - Advanced options configuration for overriding cloud, TLS validation, etc.
 """
 from typing import (
     Dict,
     List,
     NamedTuple,
+    Tuple,
 )
 
-import pick
+from caracara.common.csdialog import csradiolist_dialog
 
 from falcon_toolkit.common.utils import fancy_input
 
 
 CLOUDS = {
     "auto": "Automatic cloud selection (supports US-1, US-2 and EU-1)",
     "us-1": "US-1: Falcon US-1 Falcon cloud (api.crowdstrike.com)",
     "us-2": "US-2: Falcon US-2 Falcon cloud (api.us-2.crowdstrike.com)",
     "eu-1": "EU-1: Falcon EU (Germany) cloud (api.eu-1.crowdstrike.com)",
     "us-gov-1": "US-GOV-1: Falcon in GovCloud (api.laggar.gcw.crowdstrike.com)",
 }
 
 
 def cloud_choice() -> str:
-    """Configure a selection of clouds and allow the user to choose one via pick."""
-    cloud_choices: List[pick.Option] = []
+    """Configure a selection of clouds and allow the user to choose one via Prompt Toolkit."""
+    cloud_choices: List[Tuple] = []
     for cloud_id, cloud_description in CLOUDS.items():
-        cloud_choices.append(pick.Option(cloud_description, cloud_id))
+        cloud_choices.append((cloud_id, cloud_description))
 
-    chosen_option, _ = pick.pick(cloud_choices, title="Please choose a Falcon cloud")
-    chosen_falcon_cloud: str = chosen_option.value
+    chosen_falcon_cloud: str = csradiolist_dialog(
+        title="Falcon Cloud Selection",
+        text="Please choose a Falcon cloud",
+        cancel_text=None,
+        values=cloud_choices,
+    ).run()
 
     return chosen_falcon_cloud
 
 
 class AdvancedOptionsType(NamedTuple):
     """Named Tuple that contains the results of the Advanced Options Wizard."""
 
@@ -52,20 +57,24 @@
     """Define advanced connection options and return an AdvancedOptionsType."""
     advanced_options_input = fancy_input("Do you want to configure more options? [y/n]: ")
     if advanced_options_input not in ('y', 'Y'):
         return AdvancedOptionsType('auto', True, None)
 
     cloud_name = cloud_choice()
 
-    tls_verify_options: List[pick.Option] = [
-        pick.Option("Verify SSL/TLS certificates (recommended!)", value=True),
-        pick.Option("Do not verify SSL/TLS certificates (not recommended)", False),
+    tls_verify_options = [
+        (True, "Verify SSL/TLS certificates (recommended!)"),
+        (False, "Do not verify SSL/TLS certificates (not recommended)"),
     ]
-    chosen_ssl_verify, _ = pick.pick(tls_verify_options, title="Verify SSL/TLS certificates?")
-    ssl_verify: bool = chosen_ssl_verify.value
+    ssl_verify: bool = csradiolist_dialog(
+        title="Connection Security",
+        text="Enable SSL/TLS certificate verification?",
+        cancel_text=None,
+        values=tls_verify_options,
+    ).run()
 
     proxy_dict = None
     proxy_url_input = fancy_input("HTTPS proxy URL (leave blank if not needed): ", loop=False)
 
     if proxy_url_input:
         proxy_dict = {'https', proxy_url_input}
```

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/common/cli.py` & `falcon_toolkit-3.4.0/falcon_toolkit/common/cli.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/common/config.py` & `falcon_toolkit-3.4.0/falcon_toolkit/common/config.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/common/console_utils.py` & `falcon_toolkit-3.4.0/falcon_toolkit/common/console_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/common/constants.py` & `falcon_toolkit-3.4.0/falcon_toolkit/common/constants.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/common/logging_config.py` & `falcon_toolkit-3.4.0/falcon_toolkit/common/logging_config.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/common/namespace.py` & `falcon_toolkit-3.4.0/falcon_toolkit/common/namespace.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/falcon.py` & `falcon_toolkit-3.4.0/falcon_toolkit/falcon.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 """
 import logging
 import os
 import shutil
 import sys
 
 import click
-import pick
 
+from caracara.common.csdialog import csradiolist_dialog
 from caracara_filters.dialects import DIALECTS
 from colorama import (
     deinit as colorama_deinit,
     init as colorama_init,
 )
 
 from falcon_toolkit.common.config import FalconToolkitConfig
@@ -45,15 +45,17 @@
     CONFIG_FILENAME,
     DEFAULT_CONFIG_DIR,
     LOG_SUB_DIR,
     OLD_DEFAULT_CONFIG_DIR,
 )
 from falcon_toolkit.common.logging_config import configure_logger
 from falcon_toolkit.common.utils import configure_data_dir
+from falcon_toolkit.containment.cli import cli_containment
 from falcon_toolkit.hosts.cli import cli_host_search
+from falcon_toolkit.maintenance_token.cli import cli_maintenance_token
 from falcon_toolkit.policies.cli import cli_policies
 from falcon_toolkit.shell.cli import cli_shell
 
 
 @click.group()
 @click.pass_context
 @click.option(
@@ -132,55 +134,53 @@
     if (
         config_path == DEFAULT_CONFIG_DIR and
         os.path.exists(OLD_DEFAULT_CONFIG_DIR) and
         not os.path.exists(config_path)
     ):
         # The user has used Falcon Toolkit before, and uses the default directory, so we
         # offer to move the configuration folder for them.
-        choice, _ = pick.pick(
-            options=[
-                pick.Option(
-                    f"Please move my current folder contents to {config_path}",
-                    "MOVE_FOLDER",
-                ),
-                pick.Option(
-                    (
-                        f"Leave my old folder ({OLD_DEFAULT_CONFIG_DIR}) alone "
-                        f"and create a new one at {config_path}"
-                    ),
-                    "LEAVE_ALONE",
-                ),
-                pick.Option(
-                    (
-                        f"Leave my old folder ({OLD_DEFAULT_CONFIG_DIR}) alone, "
-                        f"create a new one at {config_path}, and copy my configuration "
-                        "file there."
-                    ),
-                    "COPY_CONFIG_ONLY",
-                ),
-                pick.Option(
-                    "Exit Falcon Toolkit and do nothing",
-                    "ABORT",
-                ),
-            ],
-            title=(
-                "As of Falcon Toolkit 3.3.0, the configuration directory has moved to a "
-                "platform-specific data configuration directory."
+        option_pairs = [
+            (
+                "MOVE_FOLDER",
+                f"Please move my current folder contents to {config_path}",
+            ),
+            (
+                "LEAVE_ALONE",
+                f"Leave my old folder ({OLD_DEFAULT_CONFIG_DIR}) alone "
+                f"and create a new one at {config_path}",
+            ),
+            (
+                "COPY_CONFIG_ONLY",
+                f"create a new one at {config_path}, and copy my configuration file there",
             )
-        )
+        ]
+        choice = csradiolist_dialog(
+            title="Falcon Toolkit Configuration Directory",
+            text=(
+                "As of Falcon Toolkit 3.3.0, the configuration directory has moved to a "
+                "platform-specific data configuration directory. Please choose how you "
+                "would like the Toolkit to proceed, or press Abort to exit the program "
+                "without making any changes."
+            ),
+            cancel_text="Cancel",
+            values=option_pairs,
+        ).run()
+        if choice is None:
+            click.echo(click.style("Exiting the Toolkit without making changes.", bold=True))
+            sys.exit(1)
 
-        if choice.value == "MOVE_FOLDER":
+        if choice == "MOVE_FOLDER":
             click.echo(f"Moving {OLD_DEFAULT_CONFIG_DIR} to {config_path}")
             os.rename(OLD_DEFAULT_CONFIG_DIR, config_path)
-        elif choice.value == "LEAVE_ALONE":
+        elif choice == "LEAVE_ALONE":
             click.echo(
                 f"Creating a new, empty data directory at {config_path} "
                 "and leaving the original folder alone"
             )
-        elif choice.value == "COPY_CONFIG_ONLY":
+        elif choice == "COPY_CONFIG_ONLY":
             click.echo(
                 f"Creating a new, empty data directory at {config_path} "
                 "and copying the current configuration there"
             )
             os.makedirs(config_path)
             shutil.copyfile(
                 os.path.join(OLD_DEFAULT_CONFIG_DIR, CONFIG_FILENAME),
@@ -288,11 +288,13 @@
     for unique_filter_name in unique_filters:
         click.echo(click.style(unique_filter_name, fg='blue', bold=True))
         click.echo(host_filters[unique_filter_name]['help'])
         click.echo()
 
 
 # Load all commands into the main cli object, ready for use as root falcon commands
+cli.add_command(cli_containment)
 cli.add_command(cli_host_search)
 cli.add_command(cli_list_filters)
+cli.add_command(cli_maintenance_token)
 cli.add_command(cli_policies)
 cli.add_command(cli_shell)
```

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/hosts/cli.py` & `falcon_toolkit-3.4.0/falcon_toolkit/hosts/cli.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/hosts/host_search.py` & `falcon_toolkit-3.4.0/falcon_toolkit/hosts/host_search.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/policies/cli.py` & `falcon_toolkit-3.4.0/falcon_toolkit/policies/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Falcon Toolkit: Policy Management.
 
 This file contains the command line interface for the policies commands. The implementation
 of the logic itself is contained in other files, including policies.py
 """
 import os
+import sys
 
 from typing import List
 
 import click
-import pick
 
 from caracara import Client
+from caracara.common.csdialog import csradiolist_dialog
 from caracara.common.policy_wrapper import Policy
 
 from click_option_group import (
     optgroup,
     RequiredMutuallyExclusiveOptionGroup,
 )
 
@@ -89,24 +90,31 @@
 @click.pass_context
 def policies_export(ctx: click.Context):
     """Allow a user to choose a Prevention or Response policy to export to disk."""
     # pylint: disable=too-many-locals
     policies_api: PoliciesApiModule = ctx.obj['policies_api']
     policies_type: str = ctx.obj['policies_type']
     click.echo("Loading policies...")
-    policies = policies_api.describe_policies()
+    policies: List[Policy] = policies_api.describe_policies()
 
-    options: List[pick.Option] = []
+    options = []
     for policy in policies:
         option_text = f"{policy.name} [{policy.platform_name}]"
-        option = pick.Option(label=option_text, value=policy)
-        options.append(option)
+        options.append((policy, option_text))
+
+    chosen_policy = csradiolist_dialog(
+        title="Policy Selection",
+        text="Please choose a policy to export",
+        values=options,
+    ).run()
+
+    if chosen_policy is None:
+        click.echo("No option chosen; aborting.")
+        sys.exit(1)
 
-    chosen_option, _ = pick.pick(options, "Please choose a policy to export")
-    chosen_policy: Policy = chosen_option.value
     default_filename = f"{chosen_policy.name}.json"
     reasonable_filename = False
     while not reasonable_filename:
         filename: str = click.prompt("Policy filename", type=str, default=default_filename)
         if not filename.endswith(".json"):
             click.echo(click.style("Filename must end in .json", fg='yellow'))
             continue
```

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/policies/constants.py` & `falcon_toolkit-3.4.0/falcon_toolkit/policies/constants.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/policies/container.py` & `falcon_toolkit-3.4.0/falcon_toolkit/policies/container.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/policies/describe.py` & `falcon_toolkit-3.4.0/falcon_toolkit/policies/describe.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/shell/cli.py` & `falcon_toolkit-3.4.0/falcon_toolkit/shell/cli.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/shell/cmd_generators/reg.py` & `falcon_toolkit-3.4.0/falcon_toolkit/shell/cmd_generators/reg.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/shell/parsers.py` & `falcon_toolkit-3.4.0/falcon_toolkit/shell/parsers.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/shell/prompt.py` & `falcon_toolkit-3.4.0/falcon_toolkit/shell/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -816,14 +816,19 @@
 
     @with_argparser(PARSERS.mkdir, preserve_quotes=True)
     def do_mkdir(self, args):
         """Create a new directory."""
         command = f'mkdir {args.directory}'
         self.send_generic_command(command)
 
+    @with_argparser(PARSERS.mount, preserve_quotes=True)
+    def do_mount(self, args):
+        """List mount points on a system."""
+        self.send_generic_command("mount")
+
     @with_argparser(PARSERS.mv, preserve_quotes=True)
     def do_mv(self, args):
         """Move a file or directory."""
         command = f'mv {args.source} {args.destination}'
         self.send_generic_command(command)
 
     @with_argparser(PARSERS.netstat, preserve_quotes=True)
```

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/shell/refresh.py` & `falcon_toolkit-3.4.0/falcon_toolkit/shell/refresh.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/falcon_toolkit/shell/utils.py` & `falcon_toolkit-3.4.0/falcon_toolkit/shell/utils.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.3.1/pyproject.toml` & `falcon_toolkit-3.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "falcon-toolkit"
-version = "3.3.1"
+version = "3.4.0"
 description = "Toolkit to interface with CrowdStrike Falcon via the API"
 license = "MIT"
 authors = [
     "Chris Hammond <chris.hammond@crowdstrike.com>",
     "Kira Noël <kira.noel@crowdstrike.com>",
 ]
 repository = "http://github.com/CrowdStrike/Falcon-Toolkit"
@@ -26,32 +26,33 @@
     "Topic :: Security",
     "Topic :: System :: Shells",
     "Topic :: Terminals",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-caracara = "^0.5.1"
+caracara = "^0.7.0"
 click = "^8.1.3"
-click-option-group = "^0.5.3"
+click-option-group = "^0.5.6"
 click-spinner = "^0.1.10"
 cmd2 = "^2.4"
 colorama = "^0.4.5"
-keyring = ">=23,<25"
-pick = "^2.0.2"
-platformdirs = "^3.5.1"
+keyring = ">=24,<26"
+platformdirs = "^4.2.0"
 tabulate = "^0.9.0"
+prompt-toolkit = "^3.0.43"
+setuptools = "^69.0"
 
 [tool.poetry.scripts]
 falcon = "falcon_toolkit.falcon:cli"
 
 [tool.poetry.group.dev.dependencies]
-flake8 = "^6.0.0"
-pylint = "^2.15.4"
-pytest = "^7.0.1"
+flake8 = ">=6,<8"
+pylint = "^3.0.0"
+pytest = "^8.0.1"
 pydocstyle = "^6.1.1"
 toml = "^0.10.2"
 
 [tool.pylint.messages_control]
 disable = [
     # This is required beacuse of the (delibrate) copy/paste code between the various authentication
     # backends.
@@ -68,9 +69,9 @@
 
     # This tool makes extensive use of other libraries, such as Cmd2, which may provide variables to
     # functions that we do not need to use. Alternatives are harder to maintain for little gain.
     "unused-argument",
 ]
 
 [build-system]
-requires = ["poetry-core>=1.2.0"]
+requires = ["poetry-core>=1.2.0", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `falcon_toolkit-3.3.1/PKG-INFO` & `falcon_toolkit-3.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon-toolkit
-Version: 3.3.1
+Version: 3.4.0
 Summary: Toolkit to interface with CrowdStrike Falcon via the API
 Home-page: http://github.com/CrowdStrike/Falcon-Toolkit
 License: MIT
 Keywords: automation,cli,crowdstrike,endpoint-protection,falcon,falcon-platform
 Author: Chris Hammond
 Author-email: chris.hammond@crowdstrike.com
 Requires-Python: >=3.9,<4.0
@@ -13,27 +13,29 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Terminals
-Requires-Dist: caracara (>=0.5.1,<0.6.0)
+Requires-Dist: caracara (>=0.7.0,<0.8.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: click-option-group (>=0.5.3,<0.6.0)
+Requires-Dist: click-option-group (>=0.5.6,<0.6.0)
 Requires-Dist: click-spinner (>=0.1.10,<0.2.0)
 Requires-Dist: cmd2 (>=2.4,<3.0)
 Requires-Dist: colorama (>=0.4.5,<0.5.0)
-Requires-Dist: keyring (>=23,<25)
-Requires-Dist: pick (>=2.0.2,<3.0.0)
-Requires-Dist: platformdirs (>=3.5.1,<4.0.0)
+Requires-Dist: keyring (>=24,<26)
+Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
+Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
+Requires-Dist: setuptools (>=69.0,<70.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, http://github.com/CrowdStrike/Falcon-Toolkit
 Description-Content-Type: text/markdown
 
 <!--markdownlint-disable MD033-->
 # Falcon Toolkit
 
@@ -53,16 +55,17 @@
 
 The toolkit provides:
 
 - Host searching, with filter support.
 - Multiple profile support, including support for MSSP / Falcon Flight Control configurations.
 - A shell allowing you to interface with many hosts via RTR at once, and get the output via CSV.
 - Scriptability! You can program the shell by providing pre-written routines via a file on disk, and a full Python extensibility API is provided.
-- Prevention policy import and export
-- Response policy import and export
+- Prevention policy import and export.
+- Response policy import and export.
+- Contain and uncontain systems in bulk, according to filters or a list of device IDs.
 - More functionality is coming soon! Want more functionality? Open an [Issue](https://github.com/CrowdStrike/Falcon-Toolkit/issues/new)!
 
 Since this is built on top of Caracara, you get a bunch of great functionality and flexibility free, including the ability to filter hosts using dynamically generated FQL queries, full debug logging where desired, Falcon Flight Control integration, and more! Plus, the tool is lightning quick as it leverages Caracara's parallelisation tricks to pull more information quickly.
 
 ## Getting Started
 
 There are two supported methods to install Falcon Toolkit.
@@ -214,25 +217,27 @@
 - The name you specify will be the one you use to start a shell, so if you put a space in it remember that you'll need to wrap it in quotes later. Therefore, we do not recommend using a space here.
 - The client ID and secret you specify must have full RTR admin and host querying permissions enabled; otherwise, this tool will not be able to execute any commands.
 
 Two types of configuration backends are provided out of the box: the default, which is for an API keypair associated with a standard Falcon tenant, and a Falcon Flight Control backend. Use the Flight Control backend when authenticating to a Parent CID, as you will be able to specify the desired child CID on execution.
 
 Your API keys should have the following scopes enabled in the Falcon dashboard:
 
-| &darr; API Scopes // Commands &rarr; | `host_search` | `shell` | `policies`<br>(Prevention) | `policies`<br>(Response)  |
-|--------------------------------------|:-------------:|:-------:|:--------------------------:|:-------------------------:|
-| **Falcon Flight Control: Read**      | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* |
-| **Hosts: Read**                      |       X       |    X    |                            |                           |
-| **Prevention Policies: Read**        |               |         | X<br>`describe` / `export` sub-commands |              |
-| **Prevention Policies: Write**       |               |         | X<br>`import` sub-command  |                           |
-| **Real Time Response: Read**         |               |    X    |                            |                           |
-| **Real Time Response: Write**        |               |    X    |                            |                           |
-| **Real Time Response: Admin**        |               |    X<br>*for admin commands*    |    |                           |
-| **Response Policies: Read**          |               |         |                            | X<br>`describe` / `export` sub-commands |
-| **Response Policies: Write**         |               |         |                            | X<br>`import` sub-command |
+| &darr; API Scopes // Commands &rarr; | `host_search` | `shell` | `policies`<br>(Prevention) | `policies`<br>(Response)  | `containment`<br>Host Containment | `maintenance_token`<br>Maintenance Tokens |
+|--------------------------------------|:-------------:|:-------:|:--------------------------:|:-------------------------:|:---------------------------------:|:-----------------------------------------:|
+| **Falcon Flight Control: Read**      | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | X<br>*When using parent<br>CID API Keys* | | |
+| **Hosts: Read**                      |       X       |    X    |                            |                           | X | X |
+| **Hosts: Write**                     |               |         |                            |                           | X | |
+| **Prevention Policies: Read**        |               |         | X<br>`describe` / `export` sub-commands |              |   | |
+| **Prevention Policies: Write**       |               |         | X<br>`import` sub-command  |                           |   | |
+| **Real Time Response: Read**         |               |    X    |                            |                           |   | |
+| **Real Time Response: Write**        |               |    X    |                            |                           |   | |
+| **Real Time Response: Admin**        |               |    X<br>*for admin commands*    |    |                           |   | |
+| **Response Policies: Read**          |               |         |                            | X<br>`describe` / `export` sub-commands |   | |
+| **Response Policies: Write**         |               |         |                            | X<br>`import` sub-command |   | |
+| **Sensor Update Policies: Write**    |               |         |                            |                           |   | X |
 
 ### Showing Your Profiles
 
 The command `falcon profiles list` will show you all configurations (if any) you have created using the `new` command above, listed by the name you specified.
 
 Example output:
 
@@ -387,14 +392,81 @@
 
 - Execute a batch `get` command and then cache the contents of `self.last_batch_get_successful_requests` to find out how many systems had the file on disk. Then, the script could wait `x` seconds in a loop up to a maximum amount of time, running `get_status` each time. On each iteration, the script may query `self.last_batch_get_completed_uploads` to determine whether a minimum threshold of systems have uploaded the requested file, and then once complete execute `download -e /some/output/folder` to pull those completed uploads down to a folder of choice (then extract them automatically).
 - Execute a series of commands that differ by target OS, using the contents of `self.connected_devices` to make decisions dynamically.
 - Execute `self.send_generic_command` directly, then use the returned `(stdout, stderr)` tuple to make decisions about which command to execute next (best suited to single system connections).
 
 </details>
 
+## Maintenance Tokens
+
+You can fetch maintenance tokens for systems within your Falcon tenant, or retrieve the bulk maintenance token.
+
+### Examples
+
+Show the bulk maintenance token:
+
+```shell
+$ falcon -p MyCompany maintenance_token -b
+Getting the bulk maintenance token
+Bulk maintenance token: redactedexample12345
+WARNING: this token must be kept safe, as it can uninstall all Falcon sensors!
+```
+
+Show a token for a specific system located by hostname:
+
+```shell
+$ falcon -p MyCompany maintenance_token -f Hostname=MY-TEST-BOX-1
+```
+
+Show maintenance tokens for a list of device IDs provided on the command line:
+
+```shell
+$ falcon -p MyCompany maintenance_token -d aid1,aid2,...
+```
+
+## Network Containment
+
+You can `contain` and `uncontain` systems through Falcon Toolkit. Network containment restricts the network connectivity of matching systems to just the Falcon Platform.
+
+The containment functionality accepts the same command line parameters as `host_search` and `shell` (`-d`, `-df`, or multiple instances of `-f` to apply Falcon filters).
+
+### Examples
+
+Network contain all systems that match the FQL hostname pattern `DEVTEST*`:
+
+```shell
+$ falcon -p MyCompany containment -f Hostname=DEVTEST\* contain
+...
+```
+
+Lift the containment status on the same machines:
+
+```shell
+$ falcon -p MyCompany containment -f Hostname=DEVTEST\* uncontain
+...
+```
+
+Network contain specific systems by AID:
+
+```shell
+$ falcon -p MyCompany containment -d aid1,aid2,aid3 contain
+...
+```
+
+Network contain all systems in a CID:
+
+```shell
+$ falcon -p MyCompany containment contain
+You did not specify any parameters. This command will manage the containment status of ALL devices in the Falcon tenant!
+You must enter the string "I AM SURE!" to proceed.
+Are you sure? I AM SURE!
+...
+```
+
+
 ## Policy Manipulation
 
 You can `describe`, `import` and `export` two types of policies: Prevention and Response. The three verbs are applied to the `falcon policies` command to specify what you would like to do with policies, and a command line switch is used to specify the policy type to work with. Exported policies are written to disk as JSON with some Falcon Toolkit-specific data needed to import a policy back again.
 
 ### Examples
 
 Show all Prevention policies within the `MyCompany` Falcon profile:
```

