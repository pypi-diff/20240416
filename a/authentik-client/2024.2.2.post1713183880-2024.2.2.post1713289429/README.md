# Comparing `tmp/authentik_client-2024.2.2.post1713183880.tar.gz` & `tmp/authentik_client-2024.2.2.post1713289429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentik_client-2024.2.2.post1713183880.tar", max compression
+gzip compressed data, was "authentik_client-2024.2.2.post1713289429.tar", max compression
```

## Comparing `authentik_client-2024.2.2.post1713183880.tar` & `authentik_client-2024.2.2.post1713289429.tar`

### file list

```diff
@@ -1,594 +1,594 @@
--rw-r--r--   0        0        0   143895 2024-04-15 12:24:52.941899 authentik_client-2024.2.2.post1713183880/README.md
--rw-r--r--   0        0        0    48410 2024-04-15 12:24:52.949899 authentik_client-2024.2.2.post1713183880/authentik_client/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-15 12:24:52.953899 authentik_client-2024.2.2.post1713183880/authentik_client/api/__init__.py
--rw-r--r--   0        0        0    97518 2024-04-15 12:24:52.625901 authentik_client-2024.2.2.post1713183880/authentik_client/api/admin_api.py
--rw-r--r--   0        0        0   700271 2024-04-15 12:24:52.649901 authentik_client-2024.2.2.post1713183880/authentik_client/api/authenticators_api.py
--rw-r--r--   0        0        0   701197 2024-04-15 12:24:52.673901 authentik_client-2024.2.2.post1713183880/authentik_client/api/core_api.py
--rw-r--r--   0        0        0   116805 2024-04-15 12:24:52.689900 authentik_client-2024.2.2.post1713183880/authentik_client/api/crypto_api.py
--rw-r--r--   0        0        0   107946 2024-04-15 12:24:52.697900 authentik_client-2024.2.2.post1713183880/authentik_client/api/enterprise_api.py
--rw-r--r--   0        0        0   408008 2024-04-15 12:24:52.709900 authentik_client-2024.2.2.post1713183880/authentik_client/api/events_api.py
--rw-r--r--   0        0        0   280806 2024-04-15 12:24:52.721900 authentik_client-2024.2.2.post1713183880/authentik_client/api/flows_api.py
--rw-r--r--   0        0        0   101134 2024-04-15 12:24:52.729900 authentik_client-2024.2.2.post1713183880/authentik_client/api/managed_api.py
--rw-r--r--   0        0        0   135649 2024-04-15 12:24:52.737900 authentik_client-2024.2.2.post1713183880/authentik_client/api/oauth2_api.py
--rw-r--r--   0        0        0   413301 2024-04-15 12:24:52.749900 authentik_client-2024.2.2.post1713183880/authentik_client/api/outposts_api.py
--rw-r--r--   0        0        0   725201 2024-04-15 12:24:52.769900 authentik_client-2024.2.2.post1713183880/authentik_client/api/policies_api.py
--rw-r--r--   0        0        0   552586 2024-04-15 12:24:52.789900 authentik_client-2024.2.2.post1713183880/authentik_client/api/propertymappings_api.py
--rw-r--r--   0        0        0   718066 2024-04-15 12:24:52.809900 authentik_client-2024.2.2.post1713183880/authentik_client/api/providers_api.py
--rw-r--r--   0        0        0   150485 2024-04-15 12:24:52.821900 authentik_client-2024.2.2.post1713183880/authentik_client/api/rac_api.py
--rw-r--r--   0        0        0   207550 2024-04-15 12:24:52.833900 authentik_client-2024.2.2.post1713183880/authentik_client/api/rbac_api.py
--rw-r--r--   0        0        0    10391 2024-04-15 12:24:52.837900 authentik_client-2024.2.2.post1713183880/authentik_client/api/root_api.py
--rw-r--r--   0        0        0    11845 2024-04-15 12:24:52.845900 authentik_client-2024.2.2.post1713183880/authentik_client/api/schema_api.py
--rw-r--r--   0        0        0  1037225 2024-04-15 12:24:52.865899 authentik_client-2024.2.2.post1713183880/authentik_client/api/sources_api.py
--rw-r--r--   0        0        0  1945986 2024-04-15 12:24:52.909899 authentik_client-2024.2.2.post1713183880/authentik_client/api/stages_api.py
--rw-r--r--   0        0        0   157909 2024-04-15 12:24:52.929899 authentik_client-2024.2.2.post1713183880/authentik_client/api/tenants_api.py
--rw-r--r--   0        0        0    25779 2024-04-15 12:24:52.953899 authentik_client-2024.2.2.post1713183880/authentik_client/api_client.py
--rw-r--r--   0        0        0      652 2024-04-15 12:24:52.957899 authentik_client-2024.2.2.post1713183880/authentik_client/api_response.py
--rw-r--r--   0        0        0    14724 2024-04-15 12:24:52.949899 authentik_client-2024.2.2.post1713183880/authentik_client/configuration.py
--rw-r--r--   0        0        0     5934 2024-04-15 12:24:52.953899 authentik_client-2024.2.2.post1713183880/authentik_client/exceptions.py
--rw-r--r--   0        0        0    46712 2024-04-15 12:24:52.953899 authentik_client-2024.2.2.post1713183880/authentik_client/models/__init__.py
--rw-r--r--   0        0        0     4513 2024-04-15 12:24:49.585919 authentik_client-2024.2.2.post1713183880/authentik_client/models/access_denied_challenge.py
--rw-r--r--   0        0        0     2482 2024-04-15 12:24:49.601919 authentik_client-2024.2.2.post1713183880/authentik_client/models/app.py
--rw-r--r--   0        0        0     4230 2024-04-15 12:24:49.605919 authentik_client-2024.2.2.post1713183880/authentik_client/models/app_enum.py
--rw-r--r--   0        0        0     2702 2024-04-15 12:24:49.617919 authentik_client-2024.2.2.post1713183880/authentik_client/models/apple_challenge_response_request.py
--rw-r--r--   0        0        0     4508 2024-04-15 12:24:49.629919 authentik_client-2024.2.2.post1713183880/authentik_client/models/apple_login_challenge.py
--rw-r--r--   0        0        0     6686 2024-04-15 12:24:49.637919 authentik_client-2024.2.2.post1713183880/authentik_client/models/application.py
--rw-r--r--   0        0        0     4473 2024-04-15 12:24:49.645919 authentik_client-2024.2.2.post1713183880/authentik_client/models/application_request.py
--rw-r--r--   0        0        0      711 2024-04-15 12:24:49.649919 authentik_client-2024.2.2.post1713183880/authentik_client/models/auth_mode_enum.py
--rw-r--r--   0        0        0      709 2024-04-15 12:24:49.653919 authentik_client-2024.2.2.post1713183880/authentik_client/models/auth_type_enum.py
--rw-r--r--   0        0        0     5195 2024-04-15 12:24:49.661918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session.py
--rw-r--r--   0        0        0     3064 2024-04-15 12:24:49.665919 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_asn.py
--rw-r--r--   0        0        0     2826 2024-04-15 12:24:49.673919 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_geo_ip.py
--rw-r--r--   0        0        0     3865 2024-04-15 12:24:49.677919 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_user_agent.py
--rw-r--r--   0        0        0     2646 2024-04-15 12:24:49.685918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_user_agent_device.py
--rw-r--r--   0        0        0     2792 2024-04-15 12:24:49.689918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_user_agent_os.py
--rw-r--r--   0        0        0     2725 2024-04-15 12:24:49.697919 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_user_agent_user_agent.py
--rw-r--r--   0        0        0      895 2024-04-15 12:24:49.701918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authentication_enum.py
--rw-r--r--   0        0        0      782 2024-04-15 12:24:49.705918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_attachment_enum.py
--rw-r--r--   0        0        0     4686 2024-04-15 12:24:49.709918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_challenge.py
--rw-r--r--   0        0        0     2743 2024-04-15 12:24:49.713918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_challenge_response_request.py
--rw-r--r--   0        0        0     5327 2024-04-15 12:24:49.721918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_stage.py
--rw-r--r--   0        0        0     2768 2024-04-15 12:24:49.725918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_stage_device_import_response.py
--rw-r--r--   0        0        0     2785 2024-04-15 12:24:49.729918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
--rw-r--r--   0        0        0     4744 2024-04-15 12:24:49.737918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-15 12:24:49.741918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_sms_challenge.py
--rw-r--r--   0        0        0     3022 2024-04-15 12:24:49.749918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_sms_challenge_response_request.py
--rw-r--r--   0        0        0     6409 2024-04-15 12:24:49.753918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_sms_stage.py
--rw-r--r--   0        0        0     5595 2024-04-15 12:24:49.761918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4474 2024-04-15 12:24:49.765918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_static_challenge.py
--rw-r--r--   0        0        0     2761 2024-04-15 12:24:49.773918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_static_challenge_response_request.py
--rw-r--r--   0        0        0     5363 2024-04-15 12:24:49.777918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_static_stage.py
--rw-r--r--   0        0        0     4392 2024-04-15 12:24:49.781918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4468 2024-04-15 12:24:49.789918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_totp_challenge.py
--rw-r--r--   0        0        0     2858 2024-04-15 12:24:49.793918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_totp_challenge_response_request.py
--rw-r--r--   0        0        0     5132 2024-04-15 12:24:49.797918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_totp_stage.py
--rw-r--r--   0        0        0     4201 2024-04-15 12:24:49.805918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     6722 2024-04-15 12:24:49.809918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_validate_stage.py
--rw-r--r--   0        0        0     4893 2024-04-15 12:24:49.813918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5717 2024-04-15 12:24:49.821918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_validation_challenge.py
--rw-r--r--   0        0        0     3805 2024-04-15 12:24:49.825918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_validation_challenge_response_request.py
--rw-r--r--   0        0        0     4499 2024-04-15 12:24:49.833918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_web_authn_challenge.py
--rw-r--r--   0        0        0     2852 2024-04-15 12:24:49.837918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_web_authn_challenge_response_request.py
--rw-r--r--   0        0        0     7081 2024-04-15 12:24:49.841918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_web_authn_stage.py
--rw-r--r--   0        0        0     5302 2024-04-15 12:24:49.845918 authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     2718 2024-04-15 12:24:49.849918 authentik_client-2024.2.2.post1713183880/authentik_client/models/auto_submit_challenge_response_request.py
--rw-r--r--   0        0        0     4388 2024-04-15 12:24:49.857917 authentik_client-2024.2.2.post1713183880/authentik_client/models/autosubmit_challenge.py
--rw-r--r--   0        0        0      950 2024-04-15 12:24:49.861917 authentik_client-2024.2.2.post1713183880/authentik_client/models/backends_enum.py
--rw-r--r--   0        0        0      748 2024-04-15 12:24:49.861917 authentik_client-2024.2.2.post1713183880/authentik_client/models/binding_type_enum.py
--rw-r--r--   0        0        0     2995 2024-04-15 12:24:49.865918 authentik_client-2024.2.2.post1713183880/authentik_client/models/blueprint_file.py
--rw-r--r--   0        0        0     4453 2024-04-15 12:24:49.869917 authentik_client-2024.2.2.post1713183880/authentik_client/models/blueprint_instance.py
--rw-r--r--   0        0        0     3208 2024-04-15 12:24:49.873917 authentik_client-2024.2.2.post1713183880/authentik_client/models/blueprint_instance_request.py
--rw-r--r--   0        0        0      836 2024-04-15 12:24:49.877917 authentik_client-2024.2.2.post1713183880/authentik_client/models/blueprint_instance_status_enum.py
--rw-r--r--   0        0        0     6255 2024-04-15 12:24:49.877917 authentik_client-2024.2.2.post1713183880/authentik_client/models/brand.py
--rw-r--r--   0        0        0     6307 2024-04-15 12:24:49.885917 authentik_client-2024.2.2.post1713183880/authentik_client/models/brand_request.py
--rw-r--r--   0        0        0     2501 2024-04-15 12:24:49.889917 authentik_client-2024.2.2.post1713183880/authentik_client/models/cache.py
--rw-r--r--   0        0        0      875 2024-04-15 12:24:49.893917 authentik_client-2024.2.2.post1713183880/authentik_client/models/capabilities_enum.py
--rw-r--r--   0        0        0     4476 2024-04-15 12:24:49.897917 authentik_client-2024.2.2.post1713183880/authentik_client/models/captcha_challenge.py
--rw-r--r--   0        0        0     2797 2024-04-15 12:24:49.901917 authentik_client-2024.2.2.post1713183880/authentik_client/models/captcha_challenge_response_request.py
--rw-r--r--   0        0        0     4438 2024-04-15 12:24:49.905917 authentik_client-2024.2.2.post1713183880/authentik_client/models/captcha_stage.py
--rw-r--r--   0        0        0     3774 2024-04-15 12:24:49.909917 authentik_client-2024.2.2.post1713183880/authentik_client/models/captcha_stage_request.py
--rw-r--r--   0        0        0     2522 2024-04-15 12:24:49.913917 authentik_client-2024.2.2.post1713183880/authentik_client/models/certificate_data.py
--rw-r--r--   0        0        0     2861 2024-04-15 12:24:49.917917 authentik_client-2024.2.2.post1713183880/authentik_client/models/certificate_generation_request.py
--rw-r--r--   0        0        0     6655 2024-04-15 12:24:49.921917 authentik_client-2024.2.2.post1713183880/authentik_client/models/certificate_key_pair.py
--rw-r--r--   0        0        0     2989 2024-04-15 12:24:49.925917 authentik_client-2024.2.2.post1713183880/authentik_client/models/certificate_key_pair_request.py
--rw-r--r--   0        0        0      747 2024-04-15 12:24:49.929917 authentik_client-2024.2.2.post1713183880/authentik_client/models/challenge_choices.py
--rw-r--r--   0        0        0    24236 2024-04-15 12:24:49.937917 authentik_client-2024.2.2.post1713183880/authentik_client/models/challenge_types.py
--rw-r--r--   0        0        0      729 2024-04-15 12:24:49.941917 authentik_client-2024.2.2.post1713183880/authentik_client/models/client_type_enum.py
--rw-r--r--   0        0        0     3539 2024-04-15 12:24:49.945917 authentik_client-2024.2.2.post1713183880/authentik_client/models/config.py
--rw-r--r--   0        0        0     4021 2024-04-15 12:24:49.949917 authentik_client-2024.2.2.post1713183880/authentik_client/models/connection_token.py
--rw-r--r--   0        0        0     2662 2024-04-15 12:24:49.953917 authentik_client-2024.2.2.post1713183880/authentik_client/models/connection_token_request.py
--rw-r--r--   0        0        0     5736 2024-04-15 12:24:49.957917 authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_challenge.py
--rw-r--r--   0        0        0     2838 2024-04-15 12:24:49.961917 authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_challenge_response_request.py
--rw-r--r--   0        0        0     2513 2024-04-15 12:24:49.965917 authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_permission.py
--rw-r--r--   0        0        0     4511 2024-04-15 12:24:49.969917 authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_stage.py
--rw-r--r--   0        0        0      783 2024-04-15 12:24:49.969917 authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_stage_mode_enum.py
--rw-r--r--   0        0        0     3569 2024-04-15 12:24:49.973917 authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_stage_request.py
--rw-r--r--   0        0        0     2891 2024-04-15 12:24:49.977917 authentik_client-2024.2.2.post1713183880/authentik_client/models/contextual_flow_info.py
--rw-r--r--   0        0        0      879 2024-04-15 12:24:49.981917 authentik_client-2024.2.2.post1713183880/authentik_client/models/contextual_flow_info_layout_enum.py
--rw-r--r--   0        0        0     2657 2024-04-15 12:24:49.985917 authentik_client-2024.2.2.post1713183880/authentik_client/models/coordinate.py
--rw-r--r--   0        0        0     4704 2024-04-15 12:24:49.989917 authentik_client-2024.2.2.post1713183880/authentik_client/models/current_brand.py
--rw-r--r--   0        0        0      771 2024-04-15 12:24:49.989917 authentik_client-2024.2.2.post1713183880/authentik_client/models/denied_action_enum.py
--rw-r--r--   0        0        0     4200 2024-04-15 12:24:49.993917 authentik_client-2024.2.2.post1713183880/authentik_client/models/deny_stage.py
--rw-r--r--   0        0        0     3230 2024-04-15 12:24:49.997917 authentik_client-2024.2.2.post1713183880/authentik_client/models/deny_stage_request.py
--rw-r--r--   0        0        0     3522 2024-04-15 12:24:50.001917 authentik_client-2024.2.2.post1713183880/authentik_client/models/device.py
--rw-r--r--   0        0        0     2657 2024-04-15 12:24:50.009917 authentik_client-2024.2.2.post1713183880/authentik_client/models/device_challenge.py
--rw-r--r--   0        0        0     2792 2024-04-15 12:24:50.013917 authentik_client-2024.2.2.post1713183880/authentik_client/models/device_challenge_request.py
--rw-r--r--   0        0        0      780 2024-04-15 12:24:50.017917 authentik_client-2024.2.2.post1713183880/authentik_client/models/device_classes_enum.py
--rw-r--r--   0        0        0     1244 2024-04-15 12:24:50.021916 authentik_client-2024.2.2.post1713183880/authentik_client/models/digest_algorithm_enum.py
--rw-r--r--   0        0        0      695 2024-04-15 12:24:50.021916 authentik_client-2024.2.2.post1713183880/authentik_client/models/digits_enum.py
--rw-r--r--   0        0        0     4969 2024-04-15 12:24:50.025916 authentik_client-2024.2.2.post1713183880/authentik_client/models/docker_service_connection.py
--rw-r--r--   0        0        0     4087 2024-04-15 12:24:50.029916 authentik_client-2024.2.2.post1713183880/authentik_client/models/docker_service_connection_request.py
--rw-r--r--   0        0        0     2847 2024-04-15 12:24:50.033917 authentik_client-2024.2.2.post1713183880/authentik_client/models/domain.py
--rw-r--r--   0        0        0     2746 2024-04-15 12:24:50.037917 authentik_client-2024.2.2.post1713183880/authentik_client/models/domain_request.py
--rw-r--r--   0        0        0     4155 2024-04-15 12:24:50.041916 authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_challenge.py
--rw-r--r--   0        0        0     2681 2024-04-15 12:24:50.045916 authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_challenge_response_request.py
--rw-r--r--   0        0        0     4515 2024-04-15 12:24:50.053916 authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_policy.py
--rw-r--r--   0        0        0     3237 2024-04-15 12:24:50.057916 authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_policy_request.py
--rw-r--r--   0        0        0     4213 2024-04-15 12:24:50.061916 authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_stage.py
--rw-r--r--   0        0        0     3232 2024-04-15 12:24:50.065916 authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_stage_request.py
--rw-r--r--   0        0        0     2720 2024-04-15 12:24:50.069916 authentik_client-2024.2.2.post1713183880/authentik_client/models/duo_device.py
--rw-r--r--   0        0        0     2575 2024-04-15 12:24:50.069916 authentik_client-2024.2.2.post1713183880/authentik_client/models/duo_device_enrollment_status.py
--rw-r--r--   0        0        0     2619 2024-04-15 12:24:50.073916 authentik_client-2024.2.2.post1713183880/authentik_client/models/duo_device_request.py
--rw-r--r--   0        0        0      748 2024-04-15 12:24:50.077916 authentik_client-2024.2.2.post1713183880/authentik_client/models/duo_response_enum.py
--rw-r--r--   0        0        0     4090 2024-04-15 12:24:50.081916 authentik_client-2024.2.2.post1713183880/authentik_client/models/email_challenge.py
--rw-r--r--   0        0        0     2770 2024-04-15 12:24:50.085916 authentik_client-2024.2.2.post1713183880/authentik_client/models/email_challenge_response_request.py
--rw-r--r--   0        0        0     5902 2024-04-15 12:24:50.093916 authentik_client-2024.2.2.post1713183880/authentik_client/models/email_stage.py
--rw-r--r--   0        0        0     5121 2024-04-15 12:24:50.101916 authentik_client-2024.2.2.post1713183880/authentik_client/models/email_stage_request.py
--rw-r--r--   0        0        0     4707 2024-04-15 12:24:50.109916 authentik_client-2024.2.2.post1713183880/authentik_client/models/endpoint.py
--rw-r--r--   0        0        0     3678 2024-04-15 12:24:50.113916 authentik_client-2024.2.2.post1713183880/authentik_client/models/endpoint_request.py
--rw-r--r--   0        0        0     2530 2024-04-15 12:24:50.117916 authentik_client-2024.2.2.post1713183880/authentik_client/models/error_detail.py
--rw-r--r--   0        0        0     3309 2024-04-15 12:24:50.121916 authentik_client-2024.2.2.post1713183880/authentik_client/models/error_reporting_config.py
--rw-r--r--   0        0        0     4129 2024-04-15 12:24:50.125916 authentik_client-2024.2.2.post1713183880/authentik_client/models/event.py
--rw-r--r--   0        0        0     1730 2024-04-15 12:24:50.129916 authentik_client-2024.2.2.post1713183880/authentik_client/models/event_actions.py
--rw-r--r--   0        0        0     6006 2024-04-15 12:24:50.133916 authentik_client-2024.2.2.post1713183880/authentik_client/models/event_matcher_policy.py
--rw-r--r--   0        0        0     4807 2024-04-15 12:24:50.145916 authentik_client-2024.2.2.post1713183880/authentik_client/models/event_matcher_policy_request.py
--rw-r--r--   0        0        0     3990 2024-04-15 12:24:50.149916 authentik_client-2024.2.2.post1713183880/authentik_client/models/event_request.py
--rw-r--r--   0        0        0     2697 2024-04-15 12:24:50.153916 authentik_client-2024.2.2.post1713183880/authentik_client/models/event_top_per_user.py
--rw-r--r--   0        0        0     3926 2024-04-15 12:24:50.157916 authentik_client-2024.2.2.post1713183880/authentik_client/models/expiring_base_grant_model.py
--rw-r--r--   0        0        0     4191 2024-04-15 12:24:50.161916 authentik_client-2024.2.2.post1713183880/authentik_client/models/expression_policy.py
--rw-r--r--   0        0        0     2992 2024-04-15 12:24:50.165916 authentik_client-2024.2.2.post1713183880/authentik_client/models/expression_policy_request.py
--rw-r--r--   0        0        0     4524 2024-04-15 12:24:50.169916 authentik_client-2024.2.2.post1713183880/authentik_client/models/extra_role_object_permission.py
--rw-r--r--   0        0        0     4524 2024-04-15 12:24:50.173916 authentik_client-2024.2.2.post1713183880/authentik_client/models/extra_user_object_permission.py
--rw-r--r--   0        0        0     2519 2024-04-15 12:24:50.177916 authentik_client-2024.2.2.post1713183880/authentik_client/models/file_path_request.py
--rw-r--r--   0        0        0     6047 2024-04-15 12:24:50.185916 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow.py
--rw-r--r--   0        0        0    25850 2024-04-15 12:24:50.193915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_challenge_response_request.py
--rw-r--r--   0        0        0      934 2024-04-15 12:24:50.193915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_designation_enum.py
--rw-r--r--   0        0        0     2533 2024-04-15 12:24:50.197915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_diagram.py
--rw-r--r--   0        0        0     4505 2024-04-15 12:24:50.205916 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_error_challenge.py
--rw-r--r--   0        0        0     3111 2024-04-15 12:24:50.209915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_import_result.py
--rw-r--r--   0        0        0     3418 2024-04-15 12:24:50.213915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_inspection.py
--rw-r--r--   0        0        0     3875 2024-04-15 12:24:50.217915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_inspector_plan.py
--rw-r--r--   0        0        0      837 2024-04-15 12:24:50.221915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_layout_enum.py
--rw-r--r--   0        0        0     4741 2024-04-15 12:24:50.225915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_request.py
--rw-r--r--   0        0        0     5223 2024-04-15 12:24:50.229915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_set.py
--rw-r--r--   0        0        0     4459 2024-04-15 12:24:50.237915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_set_request.py
--rw-r--r--   0        0        0     4763 2024-04-15 12:24:50.241915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_stage_binding.py
--rw-r--r--   0        0        0     3983 2024-04-15 12:24:50.245915 authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_stage_binding_request.py
--rw-r--r--   0        0        0     2641 2024-04-15 12:24:50.249915 authentik_client-2024.2.2.post1713183880/authentik_client/models/footer_link.py
--rw-r--r--   0        0        0     2531 2024-04-15 12:24:50.253915 authentik_client-2024.2.2.post1713183880/authentik_client/models/generic_error.py
--rw-r--r--   0        0        0      865 2024-04-15 12:24:50.253915 authentik_client-2024.2.2.post1713183880/authentik_client/models/geoip_binding_enum.py
--rw-r--r--   0        0        0     5216 2024-04-15 12:24:50.257915 authentik_client-2024.2.2.post1713183880/authentik_client/models/group.py
--rw-r--r--   0        0        0     4209 2024-04-15 12:24:50.265915 authentik_client-2024.2.2.post1713183880/authentik_client/models/group_member.py
--rw-r--r--   0        0        0     4006 2024-04-15 12:24:50.269915 authentik_client-2024.2.2.post1713183880/authentik_client/models/group_member_request.py
--rw-r--r--   0        0        0     3347 2024-04-15 12:24:50.273915 authentik_client-2024.2.2.post1713183880/authentik_client/models/group_request.py
--rw-r--r--   0        0        0     6080 2024-04-15 12:24:50.277915 authentik_client-2024.2.2.post1713183880/authentik_client/models/identification_challenge.py
--rw-r--r--   0        0        0     3174 2024-04-15 12:24:50.281915 authentik_client-2024.2.2.post1713183880/authentik_client/models/identification_challenge_response_request.py
--rw-r--r--   0        0        0     7503 2024-04-15 12:24:50.285915 authentik_client-2024.2.2.post1713183880/authentik_client/models/identification_stage.py
--rw-r--r--   0        0        0     6533 2024-04-15 12:24:50.293915 authentik_client-2024.2.2.post1713183880/authentik_client/models/identification_stage_request.py
--rw-r--r--   0        0        0     2438 2024-04-15 12:24:50.297915 authentik_client-2024.2.2.post1713183880/authentik_client/models/install_id.py
--rw-r--r--   0        0        0      771 2024-04-15 12:24:50.297915 authentik_client-2024.2.2.post1713183880/authentik_client/models/intent_enum.py
--rw-r--r--   0        0        0      800 2024-04-15 12:24:50.301915 authentik_client-2024.2.2.post1713183880/authentik_client/models/invalid_response_action_enum.py
--rw-r--r--   0        0        0     4878 2024-04-15 12:24:50.305915 authentik_client-2024.2.2.post1713183880/authentik_client/models/invitation.py
--rw-r--r--   0        0        0     3895 2024-04-15 12:24:50.313915 authentik_client-2024.2.2.post1713183880/authentik_client/models/invitation_request.py
--rw-r--r--   0        0        0     4508 2024-04-15 12:24:50.317915 authentik_client-2024.2.2.post1713183880/authentik_client/models/invitation_stage.py
--rw-r--r--   0        0        0     3527 2024-04-15 12:24:50.321915 authentik_client-2024.2.2.post1713183880/authentik_client/models/invitation_stage_request.py
--rw-r--r--   0        0        0      729 2024-04-15 12:24:50.325915 authentik_client-2024.2.2.post1713183880/authentik_client/models/issuer_mode_enum.py
--rw-r--r--   0        0        0     4386 2024-04-15 12:24:50.325915 authentik_client-2024.2.2.post1713183880/authentik_client/models/kubernetes_service_connection.py
--rw-r--r--   0        0        0     3454 2024-04-15 12:24:50.329915 authentik_client-2024.2.2.post1713183880/authentik_client/models/kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     2811 2024-04-15 12:24:50.337915 authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_debug.py
--rw-r--r--   0        0        0     5765 2024-04-15 12:24:50.341915 authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_outpost_config.py
--rw-r--r--   0        0        0     4378 2024-04-15 12:24:50.345915 authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_property_mapping.py
--rw-r--r--   0        0        0     3478 2024-04-15 12:24:50.345915 authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_property_mapping_request.py
--rw-r--r--   0        0        0     8694 2024-04-15 12:24:50.353915 authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_provider.py
--rw-r--r--   0        0        0     6192 2024-04-15 12:24:50.357915 authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_provider_request.py
--rw-r--r--   0        0        0    11791 2024-04-15 12:24:50.361914 authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_source.py
--rw-r--r--   0        0        0     9542 2024-04-15 12:24:50.365914 authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_source_request.py
--rw-r--r--   0        0        0     3129 2024-04-15 12:24:50.373915 authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_sync_status.py
--rw-r--r--   0        0        0      726 2024-04-15 12:24:50.333915 authentik_client-2024.2.2.post1713183880/authentik_client/models/ldapapi_access_mode.py
--rw-r--r--   0        0        0     3278 2024-04-15 12:24:50.377915 authentik_client-2024.2.2.post1713183880/authentik_client/models/license.py
--rw-r--r--   0        0        0     2897 2024-04-15 12:24:50.381914 authentik_client-2024.2.2.post1713183880/authentik_client/models/license_forecast.py
--rw-r--r--   0        0        0     2509 2024-04-15 12:24:50.385914 authentik_client-2024.2.2.post1713183880/authentik_client/models/license_request.py
--rw-r--r--   0        0        0     3222 2024-04-15 12:24:50.389914 authentik_client-2024.2.2.post1713183880/authentik_client/models/license_summary.py
--rw-r--r--   0        0        0     2411 2024-04-15 12:24:50.393914 authentik_client-2024.2.2.post1713183880/authentik_client/models/link.py
--rw-r--r--   0        0        0     2882 2024-04-15 12:24:50.397914 authentik_client-2024.2.2.post1713183880/authentik_client/models/log_event.py
--rw-r--r--   0        0        0      843 2024-04-15 12:24:50.401914 authentik_client-2024.2.2.post1713183880/authentik_client/models/log_level_enum.py
--rw-r--r--   0        0        0     6520 2024-04-15 12:24:50.405914 authentik_client-2024.2.2.post1713183880/authentik_client/models/login_challenge_types.py
--rw-r--r--   0        0        0     4171 2024-04-15 12:24:50.409914 authentik_client-2024.2.2.post1713183880/authentik_client/models/login_metrics.py
--rw-r--r--   0        0        0     3192 2024-04-15 12:24:50.413914 authentik_client-2024.2.2.post1713183880/authentik_client/models/login_source.py
--rw-r--r--   0        0        0     2513 2024-04-15 12:24:50.417914 authentik_client-2024.2.2.post1713183880/authentik_client/models/metadata.py
--rw-r--r--   0        0        0     7604 2024-04-15 12:24:50.417914 authentik_client-2024.2.2.post1713183880/authentik_client/models/model_enum.py
--rw-r--r--   0        0        0     9828 2024-04-15 12:24:50.425914 authentik_client-2024.2.2.post1713183880/authentik_client/models/model_request.py
--rw-r--r--   0        0        0     1559 2024-04-15 12:24:50.425914 authentik_client-2024.2.2.post1713183880/authentik_client/models/name_id_policy_enum.py
--rw-r--r--   0        0        0      831 2024-04-15 12:24:50.429914 authentik_client-2024.2.2.post1713183880/authentik_client/models/network_binding_enum.py
--rw-r--r--   0        0        0      764 2024-04-15 12:24:50.429914 authentik_client-2024.2.2.post1713183880/authentik_client/models/not_configured_action_enum.py
--rw-r--r--   0        0        0     3479 2024-04-15 12:24:50.433914 authentik_client-2024.2.2.post1713183880/authentik_client/models/notification.py
--rw-r--r--   0        0        0     2858 2024-04-15 12:24:50.437914 authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_request.py
--rw-r--r--   0        0        0     4010 2024-04-15 12:24:50.441914 authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_rule.py
--rw-r--r--   0        0        0     3549 2024-04-15 12:24:50.445914 authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_rule_request.py
--rw-r--r--   0        0        0     3760 2024-04-15 12:24:50.449914 authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_transport.py
--rw-r--r--   0        0        0      818 2024-04-15 12:24:50.449914 authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_transport_mode_enum.py
--rw-r--r--   0        0        0     3500 2024-04-15 12:24:50.453914 authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_transport_request.py
--rw-r--r--   0        0        0     2503 2024-04-15 12:24:50.457914 authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_transport_test.py
--rw-r--r--   0        0        0     2707 2024-04-15 12:24:50.461914 authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_webhook_mapping.py
--rw-r--r--   0        0        0     2717 2024-04-15 12:24:50.465914 authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     8888 2024-04-15 12:24:50.469914 authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth2_provider.py
--rw-r--r--   0        0        0     6654 2024-04-15 12:24:50.473914 authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth2_provider_request.py
--rw-r--r--   0        0        0     3482 2024-04-15 12:24:50.481914 authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth2_provider_setup_urls.py
--rw-r--r--   0        0        0     4164 2024-04-15 12:24:50.489914 authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_device_code_challenge.py
--rw-r--r--   0        0        0     2846 2024-04-15 12:24:50.497914 authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_device_code_challenge_response_request.py
--rw-r--r--   0        0        0     4213 2024-04-15 12:24:50.505914 authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_device_code_finish_challenge.py
--rw-r--r--   0        0        0     2816 2024-04-15 12:24:50.513914 authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
--rw-r--r--   0        0        0    10563 2024-04-15 12:24:50.521914 authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_source.py
--rw-r--r--   0        0        0     8013 2024-04-15 12:24:50.529914 authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_source_request.py
--rw-r--r--   0        0        0     3922 2024-04-15 12:24:50.533913 authentik_client-2024.2.2.post1713183880/authentik_client/models/open_id_connect_configuration.py
--rw-r--r--   0        0        0     5545 2024-04-15 12:24:50.541914 authentik_client-2024.2.2.post1713183880/authentik_client/models/outpost.py
--rw-r--r--   0        0        0     2541 2024-04-15 12:24:50.549914 authentik_client-2024.2.2.post1713183880/authentik_client/models/outpost_default_config.py
--rw-r--r--   0        0        0     3755 2024-04-15 12:24:50.557913 authentik_client-2024.2.2.post1713183880/authentik_client/models/outpost_health.py
--rw-r--r--   0        0        0     4050 2024-04-15 12:24:50.565913 authentik_client-2024.2.2.post1713183880/authentik_client/models/outpost_request.py
--rw-r--r--   0        0        0      752 2024-04-15 12:24:50.565913 authentik_client-2024.2.2.post1713183880/authentik_client/models/outpost_type_enum.py
--rw-r--r--   0        0        0     3322 2024-04-15 12:24:50.573913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_application_list.py
--rw-r--r--   0        0        0     3395 2024-04-15 12:24:50.577913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticated_session_list.py
--rw-r--r--   0        0        0     3404 2024-04-15 12:24:50.585913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_duo_stage_list.py
--rw-r--r--   0        0        0     3404 2024-04-15 12:24:50.593913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_sms_stage_list.py
--rw-r--r--   0        0        0     3428 2024-04-15 12:24:50.601913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_static_stage_list.py
--rw-r--r--   0        0        0     3412 2024-04-15 12:24:50.605913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_totp_stage_list.py
--rw-r--r--   0        0        0     3444 2024-04-15 12:24:50.613913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_validate_stage_list.py
--rw-r--r--   0        0        0     3445 2024-04-15 12:24:50.621913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
--rw-r--r--   0        0        0     3371 2024-04-15 12:24:50.629913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_blueprint_instance_list.py
--rw-r--r--   0        0        0     3274 2024-04-15 12:24:50.633913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_brand_list.py
--rw-r--r--   0        0        0     3331 2024-04-15 12:24:50.641913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_captcha_stage_list.py
--rw-r--r--   0        0        0     3380 2024-04-15 12:24:50.649913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_certificate_key_pair_list.py
--rw-r--r--   0        0        0     3355 2024-04-15 12:24:50.657913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_connection_token_list.py
--rw-r--r--   0        0        0     3331 2024-04-15 12:24:50.661913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_consent_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-15 12:24:50.669913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_deny_stage_list.py
--rw-r--r--   0        0        0     3420 2024-04-15 12:24:50.677913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_docker_service_connection_list.py
--rw-r--r--   0        0        0     3282 2024-04-15 12:24:50.681913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_domain_list.py
--rw-r--r--   0        0        0     3323 2024-04-15 12:24:50.689913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_dummy_policy_list.py
--rw-r--r--   0        0        0     3315 2024-04-15 12:24:50.697913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_dummy_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-15 12:24:50.701912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_duo_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-15 12:24:50.709913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_email_stage_list.py
--rw-r--r--   0        0        0     3298 2024-04-15 12:24:50.713913 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_endpoint_list.py
--rw-r--r--   0        0        0     3274 2024-04-15 12:24:50.721912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_event_list.py
--rw-r--r--   0        0        0     3380 2024-04-15 12:24:50.729912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_event_matcher_policy_list.py
--rw-r--r--   0        0        0     3413 2024-04-15 12:24:50.733912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_expiring_base_grant_model_list.py
--rw-r--r--   0        0        0     3363 2024-04-15 12:24:50.741912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_expression_policy_list.py
--rw-r--r--   0        0        0     3437 2024-04-15 12:24:50.749912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_extra_role_object_permission_list.py
--rw-r--r--   0        0        0     3437 2024-04-15 12:24:50.753912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_extra_user_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-15 12:24:50.761912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_flow_list.py
--rw-r--r--   0        0        0     3364 2024-04-15 12:24:50.765912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_flow_stage_binding_list.py
--rw-r--r--   0        0        0     3274 2024-04-15 12:24:50.773912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_group_list.py
--rw-r--r--   0        0        0     3387 2024-04-15 12:24:50.781912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_identification_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-15 12:24:50.785912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_invitation_list.py
--rw-r--r--   0        0        0     3355 2024-04-15 12:24:50.785912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_invitation_stage_list.py
--rw-r--r--   0        0        0     3452 2024-04-15 12:24:50.789912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_kubernetes_service_connection_list.py
--rw-r--r--   0        0        0     3372 2024-04-15 12:24:50.793912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_ldap_outpost_config_list.py
--rw-r--r--   0        0        0     3388 2024-04-15 12:24:50.797912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_ldap_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-15 12:24:50.801912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_ldap_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-15 12:24:50.805912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_ldap_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-15 12:24:50.805912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_license_list.py
--rw-r--r--   0        0        0     3330 2024-04-15 12:24:50.809912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_notification_list.py
--rw-r--r--   0        0        0     3363 2024-04-15 12:24:50.813912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_notification_rule_list.py
--rw-r--r--   0        0        0     3403 2024-04-15 12:24:50.817912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_notification_transport_list.py
--rw-r--r--   0        0        0     3444 2024-04-15 12:24:50.821912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_notification_webhook_mapping_list.py
--rw-r--r--   0        0        0     3348 2024-04-15 12:24:50.825912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_o_auth2_provider_list.py
--rw-r--r--   0        0        0     3324 2024-04-15 12:24:50.825912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_o_auth_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-15 12:24:50.829912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_outpost_list.py
--rw-r--r--   0        0        0     3396 2024-04-15 12:24:50.833912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_password_expiry_policy_list.py
--rw-r--r--   0        0        0     3347 2024-04-15 12:24:50.837912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_password_policy_list.py
--rw-r--r--   0        0        0     3339 2024-04-15 12:24:50.841912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_password_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-15 12:24:50.845912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_permission_list.py
--rw-r--r--   0        0        0     3396 2024-04-15 12:24:50.849912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_plex_source_connection_list.py
--rw-r--r--   0        0        0     3315 2024-04-15 12:24:50.849912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_plex_source_list.py
--rw-r--r--   0        0        0     3339 2024-04-15 12:24:50.853912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_policy_binding_list.py
--rw-r--r--   0        0        0     3282 2024-04-15 12:24:50.857912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_policy_list.py
--rw-r--r--   0        0        0     3282 2024-04-15 12:24:50.861912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_prompt_list.py
--rw-r--r--   0        0        0     3323 2024-04-15 12:24:50.865912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_prompt_stage_list.py
--rw-r--r--   0        0        0     3355 2024-04-15 12:24:50.869912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_property_mapping_list.py
--rw-r--r--   0        0        0     3298 2024-04-15 12:24:50.877912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-15 12:24:50.881912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_proxy_outpost_config_list.py
--rw-r--r--   0        0        0     3339 2024-04-15 12:24:50.885912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_proxy_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-15 12:24:50.885912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_rac_property_mapping_list.py
--rw-r--r--   0        0        0     3323 2024-04-15 12:24:50.889912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_rac_provider_list.py
--rw-r--r--   0        0        0     3388 2024-04-15 12:24:50.893911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_radius_outpost_config_list.py
--rw-r--r--   0        0        0     3347 2024-04-15 12:24:50.893911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_radius_provider_list.py
--rw-r--r--   0        0        0     3314 2024-04-15 12:24:50.897911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_reputation_list.py
--rw-r--r--   0        0        0     3363 2024-04-15 12:24:50.901911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_reputation_policy_list.py
--rw-r--r--   0        0        0     3461 2024-04-15 12:24:50.901911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_role_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-15 12:24:50.905912 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_role_list.py
--rw-r--r--   0        0        0     3388 2024-04-15 12:24:50.909911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_saml_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-15 12:24:50.909911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_saml_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-15 12:24:50.913911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_saml_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-15 12:24:50.917911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scim_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-15 12:24:50.917911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scim_provider_list.py
--rw-r--r--   0        0        0     3356 2024-04-15 12:24:50.921911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scim_source_group_list.py
--rw-r--r--   0        0        0     3315 2024-04-15 12:24:50.925911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scim_source_list.py
--rw-r--r--   0        0        0     3348 2024-04-15 12:24:50.925911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scim_source_user_list.py
--rw-r--r--   0        0        0     3331 2024-04-15 12:24:50.933911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scope_mapping_list.py
--rw-r--r--   0        0        0     3371 2024-04-15 12:24:50.933911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_service_connection_list.py
--rw-r--r--   0        0        0     3307 2024-04-15 12:24:50.929911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_sms_device_list.py
--rw-r--r--   0        0        0     3282 2024-04-15 12:24:50.937911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-15 12:24:50.941911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_source_stage_list.py
--rw-r--r--   0        0        0     3274 2024-04-15 12:24:50.941911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_stage_list.py
--rw-r--r--   0        0        0     3331 2024-04-15 12:24:50.945911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_static_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-15 12:24:50.949911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_system_task_list.py
--rw-r--r--   0        0        0     3282 2024-04-15 12:24:50.953911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_tenant_list.py
--rw-r--r--   0        0        0     3274 2024-04-15 12:24:50.957911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_token_list.py
--rw-r--r--   0        0        0     3315 2024-04-15 12:24:50.961911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_token_model_list.py
--rw-r--r--   0        0        0     3315 2024-04-15 12:24:50.949911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_totp_device_list.py
--rw-r--r--   0        0        0     3461 2024-04-15 12:24:50.961911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3323 2024-04-15 12:24:50.965911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_consent_list.py
--rw-r--r--   0        0        0     3356 2024-04-15 12:24:50.969911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_delete_stage_list.py
--rw-r--r--   0        0        0     3266 2024-04-15 12:24:50.969911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_list.py
--rw-r--r--   0        0        0     3348 2024-04-15 12:24:50.973911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_login_stage_list.py
--rw-r--r--   0        0        0     3356 2024-04-15 12:24:50.977911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_logout_stage_list.py
--rw-r--r--   0        0        0     3438 2024-04-15 12:24:50.981911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_o_auth_source_connection_list.py
--rw-r--r--   0        0        0     3429 2024-04-15 12:24:50.981911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_saml_source_connection_list.py
--rw-r--r--   0        0        0     3396 2024-04-15 12:24:50.985911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_source_connection_list.py
--rw-r--r--   0        0        0     3348 2024-04-15 12:24:50.989911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_write_stage_list.py
--rw-r--r--   0        0        0     3348 2024-04-15 12:24:50.989911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_web_authn_device_list.py
--rw-r--r--   0        0        0     3381 2024-04-15 12:24:50.993911 authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_web_authn_device_type_list.py
--rw-r--r--   0        0        0     3076 2024-04-15 12:24:50.997911 authentik_client-2024.2.2.post1713183880/authentik_client/models/pagination.py
--rw-r--r--   0        0        0     4454 2024-04-15 12:24:51.001911 authentik_client-2024.2.2.post1713183880/authentik_client/models/password_challenge.py
--rw-r--r--   0        0        0     2819 2024-04-15 12:24:51.001911 authentik_client-2024.2.2.post1713183880/authentik_client/models/password_challenge_response_request.py
--rw-r--r--   0        0        0     4377 2024-04-15 12:24:51.005911 authentik_client-2024.2.2.post1713183880/authentik_client/models/password_expiry_policy.py
--rw-r--r--   0        0        0     3099 2024-04-15 12:24:51.009911 authentik_client-2024.2.2.post1713183880/authentik_client/models/password_expiry_policy_request.py
--rw-r--r--   0        0        0     6428 2024-04-15 12:24:51.009911 authentik_client-2024.2.2.post1713183880/authentik_client/models/password_policy.py
--rw-r--r--   0        0        0     5239 2024-04-15 12:24:51.013911 authentik_client-2024.2.2.post1713183880/authentik_client/models/password_policy_request.py
--rw-r--r--   0        0        0     5274 2024-04-15 12:24:51.017911 authentik_client-2024.2.2.post1713183880/authentik_client/models/password_stage.py
--rw-r--r--   0        0        0     4264 2024-04-15 12:24:51.021911 authentik_client-2024.2.2.post1713183880/authentik_client/models/password_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-15 12:24:51.025911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_application_request.py
--rw-r--r--   0        0        0     4833 2024-04-15 12:24:51.029911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     5701 2024-04-15 12:24:51.033911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4430 2024-04-15 12:24:51.037911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4256 2024-04-15 12:24:51.041911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     4931 2024-04-15 12:24:51.045911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5340 2024-04-15 12:24:51.049911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     3246 2024-04-15 12:24:51.049911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_blueprint_instance_request.py
--rw-r--r--   0        0        0     6352 2024-04-15 12:24:51.053911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_brand_request.py
--rw-r--r--   0        0        0     3860 2024-04-15 12:24:51.057911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_captcha_stage_request.py
--rw-r--r--   0        0        0     3051 2024-04-15 12:24:51.061910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_certificate_key_pair_request.py
--rw-r--r--   0        0        0     2717 2024-04-15 12:24:51.065910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_connection_token_request.py
--rw-r--r--   0        0        0     3607 2024-04-15 12:24:51.069910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_consent_stage_request.py
--rw-r--r--   0        0        0     3268 2024-04-15 12:24:51.073911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_deny_stage_request.py
--rw-r--r--   0        0        0     4149 2024-04-15 12:24:51.077911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_docker_service_connection_request.py
--rw-r--r--   0        0        0     2801 2024-04-15 12:24:51.077911 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_domain_request.py
--rw-r--r--   0        0        0     3275 2024-04-15 12:24:51.081910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_dummy_policy_request.py
--rw-r--r--   0        0        0     3270 2024-04-15 12:24:51.085910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_dummy_stage_request.py
--rw-r--r--   0        0        0     2674 2024-04-15 12:24:51.089910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_duo_device_request.py
--rw-r--r--   0        0        0     5159 2024-04-15 12:24:51.093910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_email_stage_request.py
--rw-r--r--   0        0        0     3784 2024-04-15 12:24:51.097910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_endpoint_request.py
--rw-r--r--   0        0        0     4845 2024-04-15 12:24:51.101910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_event_matcher_policy_request.py
--rw-r--r--   0        0        0     4045 2024-04-15 12:24:51.105910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_event_request.py
--rw-r--r--   0        0        0     3047 2024-04-15 12:24:51.105910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_expression_policy_request.py
--rw-r--r--   0        0        0     4903 2024-04-15 12:24:51.109910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_flow_request.py
--rw-r--r--   0        0        0     4055 2024-04-15 12:24:51.113910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_flow_stage_binding_request.py
--rw-r--r--   0        0        0     3385 2024-04-15 12:24:51.117910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_group_request.py
--rw-r--r--   0        0        0     6571 2024-04-15 12:24:51.121910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_identification_stage_request.py
--rw-r--r--   0        0        0     3985 2024-04-15 12:24:51.125910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_invitation_request.py
--rw-r--r--   0        0        0     3565 2024-04-15 12:24:51.129910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_invitation_stage_request.py
--rw-r--r--   0        0        0     3492 2024-04-15 12:24:51.133910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     3550 2024-04-15 12:24:51.133910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_ldap_property_mapping_request.py
--rw-r--r--   0        0        0     6254 2024-04-15 12:24:51.137910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_ldap_provider_request.py
--rw-r--r--   0        0        0     9697 2024-04-15 12:24:51.141910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_ldap_source_request.py
--rw-r--r--   0        0        0     2557 2024-04-15 12:24:51.145910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_license_request.py
--rw-r--r--   0        0        0     2879 2024-04-15 12:24:51.149910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_notification_request.py
--rw-r--r--   0        0        0     3587 2024-04-15 12:24:51.153910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_notification_rule_request.py
--rw-r--r--   0        0        0     3538 2024-04-15 12:24:51.157910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_notification_transport_request.py
--rw-r--r--   0        0        0     2782 2024-04-15 12:24:51.157910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     6716 2024-04-15 12:24:51.161910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_o_auth2_provider_request.py
--rw-r--r--   0        0        0     8185 2024-04-15 12:24:51.165910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_o_auth_source_request.py
--rw-r--r--   0        0        0     4139 2024-04-15 12:24:51.169910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_outpost_request.py
--rw-r--r--   0        0        0     3154 2024-04-15 12:24:51.173910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_password_expiry_policy_request.py
--rw-r--r--   0        0        0     5277 2024-04-15 12:24:51.177910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_password_policy_request.py
--rw-r--r--   0        0        0     4326 2024-04-15 12:24:51.181910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_password_stage_request.py
--rw-r--r--   0        0        0     2922 2024-04-15 12:24:51.181910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_permission_assign_request.py
--rw-r--r--   0        0        0     2784 2024-04-15 12:24:51.185910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_plex_source_connection_request.py
--rw-r--r--   0        0        0     5905 2024-04-15 12:24:51.189910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_plex_source_request.py
--rw-r--r--   0        0        0     4286 2024-04-15 12:24:51.193910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_policy_binding_request.py
--rw-r--r--   0        0        0     5023 2024-04-15 12:24:51.197910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_prompt_request.py
--rw-r--r--   0        0        0     3406 2024-04-15 12:24:51.201910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_prompt_stage_request.py
--rw-r--r--   0        0        0     6907 2024-04-15 12:24:51.205910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_proxy_provider_request.py
--rw-r--r--   0        0        0     3495 2024-04-15 12:24:51.209910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_rac_property_mapping_request.py
--rw-r--r--   0        0        0     4413 2024-04-15 12:24:51.213910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_rac_provider_request.py
--rw-r--r--   0        0        0     4563 2024-04-15 12:24:51.217910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_radius_provider_request.py
--rw-r--r--   0        0        0     3276 2024-04-15 12:24:51.217910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_reputation_policy_request.py
--rw-r--r--   0        0        0     2565 2024-04-15 12:24:51.221910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_role_request.py
--rw-r--r--   0        0        0     3901 2024-04-15 12:24:51.225910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_saml_property_mapping_request.py
--rw-r--r--   0        0        0     7539 2024-04-15 12:24:51.229910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_saml_provider_request.py
--rw-r--r--   0        0        0     8676 2024-04-15 12:24:51.233909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_saml_source_request.py
--rw-r--r--   0        0        0     3364 2024-04-15 12:24:51.237909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scim_mapping_request.py
--rw-r--r--   0        0        0     3888 2024-04-15 12:24:51.237909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scim_provider_request.py
--rw-r--r--   0        0        0     3095 2024-04-15 12:24:51.241910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scim_source_group_request.py
--rw-r--r--   0        0        0     3829 2024-04-15 12:24:51.245910 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scim_source_request.py
--rw-r--r--   0        0        0     3098 2024-04-15 12:24:51.249909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scim_source_user_request.py
--rw-r--r--   0        0        0     3819 2024-04-15 12:24:51.257909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scope_mapping_request.py
--rw-r--r--   0        0        0     5079 2024-04-15 12:24:51.257909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_settings_request.py
--rw-r--r--   0        0        0     2674 2024-04-15 12:24:51.253909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_sms_device_request.py
--rw-r--r--   0        0        0     3562 2024-04-15 12:24:51.261909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_source_stage_request.py
--rw-r--r--   0        0        0     2686 2024-04-15 12:24:51.265909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_static_device_request.py
--rw-r--r--   0        0        0     2820 2024-04-15 12:24:51.269909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_tenant_request.py
--rw-r--r--   0        0        0     4419 2024-04-15 12:24:51.273909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_token_request.py
--rw-r--r--   0        0        0     2678 2024-04-15 12:24:51.269909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_totp_device_request.py
--rw-r--r--   0        0        0     3167 2024-04-15 12:24:51.277909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_delete_stage_request.py
--rw-r--r--   0        0        0     4766 2024-04-15 12:24:51.281909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_login_stage_request.py
--rw-r--r--   0        0        0     3167 2024-04-15 12:24:51.285909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_logout_stage_request.py
--rw-r--r--   0        0        0     3109 2024-04-15 12:24:51.289909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3934 2024-04-15 12:24:51.293909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_request.py
--rw-r--r--   0        0        0     2733 2024-04-15 12:24:51.293909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_saml_source_connection_request.py
--rw-r--r--   0        0        0     4450 2024-04-15 12:24:51.297909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_write_stage_request.py
--rw-r--r--   0        0        0     2625 2024-04-15 12:24:51.301909 authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_web_authn_device_request.py
--rw-r--r--   0        0        0     3548 2024-04-15 12:24:51.305909 authentik_client-2024.2.2.post1713183880/authentik_client/models/permission.py
--rw-r--r--   0        0        0     2884 2024-04-15 12:24:51.309909 authentik_client-2024.2.2.post1713183880/authentik_client/models/permission_assign_request.py
--rw-r--r--   0        0        0     4315 2024-04-15 12:24:51.313909 authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_authentication_challenge.py
--rw-r--r--   0        0        0     2726 2024-04-15 12:24:51.313909 authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_authentication_challenge_response_request.py
--rw-r--r--   0        0        0     7752 2024-04-15 12:24:51.321909 authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_source.py
--rw-r--r--   0        0        0     3265 2024-04-15 12:24:51.321909 authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_source_connection.py
--rw-r--r--   0        0        0     2719 2024-04-15 12:24:51.325909 authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_source_connection_request.py
--rw-r--r--   0        0        0     5760 2024-04-15 12:24:51.333909 authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_source_request.py
--rw-r--r--   0        0        0     2576 2024-04-15 12:24:51.333909 authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_token_redeem_request.py
--rw-r--r--   0        0        0     4055 2024-04-15 12:24:51.337909 authentik_client-2024.2.2.post1713183880/authentik_client/models/policy.py
--rw-r--r--   0        0        0     5643 2024-04-15 12:24:51.341909 authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_binding.py
--rw-r--r--   0        0        0     4231 2024-04-15 12:24:51.345909 authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_binding_request.py
--rw-r--r--   0        0        0      711 2024-04-15 12:24:51.345909 authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_engine_mode.py
--rw-r--r--   0        0        0     2817 2024-04-15 12:24:51.349909 authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_request.py
--rw-r--r--   0        0        0     2583 2024-04-15 12:24:51.353909 authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_test_request.py
--rw-r--r--   0        0        0     3281 2024-04-15 12:24:51.357909 authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_test_result.py
--rw-r--r--   0        0        0     4885 2024-04-15 12:24:51.357909 authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt.py
--rw-r--r--   0        0        0     4649 2024-04-15 12:24:51.361909 authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_challenge.py
--rw-r--r--   0        0        0     3325 2024-04-15 12:24:51.365909 authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_challenge_response_request.py
--rw-r--r--   0        0        0     4927 2024-04-15 12:24:51.369909 authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_request.py
--rw-r--r--   0        0        0     4321 2024-04-15 12:24:51.373909 authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_stage.py
--rw-r--r--   0        0        0     3351 2024-04-15 12:24:51.377909 authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_stage_request.py
--rw-r--r--   0        0        0     1185 2024-04-15 12:24:51.377909 authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_type_enum.py
--rw-r--r--   0        0        0     4264 2024-04-15 12:24:51.381909 authentik_client-2024.2.2.post1713183880/authentik_client/models/property_mapping.py
--rw-r--r--   0        0        0     2610 2024-04-15 12:24:51.385909 authentik_client-2024.2.2.post1713183880/authentik_client/models/property_mapping_preview.py
--rw-r--r--   0        0        0     2744 2024-04-15 12:24:51.389909 authentik_client-2024.2.2.post1713183880/authentik_client/models/property_mapping_test_result.py
--rw-r--r--   0        0        0      715 2024-04-15 12:24:51.389909 authentik_client-2024.2.2.post1713183880/authentik_client/models/protocol_enum.py
--rw-r--r--   0        0        0     5722 2024-04-15 12:24:51.397909 authentik_client-2024.2.2.post1713183880/authentik_client/models/provider.py
--rw-r--r--   0        0        0      713 2024-04-15 12:24:51.401908 authentik_client-2024.2.2.post1713183880/authentik_client/models/provider_enum.py
--rw-r--r--   0        0        0     1314 2024-04-15 12:24:51.401908 authentik_client-2024.2.2.post1713183880/authentik_client/models/provider_model_enum.py
--rw-r--r--   0        0        0     3397 2024-04-15 12:24:51.405908 authentik_client-2024.2.2.post1713183880/authentik_client/models/provider_request.py
--rw-r--r--   0        0        0     1009 2024-04-15 12:24:51.405908 authentik_client-2024.2.2.post1713183880/authentik_client/models/provider_type_enum.py
--rw-r--r--   0        0        0      754 2024-04-15 12:24:51.405908 authentik_client-2024.2.2.post1713183880/authentik_client/models/proxy_mode.py
--rw-r--r--   0        0        0     7819 2024-04-15 12:24:51.409908 authentik_client-2024.2.2.post1713183880/authentik_client/models/proxy_outpost_config.py
--rw-r--r--   0        0        0     9552 2024-04-15 12:24:51.413909 authentik_client-2024.2.2.post1713183880/authentik_client/models/proxy_provider.py
--rw-r--r--   0        0        0     6828 2024-04-15 12:24:51.417909 authentik_client-2024.2.2.post1713183880/authentik_client/models/proxy_provider_request.py
--rw-r--r--   0        0        0     4407 2024-04-15 12:24:51.421908 authentik_client-2024.2.2.post1713183880/authentik_client/models/rac_property_mapping.py
--rw-r--r--   0        0        0     3440 2024-04-15 12:24:51.421908 authentik_client-2024.2.2.post1713183880/authentik_client/models/rac_property_mapping_request.py
--rw-r--r--   0        0        0     6813 2024-04-15 12:24:51.425908 authentik_client-2024.2.2.post1713183880/authentik_client/models/rac_provider.py
--rw-r--r--   0        0        0     4351 2024-04-15 12:24:51.429908 authentik_client-2024.2.2.post1713183880/authentik_client/models/rac_provider_request.py
--rw-r--r--   0        0        0     3833 2024-04-15 12:24:51.433908 authentik_client-2024.2.2.post1713183880/authentik_client/models/radius_outpost_config.py
--rw-r--r--   0        0        0     6924 2024-04-15 12:24:51.433908 authentik_client-2024.2.2.post1713183880/authentik_client/models/radius_provider.py
--rw-r--r--   0        0        0     4501 2024-04-15 12:24:51.437908 authentik_client-2024.2.2.post1713183880/authentik_client/models/radius_provider_request.py
--rw-r--r--   0        0        0     4184 2024-04-15 12:24:51.441908 authentik_client-2024.2.2.post1713183880/authentik_client/models/redirect_challenge.py
--rw-r--r--   0        0        0     3642 2024-04-15 12:24:51.445908 authentik_client-2024.2.2.post1713183880/authentik_client/models/reputation.py
--rw-r--r--   0        0        0     4516 2024-04-15 12:24:51.449908 authentik_client-2024.2.2.post1713183880/authentik_client/models/reputation_policy.py
--rw-r--r--   0        0        0     3238 2024-04-15 12:24:51.453908 authentik_client-2024.2.2.post1713183880/authentik_client/models/reputation_policy_request.py
--rw-r--r--   0        0        0      795 2024-04-15 12:24:51.453908 authentik_client-2024.2.2.post1713183880/authentik_client/models/resident_key_requirement_enum.py
--rw-r--r--   0        0        0     2618 2024-04-15 12:24:51.457908 authentik_client-2024.2.2.post1713183880/authentik_client/models/role.py
--rw-r--r--   0        0        0     3333 2024-04-15 12:24:51.457908 authentik_client-2024.2.2.post1713183880/authentik_client/models/role_assigned_object_permission.py
--rw-r--r--   0        0        0     3293 2024-04-15 12:24:51.461908 authentik_client-2024.2.2.post1713183880/authentik_client/models/role_object_permission.py
--rw-r--r--   0        0        0     2517 2024-04-15 12:24:51.465908 authentik_client-2024.2.2.post1713183880/authentik_client/models/role_request.py
--rw-r--r--   0        0        0     2712 2024-04-15 12:24:51.469908 authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_metadata.py
--rw-r--r--   0        0        0     4718 2024-04-15 12:24:51.473908 authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_property_mapping.py
--rw-r--r--   0        0        0     3829 2024-04-15 12:24:51.473908 authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_property_mapping_request.py
--rw-r--r--   0        0        0    11056 2024-04-15 12:24:51.477908 authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_provider.py
--rw-r--r--   0        0        0     7460 2024-04-15 12:24:51.481908 authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_provider_request.py
--rw-r--r--   0        0        0    10563 2024-04-15 12:24:51.485908 authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_source.py
--rw-r--r--   0        0        0     8507 2024-04-15 12:24:51.489908 authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_source_request.py
--rw-r--r--   0        0        0     4248 2024-04-15 12:24:51.493908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_mapping.py
--rw-r--r--   0        0        0     3309 2024-04-15 12:24:51.493908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_mapping_request.py
--rw-r--r--   0        0        0     5454 2024-04-15 12:24:51.497908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_provider.py
--rw-r--r--   0        0        0     3802 2024-04-15 12:24:51.501908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_provider_request.py
--rw-r--r--   0        0        0     5999 2024-04-15 12:24:51.501908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source.py
--rw-r--r--   0        0        0     3369 2024-04-15 12:24:51.505908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source_group.py
--rw-r--r--   0        0        0     3023 2024-04-15 12:24:51.509908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source_group_request.py
--rw-r--r--   0        0        0     3708 2024-04-15 12:24:51.513908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source_request.py
--rw-r--r--   0        0        0     3370 2024-04-15 12:24:51.517908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source_user.py
--rw-r--r--   0        0        0     3026 2024-04-15 12:24:51.521908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source_user_request.py
--rw-r--r--   0        0        0     3131 2024-04-15 12:24:51.525908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_sync_status.py
--rw-r--r--   0        0        0     4629 2024-04-15 12:24:51.533908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scope_mapping.py
--rw-r--r--   0        0        0     3740 2024-04-15 12:24:51.537908 authentik_client-2024.2.2.post1713183880/authentik_client/models/scope_mapping_request.py
--rw-r--r--   0        0        0     2738 2024-04-15 12:24:51.541908 authentik_client-2024.2.2.post1713183880/authentik_client/models/selectable_stage.py
--rw-r--r--   0        0        0     3773 2024-04-15 12:24:51.541908 authentik_client-2024.2.2.post1713183880/authentik_client/models/service_connection.py
--rw-r--r--   0        0        0     2776 2024-04-15 12:24:51.545908 authentik_client-2024.2.2.post1713183880/authentik_client/models/service_connection_request.py
--rw-r--r--   0        0        0     2731 2024-04-15 12:24:51.549908 authentik_client-2024.2.2.post1713183880/authentik_client/models/service_connection_state.py
--rw-r--r--   0        0        0     3178 2024-04-15 12:24:51.553908 authentik_client-2024.2.2.post1713183880/authentik_client/models/session_user.py
--rw-r--r--   0        0        0     4931 2024-04-15 12:24:51.557908 authentik_client-2024.2.2.post1713183880/authentik_client/models/settings.py
--rw-r--r--   0        0        0     5058 2024-04-15 12:24:51.561908 authentik_client-2024.2.2.post1713183880/authentik_client/models/settings_request.py
--rw-r--r--   0        0        0      733 2024-04-15 12:24:51.565908 authentik_client-2024.2.2.post1713183880/authentik_client/models/severity_enum.py
--rw-r--r--   0        0        0     4175 2024-04-15 12:24:51.569908 authentik_client-2024.2.2.post1713183880/authentik_client/models/shell_challenge.py
--rw-r--r--   0        0        0     1492 2024-04-15 12:24:51.573907 authentik_client-2024.2.2.post1713183880/authentik_client/models/signature_algorithm_enum.py
--rw-r--r--   0        0        0     2906 2024-04-15 12:24:51.525908 authentik_client-2024.2.2.post1713183880/authentik_client/models/sms_device.py
--rw-r--r--   0        0        0     2619 2024-04-15 12:24:51.529908 authentik_client-2024.2.2.post1713183880/authentik_client/models/sms_device_request.py
--rw-r--r--   0        0        0     6945 2024-04-15 12:24:51.573907 authentik_client-2024.2.2.post1713183880/authentik_client/models/source.py
--rw-r--r--   0        0        0     4836 2024-04-15 12:24:51.577907 authentik_client-2024.2.2.post1713183880/authentik_client/models/source_request.py
--rw-r--r--   0        0        0     4438 2024-04-15 12:24:51.581907 authentik_client-2024.2.2.post1713183880/authentik_client/models/source_stage.py
--rw-r--r--   0        0        0     3507 2024-04-15 12:24:51.585907 authentik_client-2024.2.2.post1713183880/authentik_client/models/source_stage_request.py
--rw-r--r--   0        0        0     5355 2024-04-15 12:24:51.585907 authentik_client-2024.2.2.post1713183880/authentik_client/models/source_type.py
--rw-r--r--   0        0        0      714 2024-04-15 12:24:51.589908 authentik_client-2024.2.2.post1713183880/authentik_client/models/sp_binding_enum.py
--rw-r--r--   0        0        0     4070 2024-04-15 12:24:51.593907 authentik_client-2024.2.2.post1713183880/authentik_client/models/stage.py
--rw-r--r--   0        0        0     3437 2024-04-15 12:24:51.593907 authentik_client-2024.2.2.post1713183880/authentik_client/models/stage_prompt.py
--rw-r--r--   0        0        0     3089 2024-04-15 12:24:51.597907 authentik_client-2024.2.2.post1713183880/authentik_client/models/stage_request.py
--rw-r--r--   0        0        0     3385 2024-04-15 12:24:51.601907 authentik_client-2024.2.2.post1713183880/authentik_client/models/static_device.py
--rw-r--r--   0        0        0     2631 2024-04-15 12:24:51.605907 authentik_client-2024.2.2.post1713183880/authentik_client/models/static_device_request.py
--rw-r--r--   0        0        0     2546 2024-04-15 12:24:51.609907 authentik_client-2024.2.2.post1713183880/authentik_client/models/static_device_token.py
--rw-r--r--   0        0        0     2581 2024-04-15 12:24:51.609907 authentik_client-2024.2.2.post1713183880/authentik_client/models/static_device_token_request.py
--rw-r--r--   0        0        0      846 2024-04-15 12:24:51.613907 authentik_client-2024.2.2.post1713183880/authentik_client/models/sub_mode_enum.py
--rw-r--r--   0        0        0     4463 2024-04-15 12:24:51.613907 authentik_client-2024.2.2.post1713183880/authentik_client/models/system_info.py
--rw-r--r--   0        0        0     2934 2024-04-15 12:24:51.617907 authentik_client-2024.2.2.post1713183880/authentik_client/models/system_info_runtime.py
--rw-r--r--   0        0        0     4286 2024-04-15 12:24:51.621907 authentik_client-2024.2.2.post1713183880/authentik_client/models/system_task.py
--rw-r--r--   0        0        0      789 2024-04-15 12:24:51.621907 authentik_client-2024.2.2.post1713183880/authentik_client/models/system_task_status_enum.py
--rw-r--r--   0        0        0     2872 2024-04-15 12:24:51.633907 authentik_client-2024.2.2.post1713183880/authentik_client/models/tenant.py
--rw-r--r--   0        0        0     2589 2024-04-15 12:24:51.633907 authentik_client-2024.2.2.post1713183880/authentik_client/models/tenant_admin_group_request_request.py
--rw-r--r--   0        0        0     2705 2024-04-15 12:24:51.637907 authentik_client-2024.2.2.post1713183880/authentik_client/models/tenant_recovery_key_request_request.py
--rw-r--r--   0        0        0     2599 2024-04-15 12:24:51.641907 authentik_client-2024.2.2.post1713183880/authentik_client/models/tenant_recovery_key_response.py
--rw-r--r--   0        0        0     2765 2024-04-15 12:24:51.641907 authentik_client-2024.2.2.post1713183880/authentik_client/models/tenant_request.py
--rw-r--r--   0        0        0     4802 2024-04-15 12:24:51.645907 authentik_client-2024.2.2.post1713183880/authentik_client/models/token.py
--rw-r--r--   0        0        0     4198 2024-04-15 12:24:51.649907 authentik_client-2024.2.2.post1713183880/authentik_client/models/token_model.py
--rw-r--r--   0        0        0     4329 2024-04-15 12:24:51.653907 authentik_client-2024.2.2.post1713183880/authentik_client/models/token_request.py
--rw-r--r--   0        0        0     2521 2024-04-15 12:24:51.657907 authentik_client-2024.2.2.post1713183880/authentik_client/models/token_set_key_request.py
--rw-r--r--   0        0        0     2494 2024-04-15 12:24:51.657907 authentik_client-2024.2.2.post1713183880/authentik_client/models/token_view.py
--rw-r--r--   0        0        0     2724 2024-04-15 12:24:51.625907 authentik_client-2024.2.2.post1713183880/authentik_client/models/totp_device.py
--rw-r--r--   0        0        0     2623 2024-04-15 12:24:51.629907 authentik_client-2024.2.2.post1713183880/authentik_client/models/totp_device_request.py
--rw-r--r--   0        0        0     3389 2024-04-15 12:24:51.661907 authentik_client-2024.2.2.post1713183880/authentik_client/models/transaction_application_request.py
--rw-r--r--   0        0        0     2595 2024-04-15 12:24:51.665907 authentik_client-2024.2.2.post1713183880/authentik_client/models/transaction_application_response.py
--rw-r--r--   0        0        0     2936 2024-04-15 12:24:51.669907 authentik_client-2024.2.2.post1713183880/authentik_client/models/type_create.py
--rw-r--r--   0        0        0      730 2024-04-15 12:24:51.669907 authentik_client-2024.2.2.post1713183880/authentik_client/models/ui_theme_enum.py
--rw-r--r--   0        0        0     2808 2024-04-15 12:24:51.673907 authentik_client-2024.2.2.post1713183880/authentik_client/models/used_by.py
--rw-r--r--   0        0        0      795 2024-04-15 12:24:51.673907 authentik_client-2024.2.2.post1713183880/authentik_client/models/used_by_action_enum.py
--rw-r--r--   0        0        0     5226 2024-04-15 12:24:51.677907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user.py
--rw-r--r--   0        0        0     2458 2024-04-15 12:24:51.677907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_account_request.py
--rw-r--r--   0        0        0     4946 2024-04-15 12:24:51.681907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_assigned_object_permission.py
--rw-r--r--   0        0        0     3828 2024-04-15 12:24:51.685907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_consent.py
--rw-r--r--   0        0        0      811 2024-04-15 12:24:51.685907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_creation_mode_enum.py
--rw-r--r--   0        0        0     4110 2024-04-15 12:24:51.689907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_delete_stage.py
--rw-r--r--   0        0        0     3129 2024-04-15 12:24:51.693907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_delete_stage_request.py
--rw-r--r--   0        0        0      735 2024-04-15 12:24:51.693907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_fields_enum.py
--rw-r--r--   0        0        0     3909 2024-04-15 12:24:51.697907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_group.py
--rw-r--r--   0        0        0     4334 2024-04-15 12:24:51.697907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_login_challenge.py
--rw-r--r--   0        0        0     2805 2024-04-15 12:24:51.701907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_login_challenge_response_request.py
--rw-r--r--   0        0        0     5631 2024-04-15 12:24:51.705907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_login_stage.py
--rw-r--r--   0        0        0     4728 2024-04-15 12:24:51.709907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_login_stage_request.py
--rw-r--r--   0        0        0     4110 2024-04-15 12:24:51.709907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_logout_stage.py
--rw-r--r--   0        0        0     3129 2024-04-15 12:24:51.713907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_logout_stage_request.py
--rw-r--r--   0        0        0      853 2024-04-15 12:24:51.717907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_matching_mode_enum.py
--rw-r--r--   0        0        0     4160 2024-04-15 12:24:51.717907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_metrics.py
--rw-r--r--   0        0        0     3188 2024-04-15 12:24:51.721907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_o_auth_source_connection.py
--rw-r--r--   0        0        0     3054 2024-04-15 12:24:51.721907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3293 2024-04-15 12:24:51.725906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_object_permission.py
--rw-r--r--   0        0        0     2557 2024-04-15 12:24:51.729906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_password_set_request.py
--rw-r--r--   0        0        0     2491 2024-04-15 12:24:51.729906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_path.py
--rw-r--r--   0        0        0     3872 2024-04-15 12:24:51.733907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_request.py
--rw-r--r--   0        0        0     3107 2024-04-15 12:24:51.737907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_saml_source_connection.py
--rw-r--r--   0        0        0     2668 2024-04-15 12:24:51.737907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_saml_source_connection_request.py
--rw-r--r--   0        0        0     5465 2024-04-15 12:24:51.741907 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_self.py
--rw-r--r--   0        0        0     2629 2024-04-15 12:24:51.745906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_self_groups.py
--rw-r--r--   0        0        0     3074 2024-04-15 12:24:51.745906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_service_account_request.py
--rw-r--r--   0        0        0     2844 2024-04-15 12:24:51.749906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_service_account_response.py
--rw-r--r--   0        0        0     2866 2024-04-15 12:24:51.753906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_setting.py
--rw-r--r--   0        0        0     3245 2024-04-15 12:24:51.753906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_source_connection.py
--rw-r--r--   0        0        0      817 2024-04-15 12:24:51.757906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_type_enum.py
--rw-r--r--   0        0        0      777 2024-04-15 12:24:51.757906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_verification_enum.py
--rw-r--r--   0        0        0     5382 2024-04-15 12:24:51.761906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_write_stage.py
--rw-r--r--   0        0        0     4412 2024-04-15 12:24:51.761906 authentik_client-2024.2.2.post1713183880/authentik_client/models/user_write_stage_request.py
--rw-r--r--   0        0        0     3197 2024-04-15 12:24:51.765906 authentik_client-2024.2.2.post1713183880/authentik_client/models/validation_error.py
--rw-r--r--   0        0        0     3589 2024-04-15 12:24:51.769906 authentik_client-2024.2.2.post1713183880/authentik_client/models/version.py
--rw-r--r--   0        0        0     3630 2024-04-15 12:24:51.769906 authentik_client-2024.2.2.post1713183880/authentik_client/models/web_authn_device.py
--rw-r--r--   0        0        0     2577 2024-04-15 12:24:51.773906 authentik_client-2024.2.2.post1713183880/authentik_client/models/web_authn_device_request.py
--rw-r--r--   0        0        0     2562 2024-04-15 12:24:51.777906 authentik_client-2024.2.2.post1713183880/authentik_client/models/web_authn_device_type.py
--rw-r--r--   0        0        0     2669 2024-04-15 12:24:51.777906 authentik_client-2024.2.2.post1713183880/authentik_client/models/web_authn_device_type_request.py
--rw-r--r--   0        0        0     2410 2024-04-15 12:24:51.781906 authentik_client-2024.2.2.post1713183880/authentik_client/models/workers.py
--rw-r--r--   0        0        0        0 2024-04-15 12:24:52.949899 authentik_client-2024.2.2.post1713183880/authentik_client/py.typed
--rw-r--r--   0        0        0     9196 2024-04-15 12:24:52.957899 authentik_client-2024.2.2.post1713183880/authentik_client/rest.py
--rw-r--r--   0        0        0     1936 2024-04-15 12:24:52.945899 authentik_client-2024.2.2.post1713183880/pyproject.toml
--rw-r--r--   0        0        0   144847 1970-01-01 00:00:00.000000 authentik_client-2024.2.2.post1713183880/PKG-INFO
+-rw-r--r--   0        0        0   143895 2024-04-16 17:44:03.282151 authentik_client-2024.2.2.post1713289429/README.md
+-rw-r--r--   0        0        0    48410 2024-04-16 17:44:03.294151 authentik_client-2024.2.2.post1713289429/authentik_client/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/api/__init__.py
+-rw-r--r--   0        0        0    97518 2024-04-16 17:44:02.938151 authentik_client-2024.2.2.post1713289429/authentik_client/api/admin_api.py
+-rw-r--r--   0        0        0   700271 2024-04-16 17:44:02.958151 authentik_client-2024.2.2.post1713289429/authentik_client/api/authenticators_api.py
+-rw-r--r--   0        0        0   701197 2024-04-16 17:44:02.982151 authentik_client-2024.2.2.post1713289429/authentik_client/api/core_api.py
+-rw-r--r--   0        0        0   116805 2024-04-16 17:44:02.994151 authentik_client-2024.2.2.post1713289429/authentik_client/api/crypto_api.py
+-rw-r--r--   0        0        0   107946 2024-04-16 17:44:03.002151 authentik_client-2024.2.2.post1713289429/authentik_client/api/enterprise_api.py
+-rw-r--r--   0        0        0   408008 2024-04-16 17:44:03.014151 authentik_client-2024.2.2.post1713289429/authentik_client/api/events_api.py
+-rw-r--r--   0        0        0   280806 2024-04-16 17:44:03.030151 authentik_client-2024.2.2.post1713289429/authentik_client/api/flows_api.py
+-rw-r--r--   0        0        0   101134 2024-04-16 17:44:03.038151 authentik_client-2024.2.2.post1713289429/authentik_client/api/managed_api.py
+-rw-r--r--   0        0        0   135649 2024-04-16 17:44:03.046151 authentik_client-2024.2.2.post1713289429/authentik_client/api/oauth2_api.py
+-rw-r--r--   0        0        0   413301 2024-04-16 17:44:03.058151 authentik_client-2024.2.2.post1713289429/authentik_client/api/outposts_api.py
+-rw-r--r--   0        0        0   725201 2024-04-16 17:44:03.078151 authentik_client-2024.2.2.post1713289429/authentik_client/api/policies_api.py
+-rw-r--r--   0        0        0   552586 2024-04-16 17:44:03.102151 authentik_client-2024.2.2.post1713289429/authentik_client/api/propertymappings_api.py
+-rw-r--r--   0        0        0   718066 2024-04-16 17:44:03.126151 authentik_client-2024.2.2.post1713289429/authentik_client/api/providers_api.py
+-rw-r--r--   0        0        0   150485 2024-04-16 17:44:03.138152 authentik_client-2024.2.2.post1713289429/authentik_client/api/rac_api.py
+-rw-r--r--   0        0        0   207550 2024-04-16 17:44:03.150151 authentik_client-2024.2.2.post1713289429/authentik_client/api/rbac_api.py
+-rw-r--r--   0        0        0    10391 2024-04-16 17:44:03.166151 authentik_client-2024.2.2.post1713289429/authentik_client/api/root_api.py
+-rw-r--r--   0        0        0    11845 2024-04-16 17:44:03.170151 authentik_client-2024.2.2.post1713289429/authentik_client/api/schema_api.py
+-rw-r--r--   0        0        0  1037225 2024-04-16 17:44:03.198151 authentik_client-2024.2.2.post1713289429/authentik_client/api/sources_api.py
+-rw-r--r--   0        0        0  1945986 2024-04-16 17:44:03.250151 authentik_client-2024.2.2.post1713289429/authentik_client/api/stages_api.py
+-rw-r--r--   0        0        0   157909 2024-04-16 17:44:03.270151 authentik_client-2024.2.2.post1713289429/authentik_client/api/tenants_api.py
+-rw-r--r--   0        0        0    25779 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/api_client.py
+-rw-r--r--   0        0        0      652 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/api_response.py
+-rw-r--r--   0        0        0    14724 2024-04-16 17:44:03.294151 authentik_client-2024.2.2.post1713289429/authentik_client/configuration.py
+-rw-r--r--   0        0        0     5934 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/exceptions.py
+-rw-r--r--   0        0        0    46712 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/models/__init__.py
+-rw-r--r--   0        0        0     4513 2024-04-16 17:44:00.006152 authentik_client-2024.2.2.post1713289429/authentik_client/models/access_denied_challenge.py
+-rw-r--r--   0        0        0     2482 2024-04-16 17:44:00.022152 authentik_client-2024.2.2.post1713289429/authentik_client/models/app.py
+-rw-r--r--   0        0        0     4230 2024-04-16 17:44:00.030152 authentik_client-2024.2.2.post1713289429/authentik_client/models/app_enum.py
+-rw-r--r--   0        0        0     2702 2024-04-16 17:44:00.042152 authentik_client-2024.2.2.post1713289429/authentik_client/models/apple_challenge_response_request.py
+-rw-r--r--   0        0        0     4508 2024-04-16 17:44:00.050152 authentik_client-2024.2.2.post1713289429/authentik_client/models/apple_login_challenge.py
+-rw-r--r--   0        0        0     6686 2024-04-16 17:44:00.062152 authentik_client-2024.2.2.post1713289429/authentik_client/models/application.py
+-rw-r--r--   0        0        0     4473 2024-04-16 17:44:00.070152 authentik_client-2024.2.2.post1713289429/authentik_client/models/application_request.py
+-rw-r--r--   0        0        0      711 2024-04-16 17:44:00.074152 authentik_client-2024.2.2.post1713289429/authentik_client/models/auth_mode_enum.py
+-rw-r--r--   0        0        0      709 2024-04-16 17:44:00.078152 authentik_client-2024.2.2.post1713289429/authentik_client/models/auth_type_enum.py
+-rw-r--r--   0        0        0     5195 2024-04-16 17:44:00.082152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session.py
+-rw-r--r--   0        0        0     3064 2024-04-16 17:44:00.090152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_asn.py
+-rw-r--r--   0        0        0     2826 2024-04-16 17:44:00.094152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_geo_ip.py
+-rw-r--r--   0        0        0     3865 2024-04-16 17:44:00.118152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent.py
+-rw-r--r--   0        0        0     2646 2024-04-16 17:44:00.122152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_device.py
+-rw-r--r--   0        0        0     2792 2024-04-16 17:44:00.130152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_os.py
+-rw-r--r--   0        0        0     2725 2024-04-16 17:44:00.134152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_user_agent.py
+-rw-r--r--   0        0        0      895 2024-04-16 17:44:00.138152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authentication_enum.py
+-rw-r--r--   0        0        0      782 2024-04-16 17:44:00.142152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_attachment_enum.py
+-rw-r--r--   0        0        0     4686 2024-04-16 17:44:00.146152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_challenge.py
+-rw-r--r--   0        0        0     2743 2024-04-16 17:44:00.154152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_challenge_response_request.py
+-rw-r--r--   0        0        0     5327 2024-04-16 17:44:00.158152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage.py
+-rw-r--r--   0        0        0     2768 2024-04-16 17:44:00.166152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_device_import_response.py
+-rw-r--r--   0        0        0     2785 2024-04-16 17:44:00.170152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
+-rw-r--r--   0        0        0     4744 2024-04-16 17:44:00.178152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-16 17:44:00.182152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_challenge.py
+-rw-r--r--   0        0        0     3022 2024-04-16 17:44:00.190152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_challenge_response_request.py
+-rw-r--r--   0        0        0     6409 2024-04-16 17:44:00.194152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_stage.py
+-rw-r--r--   0        0        0     5595 2024-04-16 17:44:00.202152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4474 2024-04-16 17:44:00.210152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_challenge.py
+-rw-r--r--   0        0        0     2761 2024-04-16 17:44:00.214152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_challenge_response_request.py
+-rw-r--r--   0        0        0     5363 2024-04-16 17:44:00.222152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_stage.py
+-rw-r--r--   0        0        0     4392 2024-04-16 17:44:00.226152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4468 2024-04-16 17:44:00.230152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_challenge.py
+-rw-r--r--   0        0        0     2858 2024-04-16 17:44:00.234152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_challenge_response_request.py
+-rw-r--r--   0        0        0     5132 2024-04-16 17:44:00.242152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_stage.py
+-rw-r--r--   0        0        0     4201 2024-04-16 17:44:00.246152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     6722 2024-04-16 17:44:00.254152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validate_stage.py
+-rw-r--r--   0        0        0     4893 2024-04-16 17:44:00.258152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5717 2024-04-16 17:44:00.266152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validation_challenge.py
+-rw-r--r--   0        0        0     3805 2024-04-16 17:44:00.270152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validation_challenge_response_request.py
+-rw-r--r--   0        0        0     4499 2024-04-16 17:44:00.274152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_challenge.py
+-rw-r--r--   0        0        0     2852 2024-04-16 17:44:00.282152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_challenge_response_request.py
+-rw-r--r--   0        0        0     7081 2024-04-16 17:44:00.286152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_stage.py
+-rw-r--r--   0        0        0     5302 2024-04-16 17:44:00.290152 authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     2718 2024-04-16 17:44:00.298152 authentik_client-2024.2.2.post1713289429/authentik_client/models/auto_submit_challenge_response_request.py
+-rw-r--r--   0        0        0     4388 2024-04-16 17:44:00.302152 authentik_client-2024.2.2.post1713289429/authentik_client/models/autosubmit_challenge.py
+-rw-r--r--   0        0        0      950 2024-04-16 17:44:00.306152 authentik_client-2024.2.2.post1713289429/authentik_client/models/backends_enum.py
+-rw-r--r--   0        0        0      748 2024-04-16 17:44:00.310152 authentik_client-2024.2.2.post1713289429/authentik_client/models/binding_type_enum.py
+-rw-r--r--   0        0        0     2995 2024-04-16 17:44:00.314152 authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_file.py
+-rw-r--r--   0        0        0     4453 2024-04-16 17:44:00.318152 authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance.py
+-rw-r--r--   0        0        0     3208 2024-04-16 17:44:00.322152 authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance_request.py
+-rw-r--r--   0        0        0      836 2024-04-16 17:44:00.322152 authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance_status_enum.py
+-rw-r--r--   0        0        0     6255 2024-04-16 17:44:00.326152 authentik_client-2024.2.2.post1713289429/authentik_client/models/brand.py
+-rw-r--r--   0        0        0     6307 2024-04-16 17:44:00.330152 authentik_client-2024.2.2.post1713289429/authentik_client/models/brand_request.py
+-rw-r--r--   0        0        0     2501 2024-04-16 17:44:00.334152 authentik_client-2024.2.2.post1713289429/authentik_client/models/cache.py
+-rw-r--r--   0        0        0      875 2024-04-16 17:44:00.338152 authentik_client-2024.2.2.post1713289429/authentik_client/models/capabilities_enum.py
+-rw-r--r--   0        0        0     4476 2024-04-16 17:44:00.342152 authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_challenge.py
+-rw-r--r--   0        0        0     2797 2024-04-16 17:44:00.346152 authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_challenge_response_request.py
+-rw-r--r--   0        0        0     4438 2024-04-16 17:44:00.350152 authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_stage.py
+-rw-r--r--   0        0        0     3774 2024-04-16 17:44:00.354152 authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_stage_request.py
+-rw-r--r--   0        0        0     2522 2024-04-16 17:44:00.358152 authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_data.py
+-rw-r--r--   0        0        0     2861 2024-04-16 17:44:00.362152 authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_generation_request.py
+-rw-r--r--   0        0        0     6655 2024-04-16 17:44:00.366152 authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_key_pair.py
+-rw-r--r--   0        0        0     2989 2024-04-16 17:44:00.374152 authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_key_pair_request.py
+-rw-r--r--   0        0        0      747 2024-04-16 17:44:00.378152 authentik_client-2024.2.2.post1713289429/authentik_client/models/challenge_choices.py
+-rw-r--r--   0        0        0    24236 2024-04-16 17:44:00.386152 authentik_client-2024.2.2.post1713289429/authentik_client/models/challenge_types.py
+-rw-r--r--   0        0        0      729 2024-04-16 17:44:00.390152 authentik_client-2024.2.2.post1713289429/authentik_client/models/client_type_enum.py
+-rw-r--r--   0        0        0     3539 2024-04-16 17:44:00.394152 authentik_client-2024.2.2.post1713289429/authentik_client/models/config.py
+-rw-r--r--   0        0        0     4021 2024-04-16 17:44:00.398152 authentik_client-2024.2.2.post1713289429/authentik_client/models/connection_token.py
+-rw-r--r--   0        0        0     2662 2024-04-16 17:44:00.402152 authentik_client-2024.2.2.post1713289429/authentik_client/models/connection_token_request.py
+-rw-r--r--   0        0        0     5736 2024-04-16 17:44:00.410152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_challenge.py
+-rw-r--r--   0        0        0     2838 2024-04-16 17:44:00.414152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_challenge_response_request.py
+-rw-r--r--   0        0        0     2513 2024-04-16 17:44:00.418152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_permission.py
+-rw-r--r--   0        0        0     4511 2024-04-16 17:44:00.422152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage.py
+-rw-r--r--   0        0        0      783 2024-04-16 17:44:00.426152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage_mode_enum.py
+-rw-r--r--   0        0        0     3569 2024-04-16 17:44:00.430152 authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage_request.py
+-rw-r--r--   0        0        0     2891 2024-04-16 17:44:00.434152 authentik_client-2024.2.2.post1713289429/authentik_client/models/contextual_flow_info.py
+-rw-r--r--   0        0        0      879 2024-04-16 17:44:00.438152 authentik_client-2024.2.2.post1713289429/authentik_client/models/contextual_flow_info_layout_enum.py
+-rw-r--r--   0        0        0     2657 2024-04-16 17:44:00.442152 authentik_client-2024.2.2.post1713289429/authentik_client/models/coordinate.py
+-rw-r--r--   0        0        0     4704 2024-04-16 17:44:00.446152 authentik_client-2024.2.2.post1713289429/authentik_client/models/current_brand.py
+-rw-r--r--   0        0        0      771 2024-04-16 17:44:00.450152 authentik_client-2024.2.2.post1713289429/authentik_client/models/denied_action_enum.py
+-rw-r--r--   0        0        0     4200 2024-04-16 17:44:00.454152 authentik_client-2024.2.2.post1713289429/authentik_client/models/deny_stage.py
+-rw-r--r--   0        0        0     3230 2024-04-16 17:44:00.458152 authentik_client-2024.2.2.post1713289429/authentik_client/models/deny_stage_request.py
+-rw-r--r--   0        0        0     3522 2024-04-16 17:44:00.462152 authentik_client-2024.2.2.post1713289429/authentik_client/models/device.py
+-rw-r--r--   0        0        0     2657 2024-04-16 17:44:00.470152 authentik_client-2024.2.2.post1713289429/authentik_client/models/device_challenge.py
+-rw-r--r--   0        0        0     2792 2024-04-16 17:44:00.474152 authentik_client-2024.2.2.post1713289429/authentik_client/models/device_challenge_request.py
+-rw-r--r--   0        0        0      780 2024-04-16 17:44:00.478152 authentik_client-2024.2.2.post1713289429/authentik_client/models/device_classes_enum.py
+-rw-r--r--   0        0        0     1244 2024-04-16 17:44:00.482152 authentik_client-2024.2.2.post1713289429/authentik_client/models/digest_algorithm_enum.py
+-rw-r--r--   0        0        0      695 2024-04-16 17:44:00.482152 authentik_client-2024.2.2.post1713289429/authentik_client/models/digits_enum.py
+-rw-r--r--   0        0        0     4969 2024-04-16 17:44:00.486152 authentik_client-2024.2.2.post1713289429/authentik_client/models/docker_service_connection.py
+-rw-r--r--   0        0        0     4087 2024-04-16 17:44:00.490152 authentik_client-2024.2.2.post1713289429/authentik_client/models/docker_service_connection_request.py
+-rw-r--r--   0        0        0     2847 2024-04-16 17:44:00.494152 authentik_client-2024.2.2.post1713289429/authentik_client/models/domain.py
+-rw-r--r--   0        0        0     2746 2024-04-16 17:44:00.498152 authentik_client-2024.2.2.post1713289429/authentik_client/models/domain_request.py
+-rw-r--r--   0        0        0     4155 2024-04-16 17:44:00.506152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_challenge.py
+-rw-r--r--   0        0        0     2681 2024-04-16 17:44:00.510152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_challenge_response_request.py
+-rw-r--r--   0        0        0     4515 2024-04-16 17:44:00.514152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_policy.py
+-rw-r--r--   0        0        0     3237 2024-04-16 17:44:00.518152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_policy_request.py
+-rw-r--r--   0        0        0     4213 2024-04-16 17:44:00.522152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_stage.py
+-rw-r--r--   0        0        0     3232 2024-04-16 17:44:00.526152 authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_stage_request.py
+-rw-r--r--   0        0        0     2720 2024-04-16 17:44:00.530152 authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device.py
+-rw-r--r--   0        0        0     2575 2024-04-16 17:44:00.534152 authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device_enrollment_status.py
+-rw-r--r--   0        0        0     2619 2024-04-16 17:44:00.538152 authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device_request.py
+-rw-r--r--   0        0        0      748 2024-04-16 17:44:00.542152 authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_response_enum.py
+-rw-r--r--   0        0        0     4090 2024-04-16 17:44:00.546152 authentik_client-2024.2.2.post1713289429/authentik_client/models/email_challenge.py
+-rw-r--r--   0        0        0     2770 2024-04-16 17:44:00.554152 authentik_client-2024.2.2.post1713289429/authentik_client/models/email_challenge_response_request.py
+-rw-r--r--   0        0        0     5902 2024-04-16 17:44:00.558152 authentik_client-2024.2.2.post1713289429/authentik_client/models/email_stage.py
+-rw-r--r--   0        0        0     5121 2024-04-16 17:44:00.562152 authentik_client-2024.2.2.post1713289429/authentik_client/models/email_stage_request.py
+-rw-r--r--   0        0        0     4707 2024-04-16 17:44:00.566152 authentik_client-2024.2.2.post1713289429/authentik_client/models/endpoint.py
+-rw-r--r--   0        0        0     3678 2024-04-16 17:44:00.574152 authentik_client-2024.2.2.post1713289429/authentik_client/models/endpoint_request.py
+-rw-r--r--   0        0        0     2530 2024-04-16 17:44:00.578152 authentik_client-2024.2.2.post1713289429/authentik_client/models/error_detail.py
+-rw-r--r--   0        0        0     3309 2024-04-16 17:44:00.582152 authentik_client-2024.2.2.post1713289429/authentik_client/models/error_reporting_config.py
+-rw-r--r--   0        0        0     4129 2024-04-16 17:44:00.586152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event.py
+-rw-r--r--   0        0        0     1730 2024-04-16 17:44:00.590152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event_actions.py
+-rw-r--r--   0        0        0     6006 2024-04-16 17:44:00.594152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event_matcher_policy.py
+-rw-r--r--   0        0        0     4807 2024-04-16 17:44:00.598152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event_matcher_policy_request.py
+-rw-r--r--   0        0        0     3990 2024-04-16 17:44:00.602152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event_request.py
+-rw-r--r--   0        0        0     2697 2024-04-16 17:44:00.606152 authentik_client-2024.2.2.post1713289429/authentik_client/models/event_top_per_user.py
+-rw-r--r--   0        0        0     3926 2024-04-16 17:44:00.610152 authentik_client-2024.2.2.post1713289429/authentik_client/models/expiring_base_grant_model.py
+-rw-r--r--   0        0        0     4191 2024-04-16 17:44:00.614152 authentik_client-2024.2.2.post1713289429/authentik_client/models/expression_policy.py
+-rw-r--r--   0        0        0     2992 2024-04-16 17:44:00.618152 authentik_client-2024.2.2.post1713289429/authentik_client/models/expression_policy_request.py
+-rw-r--r--   0        0        0     4524 2024-04-16 17:44:00.622152 authentik_client-2024.2.2.post1713289429/authentik_client/models/extra_role_object_permission.py
+-rw-r--r--   0        0        0     4524 2024-04-16 17:44:00.626152 authentik_client-2024.2.2.post1713289429/authentik_client/models/extra_user_object_permission.py
+-rw-r--r--   0        0        0     2519 2024-04-16 17:44:00.630152 authentik_client-2024.2.2.post1713289429/authentik_client/models/file_path_request.py
+-rw-r--r--   0        0        0     6047 2024-04-16 17:44:00.638152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow.py
+-rw-r--r--   0        0        0    25850 2024-04-16 17:44:00.646152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_challenge_response_request.py
+-rw-r--r--   0        0        0      934 2024-04-16 17:44:00.650152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_designation_enum.py
+-rw-r--r--   0        0        0     2533 2024-04-16 17:44:00.654152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_diagram.py
+-rw-r--r--   0        0        0     4505 2024-04-16 17:44:00.662152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_error_challenge.py
+-rw-r--r--   0        0        0     3111 2024-04-16 17:44:00.670152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_import_result.py
+-rw-r--r--   0        0        0     3418 2024-04-16 17:44:00.678152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_inspection.py
+-rw-r--r--   0        0        0     3875 2024-04-16 17:44:00.686152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_inspector_plan.py
+-rw-r--r--   0        0        0      837 2024-04-16 17:44:00.686152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_layout_enum.py
+-rw-r--r--   0        0        0     4741 2024-04-16 17:44:00.694152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_request.py
+-rw-r--r--   0        0        0     5223 2024-04-16 17:44:00.702152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_set.py
+-rw-r--r--   0        0        0     4459 2024-04-16 17:44:00.710152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_set_request.py
+-rw-r--r--   0        0        0     4763 2024-04-16 17:44:00.718152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_stage_binding.py
+-rw-r--r--   0        0        0     3983 2024-04-16 17:44:00.722152 authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_stage_binding_request.py
+-rw-r--r--   0        0        0     2641 2024-04-16 17:44:00.730152 authentik_client-2024.2.2.post1713289429/authentik_client/models/footer_link.py
+-rw-r--r--   0        0        0     2531 2024-04-16 17:44:00.734152 authentik_client-2024.2.2.post1713289429/authentik_client/models/generic_error.py
+-rw-r--r--   0        0        0      865 2024-04-16 17:44:00.738152 authentik_client-2024.2.2.post1713289429/authentik_client/models/geoip_binding_enum.py
+-rw-r--r--   0        0        0     5445 2024-04-16 17:44:00.746152 authentik_client-2024.2.2.post1713289429/authentik_client/models/group.py
+-rw-r--r--   0        0        0     4209 2024-04-16 17:44:00.750152 authentik_client-2024.2.2.post1713289429/authentik_client/models/group_member.py
+-rw-r--r--   0        0        0     4006 2024-04-16 17:44:00.758152 authentik_client-2024.2.2.post1713289429/authentik_client/models/group_member_request.py
+-rw-r--r--   0        0        0     3347 2024-04-16 17:44:00.766152 authentik_client-2024.2.2.post1713289429/authentik_client/models/group_request.py
+-rw-r--r--   0        0        0     6080 2024-04-16 17:44:00.770152 authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_challenge.py
+-rw-r--r--   0        0        0     3174 2024-04-16 17:44:00.778152 authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_challenge_response_request.py
+-rw-r--r--   0        0        0     7503 2024-04-16 17:44:00.786152 authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_stage.py
+-rw-r--r--   0        0        0     6533 2024-04-16 17:44:00.794152 authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_stage_request.py
+-rw-r--r--   0        0        0     2438 2024-04-16 17:44:00.798152 authentik_client-2024.2.2.post1713289429/authentik_client/models/install_id.py
+-rw-r--r--   0        0        0      771 2024-04-16 17:44:00.802152 authentik_client-2024.2.2.post1713289429/authentik_client/models/intent_enum.py
+-rw-r--r--   0        0        0      800 2024-04-16 17:44:00.802152 authentik_client-2024.2.2.post1713289429/authentik_client/models/invalid_response_action_enum.py
+-rw-r--r--   0        0        0     4878 2024-04-16 17:44:00.810152 authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation.py
+-rw-r--r--   0        0        0     3895 2024-04-16 17:44:00.818152 authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_request.py
+-rw-r--r--   0        0        0     4508 2024-04-16 17:44:00.826152 authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_stage.py
+-rw-r--r--   0        0        0     3527 2024-04-16 17:44:00.834152 authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_stage_request.py
+-rw-r--r--   0        0        0      729 2024-04-16 17:44:00.838152 authentik_client-2024.2.2.post1713289429/authentik_client/models/issuer_mode_enum.py
+-rw-r--r--   0        0        0     4386 2024-04-16 17:44:00.842152 authentik_client-2024.2.2.post1713289429/authentik_client/models/kubernetes_service_connection.py
+-rw-r--r--   0        0        0     3454 2024-04-16 17:44:00.846152 authentik_client-2024.2.2.post1713289429/authentik_client/models/kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     2811 2024-04-16 17:44:00.858152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_debug.py
+-rw-r--r--   0        0        0     5765 2024-04-16 17:44:00.862152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_outpost_config.py
+-rw-r--r--   0        0        0     4378 2024-04-16 17:44:00.866152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_property_mapping.py
+-rw-r--r--   0        0        0     3478 2024-04-16 17:44:00.874152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     8694 2024-04-16 17:44:00.878152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_provider.py
+-rw-r--r--   0        0        0     6192 2024-04-16 17:44:00.882152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_provider_request.py
+-rw-r--r--   0        0        0    11791 2024-04-16 17:44:00.890152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_source.py
+-rw-r--r--   0        0        0     9542 2024-04-16 17:44:00.898152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_source_request.py
+-rw-r--r--   0        0        0     3129 2024-04-16 17:44:00.902152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_sync_status.py
+-rw-r--r--   0        0        0      726 2024-04-16 17:44:00.850152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ldapapi_access_mode.py
+-rw-r--r--   0        0        0     3278 2024-04-16 17:44:00.910152 authentik_client-2024.2.2.post1713289429/authentik_client/models/license.py
+-rw-r--r--   0        0        0     2897 2024-04-16 17:44:00.914152 authentik_client-2024.2.2.post1713289429/authentik_client/models/license_forecast.py
+-rw-r--r--   0        0        0     2509 2024-04-16 17:44:00.922152 authentik_client-2024.2.2.post1713289429/authentik_client/models/license_request.py
+-rw-r--r--   0        0        0     3222 2024-04-16 17:44:00.926152 authentik_client-2024.2.2.post1713289429/authentik_client/models/license_summary.py
+-rw-r--r--   0        0        0     2411 2024-04-16 17:44:00.930152 authentik_client-2024.2.2.post1713289429/authentik_client/models/link.py
+-rw-r--r--   0        0        0     2882 2024-04-16 17:44:00.934152 authentik_client-2024.2.2.post1713289429/authentik_client/models/log_event.py
+-rw-r--r--   0        0        0      843 2024-04-16 17:44:00.934152 authentik_client-2024.2.2.post1713289429/authentik_client/models/log_level_enum.py
+-rw-r--r--   0        0        0     6520 2024-04-16 17:44:00.938152 authentik_client-2024.2.2.post1713289429/authentik_client/models/login_challenge_types.py
+-rw-r--r--   0        0        0     4171 2024-04-16 17:44:00.942152 authentik_client-2024.2.2.post1713289429/authentik_client/models/login_metrics.py
+-rw-r--r--   0        0        0     3192 2024-04-16 17:44:00.942152 authentik_client-2024.2.2.post1713289429/authentik_client/models/login_source.py
+-rw-r--r--   0        0        0     2513 2024-04-16 17:44:00.946152 authentik_client-2024.2.2.post1713289429/authentik_client/models/metadata.py
+-rw-r--r--   0        0        0     7604 2024-04-16 17:44:00.950152 authentik_client-2024.2.2.post1713289429/authentik_client/models/model_enum.py
+-rw-r--r--   0        0        0     9828 2024-04-16 17:44:00.954152 authentik_client-2024.2.2.post1713289429/authentik_client/models/model_request.py
+-rw-r--r--   0        0        0     1559 2024-04-16 17:44:00.954152 authentik_client-2024.2.2.post1713289429/authentik_client/models/name_id_policy_enum.py
+-rw-r--r--   0        0        0      831 2024-04-16 17:44:00.958152 authentik_client-2024.2.2.post1713289429/authentik_client/models/network_binding_enum.py
+-rw-r--r--   0        0        0      764 2024-04-16 17:44:00.958152 authentik_client-2024.2.2.post1713289429/authentik_client/models/not_configured_action_enum.py
+-rw-r--r--   0        0        0     3479 2024-04-16 17:44:00.962152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification.py
+-rw-r--r--   0        0        0     2858 2024-04-16 17:44:00.966152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_request.py
+-rw-r--r--   0        0        0     4010 2024-04-16 17:44:00.966152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_rule.py
+-rw-r--r--   0        0        0     3549 2024-04-16 17:44:00.970152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_rule_request.py
+-rw-r--r--   0        0        0     3760 2024-04-16 17:44:00.974152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport.py
+-rw-r--r--   0        0        0      818 2024-04-16 17:44:00.974152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_mode_enum.py
+-rw-r--r--   0        0        0     3500 2024-04-16 17:44:00.978152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_request.py
+-rw-r--r--   0        0        0     2503 2024-04-16 17:44:00.982152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_test.py
+-rw-r--r--   0        0        0     2707 2024-04-16 17:44:00.986152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_webhook_mapping.py
+-rw-r--r--   0        0        0     2717 2024-04-16 17:44:00.990152 authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     8888 2024-04-16 17:44:00.994152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider.py
+-rw-r--r--   0        0        0     6654 2024-04-16 17:44:00.998152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider_request.py
+-rw-r--r--   0        0        0     3482 2024-04-16 17:44:01.002152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider_setup_urls.py
+-rw-r--r--   0        0        0     4164 2024-04-16 17:44:01.006152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_challenge.py
+-rw-r--r--   0        0        0     2846 2024-04-16 17:44:01.010152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_challenge_response_request.py
+-rw-r--r--   0        0        0     4213 2024-04-16 17:44:01.014152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_finish_challenge.py
+-rw-r--r--   0        0        0     2816 2024-04-16 17:44:01.018152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
+-rw-r--r--   0        0        0    10563 2024-04-16 17:44:01.022152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_source.py
+-rw-r--r--   0        0        0     8013 2024-04-16 17:44:01.026152 authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_source_request.py
+-rw-r--r--   0        0        0     3922 2024-04-16 17:44:01.030152 authentik_client-2024.2.2.post1713289429/authentik_client/models/open_id_connect_configuration.py
+-rw-r--r--   0        0        0     5545 2024-04-16 17:44:01.034152 authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost.py
+-rw-r--r--   0        0        0     2541 2024-04-16 17:44:01.038152 authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_default_config.py
+-rw-r--r--   0        0        0     3755 2024-04-16 17:44:01.042152 authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_health.py
+-rw-r--r--   0        0        0     4050 2024-04-16 17:44:01.042152 authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_request.py
+-rw-r--r--   0        0        0      752 2024-04-16 17:44:01.046152 authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_type_enum.py
+-rw-r--r--   0        0        0     3322 2024-04-16 17:44:01.050152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_application_list.py
+-rw-r--r--   0        0        0     3395 2024-04-16 17:44:01.050152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticated_session_list.py
+-rw-r--r--   0        0        0     3404 2024-04-16 17:44:01.054152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_duo_stage_list.py
+-rw-r--r--   0        0        0     3404 2024-04-16 17:44:01.058152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_sms_stage_list.py
+-rw-r--r--   0        0        0     3428 2024-04-16 17:44:01.062152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_static_stage_list.py
+-rw-r--r--   0        0        0     3412 2024-04-16 17:44:01.066152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_totp_stage_list.py
+-rw-r--r--   0        0        0     3444 2024-04-16 17:44:01.070152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_validate_stage_list.py
+-rw-r--r--   0        0        0     3445 2024-04-16 17:44:01.070152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
+-rw-r--r--   0        0        0     3371 2024-04-16 17:44:01.074152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_blueprint_instance_list.py
+-rw-r--r--   0        0        0     3274 2024-04-16 17:44:01.078152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_brand_list.py
+-rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.082152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_captcha_stage_list.py
+-rw-r--r--   0        0        0     3380 2024-04-16 17:44:01.082152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_certificate_key_pair_list.py
+-rw-r--r--   0        0        0     3355 2024-04-16 17:44:01.086152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_connection_token_list.py
+-rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.090152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_consent_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-16 17:44:01.094152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_deny_stage_list.py
+-rw-r--r--   0        0        0     3420 2024-04-16 17:44:01.094152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_docker_service_connection_list.py
+-rw-r--r--   0        0        0     3282 2024-04-16 17:44:01.098152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_domain_list.py
+-rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.102152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_dummy_policy_list.py
+-rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.102152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_dummy_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-16 17:44:01.106152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_duo_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.110152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_email_stage_list.py
+-rw-r--r--   0        0        0     3298 2024-04-16 17:44:01.114152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_endpoint_list.py
+-rw-r--r--   0        0        0     3274 2024-04-16 17:44:01.114152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_event_list.py
+-rw-r--r--   0        0        0     3380 2024-04-16 17:44:01.118152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_event_matcher_policy_list.py
+-rw-r--r--   0        0        0     3413 2024-04-16 17:44:01.122152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_expiring_base_grant_model_list.py
+-rw-r--r--   0        0        0     3363 2024-04-16 17:44:01.126152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_expression_policy_list.py
+-rw-r--r--   0        0        0     3437 2024-04-16 17:44:01.126152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_extra_role_object_permission_list.py
+-rw-r--r--   0        0        0     3437 2024-04-16 17:44:01.130152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_extra_user_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-16 17:44:01.134152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_flow_list.py
+-rw-r--r--   0        0        0     3364 2024-04-16 17:44:01.138152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_flow_stage_binding_list.py
+-rw-r--r--   0        0        0     3274 2024-04-16 17:44:01.138152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_group_list.py
+-rw-r--r--   0        0        0     3387 2024-04-16 17:44:01.142152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_identification_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-16 17:44:01.146152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_invitation_list.py
+-rw-r--r--   0        0        0     3355 2024-04-16 17:44:01.150152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_invitation_stage_list.py
+-rw-r--r--   0        0        0     3452 2024-04-16 17:44:01.154152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_kubernetes_service_connection_list.py
+-rw-r--r--   0        0        0     3372 2024-04-16 17:44:01.154152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_outpost_config_list.py
+-rw-r--r--   0        0        0     3388 2024-04-16 17:44:01.158152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.162152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.166152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-16 17:44:01.170152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_license_list.py
+-rw-r--r--   0        0        0     3330 2024-04-16 17:44:01.170152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_list.py
+-rw-r--r--   0        0        0     3363 2024-04-16 17:44:01.174152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_rule_list.py
+-rw-r--r--   0        0        0     3403 2024-04-16 17:44:01.178152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_transport_list.py
+-rw-r--r--   0        0        0     3444 2024-04-16 17:44:01.182152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_webhook_mapping_list.py
+-rw-r--r--   0        0        0     3348 2024-04-16 17:44:01.182152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_o_auth2_provider_list.py
+-rw-r--r--   0        0        0     3324 2024-04-16 17:44:01.186152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_o_auth_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-16 17:44:01.190152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_outpost_list.py
+-rw-r--r--   0        0        0     3396 2024-04-16 17:44:01.194152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_expiry_policy_list.py
+-rw-r--r--   0        0        0     3347 2024-04-16 17:44:01.198152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_policy_list.py
+-rw-r--r--   0        0        0     3339 2024-04-16 17:44:01.202152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-16 17:44:01.206152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_permission_list.py
+-rw-r--r--   0        0        0     3396 2024-04-16 17:44:01.214152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_plex_source_connection_list.py
+-rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.218152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_plex_source_list.py
+-rw-r--r--   0        0        0     3339 2024-04-16 17:44:01.222152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_policy_binding_list.py
+-rw-r--r--   0        0        0     3282 2024-04-16 17:44:01.226152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_policy_list.py
+-rw-r--r--   0        0        0     3282 2024-04-16 17:44:01.230152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_prompt_list.py
+-rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.234152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_prompt_stage_list.py
+-rw-r--r--   0        0        0     3355 2024-04-16 17:44:01.238152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_property_mapping_list.py
+-rw-r--r--   0        0        0     3298 2024-04-16 17:44:01.238152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-16 17:44:01.242152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_proxy_outpost_config_list.py
+-rw-r--r--   0        0        0     3339 2024-04-16 17:44:01.246152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_proxy_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-16 17:44:01.250152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_rac_property_mapping_list.py
+-rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.254152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_rac_provider_list.py
+-rw-r--r--   0        0        0     3388 2024-04-16 17:44:01.254152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_radius_outpost_config_list.py
+-rw-r--r--   0        0        0     3347 2024-04-16 17:44:01.258152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_radius_provider_list.py
+-rw-r--r--   0        0        0     3314 2024-04-16 17:44:01.262152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_reputation_list.py
+-rw-r--r--   0        0        0     3363 2024-04-16 17:44:01.266152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_reputation_policy_list.py
+-rw-r--r--   0        0        0     3461 2024-04-16 17:44:01.266152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_role_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-16 17:44:01.270152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_role_list.py
+-rw-r--r--   0        0        0     3388 2024-04-16 17:44:01.274152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.278152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.282152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.286152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.286152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_provider_list.py
+-rw-r--r--   0        0        0     3356 2024-04-16 17:44:01.290152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_group_list.py
+-rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.294152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_list.py
+-rw-r--r--   0        0        0     3348 2024-04-16 17:44:01.298152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_user_list.py
+-rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.306152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scope_mapping_list.py
+-rw-r--r--   0        0        0     3371 2024-04-16 17:44:01.310152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_service_connection_list.py
+-rw-r--r--   0        0        0     3307 2024-04-16 17:44:01.302152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_sms_device_list.py
+-rw-r--r--   0        0        0     3282 2024-04-16 17:44:01.314152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.318152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_source_stage_list.py
+-rw-r--r--   0        0        0     3274 2024-04-16 17:44:01.322152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_stage_list.py
+-rw-r--r--   0        0        0     3331 2024-04-16 17:44:01.322152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_static_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.326152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_system_task_list.py
+-rw-r--r--   0        0        0     3282 2024-04-16 17:44:01.334152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_tenant_list.py
+-rw-r--r--   0        0        0     3274 2024-04-16 17:44:01.338152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_token_list.py
+-rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.342152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_token_model_list.py
+-rw-r--r--   0        0        0     3315 2024-04-16 17:44:01.330152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_totp_device_list.py
+-rw-r--r--   0        0        0     3461 2024-04-16 17:44:01.342152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3323 2024-04-16 17:44:01.346152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_consent_list.py
+-rw-r--r--   0        0        0     3356 2024-04-16 17:44:01.350152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_delete_stage_list.py
+-rw-r--r--   0        0        0     3266 2024-04-16 17:44:01.354152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_list.py
+-rw-r--r--   0        0        0     3348 2024-04-16 17:44:01.358152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_login_stage_list.py
+-rw-r--r--   0        0        0     3356 2024-04-16 17:44:01.362152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_logout_stage_list.py
+-rw-r--r--   0        0        0     3438 2024-04-16 17:44:01.366152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_o_auth_source_connection_list.py
+-rw-r--r--   0        0        0     3429 2024-04-16 17:44:01.370152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_saml_source_connection_list.py
+-rw-r--r--   0        0        0     3396 2024-04-16 17:44:01.370152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_source_connection_list.py
+-rw-r--r--   0        0        0     3348 2024-04-16 17:44:01.374152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_write_stage_list.py
+-rw-r--r--   0        0        0     3348 2024-04-16 17:44:01.378152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_web_authn_device_list.py
+-rw-r--r--   0        0        0     3381 2024-04-16 17:44:01.382152 authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_web_authn_device_type_list.py
+-rw-r--r--   0        0        0     3076 2024-04-16 17:44:01.386152 authentik_client-2024.2.2.post1713289429/authentik_client/models/pagination.py
+-rw-r--r--   0        0        0     4454 2024-04-16 17:44:01.390152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_challenge.py
+-rw-r--r--   0        0        0     2819 2024-04-16 17:44:01.390152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_challenge_response_request.py
+-rw-r--r--   0        0        0     4377 2024-04-16 17:44:01.394152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_expiry_policy.py
+-rw-r--r--   0        0        0     3099 2024-04-16 17:44:01.398152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_expiry_policy_request.py
+-rw-r--r--   0        0        0     6428 2024-04-16 17:44:01.398152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_policy.py
+-rw-r--r--   0        0        0     5239 2024-04-16 17:44:01.402152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_policy_request.py
+-rw-r--r--   0        0        0     5274 2024-04-16 17:44:01.402152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_stage.py
+-rw-r--r--   0        0        0     4264 2024-04-16 17:44:01.406152 authentik_client-2024.2.2.post1713289429/authentik_client/models/password_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-16 17:44:01.410152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_application_request.py
+-rw-r--r--   0        0        0     4833 2024-04-16 17:44:01.414152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     5701 2024-04-16 17:44:01.414152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4430 2024-04-16 17:44:01.418152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4256 2024-04-16 17:44:01.422152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     4931 2024-04-16 17:44:01.422152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5340 2024-04-16 17:44:01.426152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     3246 2024-04-16 17:44:01.430152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_blueprint_instance_request.py
+-rw-r--r--   0        0        0     6352 2024-04-16 17:44:01.430152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_brand_request.py
+-rw-r--r--   0        0        0     3860 2024-04-16 17:44:01.434152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_captcha_stage_request.py
+-rw-r--r--   0        0        0     3051 2024-04-16 17:44:01.434152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_certificate_key_pair_request.py
+-rw-r--r--   0        0        0     2717 2024-04-16 17:44:01.438152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_connection_token_request.py
+-rw-r--r--   0        0        0     3607 2024-04-16 17:44:01.438152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_consent_stage_request.py
+-rw-r--r--   0        0        0     3268 2024-04-16 17:44:01.442152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_deny_stage_request.py
+-rw-r--r--   0        0        0     4149 2024-04-16 17:44:01.446152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_docker_service_connection_request.py
+-rw-r--r--   0        0        0     2801 2024-04-16 17:44:01.446152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_domain_request.py
+-rw-r--r--   0        0        0     3275 2024-04-16 17:44:01.450152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_dummy_policy_request.py
+-rw-r--r--   0        0        0     3270 2024-04-16 17:44:01.454152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_dummy_stage_request.py
+-rw-r--r--   0        0        0     2674 2024-04-16 17:44:01.454152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_duo_device_request.py
+-rw-r--r--   0        0        0     5159 2024-04-16 17:44:01.458152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_email_stage_request.py
+-rw-r--r--   0        0        0     3784 2024-04-16 17:44:01.462152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_endpoint_request.py
+-rw-r--r--   0        0        0     4845 2024-04-16 17:44:01.466152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_event_matcher_policy_request.py
+-rw-r--r--   0        0        0     4045 2024-04-16 17:44:01.474152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_event_request.py
+-rw-r--r--   0        0        0     3047 2024-04-16 17:44:01.478152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_expression_policy_request.py
+-rw-r--r--   0        0        0     4903 2024-04-16 17:44:01.482152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_flow_request.py
+-rw-r--r--   0        0        0     4055 2024-04-16 17:44:01.486152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_flow_stage_binding_request.py
+-rw-r--r--   0        0        0     3385 2024-04-16 17:44:01.486152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_group_request.py
+-rw-r--r--   0        0        0     6571 2024-04-16 17:44:01.490152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_identification_stage_request.py
+-rw-r--r--   0        0        0     3985 2024-04-16 17:44:01.494152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_invitation_request.py
+-rw-r--r--   0        0        0     3565 2024-04-16 17:44:01.498152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_invitation_stage_request.py
+-rw-r--r--   0        0        0     3492 2024-04-16 17:44:01.502152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     3550 2024-04-16 17:44:01.502152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     6254 2024-04-16 17:44:01.506152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_provider_request.py
+-rw-r--r--   0        0        0     9697 2024-04-16 17:44:01.510152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_source_request.py
+-rw-r--r--   0        0        0     2557 2024-04-16 17:44:01.514152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_license_request.py
+-rw-r--r--   0        0        0     2879 2024-04-16 17:44:01.514152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_request.py
+-rw-r--r--   0        0        0     3587 2024-04-16 17:44:01.518152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_rule_request.py
+-rw-r--r--   0        0        0     3538 2024-04-16 17:44:01.522152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_transport_request.py
+-rw-r--r--   0        0        0     2782 2024-04-16 17:44:01.526152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     6716 2024-04-16 17:44:01.530152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_o_auth2_provider_request.py
+-rw-r--r--   0        0        0     8185 2024-04-16 17:44:01.534152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_o_auth_source_request.py
+-rw-r--r--   0        0        0     4139 2024-04-16 17:44:01.534152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_outpost_request.py
+-rw-r--r--   0        0        0     3154 2024-04-16 17:44:01.538152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_expiry_policy_request.py
+-rw-r--r--   0        0        0     5277 2024-04-16 17:44:01.542152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_policy_request.py
+-rw-r--r--   0        0        0     4326 2024-04-16 17:44:01.546152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_stage_request.py
+-rw-r--r--   0        0        0     2922 2024-04-16 17:44:01.550152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_permission_assign_request.py
+-rw-r--r--   0        0        0     2784 2024-04-16 17:44:01.550152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_plex_source_connection_request.py
+-rw-r--r--   0        0        0     5905 2024-04-16 17:44:01.554152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_plex_source_request.py
+-rw-r--r--   0        0        0     4286 2024-04-16 17:44:01.558152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_policy_binding_request.py
+-rw-r--r--   0        0        0     5023 2024-04-16 17:44:01.562152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_prompt_request.py
+-rw-r--r--   0        0        0     3406 2024-04-16 17:44:01.566152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_prompt_stage_request.py
+-rw-r--r--   0        0        0     6907 2024-04-16 17:44:01.570152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_proxy_provider_request.py
+-rw-r--r--   0        0        0     3495 2024-04-16 17:44:01.570152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_rac_property_mapping_request.py
+-rw-r--r--   0        0        0     4413 2024-04-16 17:44:01.574152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_rac_provider_request.py
+-rw-r--r--   0        0        0     4563 2024-04-16 17:44:01.578152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_radius_provider_request.py
+-rw-r--r--   0        0        0     3276 2024-04-16 17:44:01.582152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_reputation_policy_request.py
+-rw-r--r--   0        0        0     2565 2024-04-16 17:44:01.582152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_role_request.py
+-rw-r--r--   0        0        0     3901 2024-04-16 17:44:01.586152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_property_mapping_request.py
+-rw-r--r--   0        0        0     7539 2024-04-16 17:44:01.590152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_provider_request.py
+-rw-r--r--   0        0        0     8676 2024-04-16 17:44:01.590152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_source_request.py
+-rw-r--r--   0        0        0     3364 2024-04-16 17:44:01.594152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_mapping_request.py
+-rw-r--r--   0        0        0     3888 2024-04-16 17:44:01.594152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_provider_request.py
+-rw-r--r--   0        0        0     3095 2024-04-16 17:44:01.598152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_group_request.py
+-rw-r--r--   0        0        0     3829 2024-04-16 17:44:01.602152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_request.py
+-rw-r--r--   0        0        0     3098 2024-04-16 17:44:01.602152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_user_request.py
+-rw-r--r--   0        0        0     3819 2024-04-16 17:44:01.610152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scope_mapping_request.py
+-rw-r--r--   0        0        0     5079 2024-04-16 17:44:01.610152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_settings_request.py
+-rw-r--r--   0        0        0     2674 2024-04-16 17:44:01.606152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_sms_device_request.py
+-rw-r--r--   0        0        0     3562 2024-04-16 17:44:01.614152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_source_stage_request.py
+-rw-r--r--   0        0        0     2686 2024-04-16 17:44:01.614152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_static_device_request.py
+-rw-r--r--   0        0        0     2820 2024-04-16 17:44:01.618152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_tenant_request.py
+-rw-r--r--   0        0        0     4419 2024-04-16 17:44:01.622152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_token_request.py
+-rw-r--r--   0        0        0     2678 2024-04-16 17:44:01.618152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_totp_device_request.py
+-rw-r--r--   0        0        0     3167 2024-04-16 17:44:01.626152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_delete_stage_request.py
+-rw-r--r--   0        0        0     4766 2024-04-16 17:44:01.626152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_login_stage_request.py
+-rw-r--r--   0        0        0     3167 2024-04-16 17:44:01.630152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_logout_stage_request.py
+-rw-r--r--   0        0        0     3109 2024-04-16 17:44:01.630152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3934 2024-04-16 17:44:01.634152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_request.py
+-rw-r--r--   0        0        0     2733 2024-04-16 17:44:01.634152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     4450 2024-04-16 17:44:01.638152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_write_stage_request.py
+-rw-r--r--   0        0        0     2625 2024-04-16 17:44:01.642152 authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_web_authn_device_request.py
+-rw-r--r--   0        0        0     3548 2024-04-16 17:44:01.642152 authentik_client-2024.2.2.post1713289429/authentik_client/models/permission.py
+-rw-r--r--   0        0        0     2884 2024-04-16 17:44:01.646152 authentik_client-2024.2.2.post1713289429/authentik_client/models/permission_assign_request.py
+-rw-r--r--   0        0        0     4315 2024-04-16 17:44:01.646152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_authentication_challenge.py
+-rw-r--r--   0        0        0     2726 2024-04-16 17:44:01.650152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_authentication_challenge_response_request.py
+-rw-r--r--   0        0        0     7752 2024-04-16 17:44:01.654152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source.py
+-rw-r--r--   0        0        0     3265 2024-04-16 17:44:01.654152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_connection.py
+-rw-r--r--   0        0        0     2719 2024-04-16 17:44:01.658152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_connection_request.py
+-rw-r--r--   0        0        0     5760 2024-04-16 17:44:01.662152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_request.py
+-rw-r--r--   0        0        0     2576 2024-04-16 17:44:01.666152 authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_token_redeem_request.py
+-rw-r--r--   0        0        0     4055 2024-04-16 17:44:01.670152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy.py
+-rw-r--r--   0        0        0     5643 2024-04-16 17:44:01.670152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_binding.py
+-rw-r--r--   0        0        0     4231 2024-04-16 17:44:01.674152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_binding_request.py
+-rw-r--r--   0        0        0      711 2024-04-16 17:44:01.674152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_engine_mode.py
+-rw-r--r--   0        0        0     2817 2024-04-16 17:44:01.678152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_request.py
+-rw-r--r--   0        0        0     2583 2024-04-16 17:44:01.678152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_test_request.py
+-rw-r--r--   0        0        0     3281 2024-04-16 17:44:01.682152 authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_test_result.py
+-rw-r--r--   0        0        0     4885 2024-04-16 17:44:01.686152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt.py
+-rw-r--r--   0        0        0     4649 2024-04-16 17:44:01.690152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_challenge.py
+-rw-r--r--   0        0        0     3325 2024-04-16 17:44:01.690152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_challenge_response_request.py
+-rw-r--r--   0        0        0     4927 2024-04-16 17:44:01.694152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_request.py
+-rw-r--r--   0        0        0     4321 2024-04-16 17:44:01.698152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_stage.py
+-rw-r--r--   0        0        0     3351 2024-04-16 17:44:01.698152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_stage_request.py
+-rw-r--r--   0        0        0     1185 2024-04-16 17:44:01.702152 authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_type_enum.py
+-rw-r--r--   0        0        0     4264 2024-04-16 17:44:01.702152 authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping.py
+-rw-r--r--   0        0        0     2610 2024-04-16 17:44:01.706152 authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping_preview.py
+-rw-r--r--   0        0        0     2744 2024-04-16 17:44:01.706152 authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping_test_result.py
+-rw-r--r--   0        0        0      715 2024-04-16 17:44:01.706152 authentik_client-2024.2.2.post1713289429/authentik_client/models/protocol_enum.py
+-rw-r--r--   0        0        0     5722 2024-04-16 17:44:01.710152 authentik_client-2024.2.2.post1713289429/authentik_client/models/provider.py
+-rw-r--r--   0        0        0      713 2024-04-16 17:44:01.710152 authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_enum.py
+-rw-r--r--   0        0        0     1314 2024-04-16 17:44:01.714152 authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_model_enum.py
+-rw-r--r--   0        0        0     3397 2024-04-16 17:44:01.714152 authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_request.py
+-rw-r--r--   0        0        0     1009 2024-04-16 17:44:01.714152 authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_type_enum.py
+-rw-r--r--   0        0        0      754 2024-04-16 17:44:01.718152 authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_mode.py
+-rw-r--r--   0        0        0     7819 2024-04-16 17:44:01.718152 authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_outpost_config.py
+-rw-r--r--   0        0        0     9552 2024-04-16 17:44:01.722152 authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_provider.py
+-rw-r--r--   0        0        0     6828 2024-04-16 17:44:01.722152 authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_provider_request.py
+-rw-r--r--   0        0        0     4407 2024-04-16 17:44:01.726152 authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_property_mapping.py
+-rw-r--r--   0        0        0     3440 2024-04-16 17:44:01.726152 authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_property_mapping_request.py
+-rw-r--r--   0        0        0     6813 2024-04-16 17:44:01.730152 authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_provider.py
+-rw-r--r--   0        0        0     4351 2024-04-16 17:44:01.730152 authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_provider_request.py
+-rw-r--r--   0        0        0     3833 2024-04-16 17:44:01.734152 authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_outpost_config.py
+-rw-r--r--   0        0        0     6924 2024-04-16 17:44:01.734152 authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_provider.py
+-rw-r--r--   0        0        0     4501 2024-04-16 17:44:01.738152 authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_provider_request.py
+-rw-r--r--   0        0        0     4184 2024-04-16 17:44:01.738152 authentik_client-2024.2.2.post1713289429/authentik_client/models/redirect_challenge.py
+-rw-r--r--   0        0        0     3642 2024-04-16 17:44:01.742152 authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation.py
+-rw-r--r--   0        0        0     4516 2024-04-16 17:44:01.746152 authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation_policy.py
+-rw-r--r--   0        0        0     3238 2024-04-16 17:44:01.750152 authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation_policy_request.py
+-rw-r--r--   0        0        0      795 2024-04-16 17:44:01.750152 authentik_client-2024.2.2.post1713289429/authentik_client/models/resident_key_requirement_enum.py
+-rw-r--r--   0        0        0     2618 2024-04-16 17:44:01.750152 authentik_client-2024.2.2.post1713289429/authentik_client/models/role.py
+-rw-r--r--   0        0        0     3333 2024-04-16 17:44:01.754152 authentik_client-2024.2.2.post1713289429/authentik_client/models/role_assigned_object_permission.py
+-rw-r--r--   0        0        0     3293 2024-04-16 17:44:01.758152 authentik_client-2024.2.2.post1713289429/authentik_client/models/role_object_permission.py
+-rw-r--r--   0        0        0     2517 2024-04-16 17:44:01.758152 authentik_client-2024.2.2.post1713289429/authentik_client/models/role_request.py
+-rw-r--r--   0        0        0     2712 2024-04-16 17:44:01.762152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_metadata.py
+-rw-r--r--   0        0        0     4718 2024-04-16 17:44:01.762152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_property_mapping.py
+-rw-r--r--   0        0        0     3829 2024-04-16 17:44:01.766152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_property_mapping_request.py
+-rw-r--r--   0        0        0    11056 2024-04-16 17:44:01.766152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_provider.py
+-rw-r--r--   0        0        0     7460 2024-04-16 17:44:01.770152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_provider_request.py
+-rw-r--r--   0        0        0    10563 2024-04-16 17:44:01.770152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_source.py
+-rw-r--r--   0        0        0     8507 2024-04-16 17:44:01.774152 authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_source_request.py
+-rw-r--r--   0        0        0     4248 2024-04-16 17:44:01.778152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_mapping.py
+-rw-r--r--   0        0        0     3309 2024-04-16 17:44:01.778152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_mapping_request.py
+-rw-r--r--   0        0        0     5454 2024-04-16 17:44:01.782152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_provider.py
+-rw-r--r--   0        0        0     3802 2024-04-16 17:44:01.782152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_provider_request.py
+-rw-r--r--   0        0        0     5999 2024-04-16 17:44:01.786152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source.py
+-rw-r--r--   0        0        0     3369 2024-04-16 17:44:01.786152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_group.py
+-rw-r--r--   0        0        0     3023 2024-04-16 17:44:01.790152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_group_request.py
+-rw-r--r--   0        0        0     3708 2024-04-16 17:44:01.794152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_request.py
+-rw-r--r--   0        0        0     3370 2024-04-16 17:44:01.794152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_user.py
+-rw-r--r--   0        0        0     3026 2024-04-16 17:44:01.798152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_user_request.py
+-rw-r--r--   0        0        0     3131 2024-04-16 17:44:01.802152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_sync_status.py
+-rw-r--r--   0        0        0     4629 2024-04-16 17:44:01.806152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scope_mapping.py
+-rw-r--r--   0        0        0     3740 2024-04-16 17:44:01.810152 authentik_client-2024.2.2.post1713289429/authentik_client/models/scope_mapping_request.py
+-rw-r--r--   0        0        0     2738 2024-04-16 17:44:01.814152 authentik_client-2024.2.2.post1713289429/authentik_client/models/selectable_stage.py
+-rw-r--r--   0        0        0     3773 2024-04-16 17:44:01.814152 authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection.py
+-rw-r--r--   0        0        0     2776 2024-04-16 17:44:01.818152 authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection_request.py
+-rw-r--r--   0        0        0     2731 2024-04-16 17:44:01.818152 authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection_state.py
+-rw-r--r--   0        0        0     3178 2024-04-16 17:44:01.822152 authentik_client-2024.2.2.post1713289429/authentik_client/models/session_user.py
+-rw-r--r--   0        0        0     4931 2024-04-16 17:44:01.826152 authentik_client-2024.2.2.post1713289429/authentik_client/models/settings.py
+-rw-r--r--   0        0        0     5058 2024-04-16 17:44:01.826152 authentik_client-2024.2.2.post1713289429/authentik_client/models/settings_request.py
+-rw-r--r--   0        0        0      733 2024-04-16 17:44:01.830152 authentik_client-2024.2.2.post1713289429/authentik_client/models/severity_enum.py
+-rw-r--r--   0        0        0     4175 2024-04-16 17:44:01.830152 authentik_client-2024.2.2.post1713289429/authentik_client/models/shell_challenge.py
+-rw-r--r--   0        0        0     1492 2024-04-16 17:44:01.834152 authentik_client-2024.2.2.post1713289429/authentik_client/models/signature_algorithm_enum.py
+-rw-r--r--   0        0        0     2906 2024-04-16 17:44:01.802152 authentik_client-2024.2.2.post1713289429/authentik_client/models/sms_device.py
+-rw-r--r--   0        0        0     2619 2024-04-16 17:44:01.806152 authentik_client-2024.2.2.post1713289429/authentik_client/models/sms_device_request.py
+-rw-r--r--   0        0        0     6945 2024-04-16 17:44:01.834152 authentik_client-2024.2.2.post1713289429/authentik_client/models/source.py
+-rw-r--r--   0        0        0     4836 2024-04-16 17:44:01.838152 authentik_client-2024.2.2.post1713289429/authentik_client/models/source_request.py
+-rw-r--r--   0        0        0     4438 2024-04-16 17:44:01.842152 authentik_client-2024.2.2.post1713289429/authentik_client/models/source_stage.py
+-rw-r--r--   0        0        0     3507 2024-04-16 17:44:01.842152 authentik_client-2024.2.2.post1713289429/authentik_client/models/source_stage_request.py
+-rw-r--r--   0        0        0     5355 2024-04-16 17:44:01.846152 authentik_client-2024.2.2.post1713289429/authentik_client/models/source_type.py
+-rw-r--r--   0        0        0      714 2024-04-16 17:44:01.846152 authentik_client-2024.2.2.post1713289429/authentik_client/models/sp_binding_enum.py
+-rw-r--r--   0        0        0     4070 2024-04-16 17:44:01.850152 authentik_client-2024.2.2.post1713289429/authentik_client/models/stage.py
+-rw-r--r--   0        0        0     3437 2024-04-16 17:44:01.854152 authentik_client-2024.2.2.post1713289429/authentik_client/models/stage_prompt.py
+-rw-r--r--   0        0        0     3089 2024-04-16 17:44:01.854152 authentik_client-2024.2.2.post1713289429/authentik_client/models/stage_request.py
+-rw-r--r--   0        0        0     3385 2024-04-16 17:44:01.858152 authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device.py
+-rw-r--r--   0        0        0     2631 2024-04-16 17:44:01.858152 authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_request.py
+-rw-r--r--   0        0        0     2546 2024-04-16 17:44:01.862152 authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_token.py
+-rw-r--r--   0        0        0     2581 2024-04-16 17:44:01.866152 authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_token_request.py
+-rw-r--r--   0        0        0      846 2024-04-16 17:44:01.866152 authentik_client-2024.2.2.post1713289429/authentik_client/models/sub_mode_enum.py
+-rw-r--r--   0        0        0     4463 2024-04-16 17:44:01.870152 authentik_client-2024.2.2.post1713289429/authentik_client/models/system_info.py
+-rw-r--r--   0        0        0     2934 2024-04-16 17:44:01.870152 authentik_client-2024.2.2.post1713289429/authentik_client/models/system_info_runtime.py
+-rw-r--r--   0        0        0     4286 2024-04-16 17:44:01.874152 authentik_client-2024.2.2.post1713289429/authentik_client/models/system_task.py
+-rw-r--r--   0        0        0      789 2024-04-16 17:44:01.874152 authentik_client-2024.2.2.post1713289429/authentik_client/models/system_task_status_enum.py
+-rw-r--r--   0        0        0     2872 2024-04-16 17:44:01.882152 authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant.py
+-rw-r--r--   0        0        0     2589 2024-04-16 17:44:01.886152 authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_admin_group_request_request.py
+-rw-r--r--   0        0        0     2705 2024-04-16 17:44:01.886152 authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_recovery_key_request_request.py
+-rw-r--r--   0        0        0     2599 2024-04-16 17:44:01.890152 authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_recovery_key_response.py
+-rw-r--r--   0        0        0     2765 2024-04-16 17:44:01.894152 authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_request.py
+-rw-r--r--   0        0        0     4802 2024-04-16 17:44:01.894152 authentik_client-2024.2.2.post1713289429/authentik_client/models/token.py
+-rw-r--r--   0        0        0     4198 2024-04-16 17:44:01.898152 authentik_client-2024.2.2.post1713289429/authentik_client/models/token_model.py
+-rw-r--r--   0        0        0     4329 2024-04-16 17:44:01.898152 authentik_client-2024.2.2.post1713289429/authentik_client/models/token_request.py
+-rw-r--r--   0        0        0     2521 2024-04-16 17:44:01.902152 authentik_client-2024.2.2.post1713289429/authentik_client/models/token_set_key_request.py
+-rw-r--r--   0        0        0     2494 2024-04-16 17:44:01.906152 authentik_client-2024.2.2.post1713289429/authentik_client/models/token_view.py
+-rw-r--r--   0        0        0     2724 2024-04-16 17:44:01.878152 authentik_client-2024.2.2.post1713289429/authentik_client/models/totp_device.py
+-rw-r--r--   0        0        0     2623 2024-04-16 17:44:01.882152 authentik_client-2024.2.2.post1713289429/authentik_client/models/totp_device_request.py
+-rw-r--r--   0        0        0     3389 2024-04-16 17:44:01.906152 authentik_client-2024.2.2.post1713289429/authentik_client/models/transaction_application_request.py
+-rw-r--r--   0        0        0     2595 2024-04-16 17:44:01.910152 authentik_client-2024.2.2.post1713289429/authentik_client/models/transaction_application_response.py
+-rw-r--r--   0        0        0     2936 2024-04-16 17:44:01.910152 authentik_client-2024.2.2.post1713289429/authentik_client/models/type_create.py
+-rw-r--r--   0        0        0      730 2024-04-16 17:44:01.914152 authentik_client-2024.2.2.post1713289429/authentik_client/models/ui_theme_enum.py
+-rw-r--r--   0        0        0     2808 2024-04-16 17:44:01.914152 authentik_client-2024.2.2.post1713289429/authentik_client/models/used_by.py
+-rw-r--r--   0        0        0      795 2024-04-16 17:44:01.914152 authentik_client-2024.2.2.post1713289429/authentik_client/models/used_by_action_enum.py
+-rw-r--r--   0        0        0     5459 2024-04-16 17:44:01.918152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user.py
+-rw-r--r--   0        0        0     2458 2024-04-16 17:44:01.922152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_account_request.py
+-rw-r--r--   0        0        0     4946 2024-04-16 17:44:01.922152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_assigned_object_permission.py
+-rw-r--r--   0        0        0     3828 2024-04-16 17:44:01.926152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_consent.py
+-rw-r--r--   0        0        0      811 2024-04-16 17:44:01.926152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_creation_mode_enum.py
+-rw-r--r--   0        0        0     4110 2024-04-16 17:44:01.930152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_delete_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-16 17:44:01.930152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_delete_stage_request.py
+-rw-r--r--   0        0        0      735 2024-04-16 17:44:01.934152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_fields_enum.py
+-rw-r--r--   0        0        0     3909 2024-04-16 17:44:01.934152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_group.py
+-rw-r--r--   0        0        0     4334 2024-04-16 17:44:01.938152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_challenge.py
+-rw-r--r--   0        0        0     2805 2024-04-16 17:44:01.938152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_challenge_response_request.py
+-rw-r--r--   0        0        0     5631 2024-04-16 17:44:01.942152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_stage.py
+-rw-r--r--   0        0        0     4728 2024-04-16 17:44:01.942152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_stage_request.py
+-rw-r--r--   0        0        0     4110 2024-04-16 17:44:01.946152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_logout_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-16 17:44:01.950152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_logout_stage_request.py
+-rw-r--r--   0        0        0      853 2024-04-16 17:44:01.950152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_matching_mode_enum.py
+-rw-r--r--   0        0        0     4160 2024-04-16 17:44:01.950152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_metrics.py
+-rw-r--r--   0        0        0     3188 2024-04-16 17:44:01.954152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_o_auth_source_connection.py
+-rw-r--r--   0        0        0     3054 2024-04-16 17:44:01.954152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3293 2024-04-16 17:44:01.958152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_object_permission.py
+-rw-r--r--   0        0        0     2557 2024-04-16 17:44:01.958152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_password_set_request.py
+-rw-r--r--   0        0        0     2491 2024-04-16 17:44:01.962152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_path.py
+-rw-r--r--   0        0        0     3872 2024-04-16 17:44:01.962152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_request.py
+-rw-r--r--   0        0        0     3107 2024-04-16 17:44:01.966152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_saml_source_connection.py
+-rw-r--r--   0        0        0     2668 2024-04-16 17:44:01.970152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     5465 2024-04-16 17:44:01.974152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_self.py
+-rw-r--r--   0        0        0     2629 2024-04-16 17:44:01.974152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_self_groups.py
+-rw-r--r--   0        0        0     3074 2024-04-16 17:44:01.978152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_service_account_request.py
+-rw-r--r--   0        0        0     2844 2024-04-16 17:44:01.978152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_service_account_response.py
+-rw-r--r--   0        0        0     2866 2024-04-16 17:44:01.982152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_setting.py
+-rw-r--r--   0        0        0     3245 2024-04-16 17:44:01.986152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_source_connection.py
+-rw-r--r--   0        0        0      817 2024-04-16 17:44:01.986152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_type_enum.py
+-rw-r--r--   0        0        0      777 2024-04-16 17:44:01.986152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_verification_enum.py
+-rw-r--r--   0        0        0     5382 2024-04-16 17:44:01.990152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_write_stage.py
+-rw-r--r--   0        0        0     4412 2024-04-16 17:44:01.990152 authentik_client-2024.2.2.post1713289429/authentik_client/models/user_write_stage_request.py
+-rw-r--r--   0        0        0     3197 2024-04-16 17:44:01.994152 authentik_client-2024.2.2.post1713289429/authentik_client/models/validation_error.py
+-rw-r--r--   0        0        0     3589 2024-04-16 17:44:01.998152 authentik_client-2024.2.2.post1713289429/authentik_client/models/version.py
+-rw-r--r--   0        0        0     3630 2024-04-16 17:44:01.998152 authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device.py
+-rw-r--r--   0        0        0     2577 2024-04-16 17:44:02.002152 authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_request.py
+-rw-r--r--   0        0        0     2562 2024-04-16 17:44:02.002152 authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_type.py
+-rw-r--r--   0        0        0     2669 2024-04-16 17:44:02.006152 authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_type_request.py
+-rw-r--r--   0        0        0     2410 2024-04-16 17:44:02.006152 authentik_client-2024.2.2.post1713289429/authentik_client/models/workers.py
+-rw-r--r--   0        0        0        0 2024-04-16 17:44:03.290151 authentik_client-2024.2.2.post1713289429/authentik_client/py.typed
+-rw-r--r--   0        0        0     9196 2024-04-16 17:44:03.298151 authentik_client-2024.2.2.post1713289429/authentik_client/rest.py
+-rw-r--r--   0        0        0     1936 2024-04-16 17:44:03.290151 authentik_client-2024.2.2.post1713289429/pyproject.toml
+-rw-r--r--   0        0        0   144847 1970-01-01 00:00:00.000000 authentik_client-2024.2.2.post1713289429/PKG-INFO
```

### Comparing `authentik_client-2024.2.2.post1713183880/README.md` & `authentik_client-2024.2.2.post1713289429/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.2.2
-- Package version: 2024.2.2-1713183880
+- Package version: 2024.2.2-1713289429
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/__init__.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2024.2.2-1713183880"
+__version__ = "2024.2.2-1713289429"
 
 # import apis into sdk package
 from authentik_client.api.admin_api import AdminApi
 from authentik_client.api.authenticators_api import AuthenticatorsApi
 from authentik_client.api.core_api import CoreApi
 from authentik_client.api.crypto_api import CryptoApi
 from authentik_client.api.enterprise_api import EnterpriseApi
```

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/__init__.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/admin_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/authenticators_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/authenticators_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/core_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/crypto_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/crypto_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/enterprise_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/enterprise_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/events_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/flows_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/flows_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/managed_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/managed_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/oauth2_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/oauth2_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/outposts_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/outposts_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/policies_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/propertymappings_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/propertymappings_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/providers_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/providers_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/rac_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/rac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/rbac_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/rbac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/root_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/root_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/schema_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/sources_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/sources_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/stages_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/stages_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api/tenants_api.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api/tenants_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api_client.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.2.2-1713183880/python'
+        self.user_agent = 'OpenAPI-Generator/2024.2.2-1713289429/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/api_response.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/api_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/configuration.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2024.2.2\n"\
-               "SDK Package Version: 2024.2.2-1713183880".\
+               "SDK Package Version: 2024.2.2-1713289429".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/exceptions.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/__init__.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/access_denied_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/access_denied_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/app.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/app.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/app_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/app_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/apple_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/apple_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/apple_login_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/apple_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/application.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/application.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/application_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/auth_mode_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/auth_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/auth_type_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/auth_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_asn.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_asn.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_geo_ip.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_geo_ip.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_user_agent.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_user_agent_device.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_user_agent_os.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_os.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticated_session_user_agent_user_agent.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticated_session_user_agent_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authentication_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authentication_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_attachment_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_attachment_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_stage_device_import_response.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_device_import_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_duo_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_sms_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_sms_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_sms_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_sms_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_static_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_static_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_static_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_static_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_totp_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_totp_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_totp_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_totp_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_validate_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validate_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_validate_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_validation_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validation_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_validation_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_validation_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_web_authn_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_web_authn_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_web_authn_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/authenticator_web_authn_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/auto_submit_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/auto_submit_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/autosubmit_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/autosubmit_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/backends_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/backends_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/binding_type_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/binding_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/blueprint_file.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_file.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/blueprint_instance.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/blueprint_instance_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/blueprint_instance_status_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/blueprint_instance_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/brand.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/brand_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/cache.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/cache.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/capabilities_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/capabilities_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/captcha_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/captcha_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/captcha_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/captcha_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/certificate_data.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_data.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/certificate_generation_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_generation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/certificate_key_pair.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_key_pair.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/certificate_key_pair_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/challenge_choices.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/challenge_choices.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/challenge_types.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/client_type_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/client_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/config.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/connection_token.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/connection_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/connection_token_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_permission.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_stage_mode_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/consent_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/contextual_flow_info.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/contextual_flow_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/contextual_flow_info_layout_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/contextual_flow_info_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/coordinate.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/coordinate.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/current_brand.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/current_brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/denied_action_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/denied_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/deny_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/deny_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/deny_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/device.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/device_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/device_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/device_challenge_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/device_challenge_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/device_classes_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/device_classes_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/digest_algorithm_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/digest_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/digits_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/digits_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/docker_service_connection.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/docker_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/docker_service_connection_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/domain.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/domain.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/domain_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_policy.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/dummy_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/duo_device.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/duo_device_enrollment_status.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device_enrollment_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/duo_device_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/duo_response_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/duo_response_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/email_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/email_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/email_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/email_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/email_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/email_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/email_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/endpoint.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/endpoint_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/error_detail.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/error_reporting_config.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/error_reporting_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/event.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/event_actions.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/event_actions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/event_matcher_policy.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/event_matcher_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/event_matcher_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/event_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/event_top_per_user.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/event_top_per_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/expiring_base_grant_model.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/expiring_base_grant_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/expression_policy.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/expression_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/expression_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/extra_role_object_permission.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/extra_role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/extra_user_object_permission.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/extra_user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/file_path_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/file_path_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_designation_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_designation_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_diagram.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_diagram.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_error_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_error_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_import_result.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_import_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_inspection.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_inspection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_inspector_plan.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_inspector_plan.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_layout_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_set.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_set.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_set_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_stage_binding.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_stage_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/flow_stage_binding_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/footer_link.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/footer_link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/generic_error.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/generic_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/geoip_binding_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/geoip_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/group.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     pk: StrictStr
     num_pk: StrictInt
     name: Annotated[str, Field(strict=True, max_length=80)]
     is_superuser: Optional[StrictBool] = Field(default=None, description="Users added to this group will be superusers.")
     parent: Optional[StrictStr] = None
     parent_name: Optional[StrictStr]
     users: Optional[List[StrictInt]] = None
-    users_obj: List[GroupMember]
+    users_obj: Optional[List[GroupMember]]
     attributes: Optional[Dict[str, Any]] = None
     roles: Optional[List[StrictStr]] = None
     roles_obj: List[Role]
     __properties: ClassVar[List[str]] = ["pk", "num_pk", "name", "is_superuser", "parent", "parent_name", "users", "users_obj", "attributes", "roles", "roles_obj"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -112,14 +112,19 @@
             _dict['parent'] = None
 
         # set to None if parent_name (nullable) is None
         # and model_fields_set contains the field
         if self.parent_name is None and "parent_name" in self.model_fields_set:
             _dict['parent_name'] = None
 
+        # set to None if users_obj (nullable) is None
+        # and model_fields_set contains the field
+        if self.users_obj is None and "users_obj" in self.model_fields_set:
+            _dict['users_obj'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of Group from a dict"""
         if obj is None:
             return None
```

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/group_member.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/group_member_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/group_member_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/group_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/identification_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/identification_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/identification_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/identification_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/install_id.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/install_id.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/intent_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/intent_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/invalid_response_action_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/invalid_response_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/invitation.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/invitation_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/invitation_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/invitation_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/issuer_mode_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/issuer_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/kubernetes_service_connection.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/kubernetes_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/kubernetes_service_connection_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_debug.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_debug.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_outpost_config.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_property_mapping.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_property_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_provider.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_source.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_source_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/ldap_sync_status.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldap_sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/ldapapi_access_mode.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/ldapapi_access_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/license.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/license.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/license_forecast.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/license_forecast.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/license_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/license_summary.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/license_summary.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/link.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/log_event.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/log_event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/log_level_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/log_level_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/login_challenge_types.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/login_challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/login_metrics.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/login_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/login_source.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/login_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/metadata.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/model_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/model_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/model_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/name_id_policy_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/name_id_policy_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/network_binding_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/network_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/not_configured_action_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/not_configured_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/notification.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_rule.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_rule.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_rule_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_transport.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_transport_mode_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_transport_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_transport_test.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_transport_test.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_webhook_mapping.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_webhook_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/notification_webhook_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth2_provider.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth2_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth2_provider_setup_urls.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth2_provider_setup_urls.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_device_code_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_device_code_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_device_code_finish_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_finish_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_source.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/o_auth_source_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/open_id_connect_configuration.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/open_id_connect_configuration.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/outpost.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/outpost_default_config.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_default_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/outpost_health.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_health.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/outpost_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/outpost_type_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/outpost_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_application_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticated_session_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticated_session_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_duo_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_duo_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_sms_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_sms_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_static_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_static_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_totp_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_totp_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_validate_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_validate_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_authenticator_web_authn_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_authenticator_web_authn_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_blueprint_instance_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_blueprint_instance_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_brand_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_brand_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_captcha_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_captcha_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_certificate_key_pair_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_certificate_key_pair_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_connection_token_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_connection_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_consent_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_consent_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_deny_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_deny_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_docker_service_connection_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_docker_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_domain_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_domain_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_dummy_policy_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_dummy_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_dummy_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_dummy_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_duo_device_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_duo_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_email_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_email_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_endpoint_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_endpoint_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_event_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_event_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_event_matcher_policy_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_event_matcher_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_expiring_base_grant_model_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_expiring_base_grant_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_expression_policy_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_expression_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_extra_role_object_permission_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_extra_role_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_extra_user_object_permission_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_extra_user_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_flow_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_flow_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_flow_stage_binding_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_flow_stage_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_group_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_identification_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_identification_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_invitation_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_invitation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_invitation_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_invitation_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_kubernetes_service_connection_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_kubernetes_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_ldap_outpost_config_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_ldap_property_mapping_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_ldap_provider_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_ldap_source_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_ldap_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_license_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_license_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_notification_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_notification_rule_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_rule_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_notification_transport_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_transport_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_notification_webhook_mapping_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_notification_webhook_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_o_auth2_provider_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_o_auth2_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_o_auth_source_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_o_auth_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_outpost_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_outpost_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_password_expiry_policy_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_expiry_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_password_policy_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_password_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_password_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_permission_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_plex_source_connection_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_plex_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_plex_source_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_plex_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_policy_binding_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_policy_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_policy_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_prompt_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_prompt_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_prompt_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_prompt_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_property_mapping_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_provider_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_proxy_outpost_config_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_proxy_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_proxy_provider_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_proxy_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_rac_property_mapping_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_rac_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_rac_provider_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_rac_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_radius_outpost_config_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_radius_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_radius_provider_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_radius_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_reputation_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_reputation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_reputation_policy_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_reputation_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_role_assigned_object_permission_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_role_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_role_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_role_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_saml_property_mapping_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_saml_provider_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_saml_source_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_saml_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scim_mapping_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scim_provider_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scim_source_group_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scim_source_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scim_source_user_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scim_source_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_scope_mapping_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_scope_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_service_connection_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_sms_device_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_sms_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_source_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_source_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_source_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_static_device_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_static_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_system_task_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_system_task_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_tenant_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_tenant_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_token_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_token_model_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_token_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_totp_device_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_totp_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_assigned_object_permission_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_consent_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_consent_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_delete_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_delete_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_login_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_login_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_logout_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_logout_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_o_auth_source_connection_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_o_auth_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_saml_source_connection_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_saml_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_source_connection_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_user_write_stage_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_user_write_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_web_authn_device_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_web_authn_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/paginated_web_authn_device_type_list.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/paginated_web_authn_device_type_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/pagination.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/pagination.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/password_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/password_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/password_expiry_policy.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_expiry_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/password_expiry_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/password_policy.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/password_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/password_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/password_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_application_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_duo_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_sms_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_static_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_totp_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_validate_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_authenticator_web_authn_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_blueprint_instance_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_brand_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_captcha_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_certificate_key_pair_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_connection_token_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_consent_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_deny_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_docker_service_connection_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_domain_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_dummy_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_dummy_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_duo_device_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_email_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_endpoint_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_event_matcher_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_event_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_expression_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_flow_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_flow_stage_binding_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_group_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_identification_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_invitation_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_invitation_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_kubernetes_service_connection_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_ldap_property_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_ldap_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_ldap_source_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_license_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_notification_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_notification_rule_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_notification_transport_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_notification_webhook_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_o_auth2_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_o_auth_source_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_outpost_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_password_expiry_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_password_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_password_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_permission_assign_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_plex_source_connection_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_plex_source_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_policy_binding_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_prompt_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_prompt_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_proxy_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_rac_property_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_rac_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_radius_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_reputation_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_role_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_saml_property_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_saml_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_saml_source_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scim_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scim_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scim_source_group_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scim_source_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scim_source_user_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scim_source_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_scope_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_settings_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_sms_device_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_source_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_static_device_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_tenant_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_token_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_totp_device_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_delete_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_login_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_logout_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_o_auth_source_connection_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_saml_source_connection_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_user_write_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/patched_web_authn_device_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/patched_web_authn_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/permission.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/permission_assign_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_authentication_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_authentication_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_authentication_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_authentication_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_source.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_source_connection.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_source_connection_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_source_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/plex_token_redeem_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/plex_token_redeem_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/policy.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_binding.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_binding_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_engine_mode.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_engine_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_test_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_test_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/policy_test_result.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/policy_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/prompt_type_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/prompt_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/property_mapping.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/property_mapping_preview.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping_preview.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/property_mapping_test_result.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/property_mapping_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/protocol_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/protocol_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/provider.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/provider_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/provider_model_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/provider_type_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/provider_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/proxy_mode.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/proxy_outpost_config.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/proxy_provider.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/proxy_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/rac_property_mapping.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/rac_property_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/rac_provider.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/rac_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/radius_outpost_config.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/radius_provider.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/radius_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/redirect_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/redirect_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/reputation.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/reputation_policy.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/reputation_policy_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/resident_key_requirement_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/resident_key_requirement_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/role.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/role.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/role_assigned_object_permission.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/role_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/role_object_permission.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/role_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_metadata.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_property_mapping.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_property_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_provider.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_source.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/saml_source_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_mapping.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_provider.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_provider_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source_group.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source_group_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source_user.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_source_user_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_source_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scim_sync_status.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scim_sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scope_mapping.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scope_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/scope_mapping_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/selectable_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/selectable_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/service_connection.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/service_connection_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/service_connection_state.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/service_connection_state.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/session_user.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/session_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/settings.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/settings.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/settings_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/severity_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/severity_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/shell_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/shell_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/signature_algorithm_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/signature_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/sms_device.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/sms_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/sms_device_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/source.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/source_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/source_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/source_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/source_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/source_type.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/source_type.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/sp_binding_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/sp_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/stage_prompt.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/stage_prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/static_device.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/static_device_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/static_device_token.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/static_device_token_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/static_device_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/sub_mode_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/sub_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/system_info.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/system_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/system_info_runtime.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/system_info_runtime.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/system_task.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/system_task.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/system_task_status_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/system_task_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/tenant.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/tenant_admin_group_request_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_admin_group_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/tenant_recovery_key_request_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_recovery_key_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/tenant_recovery_key_response.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_recovery_key_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/tenant_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/token.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/token_model.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/token_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/token_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/token_set_key_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/token_set_key_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/token_view.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/token_view.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/totp_device.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/totp_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/totp_device_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/transaction_application_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/transaction_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/transaction_application_response.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/transaction_application_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/type_create.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/type_create.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/ui_theme_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/ui_theme_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/used_by.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/used_by.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/used_by_action_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/used_by_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     pk: StrictInt
     username: Annotated[str, Field(strict=True, max_length=150)]
     name: StrictStr = Field(description="User's display name.")
     is_active: Optional[StrictBool] = Field(default=None, description="Designates whether this user should be treated as active. Unselect this instead of deleting accounts.")
     last_login: Optional[datetime] = None
     is_superuser: StrictBool
     groups: Optional[List[StrictStr]] = None
-    groups_obj: List[UserGroup]
+    groups_obj: Optional[List[UserGroup]]
     email: Optional[Annotated[str, Field(strict=True, max_length=254)]] = None
     avatar: StrictStr = Field(description="User's avatar, either a http/https URL or a data URI")
     attributes: Optional[Dict[str, Any]] = None
     uid: StrictStr
     path: Optional[StrictStr] = None
     type: Optional[UserTypeEnum] = None
     uuid: StrictStr
@@ -107,14 +107,19 @@
                     _items.append(_item.to_dict())
             _dict['groups_obj'] = _items
         # set to None if last_login (nullable) is None
         # and model_fields_set contains the field
         if self.last_login is None and "last_login" in self.model_fields_set:
             _dict['last_login'] = None
 
+        # set to None if groups_obj (nullable) is None
+        # and model_fields_set contains the field
+        if self.groups_obj is None and "groups_obj" in self.model_fields_set:
+            _dict['groups_obj'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of User from a dict"""
         if obj is None:
             return None
```

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_account_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_account_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_assigned_object_permission.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_consent.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_consent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_creation_mode_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_creation_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_delete_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_delete_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_delete_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_fields_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_fields_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_group.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_login_challenge.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_login_challenge_response_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_login_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_login_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_logout_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_logout_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_logout_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_matching_mode_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_matching_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_metrics.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_o_auth_source_connection.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_o_auth_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_o_auth_source_connection_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_object_permission.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_password_set_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_password_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_path.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_path.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_saml_source_connection.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_saml_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_saml_source_connection_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_self.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_self.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_self_groups.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_self_groups.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_service_account_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_service_account_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_service_account_response.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_service_account_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_setting.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_setting.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_source_connection.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_type_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_verification_enum.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_verification_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_write_stage.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_write_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/user_write_stage_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/validation_error.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/version.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/version.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/web_authn_device.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/web_authn_device_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/web_authn_device_type.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_type.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/web_authn_device_type_request.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/web_authn_device_type_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/models/workers.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/models/workers.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/authentik_client/rest.py` & `authentik_client-2024.2.2.post1713289429/authentik_client/rest.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1713183880/pyproject.toml` & `authentik_client-2024.2.2.post1713289429/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "authentik_client"
-version = "2024.2.2-1713183880"
+version = "2024.2.2-1713289429"
 description = "authentik"
 authors = ["authentik Team <hello@goauthentik.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/goauthentik/authentik"
 keywords = ["OpenAPI", "OpenAPI-Generator", "authentik"]
 include = ["authentik_client/py.typed"]
```

### Comparing `authentik_client-2024.2.2.post1713183880/PKG-INFO` & `authentik_client-2024.2.2.post1713289429/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentik_client
-Version: 2024.2.2.post1713183880
+Version: 2024.2.2.post1713289429
 Summary: authentik
 Home-page: https://github.com/goauthentik/authentik
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,authentik
 Author: authentik Team
 Author-email: hello@goauthentik.io
 Requires-Python: >=3.7,<4.0
@@ -25,15 +25,15 @@
 
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.2.2
-- Package version: 2024.2.2-1713183880
+- Package version: 2024.2.2-1713289429
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

