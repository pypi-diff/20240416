# Comparing `tmp/tunnelgraf-0.7.0.tar.gz` & `tmp/tunnelgraf-0.7.1.tar.gz`

## Comparing `tunnelgraf-0.7.0.tar` & `tunnelgraf-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/Makefile
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/README.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/cli.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/tunnelgraf.spec
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tests/test_tunnel_def.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/__init__.py
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/__main__.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/lastpass_secrets.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/nslookup.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/run_remote.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/tunnel_builder.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/tunnel_definition.py
--rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/tunnels.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/LICENSE
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/Makefile
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/README.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/cli.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/tunnelgraf.spec
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/src/tests/test_tunnel_def.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/src/tunnelgraf/__init__.py
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/src/tunnelgraf/__main__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/src/tunnelgraf/lastpass_secrets.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/src/tunnelgraf/nslookup.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/src/tunnelgraf/run_remote.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/src/tunnelgraf/tunnel_builder.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/src/tunnelgraf/tunnel_definition.py
+-rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/src/tunnelgraf/tunnels.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 tunnelgraf-0.7.1/PKG-INFO
```

### Comparing `tunnelgraf-0.7.0/Makefile` & `tunnelgraf-0.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.7.0/README.md` & `tunnelgraf-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.7.0/tunnelgraf.spec` & `tunnelgraf-0.7.1/tunnelgraf.spec`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.7.0/src/tests/test_tunnel_def.py` & `tunnelgraf-0.7.1/src/tests/test_tunnel_def.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.7.0/src/tunnelgraf/__init__.py` & `tunnelgraf-0.7.1/src/tunnelgraf/__init__.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.7.0/src/tunnelgraf/lastpass_secrets.py` & `tunnelgraf-0.7.1/src/tunnelgraf/lastpass_secrets.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.7.0/src/tunnelgraf/nslookup.py` & `tunnelgraf-0.7.1/src/tunnelgraf/nslookup.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.7.0/src/tunnelgraf/run_remote.py` & `tunnelgraf-0.7.1/src/tunnelgraf/run_remote.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.7.0/src/tunnelgraf/tunnel_builder.py` & `tunnelgraf-0.7.1/src/tunnelgraf/tunnel_builder.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.7.0/src/tunnelgraf/tunnel_definition.py` & `tunnelgraf-0.7.1/src/tunnelgraf/tunnel_definition.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.7.0/src/tunnelgraf/tunnels.py` & `tunnelgraf-0.7.1/src/tunnelgraf/tunnels.py`

 * *Files 11% similar despite different names*

```diff
@@ -89,19 +89,25 @@
         except HostsException as e:
             print(
                 f"Error writing hosts file. Are you root or do you own the hosts file? Error: {e}"
             )
             sys.exit(1)
 
     def _add_to_hosts(
-        self, what_for: str, hosts: list, this_host: str | None = None
+        self,
+        what_for: str,
+        hosts: list,
+        this_host: str | None = None,
+        this_host_lookup: str | None = None,
     ) -> None:
         """Adds a host to the hosts list."""
         if this_host is not None:
             hosts.append(this_host)
+        if this_host_lookup is not None:
+            hosts.append(this_host_lookup)
         if len(hosts) > 0:
             for host in hosts:
                 if self._connect_tunnels:
                     print(f"Adding {host} to hosts file.")
                 this_entry = HostsEntry(
                     address="127.0.0.1",
                     names=[host],
@@ -131,14 +137,15 @@
                 print(
                     f"Created tunnel {this_tunnel_def.id}: {tc.local_bind_host}:{tc.local_bind_port} to {tc._remote_binds[0][0]}:{tc._remote_binds[0][1]}"
                 )
             self._add_to_hosts(
                 this_tunnel_def.nexthop.id,
                 this_tunnel_def.nexthop.hosts_file_entries,
                 this_tunnel_def.nexthop.hosts_file_entry,
+                this_tunnel_def.nexthop.hostlookup,
             )
 
             nexthop_config = self._update_bastion_address(this_tunnel_def.nexthop)
             self.make_tunnel(nexthop_config)
 
         if this_tunnel_def.nexthops is not None:
             for tunnel in this_tunnel_def.nexthops:
```

### Comparing `tunnelgraf-0.7.0/LICENSE` & `tunnelgraf-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.7.0/pyproject.toml` & `tunnelgraf-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tunnelgraf"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
   "click~=8.0.0",
   "sshtunnel~=0.4.0",
   "pyyaml~=6.0.0",
   "python-hosts~=1.0.5",
   "pydantic~=2.5.0",
   "paramiko~=3.4.0",
```

### Comparing `tunnelgraf-0.7.0/PKG-INFO` & `tunnelgraf-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tunnelgraf
-Version: 0.7.0
+Version: 0.7.1
 Summary: Hierarchical SSH tunnel management made easy. Securely define and share multihop connection profiles that expose a graph of remote endpoints as localhost.
 Project-URL: Homepage, https://github.com/denniswalker/tunnelgraf
 Project-URL: Documentation, https://github.com/denniswalker/tunnelgraf/blob/main/README.md
 Project-URL: Repository, https://github.com/denniswalker/tunnelgraf
 Project-URL: Issues, https://github.com/denniswalker/tunnelgraf/issues
 Author-email: Dennis Walker <denniswalker@me.com>
 Maintainer-email: Dennis Walker <denniswalker@me.com>
```

