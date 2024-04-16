# Comparing `tmp/stytch-9.1.0.tar.gz` & `tmp/stytch-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-9.1.0.tar", last modified: Thu Apr 11 14:35:33 2024, max compression
+gzip compressed data, was "stytch-9.2.0.tar", last modified: Tue Apr 16 01:46:52 2024, max compression
```

## Comparing `stytch-9.1.0.tar` & `stytch-9.2.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-11 14:35:20.000000 stytch-9.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-11 14:35:33.359014 stytch-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-11 14:35:20.000000 stytch-9.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 14:35:33.359014 stytch-9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-11 14:35:20.000000 stytch-9.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.339014 stytch-9.1.0/stytch/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.343014 stytch-9.1.0/stytch/b2b/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.347014 stytch-9.1.0/stytch/b2b/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31578 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    52376 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    54059 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/organizations_members_oauth_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)    26141 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    28071 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)    22956 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/scim.py
--rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/scim_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    44453 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.351014 stytch-9.1.0/stytch/b2b/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    19720 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/organizations_members_oauth_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/scim.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/scim_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/b2b/models/totps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.351014 stytch-9.1.0/stytch/consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.355014 stytch-9.1.0/stytch/consumer/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/m2m_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/m2m_clients_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    33050 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)    16939 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    17491 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    30883 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)    32914 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/api/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/stytch/consumer/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/m2m_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/m2m_clients_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/consumer/models/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/stytch/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/api_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/client_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/stytch/core/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/http/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/core/response_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/stytch/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/jwt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/lazy_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/method_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/policy_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/shared/rbac_local.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 14:35:20.000000 stytch-9.1.0/stytch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/stytch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-11 14:35:33.000000 stytch-9.1.0/stytch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-11 14:35:33.000000 stytch-9.1.0/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:35:33.000000 stytch-9.1.0/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 14:35:33.000000 stytch-9.1.0/stytch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 14:35:33.000000 stytch-9.1.0/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:35:33.359014 stytch-9.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-04-11 14:35:20.000000 stytch-9.1.0/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-04-11 14:35:20.000000 stytch-9.1.0/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.903933 stytch-9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-16 01:46:39.000000 stytch-9.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-16 01:46:52.903933 stytch-9.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-16 01:46:39.000000 stytch-9.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 01:46:52.903933 stytch-9.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-16 01:46:39.000000 stytch-9.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.883932 stytch-9.2.0/stytch/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.883932 stytch-9.2.0/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.891933 stytch-9.2.0/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31578 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52376 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54059 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/organizations_members_oauth_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26141 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28071 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22956 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/scim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/scim_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44531 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.895933 stytch-9.2.0/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/organizations_members_oauth_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/scim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/scim_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/b2b/models/totps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.895933 stytch-9.2.0/stytch/consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.899932 stytch-9.2.0/stytch/consumer/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/m2m_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/m2m_clients_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33050 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16939 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17491 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30883 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32914 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/api/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.899932 stytch-9.2.0/stytch/consumer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/m2m_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/m2m_clients_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/consumer/models/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.903933 stytch-9.2.0/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/core/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/core/client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.903933 stytch-9.2.0/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/core/response_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.903933 stytch-9.2.0/stytch/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/shared/jwt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/shared/lazy_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/shared/method_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/shared/policy_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/shared/rbac_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 01:46:39.000000 stytch-9.2.0/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.903933 stytch-9.2.0/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-16 01:46:52.000000 stytch-9.2.0/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-16 01:46:52.000000 stytch-9.2.0/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:46:52.000000 stytch-9.2.0/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 01:46:52.000000 stytch-9.2.0/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 01:46:52.000000 stytch-9.2.0/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:46:52.903933 stytch-9.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-04-16 01:46:39.000000 stytch-9.2.0/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-04-16 01:46:39.000000 stytch-9.2.0/test/test_integration_async.py
```

### Comparing `stytch-9.1.0/LICENSE.txt` & `stytch-9.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/PKG-INFO` & `stytch-9.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 9.1.0
+Version: 9.2.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-9.1.0/README.md` & `stytch-9.2.0/README.md`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/setup.py` & `stytch-9.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/discovery.py` & `stytch-9.2.0/stytch/b2b/api/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/discovery_intermediate_sessions.py` & `stytch-9.2.0/stytch/b2b/api/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/discovery_organizations.py` & `stytch-9.2.0/stytch/b2b/api/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/magic_links.py` & `stytch-9.2.0/stytch/b2b/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/magic_links_discovery.py` & `stytch-9.2.0/stytch/b2b/api/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/magic_links_email.py` & `stytch-9.2.0/stytch/b2b/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/magic_links_email_discovery.py` & `stytch-9.2.0/stytch/b2b/api/magic_links_email_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/oauth.py` & `stytch-9.2.0/stytch/b2b/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/oauth_discovery.py` & `stytch-9.2.0/stytch/b2b/api/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/organizations.py` & `stytch-9.2.0/stytch/b2b/api/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/organizations_members.py` & `stytch-9.2.0/stytch/b2b/api/organizations_members.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/organizations_members_oauth_providers.py` & `stytch-9.2.0/stytch/b2b/api/organizations_members_oauth_providers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/otp.py` & `stytch-9.2.0/stytch/b2b/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/otp_sms.py` & `stytch-9.2.0/stytch/b2b/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/passwords.py` & `stytch-9.2.0/stytch/b2b/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/passwords_email.py` & `stytch-9.2.0/stytch/b2b/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/passwords_existing_password.py` & `stytch-9.2.0/stytch/b2b/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/passwords_session.py` & `stytch-9.2.0/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/rbac.py` & `stytch-9.2.0/stytch/b2b/api/rbac.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/recovery_codes.py` & `stytch-9.2.0/stytch/b2b/api/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/scim.py` & `stytch-9.2.0/stytch/b2b/api/scim.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/scim_connections.py` & `stytch-9.2.0/stytch/b2b/api/scim_connections.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/sessions.py` & `stytch-9.2.0/stytch/b2b/api/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,15 +420,15 @@
     def migrate(
         self,
         session_token: str,
         organization_id: str,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> MigrateResponse:
-        """Migrate a session from an external endpoint. Stytch will call the UserInfo endpoint specified in your project settings, performing a lookup using the session token passed in. If the endpoint repsonds and the response contains a valid email, Stytch will attempt to match that email with a member in your organization, and create a Stytch Session for you.
+        """Migrate a session from an external OIDC compliant endpoint. Stytch will call the external UserInfo endpoint defined in your Stytch Project settings in the [Dashboard](/dashboard), and then perform a lookup using the `session_token`. If the response contains a valid email address, Stytch will attempt to match that email address with a Member in your Organization and create a Stytch Session.
 
         Fields:
           - session_token: The authorization token Stytch will pass in to the external userinfo endpoint.
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
@@ -461,15 +461,15 @@
     async def migrate_async(
         self,
         session_token: str,
         organization_id: str,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> MigrateResponse:
-        """Migrate a session from an external endpoint. Stytch will call the UserInfo endpoint specified in your project settings, performing a lookup using the session token passed in. If the endpoint repsonds and the response contains a valid email, Stytch will attempt to match that email with a member in your organization, and create a Stytch Session for you.
+        """Migrate a session from an external OIDC compliant endpoint. Stytch will call the external UserInfo endpoint defined in your Stytch Project settings in the [Dashboard](/dashboard), and then perform a lookup using the `session_token`. If the response contains a valid email address, Stytch will attempt to match that email address with a Member in your Organization and create a Stytch Session.
 
         Fields:
           - session_token: The authorization token Stytch will pass in to the external userinfo endpoint.
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
```

### Comparing `stytch-9.1.0/stytch/b2b/api/sso.py` & `stytch-9.2.0/stytch/b2b/api/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/sso_oidc.py` & `stytch-9.2.0/stytch/b2b/api/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/sso_saml.py` & `stytch-9.2.0/stytch/b2b/api/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/api/totps.py` & `stytch-9.2.0/stytch/b2b/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/client.py` & `stytch-9.2.0/stytch/b2b/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/discovery.py` & `stytch-9.2.0/stytch/b2b/models/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/discovery_intermediate_sessions.py` & `stytch-9.2.0/stytch/b2b/models/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/discovery_organizations.py` & `stytch-9.2.0/stytch/b2b/models/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/magic_links.py` & `stytch-9.2.0/stytch/b2b/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/magic_links_discovery.py` & `stytch-9.2.0/stytch/b2b/models/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/magic_links_email.py` & `stytch-9.2.0/stytch/b2b/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/mfa.py` & `stytch-9.2.0/stytch/b2b/models/mfa.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/oauth.py` & `stytch-9.2.0/stytch/b2b/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/oauth_discovery.py` & `stytch-9.2.0/stytch/b2b/models/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/organizations.py` & `stytch-9.2.0/stytch/b2b/models/organizations.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 
 class SearchQueryOperator(str, enum.Enum):
     OR = "OR"
     AND = "AND"
 
 
 class ActiveSCIMConnection(pydantic.BaseModel):
+    """
+    Fields:
+      - connection_id: The ID of the SCIM connection.
+      - display_name: A human-readable display name for the connection.
+      - bearer_token_last_four: (no documentation yet)
+      - bearer_token_expires_at: (no documentation yet)
+    """  # noqa
+
     connection_id: str
     display_name: str
     bearer_token_last_four: str
     bearer_token_expires_at: Optional[datetime.datetime] = None
 
 
 class ActiveSSOConnection(pydantic.BaseModel):
@@ -179,15 +187,15 @@
 
       `RESTRICTED` – only new Members with SSO logins that comply with `sso_jit_provisioning_allowed_connections` can be provisioned upon authentication.
 
       `NOT_ALLOWED` – disable JIT provisioning via SSO.
 
       - sso_jit_provisioning_allowed_connections: An array of `connection_id`s that reference [SAML Connection objects](https://stytch.com/docs/b2b/api/saml-connection-object).
       Only these connections will be allowed to JIT provision Members via SSO when `sso_jit_provisioning` is set to `RESTRICTED`.
-      - sso_active_connections: An array of active [SAML Connection references](https://stytch.com/docs/b2b/api/saml-connection-object).
+      - sso_active_connections: An array of active [SAML Connection references](https://stytch.com/docs/b2b/api/saml-connection-object) or [OIDC Connection references](https://stytch.com/docs/b2b/api/oidc-connection-object).
       - email_allowed_domains: An array of email domains that allow invites or JIT provisioning for new Members. This list is enforced when either `email_invites` or `email_jit_provisioning` is set to `RESTRICTED`.
 
 
         Common domains such as `gmail.com` are not allowed. See the [common email domains resource](https://stytch.com/docs/b2b/api/common-email-domains) for the full list.
       - email_jit_provisioning: The authentication setting that controls how a new Member can be provisioned by authenticating via Email Magic Link or OAuth. The accepted values are:
 
       `RESTRICTED` – only new Members with verified emails that comply with `email_allowed_domains` can be provisioned upon authentication via Email Magic Link or OAuth.
@@ -221,15 +229,15 @@
       `ALL_ALLOWED` – the default setting which allows all authentication methods to be used.
 
       `RESTRICTED` – only methods that comply with `allowed_mfa_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
       - allowed_mfa_methods: An array of allowed MFA authentication methods. This list is enforced when `mfa_methods` is set to `RESTRICTED`.
       The list's accepted values are: `sms_otp` and `totp`.
 
-      - scim_active_connections: (no documentation yet)
+      - scim_active_connections: An array of active [SCIM Connection references](https://stytch.com/docs/b2b/api/scim-connection-object).
       - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
       - sso_default_connection_id: The default connection used for SSO when there are multiple active connections.
     """  # noqa
 
     organization_id: str
     organization_name: str
     organization_logo_url: str
@@ -258,14 +266,29 @@
       - next_cursor: The `next_cursor` string is returned when your search result contains more than one page of results. This value is passed into your next search call in the `cursor` field.
     """  # noqa
 
     total: int
     next_cursor: Optional[str] = None
 
 
+class SCIMRegistration(pydantic.BaseModel):
+    """
+    Fields:
+      - connection_id: The ID of the SCIM connection.
+      - registration_id: The unique ID of a SCIM Registration.
+      - external_id: The ID of the member given by the identity provider.
+      - scim_attributes: An object for storing SCIM attributes brought over from the identity provider.
+    """  # noqa
+
+    connection_id: str
+    registration_id: str
+    external_id: Optional[str] = None
+    scim_attributes: Optional[Dict[str, Any]] = None
+
+
 class SSORegistration(pydantic.BaseModel):
     """
     Fields:
       - connection_id: Globally unique UUID that identifies a specific SSO `connection_id` for a Member.
       - external_id: The ID of the member given by the identity provider.
       - registration_id: The unique ID of an SSO Registration.
       - sso_attributes: An object for storing SSO attributes brought over from the identity provider.
@@ -281,24 +304,25 @@
     """
     Fields:
       - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
       - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
       - email_address: The email address of the Member.
       - status: The status of the Member. The possible values are: `pending`, `invited`, `active`, or `deleted`.
       - name: The name of the Member.
-      - sso_registrations: An array of registered [SAML Connection](saml-connection-object) objects the Member has authenticated with.
+      - sso_registrations: An array of registered [SAML Connection](saml-connection-object) or [OIDC Connection](oidc-connection-object) objects the Member has authenticated with.
       - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
       - member_password_id: Globally unique UUID that identifies a Member's password.
       - oauth_registrations: A list of OAuth registrations for this member.
       - email_address_verified: Whether or not the Member's email address is verified.
       - mfa_phone_number_verified: Whether or not the Member's phone number is verified.
       - is_admin: Whether or not the Member has the `stytch_admin` Role. This Role is automatically granted to Members
       who create an Organization through the [discovery flow](https://stytch.com/docs/b2b/api/create-organization-via-discovery). See the
       [RBAC guide](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for more details on this Role.
       - totp_registration_id: (no documentation yet)
+      - scim_registrations: An array of scim member registrations, each one referencing a [SCIM Connection](scim-connection-object) object in use for the Member creation.
       - mfa_enrolled: Sets whether the Member is enrolled in MFA. If true, the Member must complete an MFA step whenever they wish to log in to their Organization. If false, the Member only needs to complete an MFA step if the Organization's MFA policy is set to `REQUIRED_FOR_ALL`.
       - mfa_phone_number: The Member's phone number. A Member may only have one phone number.
       - default_mfa_method: (no documentation yet)
       - roles: Explicit or implicit Roles assigned to this Member, along with details about the role assignment source.
        See the [RBAC guide](https://stytch.com/docs/b2b/guides/rbac/role-assignment) for more information about role assignment.
       - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
       - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
@@ -315,14 +339,15 @@
     is_breakglass: bool
     member_password_id: str
     oauth_registrations: List[OAuthRegistration]
     email_address_verified: bool
     mfa_phone_number_verified: bool
     is_admin: bool
     totp_registration_id: str
+    scim_registrations: List[SCIMRegistration]
     mfa_enrolled: bool
     mfa_phone_number: str
     default_mfa_method: str
     roles: List[MemberRole]
     trusted_metadata: Optional[Dict[str, Any]] = None
     untrusted_metadata: Optional[Dict[str, Any]] = None
```

### Comparing `stytch-9.1.0/stytch/b2b/models/organizations_members.py` & `stytch-9.2.0/stytch/b2b/models/organizations_members.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/organizations_members_oauth_providers.py` & `stytch-9.2.0/stytch/b2b/models/organizations_members_oauth_providers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/otp_sms.py` & `stytch-9.2.0/stytch/b2b/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/passwords.py` & `stytch-9.2.0/stytch/b2b/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/passwords_email.py` & `stytch-9.2.0/stytch/b2b/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/passwords_existing_password.py` & `stytch-9.2.0/stytch/b2b/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/passwords_session.py` & `stytch-9.2.0/stytch/b2b/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/rbac.py` & `stytch-9.2.0/stytch/b2b/models/rbac.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/recovery_codes.py` & `stytch-9.2.0/stytch/b2b/models/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/scim.py` & `stytch-9.2.0/stytch/b2b/models/scim.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/scim_connections.py` & `stytch-9.2.0/stytch/b2b/models/scim_connections.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/sessions.py` & `stytch-9.2.0/stytch/b2b/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/sso.py` & `stytch-9.2.0/stytch/b2b/models/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/sso_oidc.py` & `stytch-9.2.0/stytch/b2b/models/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/sso_saml.py` & `stytch-9.2.0/stytch/b2b/models/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/b2b/models/totps.py` & `stytch-9.2.0/stytch/b2b/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/crypto_wallets.py` & `stytch-9.2.0/stytch/consumer/api/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/m2m.py` & `stytch-9.2.0/stytch/consumer/api/m2m.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/m2m_clients.py` & `stytch-9.2.0/stytch/consumer/api/m2m_clients.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/m2m_clients_secrets.py` & `stytch-9.2.0/stytch/consumer/api/m2m_clients_secrets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/magic_links.py` & `stytch-9.2.0/stytch/consumer/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/magic_links_email.py` & `stytch-9.2.0/stytch/consumer/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/oauth.py` & `stytch-9.2.0/stytch/consumer/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/otp.py` & `stytch-9.2.0/stytch/consumer/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/otp_email.py` & `stytch-9.2.0/stytch/consumer/api/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/otp_sms.py` & `stytch-9.2.0/stytch/consumer/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/otp_whatsapp.py` & `stytch-9.2.0/stytch/consumer/api/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/passwords.py` & `stytch-9.2.0/stytch/consumer/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/passwords_email.py` & `stytch-9.2.0/stytch/consumer/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/passwords_existing_password.py` & `stytch-9.2.0/stytch/consumer/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/passwords_session.py` & `stytch-9.2.0/stytch/consumer/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/project.py` & `stytch-9.2.0/stytch/consumer/api/project.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/sessions.py` & `stytch-9.2.0/stytch/consumer/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/totps.py` & `stytch-9.2.0/stytch/consumer/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/users.py` & `stytch-9.2.0/stytch/consumer/api/users.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/api/webauthn.py` & `stytch-9.2.0/stytch/consumer/api/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/client.py` & `stytch-9.2.0/stytch/consumer/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/crypto_wallets.py` & `stytch-9.2.0/stytch/consumer/models/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/m2m.py` & `stytch-9.2.0/stytch/consumer/models/m2m.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/m2m_clients.py` & `stytch-9.2.0/stytch/consumer/models/m2m_clients.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/m2m_clients_secrets.py` & `stytch-9.2.0/stytch/consumer/models/m2m_clients_secrets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/magic_links.py` & `stytch-9.2.0/stytch/consumer/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/magic_links_email.py` & `stytch-9.2.0/stytch/consumer/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/oauth.py` & `stytch-9.2.0/stytch/consumer/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/otp.py` & `stytch-9.2.0/stytch/consumer/models/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/otp_email.py` & `stytch-9.2.0/stytch/consumer/models/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/otp_sms.py` & `stytch-9.2.0/stytch/consumer/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/otp_whatsapp.py` & `stytch-9.2.0/stytch/consumer/models/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/passwords.py` & `stytch-9.2.0/stytch/consumer/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/passwords_email.py` & `stytch-9.2.0/stytch/consumer/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/passwords_existing_password.py` & `stytch-9.2.0/stytch/consumer/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/passwords_session.py` & `stytch-9.2.0/stytch/consumer/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/project.py` & `stytch-9.2.0/stytch/consumer/models/project.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/sessions.py` & `stytch-9.2.0/stytch/consumer/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/totps.py` & `stytch-9.2.0/stytch/consumer/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/users.py` & `stytch-9.2.0/stytch/consumer/models/users.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/consumer/models/webauthn.py` & `stytch-9.2.0/stytch/consumer/models/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/core/api_base.py` & `stytch-9.2.0/stytch/core/api_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/core/client_base.py` & `stytch-9.2.0/stytch/core/client_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/core/http/client.py` & `stytch-9.2.0/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/core/response_base.py` & `stytch-9.2.0/stytch/core/response_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/shared/jwt_helpers.py` & `stytch-9.2.0/stytch/shared/jwt_helpers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/shared/lazy_cache.py` & `stytch-9.2.0/stytch/shared/lazy_cache.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/shared/method_options.py` & `stytch-9.2.0/stytch/shared/method_options.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/shared/policy_cache.py` & `stytch-9.2.0/stytch/shared/policy_cache.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch/shared/rbac_local.py` & `stytch-9.2.0/stytch/shared/rbac_local.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/stytch.egg-info/PKG-INFO` & `stytch-9.2.0/stytch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 9.1.0
+Version: 9.2.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-9.1.0/stytch.egg-info/SOURCES.txt` & `stytch-9.2.0/stytch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/test/test_integration.py` & `stytch-9.2.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-9.1.0/test/test_integration_async.py` & `stytch-9.2.0/test/test_integration_async.py`

 * *Files identical despite different names*

