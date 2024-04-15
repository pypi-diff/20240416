# Comparing `tmp/web3db-1.0.0.tar.gz` & `tmp/web3db-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3db-1.0.0.tar", last modified: Sun Mar 10 22:01:53 2024, max compression
+gzip compressed data, was "web3db-1.0.1.tar", max compression
```

## Comparing `web3db-1.0.0.tar` & `web3db-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 22:01:53.834982 web3db-1.0.0/
--rw-rw-rw-   0        0        0      661 2024-03-10 22:01:53.833981 web3db-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-10 22:01:53.834982 web3db-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-03-10 22:01:52.000000 web3db-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-10 22:01:53.807991 web3db-1.0.0/web3db/
--rw-rw-rw-   0        0        0       51 2024-02-26 15:25:35.000000 web3db-1.0.0/web3db/__init__.py
--rw-rw-rw-   0        0        0    18689 2024-03-01 20:45:04.000000 web3db-1.0.0/web3db/core.py
-drwxrwxrwx   0        0        0        0 2024-03-10 22:01:53.827994 web3db-1.0.0/web3db/models/
--rw-rw-rw-   0        0        0      194 2024-02-26 15:25:35.000000 web3db-1.0.0/web3db/models/__init__.py
--rw-rw-rw-   0        0        0       88 2024-01-19 19:11:12.000000 web3db-1.0.0/web3db/models/base.py
--rw-rw-rw-   0        0        0      867 2024-01-21 14:45:55.000000 web3db-1.0.0/web3db/models/discord.py
--rw-rw-rw-   0        0        0      957 2024-02-04 19:29:31.000000 web3db-1.0.0/web3db/models/email.py
--rw-rw-rw-   0        0        0      779 2024-02-04 17:48:00.000000 web3db-1.0.0/web3db/models/github.py
--rw-rw-rw-   0        0        0     2690 2024-02-26 16:52:49.000000 web3db-1.0.0/web3db/models/mixins.py
--rw-rw-rw-   0        0        0     1721 2024-03-01 20:01:48.000000 web3db-1.0.0/web3db/models/profile.py
--rw-rw-rw-   0        0        0      763 2024-02-27 20:23:16.000000 web3db-1.0.0/web3db/models/proxy.py
--rw-rw-rw-   0        0        0     1078 2024-02-18 00:57:20.000000 web3db-1.0.0/web3db/models/twitter.py
-drwxrwxrwx   0        0        0        0 2024-03-10 22:01:53.832991 web3db-1.0.0/web3db/utils/
--rw-rw-rw-   0        0        0      205 2024-01-20 14:29:59.000000 web3db-1.0.0/web3db/utils/__init__.py
--rw-rw-rw-   0        0        0      846 2024-02-04 13:29:40.000000 web3db-1.0.0/web3db/utils/encrypt_private.py
--rw-rw-rw-   0        0        0      713 2024-02-10 15:01:20.000000 web3db-1.0.0/web3db/utils/logger.py
-drwxrwxrwx   0        0        0        0 2024-03-10 22:01:53.814990 web3db-1.0.0/web3db.egg-info/
--rw-rw-rw-   0        0        0      661 2024-03-10 22:01:53.000000 web3db-1.0.0/web3db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2024-03-10 22:01:53.000000 web3db-1.0.0/web3db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 22:01:53.000000 web3db-1.0.0/web3db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-03-10 22:01:53.000000 web3db-1.0.0/web3db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-10 22:01:53.000000 web3db-1.0.0/web3db.egg-info/top_level.txt
+-rw-r--r--   0        0        0      482 2024-04-15 23:26:20.124780 web3db-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       51 2024-02-26 15:25:35.563030 web3db-1.0.1/web3db/__init__.py
+-rw-r--r--   0        0        0    20770 2024-03-29 13:46:18.804545 web3db-1.0.1/web3db/core.py
+-rw-r--r--   0        0        0      194 2024-02-26 15:25:35.549029 web3db-1.0.1/web3db/models/__init__.py
+-rw-r--r--   0        0        0      528 2024-02-26 15:27:22.333753 web3db-1.0.1/web3db/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      450 2024-01-19 19:58:55.290355 web3db-1.0.1/web3db/models/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1911 2024-01-26 16:14:20.438761 web3db-1.0.1/web3db/models/__pycache__/discord.cpython-311.pyc
+-rw-r--r--   0        0        0     2079 2024-02-04 19:59:52.544417 web3db-1.0.1/web3db/models/__pycache__/email.cpython-311.pyc
+-rw-r--r--   0        0        0     1771 2024-02-04 17:51:16.577297 web3db-1.0.1/web3db/models/__pycache__/github.cpython-311.pyc
+-rw-r--r--   0        0        0     5715 2024-02-26 17:15:22.282534 web3db-1.0.1/web3db/models/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0        0        0     3253 2024-03-24 21:28:25.779082 web3db-1.0.1/web3db/models/__pycache__/profile.cpython-311.pyc
+-rw-r--r--   0        0        0     1751 2024-02-27 20:23:48.644261 web3db-1.0.1/web3db/models/__pycache__/proxy.cpython-311.pyc
+-rw-r--r--   0        0        0     2266 2024-02-18 00:57:41.213067 web3db-1.0.1/web3db/models/__pycache__/twitter.cpython-311.pyc
+-rw-r--r--   0        0        0       88 2024-01-19 19:11:12.418624 web3db-1.0.1/web3db/models/base.py
+-rw-r--r--   0        0        0      867 2024-01-21 14:45:55.501349 web3db-1.0.1/web3db/models/discord.py
+-rw-r--r--   0        0        0      957 2024-02-04 19:29:31.959782 web3db-1.0.1/web3db/models/email.py
+-rw-r--r--   0        0        0      779 2024-02-04 17:48:00.969984 web3db-1.0.1/web3db/models/github.py
+-rw-r--r--   0        0        0     2690 2024-02-26 16:52:49.709378 web3db-1.0.1/web3db/models/mixins.py
+-rw-r--r--   0        0        0     1974 2024-03-24 21:27:16.492192 web3db-1.0.1/web3db/models/profile.py
+-rw-r--r--   0        0        0      763 2024-02-27 20:23:16.946158 web3db-1.0.1/web3db/models/proxy.py
+-rw-r--r--   0        0        0     1078 2024-02-18 00:57:20.977221 web3db-1.0.1/web3db/models/twitter.py
+-rw-r--r--   0        0        0      205 2024-01-20 14:29:59.965637 web3db-1.0.1/web3db/utils/__init__.py
+-rw-r--r--   0        0        0      422 2024-01-20 15:56:54.552567 web3db-1.0.1/web3db/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2246 2024-03-29 13:15:23.225725 web3db-1.0.1/web3db/utils/__pycache__/encrypt_private.cpython-311.pyc
+-rw-r--r--   0        0        0     1078 2024-02-10 22:53:40.648821 web3db-1.0.1/web3db/utils/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0      922 2024-03-29 13:15:22.001268 web3db-1.0.1/web3db/utils/encrypt_private.py
+-rw-r--r--   0        0        0      713 2024-02-10 15:01:20.600084 web3db-1.0.1/web3db/utils/logger.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 web3db-1.0.1/PKG-INFO
```

### Comparing `web3db-1.0.0/web3db/core.py` & `web3db-1.0.1/web3db/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 import random
-from typing import Union
+from typing import Union, Callable
 
 import base58
+from mnemonic import Mnemonic
 from eth_account import Account as EVMAccount
 from aptos_sdk.account import Account as AptosAccount
 from solana.rpc.api import Keypair
+from bitcoinutils.hdwallet import HDWallet
+from bitcoinutils.setup import setup
 from sqlalchemy import Result, func, Sequence, delete, and_, not_, desc, Select, Update, Delete, case
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.ext.asyncio import create_async_engine, async_sessionmaker
 from sqlalchemy.future import select
 from sqlalchemy.orm import joinedload
 
 from web3db.models import *
 from web3db.utils import logger
 from web3db.utils.encrypt_private import encrypt
 
 ModelType = Union[type(Email), type(Discord), type(Twitter), type(Github), type(Proxy), type(Profile)]
 INDIVIDUAL_PROXY_LIMIT = 3
 SHARED_PROXY_LIMIT = 1
+setup('mainnet')
+
+
+def prepare_strings(*s):
+    return [string.strip() if string else string for string in s]
 
 
 class DBHelper:
 
     def __init__(self, url: str, echo: bool = False):
         self.engine = create_async_engine(url=url, echo=echo)
         self.session_factory = async_sessionmaker(
             bind=self.engine,
             autoflush=False,
             autocommit=False,
             expire_on_commit=False
         )
 
+    def prepare_values(func: Callable):
+        async def wrapper(self, *args):
+            return await func(self, *prepare_strings(*args))
+
+        return wrapper
+
     async def add_record(self, record: ModelType | list) -> ModelType | None:
         async with self.session_factory() as session:
             try:
                 if isinstance(record, list):
                     session.add_all(record)
                 else:
                     session.add(record)
@@ -61,38 +75,47 @@
         if model == Proxy:
             query = select(model).where(model.proxy_string == login).options(joinedload('*'))
         else:
             query = select(model).where(model.login == login).options(joinedload('*'))
         result = await self._exec_stmt(query)
         return result.scalars().first()
 
+    @prepare_values
     async def add_email(self, login: str, password: str) -> None:
         logger.info(f'Adding Email {login}:{password}')
         await self.add_record(Email(login=login, password=password))
 
+    @prepare_values
     async def add_twitter(
             self,
             auth_token: str,
             login: str = None,
             password: str = None,
             email: str = None,
             email_password: str = None
     ) -> None:
+        (
+            auth_token, login, password,
+            email, email_password
+        ) = prepare_strings(auth_token, login, password, email, email_password)
         logger.info(f'Adding Twitter {auth_token}')
-        mail = (await self.get_row_by_login(email, Email)
-                or Email(login=email, password=email_password)) if email else None
+        if email:
+            email.strip()
+            email = (await self.get_row_by_login(email, Email)
+                     or Email(login=email, password=email_password))
         await self.add_record(
             Twitter(
-                login=login,
-                password=password,
+                login=login.strip() if login else login,
+                password=password.strip() if password else password,
                 auth_token=auth_token,
-                mail=mail
+                email=email
             )
         )
 
+    @prepare_values
     async def add_discord(
             self,
             auth_token: str,
             login: str = None,
             password: str = None,
             email_password: str = None
     ) -> None:
@@ -104,32 +127,36 @@
                 login=login,
                 password=password,
                 auth_token=auth_token,
                 email=email
             )
         )
 
+    @prepare_values
     async def add_proxy(self, proxy_string: str) -> None:
         logger.info(f'Adding Proxy {proxy_string}')
         await self.add_record(Proxy(proxy_string=proxy_string))
 
+    @prepare_values
     async def add_github(self, login: str, password: str, email_password: str = None):
         logger.info(f'Adding Github {login}')
         email = (await self.get_row_by_login(login=login, model=Email)) or Email(login=login, password=email_password)
         await self.add_record(Github(login=login, password=password, email=email))
 
+    @prepare_values
     async def add_profile(
             self,
             proxy_string: str,
             email: str,
             discord_login: str,
             twitter_login: str,
             evm_private: str,
             aptos_private: str,
             solana_private: str,
+            btc_mnemo: str,
             recipient: str,
             passphrase: str
     ) -> None:
         logger.info(f'Adding Profile {email}:{proxy_string}')
         mail = await self.get_row_by_login(email, Email)
         if not mail:
             logger.error(f'Need email {email}')
@@ -145,29 +172,38 @@
         proxy = await self.get_row_by_login(proxy_string, Proxy)
         if not proxy:
             logger.error(f'Need proxy {proxy_string}')
             return
         evm_account = EVMAccount.from_key(evm_private)
         aptos_account = AptosAccount.load_key(aptos_private)
         solana_keypair = Keypair.from_base58_string(solana_private)
+        btc_hdwallet = HDWallet(mnemonic=btc_mnemo)
+        btc_hdwallet.from_path("m/84'/0'/0'/0/0")
+        btc_native_segwit_address = btc_hdwallet.get_private_key().get_public_key().get_segwit_address().to_string()
+        btc_hdwallet.from_path("m/86'/0'/0'/0/0")
+        btc_taproot_address = btc_hdwallet.get_private_key().get_public_key().get_taproot_address().to_string()
+        btc_mnemo_encoded = encrypt(btc_mnemo, recipient, passphrase)
         evm_private_encoded = encrypt(evm_private, recipient, passphrase)
         aptos_private_encoded = encrypt(aptos_private, recipient, passphrase)
         solana_private_encoded = encrypt(solana_private, recipient, passphrase)
         await self.add_record(
             Profile(
                 proxy=proxy,
                 email=email,
                 discord=discord,
                 twitter=twitter,
                 evm_address=evm_account.address,
                 aptos_address=str(aptos_account.address()),
                 solana_address=str(solana_keypair.pubkey()),
+                btc_native_segwit_address=btc_native_segwit_address,
+                btc_taproot_address=btc_taproot_address,
                 evm_private=evm_private_encoded,
                 aptos_private=aptos_private_encoded,
-                solana_private=solana_private_encoded
+                solana_private=solana_private_encoded,
+                btc_mnemo=btc_mnemo_encoded
             )
         )
 
     async def edit(self, edited_model: ModelType | list) -> ModelType | None:
         if isinstance(edited_model, list):
             logger.info(f'Editing rows {[el.id for el in edited_model]} in "{edited_model[0].__tablename__}" table')
         else:
@@ -326,23 +362,34 @@
             limit: int = None
     ) -> list[Profile]:
         potential_profiles = await self.get_potential_profiles(limit)
         for i, profile in enumerate(potential_profiles):
             evm_account = EVMAccount.create()
             aptos_account = AptosAccount.generate()
             solana_keypair = Keypair()
+            btc_mnemo = Mnemonic().generate(256)
+            btc_hdwallet = HDWallet(mnemonic=btc_mnemo)
             profile.evm_private = encrypt(evm_account.key.hex(), recipient, passphrase)
             profile.evm_address = evm_account.address
             profile.aptos_private = encrypt(aptos_account.private_key.hex(), recipient, passphrase)
             profile.aptos_address = str(aptos_account.address())
             profile.solana_private = encrypt(
                 base58.b58encode(solana_keypair.secret() + bytes(solana_keypair.pubkey())).decode(),
                 recipient, passphrase
             )
             profile.solana_address = str(solana_keypair.pubkey())
+            profile.btc_mnemo = encrypt(btc_mnemo, recipient, passphrase)
+            btc_hdwallet.from_path("m/84'/0'/0'/0/0")
+            profile.btc_native_segwit_address = (
+                btc_hdwallet.get_private_key().get_public_key().get_segwit_address().to_string()
+            )
+            btc_hdwallet.from_path("m/86'/0'/0'/0/0")
+            profile.btc_taproot_address = (
+                btc_hdwallet.get_private_key().get_public_key().get_taproot_address().to_string()
+            )
         result = await self.add_record(potential_profiles)
         return result
 
     async def get_free_emails(self, limit: int = None) -> Sequence[Email]:
         logger.info(f'Getting free mails')
         subquery = (
             select(Twitter.email_id)
```

### Comparing `web3db-1.0.0/web3db/models/discord.py` & `web3db-1.0.1/web3db/models/discord.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.0/web3db/models/email.py` & `web3db-1.0.1/web3db/models/email.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.0/web3db/models/github.py` & `web3db-1.0.1/web3db/models/github.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.0/web3db/models/mixins.py` & `web3db-1.0.1/web3db/models/mixins.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.0/web3db/models/profile.py` & `web3db-1.0.1/web3db/models/profile.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,17 +27,20 @@
     _github_back_populates = 'profile'
     _email_id_nullable = True
 
     id: Mapped[int] = mapped_column(primary_key=True)
     evm_address: Mapped[str] = mapped_column(String, unique=True)
     aptos_address: Mapped[str] = mapped_column(String, unique=True)
     solana_address: Mapped[str] = mapped_column(String, unique=True)
+    btc_native_segwit_address: Mapped[str] = mapped_column(String, unique=True, nullable=True)
+    btc_taproot_address: Mapped[str] = mapped_column(String, unique=True, nullable=True)
     evm_private: Mapped[str] = mapped_column(String)
     aptos_private: Mapped[str] = mapped_column(String)
     solana_private: Mapped[str] = mapped_column(String)
+    btc_mnemo: Mapped[str] = mapped_column(String, nullable=True)
     okx_evm_address: Mapped[str] = mapped_column(String, nullable=True, unique=True)
     okx_aptos_address: Mapped[str] = mapped_column(String, nullable=True, unique=True)
     okx_solana_address: Mapped[str] = mapped_column(String, nullable=True, unique=True)
 
     def __repr__(self):
         return (
             f'{self.id}:{self.email.login if self.email else None}:{self.twitter.login if self.twitter else None}:'
```

### Comparing `web3db-1.0.0/web3db/models/proxy.py` & `web3db-1.0.1/web3db/models/proxy.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.0/web3db/models/twitter.py` & `web3db-1.0.1/web3db/models/twitter.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.0/web3db/utils/encrypt_private.py` & `web3db-1.0.1/web3db/utils/encrypt_private.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,39 @@
+import os
+
 import gnupg
 from eth_account import Account
 
 from .logger import logger
 from ..models import Profile
 
+from dotenv import load_dotenv
+
+load_dotenv()
+
 gpg = gnupg.GPG()
 gpg.encoding = 'utf-8'
 
+passphrase = os.getenv('PASSPHRASE')
+recipient = 'timerkhan2002@gmail.com'
+
 
-def encrypt(data: str, recipient: str, passphrase: str) -> str:
+def encrypt(data: str) -> str:
     status = gpg.encrypt(
         data=data,
         recipients=recipient,
         passphrase=passphrase,
         sign=recipient
     )
     logger.info(status.status)
     return status.data.decode('utf-8')
 
 
-def decrypt(encoded_data: str, passphrase: str, echo: bool = False) -> str:
+def decrypt(encoded_data: str, echo: bool = False) -> str:
     status = gpg.decrypt(encoded_data, passphrase=passphrase)
     if echo:
         logger.info(status.status)
     return status.data.decode('utf-8')
 
 
-def get_wallets(profiles: list[Profile], passphrase: str) -> list[Account]:
+def get_wallets(profiles: list[Profile]) -> list[Account]:
     return [Account.from_key(decrypt(profile.evm_private, passphrase)) for profile in profiles]
```

### Comparing `web3db-1.0.0/web3db/utils/logger.py` & `web3db-1.0.1/web3db/utils/logger.py`

 * *Files identical despite different names*

