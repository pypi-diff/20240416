# Comparing `tmp/dns_manager-0.0.14-py3-none-any.whl.zip` & `tmp/dns_manager-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 23406 bytes, number of entries: 19
--rw-r--r--  2.0 unx     2396 b- defN 16-Jan-01 00:00 dns_manager-0.0.14.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 dns_manager-0.0.14.dist-info/WHEEL
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 dns_manager-0.0.14.dist-info/entry_points.txt
--rw-r--r--  2.0 unx    35099 b- defN 16-Jan-01 00:00 dns_manager-0.0.14.dist-info/licenses/LICENSE
+Zip file size: 22501 bytes, number of entries: 19
+-rw-r--r--  2.0 unx     2243 b- defN 16-Jan-01 00:00 dns_manager-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 dns_manager-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 dns_manager-0.0.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx    35099 b- defN 16-Jan-01 00:00 dns_manager-0.0.8.dist-info/licenses/LICENSE
 -rw-r--r--  2.0 unx       37 b- defN 16-Jan-01 00:00 dns_manager/__init__.py
--rw-r--r--  2.0 unx     2717 b- defN 16-Jan-01 00:00 dns_manager/__main__.py
--rw-r--r--  2.0 unx       22 b- defN 16-Jan-01 00:00 dns_manager/__version__.py
+-rw-r--r--  2.0 unx     2564 b- defN 16-Jan-01 00:00 dns_manager/__main__.py
+-rw-r--r--  2.0 unx       21 b- defN 16-Jan-01 00:00 dns_manager/__version__.py
 -rw-r--r--  2.0 unx       93 b- defN 16-Jan-01 00:00 dns_manager/getter/__init__.py
 -rw-r--r--  2.0 unx      309 b- defN 16-Jan-01 00:00 dns_manager/getter/base.py
 -rw-r--r--  2.0 unx      348 b- defN 16-Jan-01 00:00 dns_manager/getter/public.py
--rw-r--r--  2.0 unx     1831 b- defN 16-Jan-01 00:00 dns_manager/getter/snmp.py
+-rw-r--r--  2.0 unx     2036 b- defN 16-Jan-01 00:00 dns_manager/getter/snmp.py
 -rw-r--r--  2.0 unx       54 b- defN 16-Jan-01 00:00 dns_manager/model/__init__.py
--rw-r--r--  2.0 unx      200 b- defN 16-Jan-01 00:00 dns_manager/model/config.py
--rw-r--r--  2.0 unx      567 b- defN 16-Jan-01 00:00 dns_manager/model/record.py
+-rw-r--r--  2.0 unx      164 b- defN 16-Jan-01 00:00 dns_manager/model/config.py
+-rw-r--r--  2.0 unx      377 b- defN 16-Jan-01 00:00 dns_manager/model/record.py
 -rw-r--r--  2.0 unx       65 b- defN 16-Jan-01 00:00 dns_manager/setter/__init__.py
--rw-r--r--  2.0 unx     4561 b- defN 16-Jan-01 00:00 dns_manager/setter/base.py
--rw-r--r--  2.0 unx     4979 b- defN 16-Jan-01 00:00 dns_manager/setter/dnspod.py
--rw-r--r--  2.0 unx     4185 b- defN 16-Jan-01 00:00 dns_manager/utils.py
-?rw-------  2.0 unx     1577 b- defN 16-Jan-01 00:00 dns_manager-0.0.14.dist-info/RECORD
-19 files, 59220 bytes uncompressed, 20810 bytes compressed:  64.9%
+-rw-r--r--  2.0 unx     3082 b- defN 16-Jan-01 00:00 dns_manager/setter/base.py
+-rw-r--r--  2.0 unx     5004 b- defN 16-Jan-01 00:00 dns_manager/setter/dnspod.py
+-rw-r--r--  2.0 unx     2291 b- defN 16-Jan-01 00:00 dns_manager/utils.py
+?rw-------  2.0 unx     1572 b- defN 16-Jan-01 00:00 dns_manager-0.0.8.dist-info/RECORD
+19 files, 55539 bytes uncompressed, 19915 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -1,17 +1,17 @@
-Filename: dns_manager-0.0.14.dist-info/METADATA
+Filename: dns_manager-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: dns_manager-0.0.14.dist-info/WHEEL
+Filename: dns_manager-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: dns_manager-0.0.14.dist-info/entry_points.txt
+Filename: dns_manager-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: dns_manager-0.0.14.dist-info/licenses/LICENSE
+Filename: dns_manager-0.0.8.dist-info/licenses/LICENSE
 Comment: 
 
 Filename: dns_manager/__init__.py
 Comment: 
 
 Filename: dns_manager/__main__.py
 Comment: 
@@ -48,11 +48,11 @@
 
 Filename: dns_manager/setter/dnspod.py
 Comment: 
 
 Filename: dns_manager/utils.py
 Comment: 
 
-Filename: dns_manager-0.0.14.dist-info/RECORD
+Filename: dns_manager-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dns_manager/__main__.py

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import asyncio
 import json
-import os
 from pathlib import Path
 
 import typer
 from loguru import logger
 from rich.console import Console
 from rich.highlighter import NullHighlighter
 from rich.live import Live
@@ -16,68 +15,51 @@
 
 from dns_manager.utils import create_setter_by_str, load_config
 
 app = typer.Typer()
 
 
 def init_logger(log_level: str):
-    log_level = os.environ.get("LOG_LEVEL", log_level)
-    handler = RichHandler(
-        console=Console(style=Style()), highlighter=NullHighlighter(), markup=True
-    )
+    handler = RichHandler(console=Console(style=Style()), highlighter=NullHighlighter(), markup=True)
     logger.remove()
     logger.add(handler, format="{message}", level=log_level)
 
 
 @app.command()
-def update(
-    path: Path,
-    setter: str = "dnspod",
-    remove_unmanaged: bool = False,
-    log_level: str = "INFO",
-):
+def update(path: Path = Path("~/.config/autoconfig/dns-manager.json"), setter: str = "dnspod", log_level: str = "INFO"):
     init_logger(log_level)
-    logger.info("Loading dns config from [bold purple]{:}[/].".format(path))
+    logger.info(f"Loading dns config from [bold purple]{path}[/].")
     config = load_config(path)
     setter_obj = create_setter_by_str(config, setter)
-    setter_obj.update_dns(remove_unmanaged=remove_unmanaged)
+    setter_obj.update_dns()
 
 
 @app.command()
-def watch(
-    path: Path,
-    setter: str = "dnspod",
-    log_level: str = "INFO",
-):
+def watch(path: Path = Path("~/.config/autoconfig/dns-manager.json"), setter: str = "dnspod", log_level: str = "INFO"):
     init_logger(log_level)
     path = path.expanduser()
     asyncio.run(watch_async(path, setter))
 
 
 async def watch_async(path: Path, setter: str):
     import watchfiles
 
-    logger.info("Loading dns config from [bold purple]{:}[/].".format(path))
+    logger.info(f"Loading dns config from [bold purple]{path}[/].")
     config = load_config(path)
     setter_obj = create_setter_by_str(config, setter)
     interval = int(config.get("interval", 300))
-    progress = Progress(
-        TextColumn("{task.description}: [bold blue]{task.completed}s/{task.total}s[/]"),
-        transient=True,
-    )
+    progress = Progress(TextColumn("{task.description}: [bold blue]{task.completed}s/{task.total}s[/]"), transient=True)
     countdown = progress.add_task("Update Timer", total=interval)
 
     async def watch_config():
         async for _ in watchfiles.awatch(path):
             with open(path) as f:
                 config = json.load(f)
             await setter_obj.update_config_async(config)
-            progress.update(
-                countdown, completed=interval, description="Update Timer([bold]Reloading Config[/])"
-            )
+            progress.update(countdown, completed=interval, description="Update Timer([bold]Reloading Config[/])")
 
     async def update_dns():
         while True:
             setter_obj.update_dns()
             progress.reset(countdown, description="Update Timer")
 
             with Live(progress):
```

## dns_manager/__version__.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.14'
+__version__ = '0.0.8'
```

## dns_manager/getter/snmp.py

```diff
@@ -13,41 +13,43 @@
     name_prefix = Suppress("STRING:")
     integer_prefix = Suppress("INTEGER:")
     equal_sign = Suppress("=")
 
     interface_id = Word(nums).set_results_name("interface_id")
     interface_name = Word(alphanums + "_").set_results_name("interface")
 
-    ifname_pattern = OneOrMore(
-        Group(mib_prefix + interface_id + equal_sign + name_prefix + interface_name)
-    )
+    ifname_pattern = OneOrMore(Group(mib_prefix + interface_id + equal_sign + name_prefix + interface_name))
 
     ip_address = Combine(Word(nums) + ("." + Word(nums)) * 3).set_results_name("ip_address")
-    ip_pattern = OneOrMore(
-        Group(mib_prefix + ip_address + equal_sign + integer_prefix + interface_id)
-    )
+    ip_pattern = OneOrMore(Group(mib_prefix + ip_address + equal_sign + integer_prefix + interface_id))
 
     def __init__(self, group: str, host: str, interface: str):
         self.group = group
         self.host = host
 
         self.interface = interface
 
     def walk(self, oid: str, pattern: ParserElement | None = None) -> Iterable[str]:
-        cmd = "snmpwalk -v 2c -c {:} {:} {:}".format(self.group, self.host, oid)
+        cmd = f"snmpwalk -v 2c -c {self.group} {self.host} {oid}"
         results = os.popen(cmd)
         if pattern is None:
             return results
         else:
             return pattern.parse_string(results.read())
 
-    def get_ip(self) -> str:
+    def get_interface_ip(self, interface: str) -> str:
         mapping_name_to_id = {
-            interface_name: interface_id
-            for interface_id, interface_name in self.walk("ifname", self.ifname_pattern)
+            interface_name: interface_id for interface_id, interface_name in self.walk("ifname", self.ifname_pattern)
         }
         mapping_id_to_ip = {
-            interface_id: ip_address
-            for ip_address, interface_id in self.walk(".1.3.6.1.2.1.4.20.1.2", self.ip_pattern)
+            interface_id: ip_address for ip_address, interface_id in self.walk(".1.3.6.1.2.1.4.20.1.2", self.ip_pattern)
         }
 
-        return mapping_id_to_ip[mapping_name_to_id[self.interface]]
+        return mapping_id_to_ip[mapping_name_to_id[interface]]
+
+    def get_ip(self):
+        return self.get_interface_ip(self.interface)
+
+
+def get_interface_ip(interface: str, *, host: str = "192.168.1.1", group: str = "public") -> str:
+    walker = SnmpGetter(group, host, interface)
+    return walker.get_ip()
```

## dns_manager/model/config.py

```diff
@@ -2,8 +2,7 @@
 
 from pydantic import BaseModel
 
 
 class Config(BaseModel):
     domain: str
     records: list[tuple[str | list[str], str | None]]
-    ignore: list[str] | None = None
```

## dns_manager/model/record.py

```diff
@@ -8,15 +8,8 @@
     value: str
     type: str | None = None
 
     def __hash__(self) -> int:
         return hash(self.subdomain)
 
     def __eq__(self, other: Record) -> bool:
-        return (
-            self.subdomain == other.subdomain
-            and self.value == other.value
-            and self.type == other.type
-        )
-
-    def __str__(self) -> str:
-        return "[bold blue]{:}[/]: {:} [bold blue]➡️[/] {:}".format(self.type, self.subdomain, self.value)
+        return self.subdomain == other.subdomain and self.value == other.value and self.type == other.type
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## dns_manager/setter/base.py

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 from abc import abstractmethod
 from enum import Enum
-from pathlib import Path
 
 from loguru import logger
 
 from ..model import Config, Record
 
 
 class RecordStatus(Enum):
@@ -29,91 +28,62 @@
                 return "[red]🔥 Deleted[/]"
             case "FAILED":
                 return "[red]❌ Failed[/]"
 
 
 class DNSSetterBase:
     def __init__(self, config: dict):
-        self.cached_records: dict[str, Record] = {}
+        self.records_cache: dict[str, Record] = {}
         self.update_config(Config.model_validate(config))
-        self.fetch()
+        self.init_records_cache()
 
     def update_config(self, config: Config):
-        self.config = config
-        self.domain = self.config.domain
-        self.record_config: list[tuple[str, str]] = []
-        self.ignored_records = set(self.config.ignore or [])
-        for name, value in self.config.records:
+        self.domain = config.domain
+        records: list[tuple[str, str]] = []
+        for name, value in config.records:
             if value == "unknown" or value is None:
                 value = self.domain
             if isinstance(name, str):
-                self.record_config.append((name, value))
+                records.append((name, value))
             else:
-                self.record_config.extend([(subdomain, value) for subdomain in name])
+                records.extend([(subdomain, value) for subdomain in name])
+        self.record_config = records
 
     async def update_config_async(self, config: Config):
         self.update_config(config)
         await asyncio.sleep(0)
 
-    def generate_records(self) -> dict[str, Record]:
+    def get_records(self) -> dict[str, Record]:
         from ..utils import generate_record
 
         records: dict[str, Record] = {}
         for subdomain, value in self.record_config:
             records[subdomain] = generate_record(subdomain, value)
         return records
 
-    def update_dns(self, remove_unmanaged: bool = False):
-        from ..utils import save_config
-
-        new_records = self.generate_records()
-        unmanaged_records = (
-            set(self.cached_records.keys()) - set(new_records.keys()) - self.ignored_records
-        )
-        if len(unmanaged_records) > 0:
-            if remove_unmanaged:
-                for subdomain in unmanaged_records:
-                    record = self.cached_records[subdomain]
-                    record_id = self.get_record_id(record)
-                    status = self.delete_record(record_id)
-                    if status == RecordStatus.DELETED:
-                        del self.cached_records[subdomain]
-                    logger.info("({:}) {:}".format(status, record))
-            else:
-                records = []
-                for subdomain in unmanaged_records:
-                    record = self.cached_records[subdomain]
-                    records.append((subdomain, record.value))
-                    logger.warning("([red]🔓 Unmanaged[/]) {:}".format(record))
-                path = Path("~/.config/dns-manager/unmanaged.json")
-                save_config(
-                    path,
-                    Config(
-                        domain=self.domain,
-                        records=records,
-                    ).model_dump(),
-                )
-                logger.info("Unmanaged records saved to [bold purple]{:}[/].".format(path))
+    def update_dns(self):
+        new_records = self.get_records()
         for subdomain, record in new_records.items():
-            cached_record = self.cached_records.get(subdomain, None)
-            if cached_record is None:
+            arrow = "[bold blue]➡️[/]"
+            record_cache = self.records_cache.get(subdomain, None)
+            if record_cache is None:
                 status = self.create_record(record)
-            elif record != cached_record:
-                status = self.modify_record(self.get_record_id(cached_record), record)
+            elif record != record_cache:
+                status = self.modify_record(self.get_record_id(record_cache), record)
             else:
                 status = RecordStatus.EXISTS
 
             if status in (RecordStatus.CREATED, RecordStatus.MODIFIED):
-                self.cached_records[subdomain] = record
-            logger.info("({:}) {:}".format(status, record))
+                self.records_cache[subdomain] = record
+            logger.info(f"({status}) [bold blue]{record.type}[/]: {subdomain} {arrow} {record.value}")
 
         # TODO: delete records which are not in new_records
 
     @abstractmethod
-    def fetch(self) -> None:
+    def init_records_cache(self) -> None:
         pass
 
     @abstractmethod
     def get_record_id(self, record: Record) -> str:
         pass
 
     @abstractmethod
@@ -123,11 +93,7 @@
     @abstractmethod
     def delete_record(self, record_id: str) -> RecordStatus:
         pass
 
     @abstractmethod
     def modify_record(self, record_id: str, record: Record) -> RecordStatus:
         pass
-
-    @abstractmethod
-    def list_records(self) -> list[Record]:
-        pass
```

## dns_manager/setter/dnspod.py

```diff
@@ -15,62 +15,60 @@
 from ..model import Record
 from .base import DNSSetterBase, RecordStatus
 
 
 class DNSPodSetter(DNSSetterBase):
     def __init__(self, config: dict, token: Token | None = None) -> None:
         if token is not None:
-            logger.info("Secret not found in env, load using token: {:}".format(token.name))
+            logger.info(f"Secret not found in env, load using token: {token.name}")
             envs = {env.name: env.value for env in token.envs}
-            secret_id = envs.get("TENCENTCLOUD_SECRET_ID")
-            secret_key = envs.get("TENCENTCLOUD_SECRET_KEY")
+            secret_id = envs.get("TENCENTCLOUD_SECRET_ID", None)
+            secret_key = envs.get("TENCENTCLOUD_SECRET_KEY", None)
         else:
             secret_id = os.environ.get("TENCENTCLOUD_SECRET_ID", None)
             secret_key = os.environ.get("TENCENTCLOUD_SECRET_KEY", None)
 
         cred = credential.Credential(secret_id, secret_key)
         self.client = dnspod_client.DnspodClient(cred, "")
-        self.mapping_record_to_id: dict[Record, str] = {}
         super().__init__(config)
 
-    def fetch(self) -> None:
-        self.list_records()
-        self.cached_records = {k.subdomain: k for k in self.mapping_record_to_id}
+    def init_records_cache(self) -> None:
+        self.records_cache = {k.subdomain: k for k in self.mapping_record_to_id}
 
-    def list_records(self) -> list[Record]:
+    def list_record(self) -> list[models.RecordListItem]:
         try:
             req = models.DescribeRecordListRequest()
             params = {"Domain": self.domain}
             req.from_json_string(json.dumps(params))
 
             resp = self.client.DescribeRecordList(req)
             logger.debug(resp.to_json_string())
             assert isinstance(resp.RecordList, list)
-            json_record_list: list[dict[str, str]] = [
-                json.loads(r.to_json_string()) for r in resp.RecordList
-            ]
-            output_record_list = []
-            for json_record in json_record_list:
-                record = Record(
-                    subdomain=json_record["Name"],
-                    type=json_record["Type"],
-                    value=json_record["Value"],
-                )
-                output_record_list.append(record)
-
-                self.mapping_record_to_id[record] = json_record["RecordId"]
-            return output_record_list
+            return resp.RecordList
 
         except TencentCloudSDKException as err:
             logger.exception(err)
             return []
 
     @property
-    def remote_records(self):
-        return self.list_records()
+    def mapping_record_to_id(self) -> dict[Record, str]:
+        _mapping_record_to_id = {}
+        remote_records = self.list_record()
+        for remote_record in remote_records:
+            match json.loads(remote_record.to_json_string()):
+                case {"RecordId": RecordId, "Name": Name, "Type": Type, "Value": Value, **kwargs}:
+                    _mapping_record_to_id[
+                        Record(
+                            subdomain=Name,
+                            value=Value,
+                            type=Type,
+                        )
+                    ] = RecordId
+                    logger.debug(f"Type: {Type}, Name: {Name}, {kwargs}")
+        return _mapping_record_to_id
 
     @cached(cache=TTLCache(maxsize=10, ttl=300))
     def get_record_id(self, record: Record) -> str:
         return self.mapping_record_to_id[record]
 
     def create_record(self, record: Record) -> RecordStatus:
         sub_domain, value, record_type = record.subdomain, record.value, record.type
@@ -127,9 +125,9 @@
             req.from_json_string(json.dumps(params))
 
             resp = self.client.ModifyRecord(req)
             logger.debug(resp.to_json_string())
             return RecordStatus.MODIFIED
 
         except TencentCloudSDKException as err:
-            logger.warning("{:}: {:}".format(sub_domain, err))
+            logger.warning(f"{sub_domain}: {err}")
             return RecordStatus.FAILED
```

## dns_manager/utils.py

```diff
@@ -1,38 +1,21 @@
 from __future__ import annotations
 
 import re
 from pathlib import Path
 
-from auto_token import get_config as get_token_config
-from auto_token import get_token
-from loguru import logger
+from auto_token import get_config, get_token
 
 from .getter import PublicGetter, SnmpGetter
 from .model import Record
 from .setter import DNSPodSetter
 
 
 def create_setter_by_str(config: dict, dns_setter: str = "dnspod"):
-    """
-    Create a DNS setter by string.
-
-    Example:
-    >>> logger.remove()
-    >>> config = {"domain": "bone6.top", "records": []}
-    >>> setter = create_setter_by_str(config, "dnspod")
-    >>> assert isinstance(setter, DNSPodSetter)
-
-    """
-    token = get_token(
-        "dnspod",
-        get_token_config(),
-        create=True,
-        env_names=["TENCENTCLOUD_SECRET_ID", "TENCENTCLOUD_SECRET_KEY"],
-    )
+    token = get_token("dnspod", get_config(), create=True)
     match dns_setter:
         case "dnspod":
             setter = DNSPodSetter(config, token)
         case _:
             raise NotImplementedError("Only dnspod is supported now")
     return setter
 
@@ -44,23 +27,20 @@
     #     case _:
     #         raise NotImplementedError("Only dnspod is supported now")
     # return setter
     pass
 
 
 def generate_record(name: str, value: str) -> Record:
-    if value.startswith("http"):
-        record_type = "显性URL"
-        return Record(subdomain=name, value=value, type=record_type)
     if ":" not in value:
         if re.match("\\b(?:\\d{1,3}\\.){3}\\d{1,3}\\b", value):
             record_type = "A"
         else:
             record_type = "CNAME"
-            value = value if value.endswith(".") else "{:}.".format(value)
+            value = value if value.endswith(".") else f"{value}."
         return Record(subdomain=name, value=value, type=record_type)
 
     match value.split(":"):
         case ("snmp", interface_name):
             record_type = "A"
             host: str = "192.168.1.1"
             group: str = "public"
@@ -71,16 +51,14 @@
             getter = PublicGetter(url)
         case _:
             raise NotImplementedError("Only snmp is supported now")
     return Record(subdomain=name, value=getter.get_ip(), type=record_type)
 
 
 def load_config(path: Path) -> dict:
-    if not path.exists():
-        raise FileNotFoundError("Config file {:} not found".format(path))
     path = path.expanduser()
     with open(path.expanduser()) as f:
         if path.suffix == ".json":
             import json
 
             config = json.load(f)
         elif path.suffix == ".toml":
@@ -89,44 +67,9 @@
             config = toml.load(f)
         elif path.suffix == ".yaml":
             import yaml
             from yaml import FullLoader
 
             config = yaml.load(f, Loader=FullLoader)
         else:
-            raise NotImplementedError("Unsupportted suffix {:}".format(path.suffix))
-    if "domain" not in config:
-        raise ValueError("Config must contain domain")
-    if "records" not in config:
-        config["records"] = []
-    if "ignore" not in config:
-        config["ignore"] = []
-    if "records_files" in config:
-        records_files: list[str] = config["records_files"]
-        for records_file in records_files:
-            sub_path = path.parent / records_file
-            try:
-                load_config(sub_path)
-            except FileNotFoundError:
-                logger.warning("Records file {:} not found".format(sub_path))
-            config["records"].extend(load_config(sub_path)["records"])
-            config["ignore"].extend(load_config(sub_path)["ignore"])
+            raise NotImplementedError(f"Unsupportted suffix {path.suffix}")
     return config
-
-
-def save_config(path: Path, config: dict) -> None:
-    path = path.expanduser()
-    with open(path, "w") as f:
-        if path.suffix == ".json":
-            import json
-
-            json.dump(config, f, indent=2)
-        elif path.suffix == ".toml":
-            import toml
-
-            toml.dump(config, f)
-        elif path.suffix == ".yaml":
-            import yaml
-
-            yaml.dump(config, f)
-        else:
-            raise NotImplementedError("Unsupportted suffix {:}".format(path.suffix))
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `dns_manager-0.0.14.dist-info/METADATA` & `dns_manager-0.0.8.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: dns-manager
-Version: 0.0.14
-Summary: Manage your DNS records with ease.
+Version: 0.0.8
+Summary: auto config dns
 Author-Email: Zhan Rongrui <2742392377@qq.com>
 License: MIT
-Project-URL: Homepage, https://github.com/zrr1999/dns-manager.git
-Project-URL: Repository, https://github.com/zrr1999/dns-manager.git
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Requires-Dist: tencentcloud-sdk-python-dnspod
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: rich>=13.7.0
 Requires-Dist: pyparsing>=3.1.1
 Requires-Dist: typer[all]>=0.9.0
 Requires-Dist: cachetools>=5.3.2
 Requires-Dist: pydantic>=2.5.3
-Requires-Dist: auto-token>=0.0.6
+Requires-Dist: auto-token>=0.0.4
 Requires-Dist: PyYaml>=6.0.1
 Requires-Dist: toml>=0.10.2
 Requires-Dist: httpx>=0.26.0
 Requires-Dist: watchfiles; extra == "watch"
 Requires-Dist: dns-manager[watch]; extra == "all"
 Provides-Extra: watch
 Provides-Extra: all
```

## Comparing `dns_manager-0.0.14.dist-info/licenses/LICENSE` & `dns_manager-0.0.8.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `dns_manager-0.0.14.dist-info/RECORD` & `dns_manager-0.0.8.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-dns_manager-0.0.14.dist-info/METADATA,sha256=lY_nLiBCI67su4pzOoNLgI38Oy9U6QFeCZJtepJMB90,2396
-dns_manager-0.0.14.dist-info/WHEEL,sha256=gZRWN_1fGFDwBnXrZ9N3dgvbKlKgo5AUcDIMajlGpKM,90
-dns_manager-0.0.14.dist-info/entry_points.txt,sha256=3b92vBu_zCkCoV7qTesBKCqI9tBeaH57i2liP5O7nEk,90
-dns_manager-0.0.14.dist-info/licenses/LICENSE,sha256=RHEtuiCSCHehhotUEyEDm3Wms1p_Jw416qZNkYIDTo4,35099
+dns_manager-0.0.8.dist-info/METADATA,sha256=Gvz-LtqPuAGOnI_oy4Qs3aBK2_cYABo5QXgUVv4yojw,2243
+dns_manager-0.0.8.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
+dns_manager-0.0.8.dist-info/entry_points.txt,sha256=3b92vBu_zCkCoV7qTesBKCqI9tBeaH57i2liP5O7nEk,90
+dns_manager-0.0.8.dist-info/licenses/LICENSE,sha256=RHEtuiCSCHehhotUEyEDm3Wms1p_Jw416qZNkYIDTo4,35099
 dns_manager/__init__.py,sha256=e3S0EcDGJlWIp2hddSFjvt633jfeZ4W7VyAeLpfTWVM,37
-dns_manager/__main__.py,sha256=Kz0CFw7BTD7X0VDV-9drio4Dvnhu8KK7JVvlDXB4QOs,2717
-dns_manager/__version__.py,sha256=DT3lXVWSM0vxCDfBsBbQ4k1SOUtDSFBhl094H35FE2w,22
+dns_manager/__main__.py,sha256=IPM0jo6m9oSorPOJEpBOOd5DVbnl7aj-Q8PyXGxWuGU,2564
+dns_manager/__version__.py,sha256=QaKrrCeLmUWRaUA8pjWo9GWzxTk9cCTRKQXEuQX5viQ,21
 dns_manager/getter/__init__.py,sha256=VOggztRLC2Cfubo9B0ijgfL3auEitpVq7bG5BZB5kAI,93
 dns_manager/getter/base.py,sha256=7qMioEGCZoDLefZ2uiaEyUQHoFTN6vGt76B7di86LW4,309
 dns_manager/getter/public.py,sha256=1YqKxudphYi1euQrOua5pLrZOep8UI1EYVTwVl5yWn4,348
-dns_manager/getter/snmp.py,sha256=3Gm5uMrqsaYG_u8jU80KkREbAnc8HlYF8h-VMHbb33A,1831
+dns_manager/getter/snmp.py,sha256=Ei9V4OyY-6ztMm-JqQQTrnFZ_uZUcV6t560ieGgq6Us,2036
 dns_manager/model/__init__.py,sha256=CGCBPTVyMZNIyGZdaN6O9Pvoc_KlfbPEyKjpi3dywVA,54
-dns_manager/model/config.py,sha256=Wz8SWn7BRgoCZyyzO1e3m0exKvFyu4YykH_of3ewAbg,200
-dns_manager/model/record.py,sha256=a1-Na4dDHaBGwFMwQWlVJGuaWTpaIMX9tpY2CCCZup4,567
+dns_manager/model/config.py,sha256=dlzkO_ZvNM50b0CWGmMqIyqKf1eEtNkVDroEam_ngeU,164
+dns_manager/model/record.py,sha256=7JuV0b0zoMZuYeqHgqXQT_JYQuGLfktAX7hzynr0mHo,377
 dns_manager/setter/__init__.py,sha256=q8cLpFF3HA7F0i4WIWIEuBdyaRF_NdfdwJpIGknTfuw,65
-dns_manager/setter/base.py,sha256=tH3enbD7l2x43jkep2GXKg8be98HDRvihG7A8kzwHsg,4561
-dns_manager/setter/dnspod.py,sha256=QhnFgm6Ydhuhy7R5sByzUrAQzn8qGWVsc_IB9hrtGM4,4979
-dns_manager/utils.py,sha256=Aa4k6RQEz4X4k64iPgDp6fZ7irjRAg44GeUoEATdQbU,4185
-dns_manager-0.0.14.dist-info/RECORD,,
+dns_manager/setter/base.py,sha256=Y-TE9KKbWRt7hQ-xrbRU5SFKgha5sqx_5Ttv6G1jYSA,3082
+dns_manager/setter/dnspod.py,sha256=HEEjHH2a42Z1mtDrm4d4yDgrNc1-3Yxq6sg-CNtLEcI,5004
+dns_manager/utils.py,sha256=Qp1Lh5ZjYEnbb-EJYu3EP-5QZXTzes1OPZv13Pc2Gog,2291
+dns_manager-0.0.8.dist-info/RECORD,,
```

