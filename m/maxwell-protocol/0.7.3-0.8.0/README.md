# Comparing `tmp/maxwell_protocol-0.7.3.tar.gz` & `tmp/maxwell_protocol-0.8.0.tar.gz`

## Comparing `maxwell_protocol-0.7.3.tar` & `maxwell_protocol-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/.git
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/Makefile
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/requirements.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/setup.py
--rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/bin/clean_protocol_code.sh
--rwxr-xr-x   0        0        0     3769 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/bin/gen_protocol_api.py
--rwxr-xr-x   0        0        0      734 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/bin/gen_protocol_code.sh
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/maxwell/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/maxwell/protocol/__init__.py
--rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/maxwell/protocol/maxwell_protocol.py
--rw-r--r--   0        0        0    12674 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/maxwell/protocol/maxwell_protocol_pb2.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/LICENSE
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/README.md
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/pyproject.toml
--rw-r--r--   0        0        0    13709 2020-02-02 00:00:00.000000 maxwell_protocol-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/.git
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/Makefile
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/requirements.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/setup.py
+-rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/bin/clean_protocol_code.sh
+-rwxr-xr-x   0        0        0     3769 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/bin/gen_protocol_api.py
+-rwxr-xr-x   0        0        0      734 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/bin/gen_protocol_code.sh
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/maxwell/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/maxwell/protocol/__init__.py
+-rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/maxwell/protocol/maxwell_protocol.py
+-rw-r--r--   0        0        0    12764 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/maxwell/protocol/maxwell_protocol_pb2.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/LICENSE
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/README.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    13709 2020-02-02 00:00:00.000000 maxwell_protocol-0.8.0/PKG-INFO
```

### Comparing `maxwell_protocol-0.7.3/Makefile` & `maxwell_protocol-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `maxwell_protocol-0.7.3/bin/gen_protocol_api.py` & `maxwell_protocol-0.8.0/bin/gen_protocol_api.py`

 * *Files identical despite different names*

### Comparing `maxwell_protocol-0.7.3/bin/gen_protocol_code.sh` & `maxwell_protocol-0.8.0/bin/gen_protocol_code.sh`

 * *Files identical despite different names*

### Comparing `maxwell_protocol-0.7.3/maxwell/protocol/maxwell_protocol.py` & `maxwell_protocol-0.8.0/maxwell/protocol/maxwell_protocol.py`

 * *Files identical despite different names*

### Comparing `maxwell_protocol-0.7.3/maxwell/protocol/maxwell_protocol_pb2.py` & `maxwell_protocol-0.8.0/maxwell/protocol/maxwell_protocol_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16maxwell_protocol.proto\x12\x10maxwell.protocol\"\x19\n\nping_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x19\n\nping_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x17\n\x08ok_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"6\n\x0b\x65rror_rep_t\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\">\n\tok2_rep_t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"]\n\x0c\x65rror2_rep_t\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"7\n\npush_req_t\x12\r\n\x05topic\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x19\n\npush_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"m\n\npull_req_t\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\x02 \x01(\x03\x12\r\n\x05limit\x18\x03 \x01(\r\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"f\n\npull_rep_t\x12%\n\x04msgs\x18\x01 \x03(\x0b\x32\x17.maxwell.protocol.msg_t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x89\x01\n\treq_req_t\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0f\n\x07payload\x18\x02 \x01(\t\x12*\n\x06header\x18\x0c \x01(\x0b\x32\x1a.maxwell.protocol.header_t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"O\n\treq_rep_t\x12\x0f\n\x07payload\x18\x01 \x01(\t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"N\n\nauth_req_t\x12\r\n\x05token\x18\x01 \x01(\t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"?\n\nauth_rep_t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"9\n\x17register_frontend_req_t\x12\x11\n\thttp_port\x18\x01 \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"&\n\x17register_frontend_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"8\n\x16register_backend_req_t\x12\x11\n\thttp_port\x18\x01 \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"%\n\x16register_backend_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"8\n\x16register_service_req_t\x12\x11\n\thttp_port\x18\x01 \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"%\n\x16register_service_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\xd6\x01\n\x10set_routes_req_t\x12\x10\n\x08ws_paths\x18\x01 \x03(\t\x12\x11\n\tget_paths\x18\x02 \x03(\t\x12\x12\n\npost_paths\x18\x03 \x03(\t\x12\x11\n\tput_paths\x18\x04 \x03(\t\x12\x13\n\x0bpatch_paths\x18\x05 \x03(\t\x12\x14\n\x0c\x64\x65lete_paths\x18\x06 \x03(\t\x12\x12\n\nhead_paths\x18\x07 \x03(\t\x12\x15\n\roptions_paths\x18\x08 \x03(\t\x12\x13\n\x0btrace_paths\x18\t \x03(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x1f\n\x10set_routes_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x1f\n\x10get_routes_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\xbe\x04\n\x10get_routes_rep_t\x12\x38\n\x0fws_route_groups\x18\x01 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12\x39\n\x10get_route_groups\x18\x02 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12:\n\x11post_route_groups\x18\x03 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12\x39\n\x10put_route_groups\x18\x04 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12;\n\x12patch_route_groups\x18\x05 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12<\n\x13\x64\x65lete_route_groups\x18\x06 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12:\n\x11head_route_groups\x18\x07 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12=\n\x14options_route_groups\x18\x08 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12;\n\x12trace_route_groups\x18\t \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\",\n\x1dget_topic_dist_checksum_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\">\n\x1dget_topic_dist_checksum_rep_t\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\",\n\x1dget_route_dist_checksum_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\">\n\x1dget_route_dist_checksum_rep_t\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\"\n\x13pick_frontend_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"4\n\x13pick_frontend_rep_t\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"#\n\x14pick_frontends_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"6\n\x14pick_frontends_rep_t\x12\x11\n\tendpoints\x18\x01 \x03(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"0\n\x12locate_topic_req_t\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"3\n\x12locate_topic_rep_t\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x1f\n\x10resolve_ip_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"+\n\x10resolve_ip_rep_t\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"9\n\x05msg_t\x12\x0e\n\x06offset\x18\x01 \x01(\x04\x12\r\n\x05value\x18\x02 \x01(\x0c\x12\x11\n\ttimestamp\x18\x03 \x01(\x04\":\n\x08header_t\x12\r\n\x05\x61gent\x18\x01 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x02 \x01(\t\x12\r\n\x05token\x18\x03 \x01(\t\"U\n\rroute_group_t\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x19\n\x11healthy_endpoints\x18\x02 \x03(\t\x12\x1b\n\x13unhealthy_endpoints\x18\x03 \x03(\t*\xff\x05\n\nmsg_type_t\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08PING_REQ\x10\x01\x12\x0c\n\x08PING_REP\x10\x02\x12\n\n\x06OK_REP\x10\x1d\x12\r\n\tERROR_REP\x10\x1e\x12\x0b\n\x07OK2_REP\x10\x1f\x12\x0e\n\nERROR2_REP\x10 \x12\x0c\n\x08PUSH_REQ\x10!\x12\x0c\n\x08PUSH_REP\x10\"\x12\x0c\n\x08PULL_REQ\x10#\x12\x0c\n\x08PULL_REP\x10$\x12\x0b\n\x07REQ_REQ\x10\'\x12\x0b\n\x07REQ_REP\x10(\x12\x0c\n\x08\x41UTH_REQ\x10)\x12\x0c\n\x08\x41UTH_REP\x10*\x12\x19\n\x15REGISTER_FRONTEND_REQ\x10\x41\x12\x19\n\x15REGISTER_FRONTEND_REP\x10\x42\x12\x18\n\x14REGISTER_BACKEND_REQ\x10\x43\x12\x18\n\x14REGISTER_BACKEND_REP\x10\x44\x12\x18\n\x14REGISTER_SERVICE_REQ\x10\x45\x12\x18\n\x14REGISTER_SERVICE_REP\x10\x46\x12\x12\n\x0eSET_ROUTES_REQ\x10G\x12\x12\n\x0eSET_ROUTES_REP\x10H\x12\x12\n\x0eGET_ROUTES_REQ\x10K\x12\x12\n\x0eGET_ROUTES_REP\x10L\x12\x1f\n\x1bGET_TOPIC_DIST_CHECKSUM_REQ\x10M\x12\x1f\n\x1bGET_TOPIC_DIST_CHECKSUM_REP\x10N\x12\x1f\n\x1bGET_ROUTE_DIST_CHECKSUM_REQ\x10O\x12\x1f\n\x1bGET_ROUTE_DIST_CHECKSUM_REP\x10P\x12\x15\n\x11PICK_FRONTEND_REQ\x10Q\x12\x15\n\x11PICK_FRONTEND_REP\x10R\x12\x16\n\x12PICK_FRONTENDS_REQ\x10S\x12\x16\n\x12PICK_FRONTENDS_REP\x10T\x12\x14\n\x10LOCATE_TOPIC_REQ\x10U\x12\x14\n\x10LOCATE_TOPIC_REP\x10V\x12\x12\n\x0eRESOLVE_IP_REQ\x10y\x12\x12\n\x0eRESOLVE_IP_REP\x10z*\xde\x03\n\x0c\x65rror_code_t\x12\x06\n\x02OK\x10\x00\x12\x0f\n\x0bUNKNOWN_MSG\x10\x01\x12$\n NOT_ALLOWED_TO_REGISTER_FRONTEND\x10\x64\x12#\n\x1fNOT_ALLOWED_TO_REGISTER_BACKEND\x10\x65\x12#\n\x1fNOT_ALLOWED_TO_REGISTER_SERVICE\x10\x66\x12\x18\n\x14\x46\x41ILED_TO_SET_ROUTES\x10g\x12\x1b\n\x17\x46\x41ILED_TO_PICK_FRONTEND\x10h\x12\x1a\n\x16\x46\x41ILED_TO_LOCATE_TOPIC\x10i\x12\x11\n\x0cMASTER_ERROR\x10\xc7\x01\x12\x1e\n\x19\x46\x41ILED_TO_REQUEST_SERVICE\x10\xc8\x01\x12\x1e\n\x19\x46\x41ILED_TO_REQUEST_BACKEND\x10\xc9\x01\x12\x13\n\x0e\x46RONTEND_ERROR\x10\xab\x02\x12\x13\n\x0e\x46\x41ILED_TO_PUSH\x10\xac\x02\x12\x13\n\x0e\x46\x41ILED_TO_PULL\x10\xad\x02\x12\x12\n\rUNKNOWN_TOPIC\x10\xae\x02\x12\x12\n\rBACKEND_ERROR\x10\x8f\x03\x12\x11\n\x0cUNKNOWN_PATH\x10\x90\x03\x12\x12\n\rSERVICE_ERROR\x10\xf3\x03\x12\x11\n\x0c\x43LIENT_ERROR\x10\xd7\x04\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16maxwell_protocol.proto\x12\x10maxwell.protocol\"\x19\n\nping_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x19\n\nping_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x17\n\x08ok_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"6\n\x0b\x65rror_rep_t\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\">\n\tok2_rep_t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"]\n\x0c\x65rror2_rep_t\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"7\n\npush_req_t\x12\r\n\x05topic\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x19\n\npush_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"m\n\npull_req_t\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\x02 \x01(\x03\x12\r\n\x05limit\x18\x03 \x01(\r\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"f\n\npull_rep_t\x12%\n\x04msgs\x18\x01 \x03(\x0b\x32\x17.maxwell.protocol.msg_t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x89\x01\n\treq_req_t\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0f\n\x07payload\x18\x02 \x01(\t\x12*\n\x06header\x18\x0c \x01(\x0b\x32\x1a.maxwell.protocol.header_t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"O\n\treq_rep_t\x12\x0f\n\x07payload\x18\x01 \x01(\t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"N\n\nauth_req_t\x12\r\n\x05token\x18\x01 \x01(\t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"?\n\nauth_rep_t\x12\x11\n\tconn0_ref\x18\r \x01(\r\x12\x11\n\tconn1_ref\x18\x0e \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"E\n\x17register_frontend_req_t\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\thttp_port\x18\x02 \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"&\n\x17register_frontend_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"D\n\x16register_backend_req_t\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\thttp_port\x18\x02 \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"%\n\x16register_backend_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"D\n\x16register_service_req_t\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\thttp_port\x18\x02 \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"%\n\x16register_service_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\xd6\x01\n\x10set_routes_req_t\x12\x10\n\x08ws_paths\x18\x01 \x03(\t\x12\x11\n\tget_paths\x18\x02 \x03(\t\x12\x12\n\npost_paths\x18\x03 \x03(\t\x12\x11\n\tput_paths\x18\x04 \x03(\t\x12\x13\n\x0bpatch_paths\x18\x05 \x03(\t\x12\x14\n\x0c\x64\x65lete_paths\x18\x06 \x03(\t\x12\x12\n\nhead_paths\x18\x07 \x03(\t\x12\x15\n\roptions_paths\x18\x08 \x03(\t\x12\x13\n\x0btrace_paths\x18\t \x03(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x1f\n\x10set_routes_rep_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x1f\n\x10get_routes_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\xbe\x04\n\x10get_routes_rep_t\x12\x38\n\x0fws_route_groups\x18\x01 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12\x39\n\x10get_route_groups\x18\x02 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12:\n\x11post_route_groups\x18\x03 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12\x39\n\x10put_route_groups\x18\x04 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12;\n\x12patch_route_groups\x18\x05 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12<\n\x13\x64\x65lete_route_groups\x18\x06 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12:\n\x11head_route_groups\x18\x07 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12=\n\x14options_route_groups\x18\x08 \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12;\n\x12trace_route_groups\x18\t \x03(\x0b\x32\x1f.maxwell.protocol.route_group_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\",\n\x1dget_topic_dist_checksum_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\">\n\x1dget_topic_dist_checksum_rep_t\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\",\n\x1dget_route_dist_checksum_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\">\n\x1dget_route_dist_checksum_rep_t\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\r\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\"\n\x13pick_frontend_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"4\n\x13pick_frontend_rep_t\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"#\n\x14pick_frontends_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"6\n\x14pick_frontends_rep_t\x12\x11\n\tendpoints\x18\x01 \x03(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"0\n\x12locate_topic_req_t\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"3\n\x12locate_topic_rep_t\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"\x1f\n\x10resolve_ip_req_t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"+\n\x10resolve_ip_rep_t\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0b\n\x03ref\x18\x0f \x01(\r\"9\n\x05msg_t\x12\x0e\n\x06offset\x18\x01 \x01(\x04\x12\r\n\x05value\x18\x02 \x01(\x0c\x12\x11\n\ttimestamp\x18\x03 \x01(\x04\":\n\x08header_t\x12\r\n\x05\x61gent\x18\x01 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x02 \x01(\t\x12\r\n\x05token\x18\x03 \x01(\t\"U\n\rroute_group_t\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x19\n\x11healthy_endpoints\x18\x02 \x03(\t\x12\x1b\n\x13unhealthy_endpoints\x18\x03 \x03(\t*\xff\x05\n\nmsg_type_t\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08PING_REQ\x10\x01\x12\x0c\n\x08PING_REP\x10\x02\x12\n\n\x06OK_REP\x10\x1d\x12\r\n\tERROR_REP\x10\x1e\x12\x0b\n\x07OK2_REP\x10\x1f\x12\x0e\n\nERROR2_REP\x10 \x12\x0c\n\x08PUSH_REQ\x10!\x12\x0c\n\x08PUSH_REP\x10\"\x12\x0c\n\x08PULL_REQ\x10#\x12\x0c\n\x08PULL_REP\x10$\x12\x0b\n\x07REQ_REQ\x10\'\x12\x0b\n\x07REQ_REP\x10(\x12\x0c\n\x08\x41UTH_REQ\x10)\x12\x0c\n\x08\x41UTH_REP\x10*\x12\x19\n\x15REGISTER_FRONTEND_REQ\x10\x41\x12\x19\n\x15REGISTER_FRONTEND_REP\x10\x42\x12\x18\n\x14REGISTER_BACKEND_REQ\x10\x43\x12\x18\n\x14REGISTER_BACKEND_REP\x10\x44\x12\x18\n\x14REGISTER_SERVICE_REQ\x10\x45\x12\x18\n\x14REGISTER_SERVICE_REP\x10\x46\x12\x12\n\x0eSET_ROUTES_REQ\x10G\x12\x12\n\x0eSET_ROUTES_REP\x10H\x12\x12\n\x0eGET_ROUTES_REQ\x10K\x12\x12\n\x0eGET_ROUTES_REP\x10L\x12\x1f\n\x1bGET_TOPIC_DIST_CHECKSUM_REQ\x10M\x12\x1f\n\x1bGET_TOPIC_DIST_CHECKSUM_REP\x10N\x12\x1f\n\x1bGET_ROUTE_DIST_CHECKSUM_REQ\x10O\x12\x1f\n\x1bGET_ROUTE_DIST_CHECKSUM_REP\x10P\x12\x15\n\x11PICK_FRONTEND_REQ\x10Q\x12\x15\n\x11PICK_FRONTEND_REP\x10R\x12\x16\n\x12PICK_FRONTENDS_REQ\x10S\x12\x16\n\x12PICK_FRONTENDS_REP\x10T\x12\x14\n\x10LOCATE_TOPIC_REQ\x10U\x12\x14\n\x10LOCATE_TOPIC_REP\x10V\x12\x12\n\x0eRESOLVE_IP_REQ\x10y\x12\x12\n\x0eRESOLVE_IP_REP\x10z*\xde\x03\n\x0c\x65rror_code_t\x12\x06\n\x02OK\x10\x00\x12\x0f\n\x0bUNKNOWN_MSG\x10\x01\x12$\n NOT_ALLOWED_TO_REGISTER_FRONTEND\x10\x64\x12#\n\x1fNOT_ALLOWED_TO_REGISTER_BACKEND\x10\x65\x12#\n\x1fNOT_ALLOWED_TO_REGISTER_SERVICE\x10\x66\x12\x18\n\x14\x46\x41ILED_TO_SET_ROUTES\x10g\x12\x1b\n\x17\x46\x41ILED_TO_PICK_FRONTEND\x10h\x12\x1a\n\x16\x46\x41ILED_TO_LOCATE_TOPIC\x10i\x12\x11\n\x0cMASTER_ERROR\x10\xc7\x01\x12\x1e\n\x19\x46\x41ILED_TO_REQUEST_SERVICE\x10\xc8\x01\x12\x1e\n\x19\x46\x41ILED_TO_REQUEST_BACKEND\x10\xc9\x01\x12\x13\n\x0e\x46RONTEND_ERROR\x10\xab\x02\x12\x13\n\x0e\x46\x41ILED_TO_PUSH\x10\xac\x02\x12\x13\n\x0e\x46\x41ILED_TO_PULL\x10\xad\x02\x12\x12\n\rUNKNOWN_TOPIC\x10\xae\x02\x12\x12\n\rBACKEND_ERROR\x10\x8f\x03\x12\x11\n\x0cUNKNOWN_PATH\x10\x90\x03\x12\x12\n\rSERVICE_ERROR\x10\xf3\x03\x12\x11\n\x0c\x43LIENT_ERROR\x10\xd7\x04\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'maxwell_protocol_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_MSG_TYPE_T']._serialized_start=2947
-  _globals['_MSG_TYPE_T']._serialized_end=3714
-  _globals['_ERROR_CODE_T']._serialized_start=3717
-  _globals['_ERROR_CODE_T']._serialized_end=4195
+  _globals['_MSG_TYPE_T']._serialized_start=2983
+  _globals['_MSG_TYPE_T']._serialized_end=3750
+  _globals['_ERROR_CODE_T']._serialized_start=3753
+  _globals['_ERROR_CODE_T']._serialized_end=4231
   _globals['_PING_REQ_T']._serialized_start=44
   _globals['_PING_REQ_T']._serialized_end=69
   _globals['_PING_REP_T']._serialized_start=71
   _globals['_PING_REP_T']._serialized_end=96
   _globals['_OK_REP_T']._serialized_start=98
   _globals['_OK_REP_T']._serialized_end=121
   _globals['_ERROR_REP_T']._serialized_start=123
@@ -50,57 +50,57 @@
   _globals['_REQ_REP_T']._serialized_start=777
   _globals['_REQ_REP_T']._serialized_end=856
   _globals['_AUTH_REQ_T']._serialized_start=858
   _globals['_AUTH_REQ_T']._serialized_end=936
   _globals['_AUTH_REP_T']._serialized_start=938
   _globals['_AUTH_REP_T']._serialized_end=1001
   _globals['_REGISTER_FRONTEND_REQ_T']._serialized_start=1003
-  _globals['_REGISTER_FRONTEND_REQ_T']._serialized_end=1060
-  _globals['_REGISTER_FRONTEND_REP_T']._serialized_start=1062
-  _globals['_REGISTER_FRONTEND_REP_T']._serialized_end=1100
-  _globals['_REGISTER_BACKEND_REQ_T']._serialized_start=1102
-  _globals['_REGISTER_BACKEND_REQ_T']._serialized_end=1158
-  _globals['_REGISTER_BACKEND_REP_T']._serialized_start=1160
-  _globals['_REGISTER_BACKEND_REP_T']._serialized_end=1197
-  _globals['_REGISTER_SERVICE_REQ_T']._serialized_start=1199
-  _globals['_REGISTER_SERVICE_REQ_T']._serialized_end=1255
-  _globals['_REGISTER_SERVICE_REP_T']._serialized_start=1257
-  _globals['_REGISTER_SERVICE_REP_T']._serialized_end=1294
-  _globals['_SET_ROUTES_REQ_T']._serialized_start=1297
-  _globals['_SET_ROUTES_REQ_T']._serialized_end=1511
-  _globals['_SET_ROUTES_REP_T']._serialized_start=1513
-  _globals['_SET_ROUTES_REP_T']._serialized_end=1544
-  _globals['_GET_ROUTES_REQ_T']._serialized_start=1546
-  _globals['_GET_ROUTES_REQ_T']._serialized_end=1577
-  _globals['_GET_ROUTES_REP_T']._serialized_start=1580
-  _globals['_GET_ROUTES_REP_T']._serialized_end=2154
-  _globals['_GET_TOPIC_DIST_CHECKSUM_REQ_T']._serialized_start=2156
-  _globals['_GET_TOPIC_DIST_CHECKSUM_REQ_T']._serialized_end=2200
-  _globals['_GET_TOPIC_DIST_CHECKSUM_REP_T']._serialized_start=2202
-  _globals['_GET_TOPIC_DIST_CHECKSUM_REP_T']._serialized_end=2264
-  _globals['_GET_ROUTE_DIST_CHECKSUM_REQ_T']._serialized_start=2266
-  _globals['_GET_ROUTE_DIST_CHECKSUM_REQ_T']._serialized_end=2310
-  _globals['_GET_ROUTE_DIST_CHECKSUM_REP_T']._serialized_start=2312
-  _globals['_GET_ROUTE_DIST_CHECKSUM_REP_T']._serialized_end=2374
-  _globals['_PICK_FRONTEND_REQ_T']._serialized_start=2376
-  _globals['_PICK_FRONTEND_REQ_T']._serialized_end=2410
-  _globals['_PICK_FRONTEND_REP_T']._serialized_start=2412
-  _globals['_PICK_FRONTEND_REP_T']._serialized_end=2464
-  _globals['_PICK_FRONTENDS_REQ_T']._serialized_start=2466
-  _globals['_PICK_FRONTENDS_REQ_T']._serialized_end=2501
-  _globals['_PICK_FRONTENDS_REP_T']._serialized_start=2503
-  _globals['_PICK_FRONTENDS_REP_T']._serialized_end=2557
-  _globals['_LOCATE_TOPIC_REQ_T']._serialized_start=2559
-  _globals['_LOCATE_TOPIC_REQ_T']._serialized_end=2607
-  _globals['_LOCATE_TOPIC_REP_T']._serialized_start=2609
-  _globals['_LOCATE_TOPIC_REP_T']._serialized_end=2660
-  _globals['_RESOLVE_IP_REQ_T']._serialized_start=2662
-  _globals['_RESOLVE_IP_REQ_T']._serialized_end=2693
-  _globals['_RESOLVE_IP_REP_T']._serialized_start=2695
-  _globals['_RESOLVE_IP_REP_T']._serialized_end=2738
-  _globals['_MSG_T']._serialized_start=2740
-  _globals['_MSG_T']._serialized_end=2797
-  _globals['_HEADER_T']._serialized_start=2799
-  _globals['_HEADER_T']._serialized_end=2857
-  _globals['_ROUTE_GROUP_T']._serialized_start=2859
-  _globals['_ROUTE_GROUP_T']._serialized_end=2944
+  _globals['_REGISTER_FRONTEND_REQ_T']._serialized_end=1072
+  _globals['_REGISTER_FRONTEND_REP_T']._serialized_start=1074
+  _globals['_REGISTER_FRONTEND_REP_T']._serialized_end=1112
+  _globals['_REGISTER_BACKEND_REQ_T']._serialized_start=1114
+  _globals['_REGISTER_BACKEND_REQ_T']._serialized_end=1182
+  _globals['_REGISTER_BACKEND_REP_T']._serialized_start=1184
+  _globals['_REGISTER_BACKEND_REP_T']._serialized_end=1221
+  _globals['_REGISTER_SERVICE_REQ_T']._serialized_start=1223
+  _globals['_REGISTER_SERVICE_REQ_T']._serialized_end=1291
+  _globals['_REGISTER_SERVICE_REP_T']._serialized_start=1293
+  _globals['_REGISTER_SERVICE_REP_T']._serialized_end=1330
+  _globals['_SET_ROUTES_REQ_T']._serialized_start=1333
+  _globals['_SET_ROUTES_REQ_T']._serialized_end=1547
+  _globals['_SET_ROUTES_REP_T']._serialized_start=1549
+  _globals['_SET_ROUTES_REP_T']._serialized_end=1580
+  _globals['_GET_ROUTES_REQ_T']._serialized_start=1582
+  _globals['_GET_ROUTES_REQ_T']._serialized_end=1613
+  _globals['_GET_ROUTES_REP_T']._serialized_start=1616
+  _globals['_GET_ROUTES_REP_T']._serialized_end=2190
+  _globals['_GET_TOPIC_DIST_CHECKSUM_REQ_T']._serialized_start=2192
+  _globals['_GET_TOPIC_DIST_CHECKSUM_REQ_T']._serialized_end=2236
+  _globals['_GET_TOPIC_DIST_CHECKSUM_REP_T']._serialized_start=2238
+  _globals['_GET_TOPIC_DIST_CHECKSUM_REP_T']._serialized_end=2300
+  _globals['_GET_ROUTE_DIST_CHECKSUM_REQ_T']._serialized_start=2302
+  _globals['_GET_ROUTE_DIST_CHECKSUM_REQ_T']._serialized_end=2346
+  _globals['_GET_ROUTE_DIST_CHECKSUM_REP_T']._serialized_start=2348
+  _globals['_GET_ROUTE_DIST_CHECKSUM_REP_T']._serialized_end=2410
+  _globals['_PICK_FRONTEND_REQ_T']._serialized_start=2412
+  _globals['_PICK_FRONTEND_REQ_T']._serialized_end=2446
+  _globals['_PICK_FRONTEND_REP_T']._serialized_start=2448
+  _globals['_PICK_FRONTEND_REP_T']._serialized_end=2500
+  _globals['_PICK_FRONTENDS_REQ_T']._serialized_start=2502
+  _globals['_PICK_FRONTENDS_REQ_T']._serialized_end=2537
+  _globals['_PICK_FRONTENDS_REP_T']._serialized_start=2539
+  _globals['_PICK_FRONTENDS_REP_T']._serialized_end=2593
+  _globals['_LOCATE_TOPIC_REQ_T']._serialized_start=2595
+  _globals['_LOCATE_TOPIC_REQ_T']._serialized_end=2643
+  _globals['_LOCATE_TOPIC_REP_T']._serialized_start=2645
+  _globals['_LOCATE_TOPIC_REP_T']._serialized_end=2696
+  _globals['_RESOLVE_IP_REQ_T']._serialized_start=2698
+  _globals['_RESOLVE_IP_REQ_T']._serialized_end=2729
+  _globals['_RESOLVE_IP_REP_T']._serialized_start=2731
+  _globals['_RESOLVE_IP_REP_T']._serialized_end=2774
+  _globals['_MSG_T']._serialized_start=2776
+  _globals['_MSG_T']._serialized_end=2833
+  _globals['_HEADER_T']._serialized_start=2835
+  _globals['_HEADER_T']._serialized_end=2893
+  _globals['_ROUTE_GROUP_T']._serialized_start=2895
+  _globals['_ROUTE_GROUP_T']._serialized_end=2980
 # @@protoc_insertion_point(module_scope)
```

### Comparing `maxwell_protocol-0.7.3/.gitignore` & `maxwell_protocol-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `maxwell_protocol-0.7.3/LICENSE` & `maxwell_protocol-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maxwell_protocol-0.7.3/pyproject.toml` & `maxwell_protocol-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 dependencies = ["protobuf >= 5.26.0"]
 description = "The maxwell protocol implementation for python."
 license = {file = "LICENSE"}
 name = "maxwell-protocol"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.7.3"
+version = "0.8.0"
 
 [project.optional-dependencies]
 test = ["pytest >= 8.1.1", "pytest-cov >= 4.1.0"]
 
 [project.urls]
 changelog = "https://github.com/maxwell-dev/maxwell-protocol-python/CHANGELOG.md"
 repository = "https://github.com/maxwell-dev/maxwell-protocol-python"
```

### Comparing `maxwell_protocol-0.7.3/PKG-INFO` & `maxwell_protocol-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: maxwell-protocol
-Version: 0.7.3
+Version: 0.8.0
 Summary: The maxwell protocol implementation for python.
 Project-URL: changelog, https://github.com/maxwell-dev/maxwell-protocol-python/CHANGELOG.md
 Project-URL: repository, https://github.com/maxwell-dev/maxwell-protocol-python
 Author-email: Xu Chaoqian <chaoranxu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

