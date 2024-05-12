# Comparing `tmp/django_restit-4.2.8.tar.gz` & `tmp/django_restit-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_restit-4.2.8.tar", max compression
+gzip compressed data, was "django_restit-4.2.9.tar", max compression
```

## Comparing `django_restit-4.2.8.tar` & `django_restit-4.2.9.tar`

### file list

```diff
@@ -1,491 +1,491 @@
--rw-r--r--   0        0        0     1068 2023-06-27 05:37:44.430230 django_restit-4.2.8/LICENSE.md
--rw-r--r--   0        0        0     6240 2023-07-18 17:15:13.487162 django_restit-4.2.8/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.430501 django_restit-4.2.8/account/__init__.py
--rw-r--r--   0        0        0     1839 2023-06-27 05:37:44.430617 django_restit-4.2.8/account/admin.py
--rw-r--r--   0        0        0      980 2023-06-27 05:37:44.430754 django_restit-4.2.8/account/fcm/__init__.py
--rw-r--r--   0        0        0    15894 2023-06-27 05:37:44.430954 django_restit-4.2.8/account/migrations/0001_initial.py
--rw-r--r--   0        0        0      738 2023-06-27 05:37:44.431054 django_restit-4.2.8/account/migrations/0003_member_phone_number.py
--rw-r--r--   0        0        0      551 2023-06-27 05:37:44.431131 django_restit-4.2.8/account/migrations/0004_group_modified_alter_group_created.py
--rw-r--r--   0        0        0      437 2023-06-27 05:37:44.431211 django_restit-4.2.8/account/migrations/0005_member_auth_code_expires.py
--rw-r--r--   0        0        0      450 2023-06-27 05:37:44.431293 django_restit-4.2.8/account/migrations/0006_member_security_token.py
--rw-r--r--   0        0        0     1654 2023-06-27 05:37:44.431375 django_restit-4.2.8/account/migrations/0007_authtoken_signature_authsession.py
--rw-r--r--   0        0        0     2379 2023-06-27 05:37:44.431464 django_restit-4.2.8/account/migrations/0008_memberdevice_memberdevicemetadata.py
--rw-r--r--   0        0        0      468 2023-06-27 05:37:44.431538 django_restit-4.2.8/account/migrations/0009_alter_member_phone_number.py
--rw-r--r--   0        0        0      305 2023-06-27 05:37:44.431613 django_restit-4.2.8/account/migrations/0010_delete_authtoken.py
--rw-r--r--   0        0        0     1062 2023-06-27 05:37:44.431685 django_restit-4.2.8/account/migrations/0011_authtoken.py
--rw-r--r--   0        0        0     2043 2023-06-27 05:37:44.431755 django_restit-4.2.8/account/migrations/0012_settings_settingsmetadata.py
--rw-r--r--   0        0        0      418 2023-07-13 15:44:27.208937 django_restit-4.2.8/account/migrations/0013_memberdevice_ip.py
--rw-r--r--   0        0        0      541 2023-11-07 12:44:14.024459 django_restit-4.2.8/account/migrations/0014_alter_notificationmemberrecord_member.py
--rw-r--r--   0        0        0      460 2023-11-15 19:46:51.612834 django_restit-4.2.8/account/migrations/0015_memberdevice_buid.py
--rw-r--r--   0        0        0      424 2023-11-15 20:20:37.084916 django_restit-4.2.8/account/migrations/0016_authsession_buid.py
--rw-r--r--   0        0        0      375 2023-11-28 23:26:56.206776 django_restit-4.2.8/account/migrations/0017_rename_requires_topt_member_requires_totp.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.431784 django_restit-4.2.8/account/migrations/__init__.py
--rw-r--r--   0        0        0      341 2023-06-27 05:37:44.431899 django_restit-4.2.8/account/models/__init__.py
--rw-r--r--   0        0        0     4105 2023-11-15 20:24:03.414109 django_restit-4.2.8/account/models/device.py
--rw-r--r--   0        0        0     1437 2023-06-27 05:37:44.432051 django_restit-4.2.8/account/models/feeds.py
--rw-r--r--   0        0        0    20064 2023-12-15 19:46:55.047382 django_restit-4.2.8/account/models/group.py
--rw-r--r--   0        0        0     2720 2023-06-27 05:37:44.432315 django_restit-4.2.8/account/models/legacy.py
--rw-r--r--   0        0        0    49327 2023-12-19 20:43:30.083308 django_restit-4.2.8/account/models/member.py
--rw-r--r--   0        0        0     7763 2023-12-09 22:24:04.788938 django_restit-4.2.8/account/models/membership.py
--rw-r--r--   0        0        0    12078 2023-11-17 21:39:46.651560 django_restit-4.2.8/account/models/notify.py
--rw-r--r--   0        0        0     3509 2023-11-15 20:20:12.123435 django_restit-4.2.8/account/models/session.py
--rw-r--r--   0        0        0     2137 2023-06-27 05:37:44.432966 django_restit-4.2.8/account/models/settings.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.433042 django_restit-4.2.8/account/oauth/__init__.py
--rw-r--r--   0        0        0     2078 2023-06-27 05:37:44.433131 django_restit-4.2.8/account/oauth/google.py
--rw-r--r--   0        0        0      874 2023-11-29 03:43:42.972754 django_restit-4.2.8/account/periodic.py
--rw-r--r--   0        0        0      152 2023-06-27 05:37:44.433297 django_restit-4.2.8/account/rpc/__init__.py
--rw-r--r--   0        0        0    14896 2023-12-19 15:38:33.959934 django_restit-4.2.8/account/rpc/auth.py
--rw-r--r--   0        0        0     2852 2023-07-13 15:33:42.583999 django_restit-4.2.8/account/rpc/device.py
--rw-r--r--   0        0        0     3472 2023-12-04 21:21:15.602286 django_restit-4.2.8/account/rpc/group.py
--rw-r--r--   0        0        0     1150 2023-06-27 05:37:44.433650 django_restit-4.2.8/account/rpc/member.py
--rw-r--r--   0        0        0     3344 2023-06-27 05:37:44.433726 django_restit-4.2.8/account/rpc/notify.py
--rw-r--r--   0        0        0     2669 2023-12-17 00:40:58.671312 django_restit-4.2.8/account/rpc/oauth.py
--rw-r--r--   0        0        0      271 2023-06-27 05:37:44.433874 django_restit-4.2.8/account/rpc/settings.py
--rw-r--r--   0        0        0       53 2023-06-27 05:37:44.433934 django_restit-4.2.8/account/settings.py
--rw-r--r--   0        0        0     9709 2023-06-27 05:37:44.434095 django_restit-4.2.8/account/templates/email/base.html
--rw-r--r--   0        0        0    10567 2023-06-27 05:37:44.434205 django_restit-4.2.8/account/templates/email/invite.html
--rw-r--r--   0        0        0    12609 2023-11-07 13:31:04.277159 django_restit-4.2.8/account/templates/email/plain/base.html
--rw-r--r--   0        0        0    15235 2023-09-13 21:51:42.921379 django_restit-4.2.8/account/templates/email/plain/invite.html
--rw-r--r--   0        0        0    13954 2023-06-27 05:37:44.434450 django_restit-4.2.8/account/templates/email/plain/reset_code.html
--rw-r--r--   0        0        0    10261 2023-06-27 05:37:44.434528 django_restit-4.2.8/account/templates/email/reset_code.html
--rw-r--r--   0        0        0    15147 2023-09-13 21:29:05.002359 django_restit-4.2.8/account/templates/email/simple/invite.html
--rw-r--r--   0        0        0    13944 2023-06-27 05:37:44.434713 django_restit-4.2.8/account/templates/email/simple/reset_code.html
--rw-r--r--   0        0        0      520 2023-06-27 05:37:44.434828 django_restit-4.2.8/auditlog/README
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.434859 django_restit-4.2.8/auditlog/__init__.py
--rw-r--r--   0        0        0     1006 2023-06-27 05:37:44.434933 django_restit-4.2.8/auditlog/admin.py
--rw-r--r--   0        0        0     6553 2023-06-27 05:37:44.435019 django_restit-4.2.8/auditlog/decorators.py
--rw-r--r--   0        0        0     1511 2023-12-17 00:38:09.426633 django_restit-4.2.8/auditlog/middleware.py
--rw-r--r--   0        0        0     3309 2023-06-27 05:37:44.435191 django_restit-4.2.8/auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435224 django_restit-4.2.8/auditlog/migrations/__init__.py
--rw-r--r--   0        0        0    16294 2023-11-28 17:50:33.116663 django_restit-4.2.8/auditlog/models.py
--rw-r--r--   0        0        0      363 2023-11-06 22:55:59.417756 django_restit-4.2.8/auditlog/periodic.py
--rw-r--r--   0        0        0     3591 2023-12-09 17:40:20.663908 django_restit-4.2.8/auditlog/rpc.py
--rw-r--r--   0        0        0     2415 2023-11-06 23:04:22.220672 django_restit-4.2.8/auditlog/tq.py
--rw-r--r--   0        0        0      163 2023-06-27 05:37:44.435623 django_restit-4.2.8/auditlog/urls.py
--rw-r--r--   0        0        0     2169 2023-06-27 05:37:44.435745 django_restit-4.2.8/inbox/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435775 django_restit-4.2.8/inbox/__init__.py
--rw-r--r--   0        0        0      243 2023-06-27 05:37:44.435850 django_restit-4.2.8/inbox/admin.py
--rw-r--r--   0        0        0     5638 2023-11-17 19:40:32.512907 django_restit-4.2.8/inbox/handlers.py
--rw-r--r--   0        0        0     6429 2023-06-27 05:37:44.436034 django_restit-4.2.8/inbox/migrations/0001_initial.py
--rw-r--r--   0        0        0      380 2023-06-27 05:37:44.436102 django_restit-4.2.8/inbox/migrations/0002_alter_message_cc.py
--rw-r--r--   0        0        0      416 2023-06-27 05:37:44.436177 django_restit-4.2.8/inbox/migrations/0003_attachment_content_type.py
--rw-r--r--   0        0        0     1140 2023-06-27 05:37:44.436249 django_restit-4.2.8/inbox/migrations/0004_mailtemplate.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.436274 django_restit-4.2.8/inbox/migrations/__init__.py
--rw-r--r--   0        0        0      174 2023-06-27 05:37:44.436383 django_restit-4.2.8/inbox/models/__init__.py
--rw-r--r--   0        0        0     2881 2023-12-09 17:43:11.500207 django_restit-4.2.8/inbox/models/bounce.py
--rw-r--r--   0        0        0     2517 2023-12-09 17:43:15.908858 django_restit-4.2.8/inbox/models/complaint.py
--rw-r--r--   0        0        0     3003 2023-12-09 17:43:26.636118 django_restit-4.2.8/inbox/models/message.py
--rw-r--r--   0        0        0     1013 2023-06-27 05:37:44.436870 django_restit-4.2.8/inbox/models/template.py
--rw-r--r--   0        0        0     1534 2023-06-27 05:37:44.436956 django_restit-4.2.8/inbox/rpc.py
--rw-r--r--   0        0        0       89 2023-06-27 05:37:44.437057 django_restit-4.2.8/inbox/utils/__init__.py
--rw-r--r--   0        0        0     4615 2023-11-17 22:20:26.650843 django_restit-4.2.8/inbox/utils/parsing.py
--rw-r--r--   0        0        0     4098 2023-06-27 05:37:44.437260 django_restit-4.2.8/inbox/utils/render.py
--rw-r--r--   0        0        0     2179 2023-11-09 19:28:02.561057 django_restit-4.2.8/inbox/utils/sending.py
--rw-r--r--   0        0        0     1114 2023-06-27 05:37:44.437469 django_restit-4.2.8/incident/README.md
--rw-r--r--   0        0        0     3249 2023-12-09 16:49:33.350637 django_restit-4.2.8/incident/__init__.py
--rw-r--r--   0        0        0     9720 2023-06-27 05:37:44.437670 django_restit-4.2.8/incident/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2023-06-27 05:37:44.437757 django_restit-4.2.8/incident/migrations/0002_event_component_event_component_id.py
--rw-r--r--   0        0        0      425 2023-06-27 05:37:44.437826 django_restit-4.2.8/incident/migrations/0003_rule_action.py
--rw-r--r--   0        0        0      662 2023-06-27 05:37:44.437890 django_restit-4.2.8/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
--rw-r--r--   0        0        0      698 2023-06-27 05:37:44.437964 django_restit-4.2.8/incident/migrations/0005_incident_component_alter_incident_state.py
--rw-r--r--   0        0        0      324 2023-06-27 05:37:44.438034 django_restit-4.2.8/incident/migrations/0006_delete_eventmetadata.py
--rw-r--r--   0        0        0      414 2023-06-27 05:37:44.438100 django_restit-4.2.8/incident/migrations/0007_event_metadata.py
--rw-r--r--   0        0        0      903 2023-06-27 05:37:44.438184 django_restit-4.2.8/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
--rw-r--r--   0        0        0      473 2023-08-22 19:29:15.953220 django_restit-4.2.8/incident/migrations/0009_incident_reporter_ip.py
--rw-r--r--   0        0        0      631 2023-11-20 03:38:24.557282 django_restit-4.2.8/incident/migrations/0010_incident_category_incident_component_id.py
--rw-r--r--   0        0        0     2142 2023-11-20 03:51:50.549436 django_restit-4.2.8/incident/migrations/0011_ticket.py
--rw-r--r--   0        0        0      372 2023-12-19 03:25:06.153029 django_restit-4.2.8/incident/migrations/0012_rule_match_by.py
--rw-r--r--   0        0        0      387 2023-12-19 17:40:50.828606 django_restit-4.2.8/incident/migrations/0013_rulecheck_is_required.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438214 django_restit-4.2.8/incident/migrations/__init__.py
--rw-r--r--   0        0        0      209 2023-11-20 03:49:22.992273 django_restit-4.2.8/incident/models/__init__.py
--rw-r--r--   0        0        0     6849 2023-12-09 19:39:18.790758 django_restit-4.2.8/incident/models/event.py
--rw-r--r--   0        0        0    15294 2023-12-20 17:41:19.779521 django_restit-4.2.8/incident/models/incident.py
--rw-r--r--   0        0        0     2227 2023-12-09 16:28:25.375197 django_restit-4.2.8/incident/models/ossec.py
--rw-r--r--   0        0        0     6024 2023-12-19 17:45:22.401412 django_restit-4.2.8/incident/models/rules.py
--rw-r--r--   0        0        0     2302 2023-11-20 03:51:47.283232 django_restit-4.2.8/incident/models/ticket.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438911 django_restit-4.2.8/incident/parsers/__init__.py
--rw-r--r--   0        0        0     6247 2023-12-19 21:01:44.694027 django_restit-4.2.8/incident/parsers/ossec.py
--rw-r--r--   0        0        0      227 2023-11-28 04:04:56.458420 django_restit-4.2.8/incident/periodic.py
--rw-r--r--   0        0        0     7546 2023-12-19 00:05:09.162867 django_restit-4.2.8/incident/rpc.py
--rw-r--r--   0        0        0    14178 2023-11-18 15:34:42.122382 django_restit-4.2.8/incident/templates/email/incident_change.html
--rw-r--r--   0        0        0    15173 2023-06-27 05:37:44.439515 django_restit-4.2.8/incident/templates/email/incident_new.html
--rw-r--r--   0        0        0    14727 2023-11-20 22:01:29.858057 django_restit-4.2.8/incident/templates/email/incident_plain.html
--rw-r--r--   0        0        0     4472 2023-11-28 04:02:53.896214 django_restit-4.2.8/incident/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.439791 django_restit-4.2.8/location/__init__.py
--rw-r--r--   0        0        0      297 2023-06-27 05:37:44.439885 django_restit-4.2.8/location/admin.py
--rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.440042 django_restit-4.2.8/location/geolocate.py
--rw-r--r--   0        0        0     7000 2023-06-27 05:37:44.440236 django_restit-4.2.8/location/migrations/0001_initial.py
--rw-r--r--   0        0        0      576 2023-06-27 05:37:44.440313 django_restit-4.2.8/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440339 django_restit-4.2.8/location/migrations/__init__.py
--rw-r--r--   0        0        0      230 2023-06-27 05:37:44.440480 django_restit-4.2.8/location/models/__init__.py
--rw-r--r--   0        0        0     2028 2023-06-27 05:37:44.440559 django_restit-4.2.8/location/models/address.py
--rw-r--r--   0        0        0     5984 2023-12-09 17:41:39.358207 django_restit-4.2.8/location/models/ip.py
--rw-r--r--   0        0        0     1994 2023-06-27 05:37:44.440722 django_restit-4.2.8/location/models/legacy.py
--rw-r--r--   0        0        0     2316 2023-06-27 05:37:44.440785 django_restit-4.2.8/location/models/location.py
--rw-r--r--   0        0        0     1474 2023-06-27 05:37:44.440843 django_restit-4.2.8/location/models/track.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440920 django_restit-4.2.8/location/providers/__init__.py
--rw-r--r--   0        0        0      727 2023-08-07 06:30:37.235541 django_restit-4.2.8/location/providers/iplookup/__init__.py
--rw-r--r--   0        0        0     2419 2023-06-27 05:37:44.441128 django_restit-4.2.8/location/providers/iplookup/abstractapi.py
--rw-r--r--   0        0        0     1345 2023-06-27 05:37:44.441192 django_restit-4.2.8/location/providers/iplookup/extremeip.py
--rw-r--r--   0        0        0     2121 2023-06-27 05:37:44.441260 django_restit-4.2.8/location/providers/iplookup/geoplugin.py
--rw-r--r--   0        0        0     1797 2023-06-27 05:37:44.441325 django_restit-4.2.8/location/providers/iplookup/ipapi.py
--rw-r--r--   0        0        0     1265 2023-06-27 05:37:44.441395 django_restit-4.2.8/location/providers/iplookup/ipinfo.py
--rw-r--r--   0        0        0      937 2023-06-27 05:37:44.441463 django_restit-4.2.8/location/providers/iplookup/restit.py
--rw-r--r--   0        0        0       42 2023-06-27 05:37:44.441569 django_restit-4.2.8/location/providers/location/__init__.py
--rw-r--r--   0        0        0     2860 2023-06-27 05:37:44.441653 django_restit-4.2.8/location/providers/location/google.py
--rw-r--r--   0        0        0       46 2023-06-27 05:37:44.441777 django_restit-4.2.8/location/providers/timezones/__init__.py
--rw-r--r--   0        0        0      619 2023-06-27 05:37:44.441855 django_restit-4.2.8/location/providers/timezones/google.py
--rw-r--r--   0        0        0     1935 2023-06-27 05:37:44.441924 django_restit-4.2.8/location/providers/zillow.py
--rw-r--r--   0        0        0      123 2023-06-27 05:37:44.442046 django_restit-4.2.8/location/rpc/__init__.py
--rw-r--r--   0        0        0     1305 2023-11-27 23:53:10.865156 django_restit-4.2.8/location/rpc/ip.py
--rw-r--r--   0        0        0      779 2023-06-27 05:37:44.442183 django_restit-4.2.8/location/rpc/location.py
--rw-r--r--   0        0        0     3735 2023-06-27 05:37:44.442254 django_restit-4.2.8/location/rpc/track.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.442312 django_restit-4.2.8/medialib/__init__.py
--rw-r--r--   0        0        0     2261 2023-06-27 05:37:44.442393 django_restit-4.2.8/medialib/admin.py
--rw-r--r--   0        0        0       27 2023-06-27 05:37:44.442482 django_restit-4.2.8/medialib/cvutil/__init__.py
--rw-r--r--   0        0        0     4269 2023-06-27 05:37:44.442556 django_restit-4.2.8/medialib/cvutil/contours.py
--rw-r--r--   0        0        0    12649 2023-06-27 05:37:44.442653 django_restit-4.2.8/medialib/cvutil/images.py
--rw-r--r--   0        0        0     9586 2023-06-27 05:37:44.442744 django_restit-4.2.8/medialib/cvutil/misc.py
--rw-r--r--   0        0        0     5824 2023-06-27 05:37:44.442838 django_restit-4.2.8/medialib/cvutil/text.py
--rw-r--r--   0        0        0    48442 2023-06-27 05:37:44.443047 django_restit-4.2.8/medialib/fixtures/initial_data.json
--rw-r--r--   0        0        0    31978 2023-06-27 05:37:44.443182 django_restit-4.2.8/medialib/fixtures/medialib.json
--rw-r--r--   0        0        0    16989 2023-06-27 05:37:44.443279 django_restit-4.2.8/medialib/fixtures/medialib_test_fixture.json
--rw-r--r--   0        0        0     5442 2023-06-27 05:37:44.443362 django_restit-4.2.8/medialib/forms.py
--rw-r--r--   0        0        0    20518 2023-06-27 05:37:44.443459 django_restit-4.2.8/medialib/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.443499 django_restit-4.2.8/medialib/migrations/__init__.py
--rw-r--r--   0        0        0    52152 2023-10-09 22:04:22.261815 django_restit-4.2.8/medialib/models.py
--rw-r--r--   0        0        0     1189 2023-06-27 05:37:44.443785 django_restit-4.2.8/medialib/ocr.py
--rw-r--r--   0        0        0     1275 2023-06-27 05:37:44.443858 django_restit-4.2.8/medialib/pdf.py
--rw-r--r--   0        0        0      545 2023-06-27 05:37:44.443925 django_restit-4.2.8/medialib/qrcode.py
--rw-r--r--   0        0        0    10312 2023-06-27 05:37:44.444059 django_restit-4.2.8/medialib/render/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444125 django_restit-4.2.8/medialib/render/engines/__init__.py
--rw-r--r--   0        0        0     3531 2023-06-27 05:37:44.444213 django_restit-4.2.8/medialib/render/engines/anigif.py
--rw-r--r--   0        0        0     6881 2023-06-27 05:37:44.444291 django_restit-4.2.8/medialib/render/engines/ffmpeg.py
--rw-r--r--   0        0        0      792 2023-06-27 05:37:44.444369 django_restit-4.2.8/medialib/render/engines/gifsicle.py
--rw-r--r--   0        0        0     3436 2023-06-27 05:37:44.444438 django_restit-4.2.8/medialib/render/engines/hls.py
--rw-r--r--   0        0        0      983 2023-06-27 05:37:44.444498 django_restit-4.2.8/medialib/render/engines/mp4box.py
--rw-r--r--   0        0        0      397 2023-06-27 05:37:44.444604 django_restit-4.2.8/medialib/render/engines/rtmp/Makefile
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444636 django_restit-4.2.8/medialib/render/engines/rtmp/__init__.py
--rw-r--r--   0        0        0     4026 2023-06-27 05:37:44.444726 django_restit-4.2.8/medialib/render/engines/rtmp/rtmp.i
--rw-r--r--   0        0        0      699 2023-06-27 05:37:44.444798 django_restit-4.2.8/medialib/render/engines/rtmpdump.py
--rw-r--r--   0        0        0     1017 2023-06-27 05:37:44.444865 django_restit-4.2.8/medialib/render/engines/rtmpsink.py
--rw-r--r--   0        0        0     3466 2023-06-27 05:37:44.444941 django_restit-4.2.8/medialib/render/engines/video_getinfo.py
--rw-r--r--   0        0        0      809 2023-06-27 05:37:44.445017 django_restit-4.2.8/medialib/render/engines/websnap.py
--rw-r--r--   0        0        0     2193 2023-06-27 05:37:44.445078 django_restit-4.2.8/medialib/render/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.445133 django_restit-4.2.8/medialib/render/presets/__init__.py
--rw-r--r--   0        0        0     4179 2023-06-27 05:37:44.445227 django_restit-4.2.8/medialib/render/presets/akamai.py
--rw-r--r--   0        0        0     3284 2023-06-27 05:37:44.445306 django_restit-4.2.8/medialib/render/presets/animated_thumbnail.py
--rw-r--r--   0        0        0     4004 2023-06-27 05:37:44.445394 django_restit-4.2.8/medialib/render/presets/ffmpeg.py
--rw-r--r--   0        0        0     2087 2023-06-27 05:37:44.445469 django_restit-4.2.8/medialib/render/presets/flv.py
--rw-r--r--   0        0        0     6567 2023-06-27 05:37:44.445567 django_restit-4.2.8/medialib/render/presets/hls.py
--rw-r--r--   0        0        0     6955 2023-06-27 05:37:44.445668 django_restit-4.2.8/medialib/render/presets/image_transcode.py
--rw-r--r--   0        0        0     1094 2023-06-27 05:37:44.445750 django_restit-4.2.8/medialib/render/presets/image_validate.py
--rw-r--r--   0        0        0     2423 2023-06-27 05:37:44.445825 django_restit-4.2.8/medialib/render/presets/mp4.py
--rw-r--r--   0        0        0     4997 2023-06-27 05:37:44.445908 django_restit-4.2.8/medialib/render/presets/video_still.py
--rw-r--r--   0        0        0     3228 2023-06-27 05:37:44.445986 django_restit-4.2.8/medialib/render/presets/video_validate.py
--rw-r--r--   0        0        0      863 2023-06-27 05:37:44.446101 django_restit-4.2.8/medialib/render/presets/websnap.py
--rw-r--r--   0        0        0     2282 2023-06-27 05:37:44.446183 django_restit-4.2.8/medialib/render/presets/youtube.py
--rw-r--r--   0        0        0    16451 2023-06-27 05:37:44.446294 django_restit-4.2.8/medialib/render/render_utils.py
--rw-r--r--   0        0        0      370 2023-06-27 05:37:44.446381 django_restit-4.2.8/medialib/render/schedule.py
--rw-r--r--   0        0        0       82 2023-06-27 05:37:44.446525 django_restit-4.2.8/medialib/rpc/__init__.py
--rw-r--r--   0        0        0    37925 2023-06-27 05:37:44.446687 django_restit-4.2.8/medialib/rpc/legacy.py
--rw-r--r--   0        0        0      617 2023-06-27 05:37:44.446776 django_restit-4.2.8/medialib/rpc/media.py
--rw-r--r--   0        0        0      956 2023-06-27 05:37:44.446852 django_restit-4.2.8/medialib/rpc/tools.py
--rwxr-xr-x   0        0        0     7875 2023-06-27 05:37:44.446994 django_restit-4.2.8/medialib/scripts/init_config
--rw-r--r--   0        0        0     4499 2023-06-27 05:37:44.447158 django_restit-4.2.8/medialib/static/css/base_medialibui.css
--rw-r--r--   0        0        0     3128 2023-06-27 05:37:44.447238 django_restit-4.2.8/medialib/static/css/base_widgets.css
--rw-r--r--   0        0        0     3263 2023-06-27 05:37:44.447311 django_restit-4.2.8/medialib/static/css/jquery.jcrop.css
--rw-r--r--   0        0        0      193 2023-06-27 05:37:44.447412 django_restit-4.2.8/medialib/static/img/arrow-down-white.png
--rw-r--r--   0        0        0     4589 2023-06-27 05:37:44.447507 django_restit-4.2.8/medialib/static/img/bg-body.gif
--rw-r--r--   0        0        0      441 2023-06-27 05:37:44.447579 django_restit-4.2.8/medialib/static/img/cancel.gif
--rw-r--r--   0        0        0      341 2023-06-27 05:37:44.447648 django_restit-4.2.8/medialib/static/img/icon-generic.gif
--rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447712 django_restit-4.2.8/medialib/static/img/icon-image.gif
--rw-r--r--   0        0        0      359 2023-06-27 05:37:44.447775 django_restit-4.2.8/medialib/static/img/icon-media.gif
--rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447850 django_restit-4.2.8/medialib/static/img/icon-zip.gif
--rw-r--r--   0        0        0     3208 2023-06-27 05:37:44.447934 django_restit-4.2.8/medialib/static/img/loading.gif
--rw-r--r--   0        0        0     2537 2023-06-27 05:37:44.448000 django_restit-4.2.8/medialib/static/img/noimage.gif
--rw-r--r--   0        0        0     1057 2023-06-27 05:37:44.448065 django_restit-4.2.8/medialib/static/img/render_err.gif
--rw-r--r--   0        0        0     6716 2023-06-27 05:37:44.448158 django_restit-4.2.8/medialib/static/img/rendering.gif
--rw-r--r--   0        0        0      292 2023-06-27 05:37:44.448225 django_restit-4.2.8/medialib/static/img/star_off.png
--rw-r--r--   0        0        0      297 2023-06-27 05:37:44.448287 django_restit-4.2.8/medialib/static/img/star_on.png
--rw-r--r--   0        0        0     1130 2023-06-27 05:37:44.448351 django_restit-4.2.8/medialib/static/img/unknown.gif
--rwxr-xr-x   0        0        0    74054 2023-06-27 05:37:44.448677 django_restit-4.2.8/medialib/static/lib/caman.full.js
--rw-r--r--   0        0        0    17360 2023-06-27 05:37:44.448823 django_restit-4.2.8/medialib/static/lib/hammer.min.js
--rwxr-xr-x   0        0        0    42434 2023-06-27 05:37:44.449017 django_restit-4.2.8/medialib/static/lib/jquery.Jcrop.js
--rw-r--r--   0        0        0      743 2023-06-27 05:37:44.449098 django_restit-4.2.8/medialib/static/lib/jquery.hammer.js
--rw-r--r--   0        0        0    16587 2023-06-27 05:37:44.449224 django_restit-4.2.8/medialib/static/lib/load-image.min.js
--rwxr-xr-x   0        0        0   111779 2023-06-27 05:37:44.449542 django_restit-4.2.8/medialib/static/lib/swiper.js
--rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449771 django_restit-4.2.8/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
--rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449850 django_restit-4.2.8/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
--rw-r--r--   0        0        0     5708 2023-06-27 05:37:44.449979 django_restit-4.2.8/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
--rw-r--r--   0        0        0     3502 2023-06-27 05:37:44.450059 django_restit-4.2.8/medialib/static/lib/tinymce/plugins/medialib/medialib.html
--rw-r--r--   0        0        0     5876 2023-06-27 05:37:44.450187 django_restit-4.2.8/medialib/stores/__init__.py
--rw-r--r--   0        0        0      601 2023-06-27 05:37:44.450314 django_restit-4.2.8/medialib/stores/apiclient/__init__.py
--rw-r--r--   0        0        0     9852 2023-06-27 05:37:44.450415 django_restit-4.2.8/medialib/stores/apiclient/channel.py
--rw-r--r--   0        0        0    35929 2023-06-27 05:37:44.450591 django_restit-4.2.8/medialib/stores/apiclient/discovery.py
--rw-r--r--   0        0        0     3516 2023-06-27 05:37:44.450684 django_restit-4.2.8/medialib/stores/apiclient/errors.py
--rw-r--r--   0        0        0    52911 2023-06-27 05:37:44.450906 django_restit-4.2.8/medialib/stores/apiclient/http.py
--rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.451002 django_restit-4.2.8/medialib/stores/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11761 2023-06-27 05:37:44.451111 django_restit-4.2.8/medialib/stores/apiclient/model.py
--rw-r--r--   0        0        0     3528 2023-06-27 05:37:44.451205 django_restit-4.2.8/medialib/stores/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9293 2023-06-27 05:37:44.451302 django_restit-4.2.8/medialib/stores/apiclient/schema.py
--rw-r--r--   0        0        0     1592 2023-06-27 05:37:44.451390 django_restit-4.2.8/medialib/stores/filestore.py
--rw-r--r--   0        0        0    69575 2023-06-27 05:37:44.451712 django_restit-4.2.8/medialib/stores/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.451937 django_restit-4.2.8/medialib/stores/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.452031 django_restit-4.2.8/medialib/stores/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.452160 django_restit-4.2.8/medialib/stores/httplib2/socks.py
--rw-r--r--   0        0        0      706 2023-06-27 05:37:44.452238 django_restit-4.2.8/medialib/stores/httpstore.py
--rw-r--r--   0        0        0      304 2023-06-27 05:37:44.452325 django_restit-4.2.8/medialib/stores/nullstore.py
--rw-r--r--   0        0        0      213 2023-06-27 05:37:44.452492 django_restit-4.2.8/medialib/stores/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.452598 django_restit-4.2.8/medialib/stores/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.452767 django_restit-4.2.8/medialib/stores/oauth2client/appengine.py
--rw-r--r--   0        0        0    44346 2023-06-27 05:37:44.452995 django_restit-4.2.8/medialib/stores/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.453091 django_restit-4.2.8/medialib/stores/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.453196 django_restit-4.2.8/medialib/stores/oauth2client/crypt.py
--rw-r--r--   0        0        0     3755 2023-06-27 05:37:44.453276 django_restit-4.2.8/medialib/stores/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.453391 django_restit-4.2.8/medialib/stores/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.453451 django_restit-4.2.8/medialib/stores/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.453541 django_restit-4.2.8/medialib/stores/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.453634 django_restit-4.2.8/medialib/stores/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.453698 django_restit-4.2.8/medialib/stores/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.453764 django_restit-4.2.8/medialib/stores/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.453855 django_restit-4.2.8/medialib/stores/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.453938 django_restit-4.2.8/medialib/stores/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.454013 django_restit-4.2.8/medialib/stores/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0      500 2023-06-27 05:37:44.454077 django_restit-4.2.8/medialib/stores/rtmpstore.py
--rw-r--r--   0        0        0     4583 2023-06-27 05:37:44.454163 django_restit-4.2.8/medialib/stores/s3store.py
--rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.454272 django_restit-4.2.8/medialib/stores/uritemplate/__init__.py
--rw-r--r--   0        0        0      406 2023-06-27 05:37:44.454334 django_restit-4.2.8/medialib/stores/youtubestore.py
--rw-r--r--   0        0        0     3691 2023-06-27 05:37:44.454500 django_restit-4.2.8/medialib/templates/medialib/base.html
--rw-r--r--   0        0        0     1277 2023-06-27 05:37:44.454591 django_restit-4.2.8/medialib/templates/medialib/instances.html
--rw-r--r--   0        0        0     1170 2023-06-27 05:37:44.454657 django_restit-4.2.8/medialib/templates/medialib/items.html
--rw-r--r--   0        0        0     8194 2023-06-27 05:37:44.454746 django_restit-4.2.8/medialib/templates/medialib/library.html
--rw-r--r--   0        0        0       65 2023-06-27 05:37:44.454810 django_restit-4.2.8/medialib/templates/medialib/notify_error.subject
--rw-r--r--   0        0        0       49 2023-06-27 05:37:44.454869 django_restit-4.2.8/medialib/templates/medialib/notify_error.to
--rw-r--r--   0        0        0      272 2023-06-27 05:37:44.454932 django_restit-4.2.8/medialib/templates/medialib/notify_error.txt
--rw-r--r--   0        0        0       71 2023-06-27 05:37:44.454996 django_restit-4.2.8/medialib/templates/medialib/notify_ready.subject
--rw-r--r--   0        0        0       49 2023-06-27 05:37:44.455056 django_restit-4.2.8/medialib/templates/medialib/notify_ready.to
--rw-r--r--   0        0        0      298 2023-06-27 05:37:44.455113 django_restit-4.2.8/medialib/templates/medialib/notify_ready.txt
--rw-r--r--   0        0        0       64 2023-06-27 05:37:44.455175 django_restit-4.2.8/medialib/templates/medialib/notify_render_error.subject
--rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455232 django_restit-4.2.8/medialib/templates/medialib/notify_render_error.to
--rw-r--r--   0        0        0      271 2023-06-27 05:37:44.455301 django_restit-4.2.8/medialib/templates/medialib/notify_render_error.txt
--rw-r--r--   0        0        0       68 2023-06-27 05:37:44.455380 django_restit-4.2.8/medialib/templates/medialib/notify_validate_error.subject
--rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455452 django_restit-4.2.8/medialib/templates/medialib/notify_validate_error.to
--rw-r--r--   0        0        0      275 2023-06-27 05:37:44.455521 django_restit-4.2.8/medialib/templates/medialib/notify_validate_error.txt
--rw-r--r--   0        0        0      206 2023-06-27 05:37:44.455593 django_restit-4.2.8/medialib/templates/medialib/smil
--rw-r--r--   0        0        0     1177 2023-06-27 05:37:44.455665 django_restit-4.2.8/medialib/templates/medialib/test.html
--rw-r--r--   0        0        0     1549 2023-06-27 05:37:44.455737 django_restit-4.2.8/medialib/templates/medialib/testpicker.html
--rw-r--r--   0        0        0     6045 2023-06-27 05:37:44.455814 django_restit-4.2.8/medialib/tests.py
--rw-r--r--   0        0        0      544 2023-06-27 05:37:44.455873 django_restit-4.2.8/medialib/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.455894 django_restit-4.2.8/medialib/urls.py
--rw-r--r--   0        0        0     3756 2023-06-27 05:37:44.455970 django_restit-4.2.8/medialib/utils.py
--rw-r--r--   0        0        0     4321 2023-06-27 05:37:44.456050 django_restit-4.2.8/medialib/views.py
--rw-r--r--   0        0        0     4303 2023-06-27 05:37:44.456166 django_restit-4.2.8/medialib/youtube/__init__.py
--rw-r--r--   0        0        0      601 2023-06-27 05:37:44.456272 django_restit-4.2.8/medialib/youtube/apiclient/__init__.py
--rw-r--r--   0        0        0     9886 2023-06-27 05:37:44.456332 django_restit-4.2.8/medialib/youtube/apiclient/channel.py
--rw-r--r--   0        0        0    35907 2023-06-27 05:37:44.456516 django_restit-4.2.8/medialib/youtube/apiclient/discovery.py
--rw-r--r--   0        0        0     3550 2023-06-27 05:37:44.456592 django_restit-4.2.8/medialib/youtube/apiclient/errors.py
--rw-r--r--   0        0        0    52945 2023-06-27 05:37:44.456694 django_restit-4.2.8/medialib/youtube/apiclient/http.py
--rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.456785 django_restit-4.2.8/medialib/youtube/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11795 2023-06-27 05:37:44.456835 django_restit-4.2.8/medialib/youtube/apiclient/model.py
--rw-r--r--   0        0        0     3596 2023-06-27 05:37:44.456895 django_restit-4.2.8/medialib/youtube/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9327 2023-06-27 05:37:44.456959 django_restit-4.2.8/medialib/youtube/apiclient/schema.py
--rw-r--r--   0        0        0    69581 2023-06-27 05:37:44.457093 django_restit-4.2.8/medialib/youtube/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.457310 django_restit-4.2.8/medialib/youtube/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.457412 django_restit-4.2.8/medialib/youtube/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.457533 django_restit-4.2.8/medialib/youtube/httplib2/socks.py
--rw-r--r--   0        0        0      213 2023-06-27 05:37:44.457629 django_restit-4.2.8/medialib/youtube/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.457687 django_restit-4.2.8/medialib/youtube/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.457830 django_restit-4.2.8/medialib/youtube/oauth2client/appengine.py
--rw-r--r--   0        0        0    44431 2023-06-27 05:37:44.457905 django_restit-4.2.8/medialib/youtube/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.457990 django_restit-4.2.8/medialib/youtube/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.458075 django_restit-4.2.8/medialib/youtube/oauth2client/crypt.py
--rw-r--r--   0        0        0     3753 2023-06-27 05:37:44.458140 django_restit-4.2.8/medialib/youtube/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.458204 django_restit-4.2.8/medialib/youtube/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.458255 django_restit-4.2.8/medialib/youtube/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.458323 django_restit-4.2.8/medialib/youtube/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.458399 django_restit-4.2.8/medialib/youtube/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.458454 django_restit-4.2.8/medialib/youtube/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.458510 django_restit-4.2.8/medialib/youtube/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.458604 django_restit-4.2.8/medialib/youtube/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.458680 django_restit-4.2.8/medialib/youtube/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.458745 django_restit-4.2.8/medialib/youtube/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0     2849 2023-06-27 05:37:44.458806 django_restit-4.2.8/medialib/youtube/upload.py
--rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.458902 django_restit-4.2.8/medialib/youtube/uritemplate/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-27 05:37:44.459001 django_restit-4.2.8/metrics/README.md
--rw-r--r--   0        0        0       90 2023-06-27 05:37:44.459061 django_restit-4.2.8/metrics/__init__.py
--rw-r--r--   0        0        0    24337 2023-11-12 22:00:50.439910 django_restit-4.2.8/metrics/client.py
--rw-r--r--   0        0        0     9182 2023-06-27 05:37:44.459333 django_restit-4.2.8/metrics/eod.py
--rw-r--r--   0        0        0     1664 2023-06-27 05:37:44.459430 django_restit-4.2.8/metrics/examples/eod_example.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459493 django_restit-4.2.8/metrics/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459564 django_restit-4.2.8/metrics/management/commands/__init__.py
--rw-r--r--   0        0        0      429 2023-06-27 05:37:44.459636 django_restit-4.2.8/metrics/management/commands/delete_gauge.py
--rw-r--r--   0        0        0      464 2023-06-27 05:37:44.459697 django_restit-4.2.8/metrics/management/commands/delete_metric.py
--rw-r--r--   0        0        0     2801 2023-06-27 05:37:44.459766 django_restit-4.2.8/metrics/management/commands/fix_redis_metrics_keys.py
--rw-r--r--   0        0        0     1928 2023-06-27 05:37:44.459829 django_restit-4.2.8/metrics/management/commands/generate_test_metrics.py
--rw-r--r--   0        0        0     1742 2023-06-27 05:37:44.459896 django_restit-4.2.8/metrics/management/commands/redis_metrics_send_mail.py
--rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.459957 django_restit-4.2.8/metrics/management/commands/reset_weekly_metrics.py
--rw-r--r--   0        0        0     4343 2023-06-27 05:37:44.460023 django_restit-4.2.8/metrics/management/commands/system_metric.py
--rw-r--r--   0        0        0     2399 2023-06-27 05:37:44.460109 django_restit-4.2.8/metrics/migrations/0001_initial.py
--rw-r--r--   0        0        0     1510 2023-06-27 05:37:44.460172 django_restit-4.2.8/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
--rw-r--r--   0        0        0      453 2023-06-27 05:37:44.460231 django_restit-4.2.8/metrics/migrations/0003_metrics_expires.py
--rw-r--r--   0        0        0     3271 2023-06-27 05:37:44.460284 django_restit-4.2.8/metrics/migrations/0004_eodmetrics.py
--rw-r--r--   0        0        0     2358 2023-06-27 05:37:44.460347 django_restit-4.2.8/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460367 django_restit-4.2.8/metrics/migrations/__init__.py
--rw-r--r--   0        0        0    13444 2023-11-14 19:47:33.877245 django_restit-4.2.8/metrics/models.py
--rw-r--r--   0        0        0      651 2023-08-07 16:07:55.926386 django_restit-4.2.8/metrics/periodic.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460587 django_restit-4.2.8/metrics/providers/__init__.py
--rw-r--r--   0        0        0     7432 2023-08-01 17:23:09.504050 django_restit-4.2.8/metrics/providers/aws.py
--rw-r--r--   0        0        0    17674 2023-12-17 00:39:40.117566 django_restit-4.2.8/metrics/rpc.py
--rw-r--r--   0        0        0      132 2023-06-27 05:37:44.460832 django_restit-4.2.8/metrics/settings.py
--rw-r--r--   0        0        0      799 2023-08-22 14:57:47.689025 django_restit-4.2.8/metrics/tq.py
--rw-r--r--   0        0        0    11995 2023-11-12 21:49:36.875626 django_restit-4.2.8/metrics/utils.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461016 django_restit-4.2.8/pushit/__init__.py
--rw-r--r--   0        0        0      451 2023-06-27 05:37:44.461079 django_restit-4.2.8/pushit/admin.py
--rw-r--r--   0        0        0     4555 2023-06-27 05:37:44.461167 django_restit-4.2.8/pushit/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461190 django_restit-4.2.8/pushit/migrations/__init__.py
--rw-r--r--   0        0        0     5066 2023-07-11 15:47:46.945937 django_restit-4.2.8/pushit/models.py
--rw-r--r--   0        0        0       88 2023-06-27 05:37:44.461351 django_restit-4.2.8/pushit/rpc/__init__.py
--rw-r--r--   0        0        0     1756 2023-07-24 17:39:38.308118 django_restit-4.2.8/pushit/rpc/githooks.py
--rw-r--r--   0        0        0     5028 2023-12-09 19:07:40.680776 django_restit-4.2.8/pushit/rpc/legacy.py
--rw-r--r--   0        0        0      378 2023-06-27 05:37:44.461520 django_restit-4.2.8/pushit/rpc/products.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461605 django_restit-4.2.8/pushit/static/js/models_pushit.js
--rw-r--r--   0        0        0      424 2023-08-01 06:36:56.109166 django_restit-4.2.8/pushit/tq.py
--rw-r--r--   0        0        0     2121 2023-07-24 17:36:54.438531 django_restit-4.2.8/pushit/utils.py
--rw-r--r--   0        0        0     1210 2023-12-20 17:42:01.789293 django_restit-4.2.8/pyproject.toml
--rw-r--r--   0        0        0      118 2023-06-27 05:37:44.461884 django_restit-4.2.8/rest/.gitignore
--rw-r--r--   0        0        0     5460 2023-06-27 05:37:44.461959 django_restit-4.2.8/rest/README.md
--rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462010 django_restit-4.2.8/rest/RemoteEvents.py
--rw-r--r--   0        0        0      120 2023-12-20 17:42:01.833778 django_restit-4.2.8/rest/__init__.py
--rw-r--r--   0        0        0     1967 2023-06-27 05:37:44.462114 django_restit-4.2.8/rest/arc4.py
--rw-r--r--   0        0        0       83 2023-06-27 05:37:44.462161 django_restit-4.2.8/rest/cache.py
--rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462295 django_restit-4.2.8/rest/crypto/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-27 05:37:44.462374 django_restit-4.2.8/rest/crypto/aes.py
--rw-r--r--   0        0        0     4082 2023-06-27 05:37:44.462442 django_restit-4.2.8/rest/crypto/privpub.py
--rw-r--r--   0        0        0     4514 2023-07-11 15:29:38.508089 django_restit-4.2.8/rest/crypto/util.py
--rw-r--r--   0        0        0     9330 2023-11-25 04:40:03.230095 django_restit-4.2.8/rest/datem.py
--rw-r--r--   0        0        0    15082 2023-12-09 17:07:25.089133 django_restit-4.2.8/rest/decorators.py
--rw-r--r--   0        0        0      788 2023-06-27 05:37:44.462816 django_restit-4.2.8/rest/encryption.py
--rw-r--r--   0        0        0      612 2023-12-19 00:02:03.767620 django_restit-4.2.8/rest/errors.py
--rw-r--r--   0        0        0       54 2023-06-27 05:37:44.462913 django_restit-4.2.8/rest/extra/__init__.py
--rw-r--r--   0        0        0     1078 2023-06-27 05:37:44.462982 django_restit-4.2.8/rest/extra/json_metadata.py
--rw-r--r--   0        0        0     9719 2023-06-27 05:37:44.463072 django_restit-4.2.8/rest/fields.py
--rw-r--r--   0        0        0     6316 2023-06-27 05:37:44.463145 django_restit-4.2.8/rest/forms.py
--rw-r--r--   0        0        0    26563 2023-12-17 18:42:16.439687 django_restit-4.2.8/rest/helpers.py
--rw-r--r--   0        0        0      260 2023-06-27 05:37:44.463338 django_restit-4.2.8/rest/joke.py
--rw-r--r--   0        0        0     2298 2023-06-27 05:37:44.463411 django_restit-4.2.8/rest/jwtoken.py
--rw-r--r--   0        0        0    20930 2023-06-27 15:33:50.289063 django_restit-4.2.8/rest/log.py
--rw-r--r--   0        0        0     7737 2023-09-13 21:40:41.824715 django_restit-4.2.8/rest/mail.py
--rw-r--r--   0        0        0     9174 2023-06-27 05:37:44.463711 django_restit-4.2.8/rest/mailman.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463776 django_restit-4.2.8/rest/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463861 django_restit-4.2.8/rest/management/commands/__init__.py
--rw-r--r--   0        0        0      389 2023-06-27 05:37:44.463942 django_restit-4.2.8/rest/management/commands/rpc.py
--rw-r--r--   0        0        0       33 2023-06-27 05:37:44.464028 django_restit-4.2.8/rest/middleware/__init__.py
--rw-r--r--   0        0        0     3513 2023-06-27 05:37:44.464096 django_restit-4.2.8/rest/middleware/cors.py
--rw-r--r--   0        0        0     2345 2023-06-27 05:37:44.464159 django_restit-4.2.8/rest/middleware/db_router.py
--rw-r--r--   0        0        0     6017 2023-11-29 03:51:44.491936 django_restit-4.2.8/rest/middleware/jwt.py
--rw-r--r--   0        0        0     4189 2023-11-15 19:37:49.027885 django_restit-4.2.8/rest/middleware/request.py
--rw-r--r--   0        0        0    10240 2023-07-17 21:30:14.707861 django_restit-4.2.8/rest/middleware/session.py
--rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.464450 django_restit-4.2.8/rest/middleware/session_store.py
--rw-r--r--   0        0        0      130 2023-07-11 15:56:36.722347 django_restit-4.2.8/rest/models/__init__.py
--rw-r--r--   0        0        0    66081 2023-12-09 19:57:57.872073 django_restit-4.2.8/rest/models/base.py
--rw-r--r--   0        0        0      578 2023-07-11 16:03:40.953305 django_restit-4.2.8/rest/models/cacher.py
--rw-r--r--   0        0        0    12631 2023-12-09 17:10:16.004033 django_restit-4.2.8/rest/models/metadata.py
--rw-r--r--   0        0        0     1691 2023-08-07 04:48:28.143401 django_restit-4.2.8/rest/net.py
--rw-r--r--   0        0        0   149463 2023-06-27 05:37:44.465139 django_restit-4.2.8/rest/regexes.yaml
--rw-r--r--   0        0        0    15701 2023-12-20 17:18:00.376275 django_restit-4.2.8/rest/requestex.py
--rw-r--r--   0        0        0     3612 2023-08-07 04:26:49.350849 django_restit-4.2.8/rest/rpc.py
--rw-r--r--   0        0        0     8362 2023-11-14 19:35:31.737708 django_restit-4.2.8/rest/search.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.465410 django_restit-4.2.8/rest/serializers/__init__.py
--rw-r--r--   0        0        0     4648 2023-11-15 20:41:11.119667 django_restit-4.2.8/rest/serializers/collection.py
--rw-r--r--   0        0        0     3251 2023-12-10 01:39:17.966410 django_restit-4.2.8/rest/serializers/csv.py
--rw-r--r--   0        0        0     1077 2023-06-27 05:37:44.465616 django_restit-4.2.8/rest/serializers/excel.py
--rw-r--r--   0        0        0     1736 2023-06-27 05:37:44.465675 django_restit-4.2.8/rest/serializers/json.py
--rw-r--r--   0        0        0    61981 2023-12-19 00:04:01.349514 django_restit-4.2.8/rest/serializers/legacy.py
--rw-r--r--   0        0        0     8598 2023-11-10 17:09:26.910604 django_restit-4.2.8/rest/serializers/model.py
--rw-r--r--   0        0        0      997 2023-07-06 18:50:18.372944 django_restit-4.2.8/rest/serializers/profiler.py
--rw-r--r--   0        0        0     7051 2023-12-19 00:03:41.185610 django_restit-4.2.8/rest/serializers/response.py
--rw-r--r--   0        0        0     2734 2023-06-27 05:37:44.466139 django_restit-4.2.8/rest/serializers/util.py
--rw-r--r--   0        0        0     1532 2023-06-27 05:37:44.466216 django_restit-4.2.8/rest/settings_helper.py
--rw-r--r--   0        0        0     1419 2023-08-07 05:26:37.128368 django_restit-4.2.8/rest/ssl_check.py
--rw-r--r--   0        0        0    95786 2023-06-27 05:37:44.466685 django_restit-4.2.8/rest/static/lib/jquery.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466742 django_restit-4.2.8/rest/static/rest/app.css
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466776 django_restit-4.2.8/rest/static/rest/app.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466808 django_restit-4.2.8/rest/static/rest/rest.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466846 django_restit-4.2.8/rest/static/rest/rest.scss
--rw-r--r--   0        0        0      529 2023-06-27 05:37:44.466992 django_restit-4.2.8/rest/templates/email/error.html
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.467020 django_restit-4.2.8/rest/templates/email/error.subject
--rw-r--r--   0        0        0     7148 2023-06-27 05:37:44.467101 django_restit-4.2.8/rest/templates/rest_docs.html
--rw-r--r--   0        0        0    10986 2023-12-17 18:47:10.126214 django_restit-4.2.8/rest/templates/rest_html.html
--rw-r--r--   0        0        0   185398 2023-07-28 01:56:34.391352 django_restit-4.2.8/rest/ua.py
--rw-r--r--   0        0        0    17064 2023-06-27 05:37:44.467734 django_restit-4.2.8/rest/uberdict.py
--rw-r--r--   0        0        0    11881 2023-06-27 05:37:44.467820 django_restit-4.2.8/rest/url_docs.py
--rw-r--r--   0        0        0     1869 2023-12-17 00:13:41.075590 django_restit-4.2.8/rest/urls.py
--rw-r--r--   0        0        0     1115 2023-12-17 00:40:15.697924 django_restit-4.2.8/rest/views.py
--rw-r--r--   0        0        0      118 2023-06-27 05:37:44.468007 django_restit-4.2.8/sessionlog/.gitignore
--rw-r--r--   0        0        0       62 2023-06-27 05:37:44.468062 django_restit-4.2.8/sessionlog/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468086 django_restit-4.2.8/sessionlog/__init__.py
--rw-r--r--   0        0        0      245 2023-06-27 05:37:44.468153 django_restit-4.2.8/sessionlog/admin.py
--rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.468231 django_restit-4.2.8/sessionlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468261 django_restit-4.2.8/sessionlog/migrations/__init__.py
--rw-r--r--   0        0        0     3662 2023-07-17 21:32:12.789126 django_restit-4.2.8/sessionlog/models.py
--rw-r--r--   0        0        0      383 2023-06-27 05:37:44.468400 django_restit-4.2.8/sessionlog/tests.py
--rw-r--r--   0        0        0       26 2023-06-27 05:37:44.468451 django_restit-4.2.8/sessionlog/views.py
--rw-r--r--   0        0        0     2196 2023-06-27 05:37:44.468543 django_restit-4.2.8/taskqueue/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468569 django_restit-4.2.8/taskqueue/__init__.py
--rw-r--r--   0        0        0      208 2023-06-27 05:37:44.468635 django_restit-4.2.8/taskqueue/admin.py
--rw-r--r--   0        0        0     4738 2023-06-27 05:37:44.468730 django_restit-4.2.8/taskqueue/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468758 django_restit-4.2.8/taskqueue/migrations/__init__.py
--rw-r--r--   0        0        0    19306 2023-12-18 15:27:25.429795 django_restit-4.2.8/taskqueue/models.py
--rw-r--r--   0        0        0     3543 2023-08-11 17:40:15.804907 django_restit-4.2.8/taskqueue/periodic.py
--rw-r--r--   0        0        0     5736 2023-12-09 17:45:37.022351 django_restit-4.2.8/taskqueue/rpc.py
--rw-r--r--   0        0        0      942 2023-06-27 05:37:44.469073 django_restit-4.2.8/taskqueue/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469126 django_restit-4.2.8/taskqueue/transports/__init__.py
--rw-r--r--   0        0        0      623 2023-06-27 05:37:44.469185 django_restit-4.2.8/taskqueue/transports/email.py
--rw-r--r--   0        0        0     2409 2023-08-31 21:55:56.632266 django_restit-4.2.8/taskqueue/transports/http.py
--rw-r--r--   0        0        0     1913 2023-10-30 22:13:38.540735 django_restit-4.2.8/taskqueue/transports/s3.py
--rw-r--r--   0        0        0     1891 2023-06-27 05:37:44.469341 django_restit-4.2.8/taskqueue/transports/sftp.py
--rw-r--r--   0        0        0      142 2023-06-27 05:37:44.469388 django_restit-4.2.8/taskqueue/transports/sms.py
--rw-r--r--   0        0        0    16050 2023-12-16 21:45:01.773610 django_restit-4.2.8/taskqueue/worker.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469517 django_restit-4.2.8/telephony/__init__.py
--rw-r--r--   0        0        0      243 2023-06-27 05:37:44.469571 django_restit-4.2.8/telephony/admin.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469591 django_restit-4.2.8/telephony/decorators.py
--rw-r--r--   0        0        0     3030 2023-06-27 05:37:44.469692 django_restit-4.2.8/telephony/migrations/0001_initial.py
--rw-r--r--   0        0        0      424 2023-11-27 22:03:30.384417 django_restit-4.2.8/telephony/migrations/0002_alter_sms_sid.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469714 django_restit-4.2.8/telephony/migrations/__init__.py
--rw-r--r--   0        0        0     8248 2023-12-09 17:49:10.656587 django_restit-4.2.8/telephony/models.py
--rw-r--r--   0        0        0     2426 2023-11-28 15:55:05.388090 django_restit-4.2.8/telephony/phone_util.py
--rw-r--r--   0        0        0     3473 2023-12-09 17:49:26.483244 django_restit-4.2.8/telephony/rpc.py
--rw-r--r--   0        0        0        1 2023-08-03 14:28:08.854157 django_restit-4.2.8/wiki/__init__.py
--rw-r--r--   0        0        0     3606 2023-08-04 04:52:16.019699 django_restit-4.2.8/wiki/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-08-04 04:52:16.018799 django_restit-4.2.8/wiki/migrations/__init__.py
--rw-r--r--   0        0        0      132 2023-08-04 03:46:50.913857 django_restit-4.2.8/wiki/models/__init__.py
--rw-r--r--   0        0        0     1745 2023-08-03 15:41:23.854674 django_restit-4.2.8/wiki/models/faq.py
--rw-r--r--   0        0        0     7203 2023-08-16 18:23:17.138555 django_restit-4.2.8/wiki/models/page.py
--rw-r--r--   0        0        0      729 2023-08-04 03:47:46.129186 django_restit-4.2.8/wiki/models/revision.py
--rw-r--r--   0        0        0      334 2023-08-03 14:28:08.854499 django_restit-4.2.8/wiki/periodic.py
--rw-r--r--   0        0        0      461 2023-08-03 15:34:25.031919 django_restit-4.2.8/wiki/renderers/__init__.py
--rwxr-xr-x   0        0        0       84 2022-09-24 04:49:32.000000 django_restit-4.2.8/wiki/renderers/mistune/__init__.py
--rwxr-xr-x   0        0        0     1264 2023-08-04 05:12:57.404938 django_restit-4.2.8/wiki/renderers/mistune/highlight.py
--rwxr-xr-x   0        0        0     1901 2022-09-24 04:49:32.000000 django_restit-4.2.8/wiki/renderers/mistune/math.py
--rw-r--r--   0        0        0     2610 2023-08-14 06:50:10.268306 django_restit-4.2.8/wiki/renderers/mistune/media.py
--rwxr-xr-x   0        0        0      805 2022-09-24 04:49:32.000000 django_restit-4.2.8/wiki/renderers/mistune/meta.py
--rw-r--r--   0        0        0     1889 2023-08-16 00:38:11.894074 django_restit-4.2.8/wiki/renderers/mistune/task_list.py
--rwxr-xr-x   0        0        0     2302 2023-08-04 05:12:30.563520 django_restit-4.2.8/wiki/renderers/mistune/toc.py
--rw-r--r--   0        0        0       40 2023-08-04 00:19:22.669056 django_restit-4.2.8/wiki/rpc/__init__.py
--rw-r--r--   0        0        0     1333 2023-08-16 18:28:15.622351 django_restit-4.2.8/wiki/rpc/wiki.py
--rw-r--r--   0        0        0      313 2023-08-03 14:28:08.854423 django_restit-4.2.8/wiki/tq.py
--rw-r--r--   0        0        0     3624 2023-06-27 05:37:44.470008 django_restit-4.2.8/ws4redis/README.md
--rwxr-xr-x   0        0        0       46 2023-06-27 05:37:44.470065 django_restit-4.2.8/ws4redis/__init__.py
--rw-r--r--   0        0        0     5049 2023-11-12 04:56:27.258942 django_restit-4.2.8/ws4redis/client.py
--rw-r--r--   0        0        0    13431 2023-08-14 17:22:44.326899 django_restit-4.2.8/ws4redis/connection.py
--rwxr-xr-x   0        0        0      636 2023-06-27 05:37:44.470295 django_restit-4.2.8/ws4redis/exceptions.py
--rw-r--r--   0        0        0     5561 2023-07-08 23:30:25.146274 django_restit-4.2.8/ws4redis/redis.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.470422 django_restit-4.2.8/ws4redis/servers/__init__.py
--rw-r--r--   0        0        0     3747 2023-06-27 05:37:44.470507 django_restit-4.2.8/ws4redis/servers/base.py
--rw-r--r--   0        0        0     4329 2023-06-27 05:37:44.470582 django_restit-4.2.8/ws4redis/servers/django.py
--rw-r--r--   0        0        0     1723 2023-06-27 05:37:44.470638 django_restit-4.2.8/ws4redis/servers/uwsgi.py
--rwxr-xr-x   0        0        0     1536 2023-08-14 17:15:40.285934 django_restit-4.2.8/ws4redis/settings.py
--rwxr-xr-x   0        0        0     5122 2023-06-27 05:37:44.470772 django_restit-4.2.8/ws4redis/utf8validator.py
--rwxr-xr-x   0        0        0    14848 2023-06-27 05:37:44.470868 django_restit-4.2.8/ws4redis/websocket.py
--rw-r--r--   0        0        0     7572 1970-01-01 00:00:00.000000 django_restit-4.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-27 05:37:44.430230 django_restit-4.2.9/LICENSE.md
+-rw-r--r--   0        0        0     6240 2023-07-18 17:15:13.487162 django_restit-4.2.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.430501 django_restit-4.2.9/account/__init__.py
+-rw-r--r--   0        0        0     1839 2023-06-27 05:37:44.430617 django_restit-4.2.9/account/admin.py
+-rw-r--r--   0        0        0      980 2023-06-27 05:37:44.430754 django_restit-4.2.9/account/fcm/__init__.py
+-rw-r--r--   0        0        0    15894 2023-06-27 05:37:44.430954 django_restit-4.2.9/account/migrations/0001_initial.py
+-rw-r--r--   0        0        0      738 2023-06-27 05:37:44.431054 django_restit-4.2.9/account/migrations/0003_member_phone_number.py
+-rw-r--r--   0        0        0      551 2023-06-27 05:37:44.431131 django_restit-4.2.9/account/migrations/0004_group_modified_alter_group_created.py
+-rw-r--r--   0        0        0      437 2023-06-27 05:37:44.431211 django_restit-4.2.9/account/migrations/0005_member_auth_code_expires.py
+-rw-r--r--   0        0        0      450 2023-06-27 05:37:44.431293 django_restit-4.2.9/account/migrations/0006_member_security_token.py
+-rw-r--r--   0        0        0     1654 2023-06-27 05:37:44.431375 django_restit-4.2.9/account/migrations/0007_authtoken_signature_authsession.py
+-rw-r--r--   0        0        0     2379 2023-06-27 05:37:44.431464 django_restit-4.2.9/account/migrations/0008_memberdevice_memberdevicemetadata.py
+-rw-r--r--   0        0        0      468 2023-06-27 05:37:44.431538 django_restit-4.2.9/account/migrations/0009_alter_member_phone_number.py
+-rw-r--r--   0        0        0      305 2023-06-27 05:37:44.431613 django_restit-4.2.9/account/migrations/0010_delete_authtoken.py
+-rw-r--r--   0        0        0     1062 2023-06-27 05:37:44.431685 django_restit-4.2.9/account/migrations/0011_authtoken.py
+-rw-r--r--   0        0        0     2043 2023-06-27 05:37:44.431755 django_restit-4.2.9/account/migrations/0012_settings_settingsmetadata.py
+-rw-r--r--   0        0        0      418 2023-07-13 15:44:27.208937 django_restit-4.2.9/account/migrations/0013_memberdevice_ip.py
+-rw-r--r--   0        0        0      541 2023-11-07 12:44:14.024459 django_restit-4.2.9/account/migrations/0014_alter_notificationmemberrecord_member.py
+-rw-r--r--   0        0        0      460 2023-11-15 19:46:51.612834 django_restit-4.2.9/account/migrations/0015_memberdevice_buid.py
+-rw-r--r--   0        0        0      424 2023-11-15 20:20:37.084916 django_restit-4.2.9/account/migrations/0016_authsession_buid.py
+-rw-r--r--   0        0        0      375 2023-11-28 23:26:56.206776 django_restit-4.2.9/account/migrations/0017_rename_requires_topt_member_requires_totp.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.431784 django_restit-4.2.9/account/migrations/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-27 05:37:44.431899 django_restit-4.2.9/account/models/__init__.py
+-rw-r--r--   0        0        0     4105 2023-11-15 20:24:03.414109 django_restit-4.2.9/account/models/device.py
+-rw-r--r--   0        0        0     1437 2023-06-27 05:37:44.432051 django_restit-4.2.9/account/models/feeds.py
+-rw-r--r--   0        0        0    20064 2023-12-15 19:46:55.047382 django_restit-4.2.9/account/models/group.py
+-rw-r--r--   0        0        0     2720 2023-06-27 05:37:44.432315 django_restit-4.2.9/account/models/legacy.py
+-rw-r--r--   0        0        0    49327 2023-12-19 20:43:30.083308 django_restit-4.2.9/account/models/member.py
+-rw-r--r--   0        0        0     7763 2023-12-09 22:24:04.788938 django_restit-4.2.9/account/models/membership.py
+-rw-r--r--   0        0        0    12078 2023-11-17 21:39:46.651560 django_restit-4.2.9/account/models/notify.py
+-rw-r--r--   0        0        0     3509 2023-11-15 20:20:12.123435 django_restit-4.2.9/account/models/session.py
+-rw-r--r--   0        0        0     2137 2023-06-27 05:37:44.432966 django_restit-4.2.9/account/models/settings.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.433042 django_restit-4.2.9/account/oauth/__init__.py
+-rw-r--r--   0        0        0     2078 2023-06-27 05:37:44.433131 django_restit-4.2.9/account/oauth/google.py
+-rw-r--r--   0        0        0      874 2023-11-29 03:43:42.972754 django_restit-4.2.9/account/periodic.py
+-rw-r--r--   0        0        0      152 2023-06-27 05:37:44.433297 django_restit-4.2.9/account/rpc/__init__.py
+-rw-r--r--   0        0        0    14896 2023-12-19 15:38:33.959934 django_restit-4.2.9/account/rpc/auth.py
+-rw-r--r--   0        0        0     2852 2023-07-13 15:33:42.583999 django_restit-4.2.9/account/rpc/device.py
+-rw-r--r--   0        0        0     3472 2023-12-04 21:21:15.602286 django_restit-4.2.9/account/rpc/group.py
+-rw-r--r--   0        0        0     1150 2023-06-27 05:37:44.433650 django_restit-4.2.9/account/rpc/member.py
+-rw-r--r--   0        0        0     3344 2023-06-27 05:37:44.433726 django_restit-4.2.9/account/rpc/notify.py
+-rw-r--r--   0        0        0     2669 2023-12-17 00:40:58.671312 django_restit-4.2.9/account/rpc/oauth.py
+-rw-r--r--   0        0        0      271 2023-06-27 05:37:44.433874 django_restit-4.2.9/account/rpc/settings.py
+-rw-r--r--   0        0        0       53 2023-06-27 05:37:44.433934 django_restit-4.2.9/account/settings.py
+-rw-r--r--   0        0        0     9709 2023-06-27 05:37:44.434095 django_restit-4.2.9/account/templates/email/base.html
+-rw-r--r--   0        0        0    10567 2023-06-27 05:37:44.434205 django_restit-4.2.9/account/templates/email/invite.html
+-rw-r--r--   0        0        0    12609 2023-11-07 13:31:04.277159 django_restit-4.2.9/account/templates/email/plain/base.html
+-rw-r--r--   0        0        0    15235 2023-09-13 21:51:42.921379 django_restit-4.2.9/account/templates/email/plain/invite.html
+-rw-r--r--   0        0        0    13954 2023-06-27 05:37:44.434450 django_restit-4.2.9/account/templates/email/plain/reset_code.html
+-rw-r--r--   0        0        0    10261 2023-06-27 05:37:44.434528 django_restit-4.2.9/account/templates/email/reset_code.html
+-rw-r--r--   0        0        0    15147 2023-09-13 21:29:05.002359 django_restit-4.2.9/account/templates/email/simple/invite.html
+-rw-r--r--   0        0        0    13944 2023-06-27 05:37:44.434713 django_restit-4.2.9/account/templates/email/simple/reset_code.html
+-rw-r--r--   0        0        0      520 2023-06-27 05:37:44.434828 django_restit-4.2.9/auditlog/README
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.434859 django_restit-4.2.9/auditlog/__init__.py
+-rw-r--r--   0        0        0     1006 2023-06-27 05:37:44.434933 django_restit-4.2.9/auditlog/admin.py
+-rw-r--r--   0        0        0     6553 2023-06-27 05:37:44.435019 django_restit-4.2.9/auditlog/decorators.py
+-rw-r--r--   0        0        0     1511 2023-12-17 00:38:09.426633 django_restit-4.2.9/auditlog/middleware.py
+-rw-r--r--   0        0        0     3309 2023-06-27 05:37:44.435191 django_restit-4.2.9/auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435224 django_restit-4.2.9/auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0    16294 2023-11-28 17:50:33.116663 django_restit-4.2.9/auditlog/models.py
+-rw-r--r--   0        0        0      363 2023-11-06 22:55:59.417756 django_restit-4.2.9/auditlog/periodic.py
+-rw-r--r--   0        0        0     3591 2023-12-09 17:40:20.663908 django_restit-4.2.9/auditlog/rpc.py
+-rw-r--r--   0        0        0     2415 2023-11-06 23:04:22.220672 django_restit-4.2.9/auditlog/tq.py
+-rw-r--r--   0        0        0      163 2023-06-27 05:37:44.435623 django_restit-4.2.9/auditlog/urls.py
+-rw-r--r--   0        0        0     2169 2023-06-27 05:37:44.435745 django_restit-4.2.9/inbox/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435775 django_restit-4.2.9/inbox/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-27 05:37:44.435850 django_restit-4.2.9/inbox/admin.py
+-rw-r--r--   0        0        0     5638 2023-11-17 19:40:32.512907 django_restit-4.2.9/inbox/handlers.py
+-rw-r--r--   0        0        0     6429 2023-06-27 05:37:44.436034 django_restit-4.2.9/inbox/migrations/0001_initial.py
+-rw-r--r--   0        0        0      380 2023-06-27 05:37:44.436102 django_restit-4.2.9/inbox/migrations/0002_alter_message_cc.py
+-rw-r--r--   0        0        0      416 2023-06-27 05:37:44.436177 django_restit-4.2.9/inbox/migrations/0003_attachment_content_type.py
+-rw-r--r--   0        0        0     1140 2023-06-27 05:37:44.436249 django_restit-4.2.9/inbox/migrations/0004_mailtemplate.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.436274 django_restit-4.2.9/inbox/migrations/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-27 05:37:44.436383 django_restit-4.2.9/inbox/models/__init__.py
+-rw-r--r--   0        0        0     2881 2023-12-09 17:43:11.500207 django_restit-4.2.9/inbox/models/bounce.py
+-rw-r--r--   0        0        0     2517 2023-12-09 17:43:15.908858 django_restit-4.2.9/inbox/models/complaint.py
+-rw-r--r--   0        0        0     3003 2023-12-09 17:43:26.636118 django_restit-4.2.9/inbox/models/message.py
+-rw-r--r--   0        0        0     1013 2023-06-27 05:37:44.436870 django_restit-4.2.9/inbox/models/template.py
+-rw-r--r--   0        0        0     1534 2023-06-27 05:37:44.436956 django_restit-4.2.9/inbox/rpc.py
+-rw-r--r--   0        0        0       89 2023-06-27 05:37:44.437057 django_restit-4.2.9/inbox/utils/__init__.py
+-rw-r--r--   0        0        0     4615 2023-11-17 22:20:26.650843 django_restit-4.2.9/inbox/utils/parsing.py
+-rw-r--r--   0        0        0     4098 2023-06-27 05:37:44.437260 django_restit-4.2.9/inbox/utils/render.py
+-rw-r--r--   0        0        0     2179 2023-11-09 19:28:02.561057 django_restit-4.2.9/inbox/utils/sending.py
+-rw-r--r--   0        0        0     1114 2023-06-27 05:37:44.437469 django_restit-4.2.9/incident/README.md
+-rw-r--r--   0        0        0     3249 2023-12-09 16:49:33.350637 django_restit-4.2.9/incident/__init__.py
+-rw-r--r--   0        0        0     9720 2023-06-27 05:37:44.437670 django_restit-4.2.9/incident/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2023-06-27 05:37:44.437757 django_restit-4.2.9/incident/migrations/0002_event_component_event_component_id.py
+-rw-r--r--   0        0        0      425 2023-06-27 05:37:44.437826 django_restit-4.2.9/incident/migrations/0003_rule_action.py
+-rw-r--r--   0        0        0      662 2023-06-27 05:37:44.437890 django_restit-4.2.9/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
+-rw-r--r--   0        0        0      698 2023-06-27 05:37:44.437964 django_restit-4.2.9/incident/migrations/0005_incident_component_alter_incident_state.py
+-rw-r--r--   0        0        0      324 2023-06-27 05:37:44.438034 django_restit-4.2.9/incident/migrations/0006_delete_eventmetadata.py
+-rw-r--r--   0        0        0      414 2023-06-27 05:37:44.438100 django_restit-4.2.9/incident/migrations/0007_event_metadata.py
+-rw-r--r--   0        0        0      903 2023-06-27 05:37:44.438184 django_restit-4.2.9/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
+-rw-r--r--   0        0        0      473 2023-08-22 19:29:15.953220 django_restit-4.2.9/incident/migrations/0009_incident_reporter_ip.py
+-rw-r--r--   0        0        0      631 2023-11-20 03:38:24.557282 django_restit-4.2.9/incident/migrations/0010_incident_category_incident_component_id.py
+-rw-r--r--   0        0        0     2142 2023-11-20 03:51:50.549436 django_restit-4.2.9/incident/migrations/0011_ticket.py
+-rw-r--r--   0        0        0      372 2023-12-19 03:25:06.153029 django_restit-4.2.9/incident/migrations/0012_rule_match_by.py
+-rw-r--r--   0        0        0      387 2023-12-19 17:40:50.828606 django_restit-4.2.9/incident/migrations/0013_rulecheck_is_required.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438214 django_restit-4.2.9/incident/migrations/__init__.py
+-rw-r--r--   0        0        0      209 2023-11-20 03:49:22.992273 django_restit-4.2.9/incident/models/__init__.py
+-rw-r--r--   0        0        0     6849 2023-12-09 19:39:18.790758 django_restit-4.2.9/incident/models/event.py
+-rw-r--r--   0        0        0    15294 2023-12-20 17:41:19.779521 django_restit-4.2.9/incident/models/incident.py
+-rw-r--r--   0        0        0     2227 2023-12-09 16:28:25.375197 django_restit-4.2.9/incident/models/ossec.py
+-rw-r--r--   0        0        0     6024 2023-12-19 17:45:22.401412 django_restit-4.2.9/incident/models/rules.py
+-rw-r--r--   0        0        0     2302 2023-11-20 03:51:47.283232 django_restit-4.2.9/incident/models/ticket.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438911 django_restit-4.2.9/incident/parsers/__init__.py
+-rw-r--r--   0        0        0     6247 2023-12-19 21:01:44.694027 django_restit-4.2.9/incident/parsers/ossec.py
+-rw-r--r--   0        0        0      227 2023-11-28 04:04:56.458420 django_restit-4.2.9/incident/periodic.py
+-rw-r--r--   0        0        0     7546 2023-12-19 00:05:09.162867 django_restit-4.2.9/incident/rpc.py
+-rw-r--r--   0        0        0    14178 2023-11-18 15:34:42.122382 django_restit-4.2.9/incident/templates/email/incident_change.html
+-rw-r--r--   0        0        0    15173 2023-06-27 05:37:44.439515 django_restit-4.2.9/incident/templates/email/incident_new.html
+-rw-r--r--   0        0        0    14727 2023-11-20 22:01:29.858057 django_restit-4.2.9/incident/templates/email/incident_plain.html
+-rw-r--r--   0        0        0     4589 2023-12-21 04:40:51.784780 django_restit-4.2.9/incident/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.439791 django_restit-4.2.9/location/__init__.py
+-rw-r--r--   0        0        0      297 2023-06-27 05:37:44.439885 django_restit-4.2.9/location/admin.py
+-rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.440042 django_restit-4.2.9/location/geolocate.py
+-rw-r--r--   0        0        0     7000 2023-06-27 05:37:44.440236 django_restit-4.2.9/location/migrations/0001_initial.py
+-rw-r--r--   0        0        0      576 2023-06-27 05:37:44.440313 django_restit-4.2.9/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440339 django_restit-4.2.9/location/migrations/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-27 05:37:44.440480 django_restit-4.2.9/location/models/__init__.py
+-rw-r--r--   0        0        0     2028 2023-06-27 05:37:44.440559 django_restit-4.2.9/location/models/address.py
+-rw-r--r--   0        0        0     5984 2023-12-09 17:41:39.358207 django_restit-4.2.9/location/models/ip.py
+-rw-r--r--   0        0        0     1994 2023-06-27 05:37:44.440722 django_restit-4.2.9/location/models/legacy.py
+-rw-r--r--   0        0        0     2316 2023-06-27 05:37:44.440785 django_restit-4.2.9/location/models/location.py
+-rw-r--r--   0        0        0     1474 2023-06-27 05:37:44.440843 django_restit-4.2.9/location/models/track.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440920 django_restit-4.2.9/location/providers/__init__.py
+-rw-r--r--   0        0        0      727 2023-08-07 06:30:37.235541 django_restit-4.2.9/location/providers/iplookup/__init__.py
+-rw-r--r--   0        0        0     2419 2023-06-27 05:37:44.441128 django_restit-4.2.9/location/providers/iplookup/abstractapi.py
+-rw-r--r--   0        0        0     1345 2023-06-27 05:37:44.441192 django_restit-4.2.9/location/providers/iplookup/extremeip.py
+-rw-r--r--   0        0        0     2121 2023-06-27 05:37:44.441260 django_restit-4.2.9/location/providers/iplookup/geoplugin.py
+-rw-r--r--   0        0        0     1797 2023-06-27 05:37:44.441325 django_restit-4.2.9/location/providers/iplookup/ipapi.py
+-rw-r--r--   0        0        0     1265 2023-06-27 05:37:44.441395 django_restit-4.2.9/location/providers/iplookup/ipinfo.py
+-rw-r--r--   0        0        0      937 2023-06-27 05:37:44.441463 django_restit-4.2.9/location/providers/iplookup/restit.py
+-rw-r--r--   0        0        0       42 2023-06-27 05:37:44.441569 django_restit-4.2.9/location/providers/location/__init__.py
+-rw-r--r--   0        0        0     2860 2023-06-27 05:37:44.441653 django_restit-4.2.9/location/providers/location/google.py
+-rw-r--r--   0        0        0       46 2023-06-27 05:37:44.441777 django_restit-4.2.9/location/providers/timezones/__init__.py
+-rw-r--r--   0        0        0      619 2023-06-27 05:37:44.441855 django_restit-4.2.9/location/providers/timezones/google.py
+-rw-r--r--   0        0        0     1935 2023-06-27 05:37:44.441924 django_restit-4.2.9/location/providers/zillow.py
+-rw-r--r--   0        0        0      123 2023-06-27 05:37:44.442046 django_restit-4.2.9/location/rpc/__init__.py
+-rw-r--r--   0        0        0     1305 2023-11-27 23:53:10.865156 django_restit-4.2.9/location/rpc/ip.py
+-rw-r--r--   0        0        0      779 2023-06-27 05:37:44.442183 django_restit-4.2.9/location/rpc/location.py
+-rw-r--r--   0        0        0     3735 2023-06-27 05:37:44.442254 django_restit-4.2.9/location/rpc/track.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.442312 django_restit-4.2.9/medialib/__init__.py
+-rw-r--r--   0        0        0     2261 2023-06-27 05:37:44.442393 django_restit-4.2.9/medialib/admin.py
+-rw-r--r--   0        0        0       27 2023-06-27 05:37:44.442482 django_restit-4.2.9/medialib/cvutil/__init__.py
+-rw-r--r--   0        0        0     4269 2023-06-27 05:37:44.442556 django_restit-4.2.9/medialib/cvutil/contours.py
+-rw-r--r--   0        0        0    12649 2023-06-27 05:37:44.442653 django_restit-4.2.9/medialib/cvutil/images.py
+-rw-r--r--   0        0        0     9586 2023-06-27 05:37:44.442744 django_restit-4.2.9/medialib/cvutil/misc.py
+-rw-r--r--   0        0        0     5824 2023-06-27 05:37:44.442838 django_restit-4.2.9/medialib/cvutil/text.py
+-rw-r--r--   0        0        0    48442 2023-06-27 05:37:44.443047 django_restit-4.2.9/medialib/fixtures/initial_data.json
+-rw-r--r--   0        0        0    31978 2023-06-27 05:37:44.443182 django_restit-4.2.9/medialib/fixtures/medialib.json
+-rw-r--r--   0        0        0    16989 2023-06-27 05:37:44.443279 django_restit-4.2.9/medialib/fixtures/medialib_test_fixture.json
+-rw-r--r--   0        0        0     5442 2023-06-27 05:37:44.443362 django_restit-4.2.9/medialib/forms.py
+-rw-r--r--   0        0        0    20518 2023-06-27 05:37:44.443459 django_restit-4.2.9/medialib/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.443499 django_restit-4.2.9/medialib/migrations/__init__.py
+-rw-r--r--   0        0        0    52152 2023-10-09 22:04:22.261815 django_restit-4.2.9/medialib/models.py
+-rw-r--r--   0        0        0     1189 2023-06-27 05:37:44.443785 django_restit-4.2.9/medialib/ocr.py
+-rw-r--r--   0        0        0     1275 2023-06-27 05:37:44.443858 django_restit-4.2.9/medialib/pdf.py
+-rw-r--r--   0        0        0      545 2023-06-27 05:37:44.443925 django_restit-4.2.9/medialib/qrcode.py
+-rw-r--r--   0        0        0    10312 2023-06-27 05:37:44.444059 django_restit-4.2.9/medialib/render/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444125 django_restit-4.2.9/medialib/render/engines/__init__.py
+-rw-r--r--   0        0        0     3531 2023-06-27 05:37:44.444213 django_restit-4.2.9/medialib/render/engines/anigif.py
+-rw-r--r--   0        0        0     6881 2023-06-27 05:37:44.444291 django_restit-4.2.9/medialib/render/engines/ffmpeg.py
+-rw-r--r--   0        0        0      792 2023-06-27 05:37:44.444369 django_restit-4.2.9/medialib/render/engines/gifsicle.py
+-rw-r--r--   0        0        0     3436 2023-06-27 05:37:44.444438 django_restit-4.2.9/medialib/render/engines/hls.py
+-rw-r--r--   0        0        0      983 2023-06-27 05:37:44.444498 django_restit-4.2.9/medialib/render/engines/mp4box.py
+-rw-r--r--   0        0        0      397 2023-06-27 05:37:44.444604 django_restit-4.2.9/medialib/render/engines/rtmp/Makefile
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444636 django_restit-4.2.9/medialib/render/engines/rtmp/__init__.py
+-rw-r--r--   0        0        0     4026 2023-06-27 05:37:44.444726 django_restit-4.2.9/medialib/render/engines/rtmp/rtmp.i
+-rw-r--r--   0        0        0      699 2023-06-27 05:37:44.444798 django_restit-4.2.9/medialib/render/engines/rtmpdump.py
+-rw-r--r--   0        0        0     1017 2023-06-27 05:37:44.444865 django_restit-4.2.9/medialib/render/engines/rtmpsink.py
+-rw-r--r--   0        0        0     3466 2023-06-27 05:37:44.444941 django_restit-4.2.9/medialib/render/engines/video_getinfo.py
+-rw-r--r--   0        0        0      809 2023-06-27 05:37:44.445017 django_restit-4.2.9/medialib/render/engines/websnap.py
+-rw-r--r--   0        0        0     2193 2023-06-27 05:37:44.445078 django_restit-4.2.9/medialib/render/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.445133 django_restit-4.2.9/medialib/render/presets/__init__.py
+-rw-r--r--   0        0        0     4179 2023-06-27 05:37:44.445227 django_restit-4.2.9/medialib/render/presets/akamai.py
+-rw-r--r--   0        0        0     3284 2023-06-27 05:37:44.445306 django_restit-4.2.9/medialib/render/presets/animated_thumbnail.py
+-rw-r--r--   0        0        0     4004 2023-06-27 05:37:44.445394 django_restit-4.2.9/medialib/render/presets/ffmpeg.py
+-rw-r--r--   0        0        0     2087 2023-06-27 05:37:44.445469 django_restit-4.2.9/medialib/render/presets/flv.py
+-rw-r--r--   0        0        0     6567 2023-06-27 05:37:44.445567 django_restit-4.2.9/medialib/render/presets/hls.py
+-rw-r--r--   0        0        0     6955 2023-06-27 05:37:44.445668 django_restit-4.2.9/medialib/render/presets/image_transcode.py
+-rw-r--r--   0        0        0     1094 2023-06-27 05:37:44.445750 django_restit-4.2.9/medialib/render/presets/image_validate.py
+-rw-r--r--   0        0        0     2423 2023-06-27 05:37:44.445825 django_restit-4.2.9/medialib/render/presets/mp4.py
+-rw-r--r--   0        0        0     4997 2023-06-27 05:37:44.445908 django_restit-4.2.9/medialib/render/presets/video_still.py
+-rw-r--r--   0        0        0     3228 2023-06-27 05:37:44.445986 django_restit-4.2.9/medialib/render/presets/video_validate.py
+-rw-r--r--   0        0        0      863 2023-06-27 05:37:44.446101 django_restit-4.2.9/medialib/render/presets/websnap.py
+-rw-r--r--   0        0        0     2282 2023-06-27 05:37:44.446183 django_restit-4.2.9/medialib/render/presets/youtube.py
+-rw-r--r--   0        0        0    16451 2023-06-27 05:37:44.446294 django_restit-4.2.9/medialib/render/render_utils.py
+-rw-r--r--   0        0        0      370 2023-06-27 05:37:44.446381 django_restit-4.2.9/medialib/render/schedule.py
+-rw-r--r--   0        0        0       82 2023-06-27 05:37:44.446525 django_restit-4.2.9/medialib/rpc/__init__.py
+-rw-r--r--   0        0        0    37925 2023-06-27 05:37:44.446687 django_restit-4.2.9/medialib/rpc/legacy.py
+-rw-r--r--   0        0        0      617 2023-06-27 05:37:44.446776 django_restit-4.2.9/medialib/rpc/media.py
+-rw-r--r--   0        0        0      956 2023-06-27 05:37:44.446852 django_restit-4.2.9/medialib/rpc/tools.py
+-rwxr-xr-x   0        0        0     7875 2023-06-27 05:37:44.446994 django_restit-4.2.9/medialib/scripts/init_config
+-rw-r--r--   0        0        0     4499 2023-06-27 05:37:44.447158 django_restit-4.2.9/medialib/static/css/base_medialibui.css
+-rw-r--r--   0        0        0     3128 2023-06-27 05:37:44.447238 django_restit-4.2.9/medialib/static/css/base_widgets.css
+-rw-r--r--   0        0        0     3263 2023-06-27 05:37:44.447311 django_restit-4.2.9/medialib/static/css/jquery.jcrop.css
+-rw-r--r--   0        0        0      193 2023-06-27 05:37:44.447412 django_restit-4.2.9/medialib/static/img/arrow-down-white.png
+-rw-r--r--   0        0        0     4589 2023-06-27 05:37:44.447507 django_restit-4.2.9/medialib/static/img/bg-body.gif
+-rw-r--r--   0        0        0      441 2023-06-27 05:37:44.447579 django_restit-4.2.9/medialib/static/img/cancel.gif
+-rw-r--r--   0        0        0      341 2023-06-27 05:37:44.447648 django_restit-4.2.9/medialib/static/img/icon-generic.gif
+-rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447712 django_restit-4.2.9/medialib/static/img/icon-image.gif
+-rw-r--r--   0        0        0      359 2023-06-27 05:37:44.447775 django_restit-4.2.9/medialib/static/img/icon-media.gif
+-rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447850 django_restit-4.2.9/medialib/static/img/icon-zip.gif
+-rw-r--r--   0        0        0     3208 2023-06-27 05:37:44.447934 django_restit-4.2.9/medialib/static/img/loading.gif
+-rw-r--r--   0        0        0     2537 2023-06-27 05:37:44.448000 django_restit-4.2.9/medialib/static/img/noimage.gif
+-rw-r--r--   0        0        0     1057 2023-06-27 05:37:44.448065 django_restit-4.2.9/medialib/static/img/render_err.gif
+-rw-r--r--   0        0        0     6716 2023-06-27 05:37:44.448158 django_restit-4.2.9/medialib/static/img/rendering.gif
+-rw-r--r--   0        0        0      292 2023-06-27 05:37:44.448225 django_restit-4.2.9/medialib/static/img/star_off.png
+-rw-r--r--   0        0        0      297 2023-06-27 05:37:44.448287 django_restit-4.2.9/medialib/static/img/star_on.png
+-rw-r--r--   0        0        0     1130 2023-06-27 05:37:44.448351 django_restit-4.2.9/medialib/static/img/unknown.gif
+-rwxr-xr-x   0        0        0    74054 2023-06-27 05:37:44.448677 django_restit-4.2.9/medialib/static/lib/caman.full.js
+-rw-r--r--   0        0        0    17360 2023-06-27 05:37:44.448823 django_restit-4.2.9/medialib/static/lib/hammer.min.js
+-rwxr-xr-x   0        0        0    42434 2023-06-27 05:37:44.449017 django_restit-4.2.9/medialib/static/lib/jquery.Jcrop.js
+-rw-r--r--   0        0        0      743 2023-06-27 05:37:44.449098 django_restit-4.2.9/medialib/static/lib/jquery.hammer.js
+-rw-r--r--   0        0        0    16587 2023-06-27 05:37:44.449224 django_restit-4.2.9/medialib/static/lib/load-image.min.js
+-rwxr-xr-x   0        0        0   111779 2023-06-27 05:37:44.449542 django_restit-4.2.9/medialib/static/lib/swiper.js
+-rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449771 django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
+-rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449850 django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
+-rw-r--r--   0        0        0     5708 2023-06-27 05:37:44.449979 django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
+-rw-r--r--   0        0        0     3502 2023-06-27 05:37:44.450059 django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/medialib.html
+-rw-r--r--   0        0        0     5876 2023-06-27 05:37:44.450187 django_restit-4.2.9/medialib/stores/__init__.py
+-rw-r--r--   0        0        0      601 2023-06-27 05:37:44.450314 django_restit-4.2.9/medialib/stores/apiclient/__init__.py
+-rw-r--r--   0        0        0     9852 2023-06-27 05:37:44.450415 django_restit-4.2.9/medialib/stores/apiclient/channel.py
+-rw-r--r--   0        0        0    35929 2023-06-27 05:37:44.450591 django_restit-4.2.9/medialib/stores/apiclient/discovery.py
+-rw-r--r--   0        0        0     3516 2023-06-27 05:37:44.450684 django_restit-4.2.9/medialib/stores/apiclient/errors.py
+-rw-r--r--   0        0        0    52911 2023-06-27 05:37:44.450906 django_restit-4.2.9/medialib/stores/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.451002 django_restit-4.2.9/medialib/stores/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11761 2023-06-27 05:37:44.451111 django_restit-4.2.9/medialib/stores/apiclient/model.py
+-rw-r--r--   0        0        0     3528 2023-06-27 05:37:44.451205 django_restit-4.2.9/medialib/stores/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9293 2023-06-27 05:37:44.451302 django_restit-4.2.9/medialib/stores/apiclient/schema.py
+-rw-r--r--   0        0        0     1592 2023-06-27 05:37:44.451390 django_restit-4.2.9/medialib/stores/filestore.py
+-rw-r--r--   0        0        0    69575 2023-06-27 05:37:44.451712 django_restit-4.2.9/medialib/stores/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.451937 django_restit-4.2.9/medialib/stores/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.452031 django_restit-4.2.9/medialib/stores/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.452160 django_restit-4.2.9/medialib/stores/httplib2/socks.py
+-rw-r--r--   0        0        0      706 2023-06-27 05:37:44.452238 django_restit-4.2.9/medialib/stores/httpstore.py
+-rw-r--r--   0        0        0      304 2023-06-27 05:37:44.452325 django_restit-4.2.9/medialib/stores/nullstore.py
+-rw-r--r--   0        0        0      213 2023-06-27 05:37:44.452492 django_restit-4.2.9/medialib/stores/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.452598 django_restit-4.2.9/medialib/stores/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.452767 django_restit-4.2.9/medialib/stores/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44346 2023-06-27 05:37:44.452995 django_restit-4.2.9/medialib/stores/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.453091 django_restit-4.2.9/medialib/stores/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.453196 django_restit-4.2.9/medialib/stores/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3755 2023-06-27 05:37:44.453276 django_restit-4.2.9/medialib/stores/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.453391 django_restit-4.2.9/medialib/stores/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.453451 django_restit-4.2.9/medialib/stores/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.453541 django_restit-4.2.9/medialib/stores/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.453634 django_restit-4.2.9/medialib/stores/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.453698 django_restit-4.2.9/medialib/stores/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.453764 django_restit-4.2.9/medialib/stores/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.453855 django_restit-4.2.9/medialib/stores/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.453938 django_restit-4.2.9/medialib/stores/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.454013 django_restit-4.2.9/medialib/stores/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0      500 2023-06-27 05:37:44.454077 django_restit-4.2.9/medialib/stores/rtmpstore.py
+-rw-r--r--   0        0        0     4583 2023-06-27 05:37:44.454163 django_restit-4.2.9/medialib/stores/s3store.py
+-rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.454272 django_restit-4.2.9/medialib/stores/uritemplate/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-27 05:37:44.454334 django_restit-4.2.9/medialib/stores/youtubestore.py
+-rw-r--r--   0        0        0     3691 2023-06-27 05:37:44.454500 django_restit-4.2.9/medialib/templates/medialib/base.html
+-rw-r--r--   0        0        0     1277 2023-06-27 05:37:44.454591 django_restit-4.2.9/medialib/templates/medialib/instances.html
+-rw-r--r--   0        0        0     1170 2023-06-27 05:37:44.454657 django_restit-4.2.9/medialib/templates/medialib/items.html
+-rw-r--r--   0        0        0     8194 2023-06-27 05:37:44.454746 django_restit-4.2.9/medialib/templates/medialib/library.html
+-rw-r--r--   0        0        0       65 2023-06-27 05:37:44.454810 django_restit-4.2.9/medialib/templates/medialib/notify_error.subject
+-rw-r--r--   0        0        0       49 2023-06-27 05:37:44.454869 django_restit-4.2.9/medialib/templates/medialib/notify_error.to
+-rw-r--r--   0        0        0      272 2023-06-27 05:37:44.454932 django_restit-4.2.9/medialib/templates/medialib/notify_error.txt
+-rw-r--r--   0        0        0       71 2023-06-27 05:37:44.454996 django_restit-4.2.9/medialib/templates/medialib/notify_ready.subject
+-rw-r--r--   0        0        0       49 2023-06-27 05:37:44.455056 django_restit-4.2.9/medialib/templates/medialib/notify_ready.to
+-rw-r--r--   0        0        0      298 2023-06-27 05:37:44.455113 django_restit-4.2.9/medialib/templates/medialib/notify_ready.txt
+-rw-r--r--   0        0        0       64 2023-06-27 05:37:44.455175 django_restit-4.2.9/medialib/templates/medialib/notify_render_error.subject
+-rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455232 django_restit-4.2.9/medialib/templates/medialib/notify_render_error.to
+-rw-r--r--   0        0        0      271 2023-06-27 05:37:44.455301 django_restit-4.2.9/medialib/templates/medialib/notify_render_error.txt
+-rw-r--r--   0        0        0       68 2023-06-27 05:37:44.455380 django_restit-4.2.9/medialib/templates/medialib/notify_validate_error.subject
+-rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455452 django_restit-4.2.9/medialib/templates/medialib/notify_validate_error.to
+-rw-r--r--   0        0        0      275 2023-06-27 05:37:44.455521 django_restit-4.2.9/medialib/templates/medialib/notify_validate_error.txt
+-rw-r--r--   0        0        0      206 2023-06-27 05:37:44.455593 django_restit-4.2.9/medialib/templates/medialib/smil
+-rw-r--r--   0        0        0     1177 2023-06-27 05:37:44.455665 django_restit-4.2.9/medialib/templates/medialib/test.html
+-rw-r--r--   0        0        0     1549 2023-06-27 05:37:44.455737 django_restit-4.2.9/medialib/templates/medialib/testpicker.html
+-rw-r--r--   0        0        0     6045 2023-06-27 05:37:44.455814 django_restit-4.2.9/medialib/tests.py
+-rw-r--r--   0        0        0      544 2023-06-27 05:37:44.455873 django_restit-4.2.9/medialib/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.455894 django_restit-4.2.9/medialib/urls.py
+-rw-r--r--   0        0        0     3756 2023-06-27 05:37:44.455970 django_restit-4.2.9/medialib/utils.py
+-rw-r--r--   0        0        0     4321 2023-06-27 05:37:44.456050 django_restit-4.2.9/medialib/views.py
+-rw-r--r--   0        0        0     4303 2023-06-27 05:37:44.456166 django_restit-4.2.9/medialib/youtube/__init__.py
+-rw-r--r--   0        0        0      601 2023-06-27 05:37:44.456272 django_restit-4.2.9/medialib/youtube/apiclient/__init__.py
+-rw-r--r--   0        0        0     9886 2023-06-27 05:37:44.456332 django_restit-4.2.9/medialib/youtube/apiclient/channel.py
+-rw-r--r--   0        0        0    35907 2023-06-27 05:37:44.456516 django_restit-4.2.9/medialib/youtube/apiclient/discovery.py
+-rw-r--r--   0        0        0     3550 2023-06-27 05:37:44.456592 django_restit-4.2.9/medialib/youtube/apiclient/errors.py
+-rw-r--r--   0        0        0    52945 2023-06-27 05:37:44.456694 django_restit-4.2.9/medialib/youtube/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.456785 django_restit-4.2.9/medialib/youtube/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11795 2023-06-27 05:37:44.456835 django_restit-4.2.9/medialib/youtube/apiclient/model.py
+-rw-r--r--   0        0        0     3596 2023-06-27 05:37:44.456895 django_restit-4.2.9/medialib/youtube/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9327 2023-06-27 05:37:44.456959 django_restit-4.2.9/medialib/youtube/apiclient/schema.py
+-rw-r--r--   0        0        0    69581 2023-06-27 05:37:44.457093 django_restit-4.2.9/medialib/youtube/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.457310 django_restit-4.2.9/medialib/youtube/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.457412 django_restit-4.2.9/medialib/youtube/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.457533 django_restit-4.2.9/medialib/youtube/httplib2/socks.py
+-rw-r--r--   0        0        0      213 2023-06-27 05:37:44.457629 django_restit-4.2.9/medialib/youtube/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.457687 django_restit-4.2.9/medialib/youtube/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.457830 django_restit-4.2.9/medialib/youtube/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44431 2023-06-27 05:37:44.457905 django_restit-4.2.9/medialib/youtube/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.457990 django_restit-4.2.9/medialib/youtube/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.458075 django_restit-4.2.9/medialib/youtube/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3753 2023-06-27 05:37:44.458140 django_restit-4.2.9/medialib/youtube/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.458204 django_restit-4.2.9/medialib/youtube/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.458255 django_restit-4.2.9/medialib/youtube/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.458323 django_restit-4.2.9/medialib/youtube/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.458399 django_restit-4.2.9/medialib/youtube/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.458454 django_restit-4.2.9/medialib/youtube/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.458510 django_restit-4.2.9/medialib/youtube/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.458604 django_restit-4.2.9/medialib/youtube/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.458680 django_restit-4.2.9/medialib/youtube/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.458745 django_restit-4.2.9/medialib/youtube/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0     2849 2023-06-27 05:37:44.458806 django_restit-4.2.9/medialib/youtube/upload.py
+-rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.458902 django_restit-4.2.9/medialib/youtube/uritemplate/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-27 05:37:44.459001 django_restit-4.2.9/metrics/README.md
+-rw-r--r--   0        0        0       90 2023-06-27 05:37:44.459061 django_restit-4.2.9/metrics/__init__.py
+-rw-r--r--   0        0        0    24337 2023-11-12 22:00:50.439910 django_restit-4.2.9/metrics/client.py
+-rw-r--r--   0        0        0     9182 2023-06-27 05:37:44.459333 django_restit-4.2.9/metrics/eod.py
+-rw-r--r--   0        0        0     1664 2023-06-27 05:37:44.459430 django_restit-4.2.9/metrics/examples/eod_example.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459493 django_restit-4.2.9/metrics/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459564 django_restit-4.2.9/metrics/management/commands/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-27 05:37:44.459636 django_restit-4.2.9/metrics/management/commands/delete_gauge.py
+-rw-r--r--   0        0        0      464 2023-06-27 05:37:44.459697 django_restit-4.2.9/metrics/management/commands/delete_metric.py
+-rw-r--r--   0        0        0     2801 2023-06-27 05:37:44.459766 django_restit-4.2.9/metrics/management/commands/fix_redis_metrics_keys.py
+-rw-r--r--   0        0        0     1928 2023-06-27 05:37:44.459829 django_restit-4.2.9/metrics/management/commands/generate_test_metrics.py
+-rw-r--r--   0        0        0     1742 2023-06-27 05:37:44.459896 django_restit-4.2.9/metrics/management/commands/redis_metrics_send_mail.py
+-rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.459957 django_restit-4.2.9/metrics/management/commands/reset_weekly_metrics.py
+-rw-r--r--   0        0        0     4343 2023-06-27 05:37:44.460023 django_restit-4.2.9/metrics/management/commands/system_metric.py
+-rw-r--r--   0        0        0     2399 2023-06-27 05:37:44.460109 django_restit-4.2.9/metrics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1510 2023-06-27 05:37:44.460172 django_restit-4.2.9/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
+-rw-r--r--   0        0        0      453 2023-06-27 05:37:44.460231 django_restit-4.2.9/metrics/migrations/0003_metrics_expires.py
+-rw-r--r--   0        0        0     3271 2023-06-27 05:37:44.460284 django_restit-4.2.9/metrics/migrations/0004_eodmetrics.py
+-rw-r--r--   0        0        0     2358 2023-06-27 05:37:44.460347 django_restit-4.2.9/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460367 django_restit-4.2.9/metrics/migrations/__init__.py
+-rw-r--r--   0        0        0    13444 2023-11-14 19:47:33.877245 django_restit-4.2.9/metrics/models.py
+-rw-r--r--   0        0        0      651 2023-08-07 16:07:55.926386 django_restit-4.2.9/metrics/periodic.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460587 django_restit-4.2.9/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     7432 2023-08-01 17:23:09.504050 django_restit-4.2.9/metrics/providers/aws.py
+-rw-r--r--   0        0        0    17674 2023-12-17 00:39:40.117566 django_restit-4.2.9/metrics/rpc.py
+-rw-r--r--   0        0        0      132 2023-06-27 05:37:44.460832 django_restit-4.2.9/metrics/settings.py
+-rw-r--r--   0        0        0      799 2023-08-22 14:57:47.689025 django_restit-4.2.9/metrics/tq.py
+-rw-r--r--   0        0        0    11995 2023-11-12 21:49:36.875626 django_restit-4.2.9/metrics/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461016 django_restit-4.2.9/pushit/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-27 05:37:44.461079 django_restit-4.2.9/pushit/admin.py
+-rw-r--r--   0        0        0     4555 2023-06-27 05:37:44.461167 django_restit-4.2.9/pushit/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461190 django_restit-4.2.9/pushit/migrations/__init__.py
+-rw-r--r--   0        0        0     5066 2023-07-11 15:47:46.945937 django_restit-4.2.9/pushit/models.py
+-rw-r--r--   0        0        0       88 2023-06-27 05:37:44.461351 django_restit-4.2.9/pushit/rpc/__init__.py
+-rw-r--r--   0        0        0     1756 2023-07-24 17:39:38.308118 django_restit-4.2.9/pushit/rpc/githooks.py
+-rw-r--r--   0        0        0     5028 2023-12-09 19:07:40.680776 django_restit-4.2.9/pushit/rpc/legacy.py
+-rw-r--r--   0        0        0      378 2023-06-27 05:37:44.461520 django_restit-4.2.9/pushit/rpc/products.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461605 django_restit-4.2.9/pushit/static/js/models_pushit.js
+-rw-r--r--   0        0        0      424 2023-08-01 06:36:56.109166 django_restit-4.2.9/pushit/tq.py
+-rw-r--r--   0        0        0     2121 2023-07-24 17:36:54.438531 django_restit-4.2.9/pushit/utils.py
+-rw-r--r--   0        0        0     1210 2023-12-21 05:47:30.691584 django_restit-4.2.9/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-06-27 05:37:44.461884 django_restit-4.2.9/rest/.gitignore
+-rw-r--r--   0        0        0     5460 2023-06-27 05:37:44.461959 django_restit-4.2.9/rest/README.md
+-rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462010 django_restit-4.2.9/rest/RemoteEvents.py
+-rw-r--r--   0        0        0      120 2023-12-21 05:47:30.734086 django_restit-4.2.9/rest/__init__.py
+-rw-r--r--   0        0        0     1967 2023-06-27 05:37:44.462114 django_restit-4.2.9/rest/arc4.py
+-rw-r--r--   0        0        0       83 2023-06-27 05:37:44.462161 django_restit-4.2.9/rest/cache.py
+-rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462295 django_restit-4.2.9/rest/crypto/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-27 05:37:44.462374 django_restit-4.2.9/rest/crypto/aes.py
+-rw-r--r--   0        0        0     4082 2023-06-27 05:37:44.462442 django_restit-4.2.9/rest/crypto/privpub.py
+-rw-r--r--   0        0        0     4514 2023-07-11 15:29:38.508089 django_restit-4.2.9/rest/crypto/util.py
+-rw-r--r--   0        0        0     9330 2023-11-25 04:40:03.230095 django_restit-4.2.9/rest/datem.py
+-rw-r--r--   0        0        0    15082 2023-12-09 17:07:25.089133 django_restit-4.2.9/rest/decorators.py
+-rw-r--r--   0        0        0      788 2023-06-27 05:37:44.462816 django_restit-4.2.9/rest/encryption.py
+-rw-r--r--   0        0        0      612 2023-12-19 00:02:03.767620 django_restit-4.2.9/rest/errors.py
+-rw-r--r--   0        0        0       54 2023-06-27 05:37:44.462913 django_restit-4.2.9/rest/extra/__init__.py
+-rw-r--r--   0        0        0     1078 2023-06-27 05:37:44.462982 django_restit-4.2.9/rest/extra/json_metadata.py
+-rw-r--r--   0        0        0     9719 2023-06-27 05:37:44.463072 django_restit-4.2.9/rest/fields.py
+-rw-r--r--   0        0        0     6316 2023-06-27 05:37:44.463145 django_restit-4.2.9/rest/forms.py
+-rw-r--r--   0        0        0    26563 2023-12-17 18:42:16.439687 django_restit-4.2.9/rest/helpers.py
+-rw-r--r--   0        0        0      260 2023-06-27 05:37:44.463338 django_restit-4.2.9/rest/joke.py
+-rw-r--r--   0        0        0     2298 2023-06-27 05:37:44.463411 django_restit-4.2.9/rest/jwtoken.py
+-rw-r--r--   0        0        0    20930 2023-06-27 15:33:50.289063 django_restit-4.2.9/rest/log.py
+-rw-r--r--   0        0        0     7737 2023-09-13 21:40:41.824715 django_restit-4.2.9/rest/mail.py
+-rw-r--r--   0        0        0     9174 2023-06-27 05:37:44.463711 django_restit-4.2.9/rest/mailman.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463776 django_restit-4.2.9/rest/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463861 django_restit-4.2.9/rest/management/commands/__init__.py
+-rw-r--r--   0        0        0      389 2023-06-27 05:37:44.463942 django_restit-4.2.9/rest/management/commands/rpc.py
+-rw-r--r--   0        0        0       33 2023-06-27 05:37:44.464028 django_restit-4.2.9/rest/middleware/__init__.py
+-rw-r--r--   0        0        0     3513 2023-06-27 05:37:44.464096 django_restit-4.2.9/rest/middleware/cors.py
+-rw-r--r--   0        0        0     2345 2023-06-27 05:37:44.464159 django_restit-4.2.9/rest/middleware/db_router.py
+-rw-r--r--   0        0        0     6017 2023-11-29 03:51:44.491936 django_restit-4.2.9/rest/middleware/jwt.py
+-rw-r--r--   0        0        0     4189 2023-11-15 19:37:49.027885 django_restit-4.2.9/rest/middleware/request.py
+-rw-r--r--   0        0        0    10240 2023-07-17 21:30:14.707861 django_restit-4.2.9/rest/middleware/session.py
+-rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.464450 django_restit-4.2.9/rest/middleware/session_store.py
+-rw-r--r--   0        0        0      130 2023-07-11 15:56:36.722347 django_restit-4.2.9/rest/models/__init__.py
+-rw-r--r--   0        0        0    66081 2023-12-09 19:57:57.872073 django_restit-4.2.9/rest/models/base.py
+-rw-r--r--   0        0        0      578 2023-07-11 16:03:40.953305 django_restit-4.2.9/rest/models/cacher.py
+-rw-r--r--   0        0        0    12631 2023-12-09 17:10:16.004033 django_restit-4.2.9/rest/models/metadata.py
+-rw-r--r--   0        0        0     1691 2023-08-07 04:48:28.143401 django_restit-4.2.9/rest/net.py
+-rw-r--r--   0        0        0   149463 2023-06-27 05:37:44.465139 django_restit-4.2.9/rest/regexes.yaml
+-rw-r--r--   0        0        0    15701 2023-12-20 17:18:00.376275 django_restit-4.2.9/rest/requestex.py
+-rw-r--r--   0        0        0     3612 2023-08-07 04:26:49.350849 django_restit-4.2.9/rest/rpc.py
+-rw-r--r--   0        0        0     8362 2023-11-14 19:35:31.737708 django_restit-4.2.9/rest/search.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.465410 django_restit-4.2.9/rest/serializers/__init__.py
+-rw-r--r--   0        0        0     4648 2023-11-15 20:41:11.119667 django_restit-4.2.9/rest/serializers/collection.py
+-rw-r--r--   0        0        0     3251 2023-12-10 01:39:17.966410 django_restit-4.2.9/rest/serializers/csv.py
+-rw-r--r--   0        0        0     1077 2023-06-27 05:37:44.465616 django_restit-4.2.9/rest/serializers/excel.py
+-rw-r--r--   0        0        0     1736 2023-06-27 05:37:44.465675 django_restit-4.2.9/rest/serializers/json.py
+-rw-r--r--   0        0        0    61981 2023-12-19 00:04:01.349514 django_restit-4.2.9/rest/serializers/legacy.py
+-rw-r--r--   0        0        0     8598 2023-11-10 17:09:26.910604 django_restit-4.2.9/rest/serializers/model.py
+-rw-r--r--   0        0        0      997 2023-07-06 18:50:18.372944 django_restit-4.2.9/rest/serializers/profiler.py
+-rw-r--r--   0        0        0     7051 2023-12-19 00:03:41.185610 django_restit-4.2.9/rest/serializers/response.py
+-rw-r--r--   0        0        0     2734 2023-06-27 05:37:44.466139 django_restit-4.2.9/rest/serializers/util.py
+-rw-r--r--   0        0        0     1532 2023-06-27 05:37:44.466216 django_restit-4.2.9/rest/settings_helper.py
+-rw-r--r--   0        0        0     1419 2023-08-07 05:26:37.128368 django_restit-4.2.9/rest/ssl_check.py
+-rw-r--r--   0        0        0    95786 2023-06-27 05:37:44.466685 django_restit-4.2.9/rest/static/lib/jquery.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466742 django_restit-4.2.9/rest/static/rest/app.css
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466776 django_restit-4.2.9/rest/static/rest/app.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466808 django_restit-4.2.9/rest/static/rest/rest.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466846 django_restit-4.2.9/rest/static/rest/rest.scss
+-rw-r--r--   0        0        0      529 2023-06-27 05:37:44.466992 django_restit-4.2.9/rest/templates/email/error.html
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.467020 django_restit-4.2.9/rest/templates/email/error.subject
+-rw-r--r--   0        0        0     7148 2023-06-27 05:37:44.467101 django_restit-4.2.9/rest/templates/rest_docs.html
+-rw-r--r--   0        0        0    10986 2023-12-17 18:47:10.126214 django_restit-4.2.9/rest/templates/rest_html.html
+-rw-r--r--   0        0        0   185398 2023-07-28 01:56:34.391352 django_restit-4.2.9/rest/ua.py
+-rw-r--r--   0        0        0    17064 2023-06-27 05:37:44.467734 django_restit-4.2.9/rest/uberdict.py
+-rw-r--r--   0        0        0    11881 2023-06-27 05:37:44.467820 django_restit-4.2.9/rest/url_docs.py
+-rw-r--r--   0        0        0     1869 2023-12-17 00:13:41.075590 django_restit-4.2.9/rest/urls.py
+-rw-r--r--   0        0        0     1115 2023-12-17 00:40:15.697924 django_restit-4.2.9/rest/views.py
+-rw-r--r--   0        0        0      118 2023-06-27 05:37:44.468007 django_restit-4.2.9/sessionlog/.gitignore
+-rw-r--r--   0        0        0       62 2023-06-27 05:37:44.468062 django_restit-4.2.9/sessionlog/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468086 django_restit-4.2.9/sessionlog/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-27 05:37:44.468153 django_restit-4.2.9/sessionlog/admin.py
+-rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.468231 django_restit-4.2.9/sessionlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468261 django_restit-4.2.9/sessionlog/migrations/__init__.py
+-rw-r--r--   0        0        0     3662 2023-07-17 21:32:12.789126 django_restit-4.2.9/sessionlog/models.py
+-rw-r--r--   0        0        0      383 2023-06-27 05:37:44.468400 django_restit-4.2.9/sessionlog/tests.py
+-rw-r--r--   0        0        0       26 2023-06-27 05:37:44.468451 django_restit-4.2.9/sessionlog/views.py
+-rw-r--r--   0        0        0     2196 2023-06-27 05:37:44.468543 django_restit-4.2.9/taskqueue/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468569 django_restit-4.2.9/taskqueue/__init__.py
+-rw-r--r--   0        0        0      208 2023-06-27 05:37:44.468635 django_restit-4.2.9/taskqueue/admin.py
+-rw-r--r--   0        0        0     4738 2023-06-27 05:37:44.468730 django_restit-4.2.9/taskqueue/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468758 django_restit-4.2.9/taskqueue/migrations/__init__.py
+-rw-r--r--   0        0        0    19306 2023-12-18 15:27:25.429795 django_restit-4.2.9/taskqueue/models.py
+-rw-r--r--   0        0        0     3543 2023-08-11 17:40:15.804907 django_restit-4.2.9/taskqueue/periodic.py
+-rw-r--r--   0        0        0     5736 2023-12-09 17:45:37.022351 django_restit-4.2.9/taskqueue/rpc.py
+-rw-r--r--   0        0        0      942 2023-06-27 05:37:44.469073 django_restit-4.2.9/taskqueue/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469126 django_restit-4.2.9/taskqueue/transports/__init__.py
+-rw-r--r--   0        0        0      623 2023-06-27 05:37:44.469185 django_restit-4.2.9/taskqueue/transports/email.py
+-rw-r--r--   0        0        0     2409 2023-08-31 21:55:56.632266 django_restit-4.2.9/taskqueue/transports/http.py
+-rw-r--r--   0        0        0     1913 2023-10-30 22:13:38.540735 django_restit-4.2.9/taskqueue/transports/s3.py
+-rw-r--r--   0        0        0     1891 2023-06-27 05:37:44.469341 django_restit-4.2.9/taskqueue/transports/sftp.py
+-rw-r--r--   0        0        0      142 2023-06-27 05:37:44.469388 django_restit-4.2.9/taskqueue/transports/sms.py
+-rw-r--r--   0        0        0    16050 2023-12-16 21:45:01.773610 django_restit-4.2.9/taskqueue/worker.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469517 django_restit-4.2.9/telephony/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-27 05:37:44.469571 django_restit-4.2.9/telephony/admin.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469591 django_restit-4.2.9/telephony/decorators.py
+-rw-r--r--   0        0        0     3030 2023-06-27 05:37:44.469692 django_restit-4.2.9/telephony/migrations/0001_initial.py
+-rw-r--r--   0        0        0      424 2023-11-27 22:03:30.384417 django_restit-4.2.9/telephony/migrations/0002_alter_sms_sid.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469714 django_restit-4.2.9/telephony/migrations/__init__.py
+-rw-r--r--   0        0        0     8248 2023-12-09 17:49:10.656587 django_restit-4.2.9/telephony/models.py
+-rw-r--r--   0        0        0     2426 2023-11-28 15:55:05.388090 django_restit-4.2.9/telephony/phone_util.py
+-rw-r--r--   0        0        0     3473 2023-12-09 17:49:26.483244 django_restit-4.2.9/telephony/rpc.py
+-rw-r--r--   0        0        0        1 2023-08-03 14:28:08.854157 django_restit-4.2.9/wiki/__init__.py
+-rw-r--r--   0        0        0     3606 2023-08-04 04:52:16.019699 django_restit-4.2.9/wiki/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-08-04 04:52:16.018799 django_restit-4.2.9/wiki/migrations/__init__.py
+-rw-r--r--   0        0        0      132 2023-08-04 03:46:50.913857 django_restit-4.2.9/wiki/models/__init__.py
+-rw-r--r--   0        0        0     1745 2023-08-03 15:41:23.854674 django_restit-4.2.9/wiki/models/faq.py
+-rw-r--r--   0        0        0     7203 2023-08-16 18:23:17.138555 django_restit-4.2.9/wiki/models/page.py
+-rw-r--r--   0        0        0      729 2023-08-04 03:47:46.129186 django_restit-4.2.9/wiki/models/revision.py
+-rw-r--r--   0        0        0      334 2023-08-03 14:28:08.854499 django_restit-4.2.9/wiki/periodic.py
+-rw-r--r--   0        0        0      461 2023-08-03 15:34:25.031919 django_restit-4.2.9/wiki/renderers/__init__.py
+-rwxr-xr-x   0        0        0       84 2022-09-24 04:49:32.000000 django_restit-4.2.9/wiki/renderers/mistune/__init__.py
+-rwxr-xr-x   0        0        0     1264 2023-08-04 05:12:57.404938 django_restit-4.2.9/wiki/renderers/mistune/highlight.py
+-rwxr-xr-x   0        0        0     1901 2022-09-24 04:49:32.000000 django_restit-4.2.9/wiki/renderers/mistune/math.py
+-rw-r--r--   0        0        0     2610 2023-08-14 06:50:10.268306 django_restit-4.2.9/wiki/renderers/mistune/media.py
+-rwxr-xr-x   0        0        0      805 2022-09-24 04:49:32.000000 django_restit-4.2.9/wiki/renderers/mistune/meta.py
+-rw-r--r--   0        0        0     1889 2023-08-16 00:38:11.894074 django_restit-4.2.9/wiki/renderers/mistune/task_list.py
+-rwxr-xr-x   0        0        0     2302 2023-08-04 05:12:30.563520 django_restit-4.2.9/wiki/renderers/mistune/toc.py
+-rw-r--r--   0        0        0       40 2023-08-04 00:19:22.669056 django_restit-4.2.9/wiki/rpc/__init__.py
+-rw-r--r--   0        0        0     1333 2023-08-16 18:28:15.622351 django_restit-4.2.9/wiki/rpc/wiki.py
+-rw-r--r--   0        0        0      313 2023-08-03 14:28:08.854423 django_restit-4.2.9/wiki/tq.py
+-rw-r--r--   0        0        0     3624 2023-06-27 05:37:44.470008 django_restit-4.2.9/ws4redis/README.md
+-rwxr-xr-x   0        0        0       46 2023-06-27 05:37:44.470065 django_restit-4.2.9/ws4redis/__init__.py
+-rw-r--r--   0        0        0     5049 2023-11-12 04:56:27.258942 django_restit-4.2.9/ws4redis/client.py
+-rw-r--r--   0        0        0    13431 2023-08-14 17:22:44.326899 django_restit-4.2.9/ws4redis/connection.py
+-rwxr-xr-x   0        0        0      636 2023-06-27 05:37:44.470295 django_restit-4.2.9/ws4redis/exceptions.py
+-rw-r--r--   0        0        0     5561 2023-07-08 23:30:25.146274 django_restit-4.2.9/ws4redis/redis.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.470422 django_restit-4.2.9/ws4redis/servers/__init__.py
+-rw-r--r--   0        0        0     3747 2023-06-27 05:37:44.470507 django_restit-4.2.9/ws4redis/servers/base.py
+-rw-r--r--   0        0        0     4329 2023-06-27 05:37:44.470582 django_restit-4.2.9/ws4redis/servers/django.py
+-rw-r--r--   0        0        0     1723 2023-06-27 05:37:44.470638 django_restit-4.2.9/ws4redis/servers/uwsgi.py
+-rwxr-xr-x   0        0        0     1536 2023-08-14 17:15:40.285934 django_restit-4.2.9/ws4redis/settings.py
+-rwxr-xr-x   0        0        0     5122 2023-06-27 05:37:44.470772 django_restit-4.2.9/ws4redis/utf8validator.py
+-rwxr-xr-x   0        0        0    14848 2023-06-27 05:37:44.470868 django_restit-4.2.9/ws4redis/websocket.py
+-rw-r--r--   0        0        0     7572 1970-01-01 00:00:00.000000 django_restit-4.2.9/PKG-INFO
```

### Comparing `django_restit-4.2.8/LICENSE.md` & `django_restit-4.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/README.md` & `django_restit-4.2.9/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/admin.py` & `django_restit-4.2.9/account/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/fcm/__init__.py` & `django_restit-4.2.9/account/fcm/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/migrations/0001_initial.py` & `django_restit-4.2.9/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/migrations/0003_member_phone_number.py` & `django_restit-4.2.9/account/migrations/0003_member_phone_number.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/migrations/0004_group_modified_alter_group_created.py` & `django_restit-4.2.9/account/migrations/0004_group_modified_alter_group_created.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/migrations/0007_authtoken_signature_authsession.py` & `django_restit-4.2.9/account/migrations/0007_authtoken_signature_authsession.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/migrations/0008_memberdevice_memberdevicemetadata.py` & `django_restit-4.2.9/account/migrations/0008_memberdevice_memberdevicemetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/migrations/0011_authtoken.py` & `django_restit-4.2.9/account/migrations/0011_authtoken.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/migrations/0012_settings_settingsmetadata.py` & `django_restit-4.2.9/account/migrations/0012_settings_settingsmetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/migrations/0014_alter_notificationmemberrecord_member.py` & `django_restit-4.2.9/account/migrations/0014_alter_notificationmemberrecord_member.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/models/device.py` & `django_restit-4.2.9/account/models/device.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/models/feeds.py` & `django_restit-4.2.9/account/models/feeds.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/models/group.py` & `django_restit-4.2.9/account/models/group.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/models/legacy.py` & `django_restit-4.2.9/account/models/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/models/member.py` & `django_restit-4.2.9/account/models/member.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/models/membership.py` & `django_restit-4.2.9/account/models/membership.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/models/notify.py` & `django_restit-4.2.9/account/models/notify.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/models/session.py` & `django_restit-4.2.9/account/models/session.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/models/settings.py` & `django_restit-4.2.9/account/models/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/oauth/google.py` & `django_restit-4.2.9/account/oauth/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/periodic.py` & `django_restit-4.2.9/account/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/rpc/auth.py` & `django_restit-4.2.9/account/rpc/auth.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/rpc/device.py` & `django_restit-4.2.9/account/rpc/device.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/rpc/group.py` & `django_restit-4.2.9/account/rpc/group.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/rpc/member.py` & `django_restit-4.2.9/account/rpc/member.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/rpc/notify.py` & `django_restit-4.2.9/account/rpc/notify.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/rpc/oauth.py` & `django_restit-4.2.9/account/rpc/oauth.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/templates/email/base.html` & `django_restit-4.2.9/account/templates/email/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/templates/email/invite.html` & `django_restit-4.2.9/account/templates/email/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/templates/email/plain/base.html` & `django_restit-4.2.9/account/templates/email/plain/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/templates/email/plain/invite.html` & `django_restit-4.2.9/account/templates/email/plain/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/templates/email/plain/reset_code.html` & `django_restit-4.2.9/account/templates/email/plain/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/templates/email/reset_code.html` & `django_restit-4.2.9/account/templates/email/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/templates/email/simple/invite.html` & `django_restit-4.2.9/account/templates/email/simple/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/account/templates/email/simple/reset_code.html` & `django_restit-4.2.9/account/templates/email/simple/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/auditlog/README` & `django_restit-4.2.9/auditlog/README`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/auditlog/admin.py` & `django_restit-4.2.9/auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/auditlog/decorators.py` & `django_restit-4.2.9/auditlog/decorators.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/auditlog/middleware.py` & `django_restit-4.2.9/auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/auditlog/migrations/0001_initial.py` & `django_restit-4.2.9/auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/auditlog/models.py` & `django_restit-4.2.9/auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/auditlog/rpc.py` & `django_restit-4.2.9/auditlog/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/auditlog/tq.py` & `django_restit-4.2.9/auditlog/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/README.md` & `django_restit-4.2.9/inbox/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/handlers.py` & `django_restit-4.2.9/inbox/handlers.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/migrations/0001_initial.py` & `django_restit-4.2.9/inbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/migrations/0004_mailtemplate.py` & `django_restit-4.2.9/inbox/migrations/0004_mailtemplate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/models/bounce.py` & `django_restit-4.2.9/inbox/models/bounce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/models/complaint.py` & `django_restit-4.2.9/inbox/models/complaint.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/models/message.py` & `django_restit-4.2.9/inbox/models/message.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/models/template.py` & `django_restit-4.2.9/inbox/models/template.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/rpc.py` & `django_restit-4.2.9/inbox/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/utils/parsing.py` & `django_restit-4.2.9/inbox/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/utils/render.py` & `django_restit-4.2.9/inbox/utils/render.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/inbox/utils/sending.py` & `django_restit-4.2.9/inbox/utils/sending.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/README.md` & `django_restit-4.2.9/incident/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/__init__.py` & `django_restit-4.2.9/incident/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/migrations/0001_initial.py` & `django_restit-4.2.9/incident/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/migrations/0002_event_component_event_component_id.py` & `django_restit-4.2.9/incident/migrations/0002_event_component_event_component_id.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py` & `django_restit-4.2.9/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/migrations/0005_incident_component_alter_incident_state.py` & `django_restit-4.2.9/incident/migrations/0005_incident_component_alter_incident_state.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py` & `django_restit-4.2.9/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/migrations/0010_incident_category_incident_component_id.py` & `django_restit-4.2.9/incident/migrations/0010_incident_category_incident_component_id.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/migrations/0011_ticket.py` & `django_restit-4.2.9/incident/migrations/0011_ticket.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/models/event.py` & `django_restit-4.2.9/incident/models/event.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/models/incident.py` & `django_restit-4.2.9/incident/models/incident.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/models/ossec.py` & `django_restit-4.2.9/incident/models/ossec.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/models/rules.py` & `django_restit-4.2.9/incident/models/rules.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/models/ticket.py` & `django_restit-4.2.9/incident/models/ticket.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/parsers/ossec.py` & `django_restit-4.2.9/incident/parsers/ossec.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/rpc.py` & `django_restit-4.2.9/incident/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/templates/email/incident_change.html` & `django_restit-4.2.9/incident/templates/email/incident_change.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/templates/email/incident_new.html` & `django_restit-4.2.9/incident/templates/email/incident_new.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/templates/email/incident_plain.html` & `django_restit-4.2.9/incident/templates/email/incident_plain.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/incident/tq.py` & `django_restit-4.2.9/incident/tq.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from account import models as account
 from location.models import GeoIP
 from rest import helpers
 from rest import settings
 from inbox import models as inbox
 import time
 from datetime import datetime, timedelta
+from django.db.models import Q
 
 
 POSIX_BODY_BREAK = "\n\n\n"
 WIN_BODY_BREAK = "\r\n\r\n\r\n"
 
 
 def new_event(task):
@@ -117,15 +118,16 @@
 def run_cleanup(task):
     stale = datetime.now() - timedelta(days=90)
     # delete all ossec alerts older then 90 days
     count = ia.ServerOssecAlert.objects.filter(created__lte=stale).delete()
     if count:
         task.log(f"deleted {count} old ServerOssecAlert")
     # delete all events older then 90 days
-    count = ia.Event.objects.filter(created__lte=stale).delete()
+    count = ia.Event.objects.filter(created__lte=stale).filter(
+        Q(incident__state=ia.INCIDENT_STATE_IGNORE)|Q(incident__isnull=True)).delete()
     if count:
         task.log(f"deleted {count} old Events")
 
     count = GeoIP.removeDuplicates()
     if count:
         task.log(f"deleted {count} duplicate IPs")
```

### Comparing `django_restit-4.2.8/location/geolocate.py` & `django_restit-4.2.9/location/geolocate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/migrations/0001_initial.py` & `django_restit-4.2.9/location/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/migrations/0002_geoip_subnet_alter_geoip_ip.py` & `django_restit-4.2.9/location/migrations/0002_geoip_subnet_alter_geoip_ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/models/address.py` & `django_restit-4.2.9/location/models/address.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/models/ip.py` & `django_restit-4.2.9/location/models/ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/models/legacy.py` & `django_restit-4.2.9/location/models/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/models/location.py` & `django_restit-4.2.9/location/models/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/models/track.py` & `django_restit-4.2.9/location/models/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/providers/iplookup/__init__.py` & `django_restit-4.2.9/location/providers/iplookup/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/providers/iplookup/abstractapi.py` & `django_restit-4.2.9/location/providers/iplookup/abstractapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/providers/iplookup/extremeip.py` & `django_restit-4.2.9/location/providers/iplookup/extremeip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/providers/iplookup/geoplugin.py` & `django_restit-4.2.9/location/providers/iplookup/geoplugin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/providers/iplookup/ipapi.py` & `django_restit-4.2.9/location/providers/iplookup/ipapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/providers/iplookup/ipinfo.py` & `django_restit-4.2.9/location/providers/iplookup/ipinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/providers/iplookup/restit.py` & `django_restit-4.2.9/location/providers/iplookup/restit.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/providers/location/google.py` & `django_restit-4.2.9/location/providers/location/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/providers/timezones/google.py` & `django_restit-4.2.9/location/providers/timezones/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/providers/zillow.py` & `django_restit-4.2.9/location/providers/zillow.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/rpc/ip.py` & `django_restit-4.2.9/location/rpc/ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/rpc/location.py` & `django_restit-4.2.9/location/rpc/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/location/rpc/track.py` & `django_restit-4.2.9/location/rpc/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/admin.py` & `django_restit-4.2.9/medialib/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/cvutil/contours.py` & `django_restit-4.2.9/medialib/cvutil/contours.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/cvutil/images.py` & `django_restit-4.2.9/medialib/cvutil/images.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/cvutil/misc.py` & `django_restit-4.2.9/medialib/cvutil/misc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/cvutil/text.py` & `django_restit-4.2.9/medialib/cvutil/text.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/fixtures/initial_data.json` & `django_restit-4.2.9/medialib/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/fixtures/medialib.json` & `django_restit-4.2.9/medialib/fixtures/medialib.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/fixtures/medialib_test_fixture.json` & `django_restit-4.2.9/medialib/fixtures/medialib_test_fixture.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/forms.py` & `django_restit-4.2.9/medialib/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/migrations/0001_initial.py` & `django_restit-4.2.9/medialib/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/models.py` & `django_restit-4.2.9/medialib/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/ocr.py` & `django_restit-4.2.9/medialib/ocr.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/pdf.py` & `django_restit-4.2.9/medialib/pdf.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/qrcode.py` & `django_restit-4.2.9/medialib/qrcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/__init__.py` & `django_restit-4.2.9/medialib/render/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/engines/anigif.py` & `django_restit-4.2.9/medialib/render/engines/anigif.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/engines/ffmpeg.py` & `django_restit-4.2.9/medialib/render/engines/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/engines/gifsicle.py` & `django_restit-4.2.9/medialib/render/engines/gifsicle.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/engines/hls.py` & `django_restit-4.2.9/medialib/render/engines/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/engines/mp4box.py` & `django_restit-4.2.9/medialib/render/engines/mp4box.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/engines/rtmp/rtmp.i` & `django_restit-4.2.9/medialib/render/engines/rtmp/rtmp.i`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/engines/rtmpdump.py` & `django_restit-4.2.9/medialib/render/engines/rtmpdump.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/engines/rtmpsink.py` & `django_restit-4.2.9/medialib/render/engines/rtmpsink.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/engines/video_getinfo.py` & `django_restit-4.2.9/medialib/render/engines/video_getinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/engines/websnap.py` & `django_restit-4.2.9/medialib/render/engines/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/exceptions.py` & `django_restit-4.2.9/medialib/render/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/akamai.py` & `django_restit-4.2.9/medialib/render/presets/akamai.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/animated_thumbnail.py` & `django_restit-4.2.9/medialib/render/presets/animated_thumbnail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/ffmpeg.py` & `django_restit-4.2.9/medialib/render/presets/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/flv.py` & `django_restit-4.2.9/medialib/render/presets/flv.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/hls.py` & `django_restit-4.2.9/medialib/render/presets/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/image_transcode.py` & `django_restit-4.2.9/medialib/render/presets/image_transcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/image_validate.py` & `django_restit-4.2.9/medialib/render/presets/image_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/mp4.py` & `django_restit-4.2.9/medialib/render/presets/mp4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/video_still.py` & `django_restit-4.2.9/medialib/render/presets/video_still.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/video_validate.py` & `django_restit-4.2.9/medialib/render/presets/video_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/websnap.py` & `django_restit-4.2.9/medialib/render/presets/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/presets/youtube.py` & `django_restit-4.2.9/medialib/render/presets/youtube.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/render/render_utils.py` & `django_restit-4.2.9/medialib/render/render_utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/rpc/legacy.py` & `django_restit-4.2.9/medialib/rpc/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/rpc/media.py` & `django_restit-4.2.9/medialib/rpc/media.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/rpc/tools.py` & `django_restit-4.2.9/medialib/rpc/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/scripts/init_config` & `django_restit-4.2.9/medialib/scripts/init_config`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/css/base_medialibui.css` & `django_restit-4.2.9/medialib/static/css/base_medialibui.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/css/base_widgets.css` & `django_restit-4.2.9/medialib/static/css/base_widgets.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/css/jquery.jcrop.css` & `django_restit-4.2.9/medialib/static/css/jquery.jcrop.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/img/bg-body.gif` & `django_restit-4.2.9/medialib/static/img/bg-body.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/img/loading.gif` & `django_restit-4.2.9/medialib/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/img/noimage.gif` & `django_restit-4.2.9/medialib/static/img/noimage.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/img/render_err.gif` & `django_restit-4.2.9/medialib/static/img/render_err.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/img/rendering.gif` & `django_restit-4.2.9/medialib/static/img/rendering.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/img/unknown.gif` & `django_restit-4.2.9/medialib/static/img/unknown.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/lib/caman.full.js` & `django_restit-4.2.9/medialib/static/lib/caman.full.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/lib/hammer.min.js` & `django_restit-4.2.9/medialib/static/lib/hammer.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/lib/jquery.Jcrop.js` & `django_restit-4.2.9/medialib/static/lib/jquery.Jcrop.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/lib/jquery.hammer.js` & `django_restit-4.2.9/medialib/static/lib/jquery.hammer.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/lib/load-image.min.js` & `django_restit-4.2.9/medialib/static/lib/load-image.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/lib/swiper.js` & `django_restit-4.2.9/medialib/static/lib/swiper.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js` & `django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js` & `django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js` & `django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/static/lib/tinymce/plugins/medialib/medialib.html` & `django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/medialib.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/__init__.py` & `django_restit-4.2.9/medialib/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/apiclient/__init__.py` & `django_restit-4.2.9/medialib/stores/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/apiclient/channel.py` & `django_restit-4.2.9/medialib/stores/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/apiclient/discovery.py` & `django_restit-4.2.9/medialib/stores/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/apiclient/errors.py` & `django_restit-4.2.9/medialib/stores/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/apiclient/http.py` & `django_restit-4.2.9/medialib/stores/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/apiclient/mimeparse.py` & `django_restit-4.2.9/medialib/stores/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/apiclient/model.py` & `django_restit-4.2.9/medialib/stores/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/apiclient/sample_tools.py` & `django_restit-4.2.9/medialib/stores/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/apiclient/schema.py` & `django_restit-4.2.9/medialib/stores/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/filestore.py` & `django_restit-4.2.9/medialib/stores/filestore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/httplib2/__init__.py` & `django_restit-4.2.9/medialib/stores/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/httplib2/cacerts.txt` & `django_restit-4.2.9/medialib/stores/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/httplib2/iri2uri.py` & `django_restit-4.2.9/medialib/stores/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/httplib2/socks.py` & `django_restit-4.2.9/medialib/stores/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/httpstore.py` & `django_restit-4.2.9/medialib/stores/httpstore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/anyjson.py` & `django_restit-4.2.9/medialib/stores/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/appengine.py` & `django_restit-4.2.9/medialib/stores/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/client.py` & `django_restit-4.2.9/medialib/stores/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/clientsecrets.py` & `django_restit-4.2.9/medialib/stores/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/crypt.py` & `django_restit-4.2.9/medialib/stores/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/django_orm.py` & `django_restit-4.2.9/medialib/stores/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/file.py` & `django_restit-4.2.9/medialib/stores/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/gce.py` & `django_restit-4.2.9/medialib/stores/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/keyring_storage.py` & `django_restit-4.2.9/medialib/stores/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/locked_file.py` & `django_restit-4.2.9/medialib/stores/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/multistore_file.py` & `django_restit-4.2.9/medialib/stores/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/old_run.py` & `django_restit-4.2.9/medialib/stores/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/tools.py` & `django_restit-4.2.9/medialib/stores/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/util.py` & `django_restit-4.2.9/medialib/stores/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/oauth2client/xsrfutil.py` & `django_restit-4.2.9/medialib/stores/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/s3store.py` & `django_restit-4.2.9/medialib/stores/s3store.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/stores/uritemplate/__init__.py` & `django_restit-4.2.9/medialib/stores/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/templates/medialib/base.html` & `django_restit-4.2.9/medialib/templates/medialib/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/templates/medialib/instances.html` & `django_restit-4.2.9/medialib/templates/medialib/instances.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/templates/medialib/items.html` & `django_restit-4.2.9/medialib/templates/medialib/items.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/templates/medialib/library.html` & `django_restit-4.2.9/medialib/templates/medialib/library.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/templates/medialib/test.html` & `django_restit-4.2.9/medialib/templates/medialib/test.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/templates/medialib/testpicker.html` & `django_restit-4.2.9/medialib/templates/medialib/testpicker.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/tests.py` & `django_restit-4.2.9/medialib/tests.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/tq.py` & `django_restit-4.2.9/medialib/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/utils.py` & `django_restit-4.2.9/medialib/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/views.py` & `django_restit-4.2.9/medialib/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/__init__.py` & `django_restit-4.2.9/medialib/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/apiclient/__init__.py` & `django_restit-4.2.9/medialib/youtube/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/apiclient/channel.py` & `django_restit-4.2.9/medialib/youtube/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/apiclient/discovery.py` & `django_restit-4.2.9/medialib/youtube/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/apiclient/errors.py` & `django_restit-4.2.9/medialib/youtube/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/apiclient/http.py` & `django_restit-4.2.9/medialib/youtube/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/apiclient/mimeparse.py` & `django_restit-4.2.9/medialib/youtube/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/apiclient/model.py` & `django_restit-4.2.9/medialib/youtube/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/apiclient/sample_tools.py` & `django_restit-4.2.9/medialib/youtube/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/apiclient/schema.py` & `django_restit-4.2.9/medialib/youtube/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/httplib2/__init__.py` & `django_restit-4.2.9/medialib/youtube/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/httplib2/cacerts.txt` & `django_restit-4.2.9/medialib/youtube/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/httplib2/iri2uri.py` & `django_restit-4.2.9/medialib/youtube/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/httplib2/socks.py` & `django_restit-4.2.9/medialib/youtube/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/anyjson.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/appengine.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/client.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/clientsecrets.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/crypt.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/django_orm.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/file.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/gce.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/keyring_storage.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/locked_file.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/multistore_file.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/old_run.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/tools.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/util.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/oauth2client/xsrfutil.py` & `django_restit-4.2.9/medialib/youtube/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/upload.py` & `django_restit-4.2.9/medialib/youtube/upload.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/medialib/youtube/uritemplate/__init__.py` & `django_restit-4.2.9/medialib/youtube/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/README.md` & `django_restit-4.2.9/metrics/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/client.py` & `django_restit-4.2.9/metrics/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/eod.py` & `django_restit-4.2.9/metrics/eod.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/examples/eod_example.py` & `django_restit-4.2.9/metrics/examples/eod_example.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/management/commands/fix_redis_metrics_keys.py` & `django_restit-4.2.9/metrics/management/commands/fix_redis_metrics_keys.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/management/commands/generate_test_metrics.py` & `django_restit-4.2.9/metrics/management/commands/generate_test_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/management/commands/redis_metrics_send_mail.py` & `django_restit-4.2.9/metrics/management/commands/redis_metrics_send_mail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/management/commands/reset_weekly_metrics.py` & `django_restit-4.2.9/metrics/management/commands/reset_weekly_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/management/commands/system_metric.py` & `django_restit-4.2.9/metrics/management/commands/system_metric.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/migrations/0001_initial.py` & `django_restit-4.2.9/metrics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py` & `django_restit-4.2.9/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/migrations/0004_eodmetrics.py` & `django_restit-4.2.9/metrics/migrations/0004_eodmetrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py` & `django_restit-4.2.9/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/models.py` & `django_restit-4.2.9/metrics/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/periodic.py` & `django_restit-4.2.9/metrics/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/providers/aws.py` & `django_restit-4.2.9/metrics/providers/aws.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/rpc.py` & `django_restit-4.2.9/metrics/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/tq.py` & `django_restit-4.2.9/metrics/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/metrics/utils.py` & `django_restit-4.2.9/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/pushit/migrations/0001_initial.py` & `django_restit-4.2.9/pushit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/pushit/models.py` & `django_restit-4.2.9/pushit/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/pushit/rpc/githooks.py` & `django_restit-4.2.9/pushit/rpc/githooks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/pushit/rpc/legacy.py` & `django_restit-4.2.9/pushit/rpc/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/pushit/utils.py` & `django_restit-4.2.9/pushit/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/pyproject.toml` & `django_restit-4.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-restit"
-version = "4.2.8"
+version = "4.2.9"
 description = "A Rest Framework for DJANGO"
 authors = ["Ian Starnes <ians@311labs.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     {include = "account"},
```

### Comparing `django_restit-4.2.8/rest/README.md` & `django_restit-4.2.9/rest/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/arc4.py` & `django_restit-4.2.9/rest/arc4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/crypto/aes.py` & `django_restit-4.2.9/rest/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/crypto/privpub.py` & `django_restit-4.2.9/rest/crypto/privpub.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/crypto/util.py` & `django_restit-4.2.9/rest/crypto/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/datem.py` & `django_restit-4.2.9/rest/datem.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/decorators.py` & `django_restit-4.2.9/rest/decorators.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/encryption.py` & `django_restit-4.2.9/rest/encryption.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/errors.py` & `django_restit-4.2.9/rest/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/extra/json_metadata.py` & `django_restit-4.2.9/rest/extra/json_metadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/fields.py` & `django_restit-4.2.9/rest/fields.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/forms.py` & `django_restit-4.2.9/rest/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/helpers.py` & `django_restit-4.2.9/rest/helpers.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/jwtoken.py` & `django_restit-4.2.9/rest/jwtoken.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/log.py` & `django_restit-4.2.9/rest/log.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/mail.py` & `django_restit-4.2.9/rest/mail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/mailman.py` & `django_restit-4.2.9/rest/mailman.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/middleware/cors.py` & `django_restit-4.2.9/rest/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/middleware/db_router.py` & `django_restit-4.2.9/rest/middleware/db_router.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/middleware/jwt.py` & `django_restit-4.2.9/rest/middleware/jwt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/middleware/request.py` & `django_restit-4.2.9/rest/middleware/request.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/middleware/session.py` & `django_restit-4.2.9/rest/middleware/session.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/middleware/session_store.py` & `django_restit-4.2.9/rest/middleware/session_store.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/models/base.py` & `django_restit-4.2.9/rest/models/base.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/models/cacher.py` & `django_restit-4.2.9/rest/models/cacher.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/models/metadata.py` & `django_restit-4.2.9/rest/models/metadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/net.py` & `django_restit-4.2.9/rest/net.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/regexes.yaml` & `django_restit-4.2.9/rest/regexes.yaml`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/requestex.py` & `django_restit-4.2.9/rest/requestex.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/rpc.py` & `django_restit-4.2.9/rest/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/search.py` & `django_restit-4.2.9/rest/search.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/serializers/collection.py` & `django_restit-4.2.9/rest/serializers/collection.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/serializers/csv.py` & `django_restit-4.2.9/rest/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/serializers/excel.py` & `django_restit-4.2.9/rest/serializers/excel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/serializers/json.py` & `django_restit-4.2.9/rest/serializers/json.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/serializers/legacy.py` & `django_restit-4.2.9/rest/serializers/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/serializers/model.py` & `django_restit-4.2.9/rest/serializers/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/serializers/profiler.py` & `django_restit-4.2.9/rest/serializers/profiler.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/serializers/response.py` & `django_restit-4.2.9/rest/serializers/response.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/serializers/util.py` & `django_restit-4.2.9/rest/serializers/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/settings_helper.py` & `django_restit-4.2.9/rest/settings_helper.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/ssl_check.py` & `django_restit-4.2.9/rest/ssl_check.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/static/lib/jquery.js` & `django_restit-4.2.9/rest/static/lib/jquery.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/templates/email/error.html` & `django_restit-4.2.9/rest/templates/email/error.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/templates/rest_docs.html` & `django_restit-4.2.9/rest/templates/rest_docs.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/templates/rest_html.html` & `django_restit-4.2.9/rest/templates/rest_html.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/ua.py` & `django_restit-4.2.9/rest/ua.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/uberdict.py` & `django_restit-4.2.9/rest/uberdict.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/url_docs.py` & `django_restit-4.2.9/rest/url_docs.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/urls.py` & `django_restit-4.2.9/rest/urls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/rest/views.py` & `django_restit-4.2.9/rest/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/sessionlog/migrations/0001_initial.py` & `django_restit-4.2.9/sessionlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/sessionlog/models.py` & `django_restit-4.2.9/sessionlog/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/taskqueue/README.md` & `django_restit-4.2.9/taskqueue/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/taskqueue/migrations/0001_initial.py` & `django_restit-4.2.9/taskqueue/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/taskqueue/models.py` & `django_restit-4.2.9/taskqueue/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/taskqueue/periodic.py` & `django_restit-4.2.9/taskqueue/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/taskqueue/rpc.py` & `django_restit-4.2.9/taskqueue/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/taskqueue/tq.py` & `django_restit-4.2.9/taskqueue/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/taskqueue/transports/email.py` & `django_restit-4.2.9/taskqueue/transports/email.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/taskqueue/transports/http.py` & `django_restit-4.2.9/taskqueue/transports/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/taskqueue/transports/s3.py` & `django_restit-4.2.9/taskqueue/transports/s3.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/taskqueue/transports/sftp.py` & `django_restit-4.2.9/taskqueue/transports/sftp.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/taskqueue/worker.py` & `django_restit-4.2.9/taskqueue/worker.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/telephony/migrations/0001_initial.py` & `django_restit-4.2.9/telephony/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/telephony/models.py` & `django_restit-4.2.9/telephony/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/telephony/phone_util.py` & `django_restit-4.2.9/telephony/phone_util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/telephony/rpc.py` & `django_restit-4.2.9/telephony/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/wiki/migrations/0001_initial.py` & `django_restit-4.2.9/wiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/wiki/models/faq.py` & `django_restit-4.2.9/wiki/models/faq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/wiki/models/page.py` & `django_restit-4.2.9/wiki/models/page.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/wiki/models/revision.py` & `django_restit-4.2.9/wiki/models/revision.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/wiki/renderers/mistune/highlight.py` & `django_restit-4.2.9/wiki/renderers/mistune/highlight.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/wiki/renderers/mistune/math.py` & `django_restit-4.2.9/wiki/renderers/mistune/math.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/wiki/renderers/mistune/media.py` & `django_restit-4.2.9/wiki/renderers/mistune/media.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/wiki/renderers/mistune/meta.py` & `django_restit-4.2.9/wiki/renderers/mistune/meta.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/wiki/renderers/mistune/task_list.py` & `django_restit-4.2.9/wiki/renderers/mistune/task_list.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/wiki/renderers/mistune/toc.py` & `django_restit-4.2.9/wiki/renderers/mistune/toc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/wiki/rpc/wiki.py` & `django_restit-4.2.9/wiki/rpc/wiki.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/ws4redis/README.md` & `django_restit-4.2.9/ws4redis/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/ws4redis/client.py` & `django_restit-4.2.9/ws4redis/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/ws4redis/connection.py` & `django_restit-4.2.9/ws4redis/connection.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/ws4redis/exceptions.py` & `django_restit-4.2.9/ws4redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/ws4redis/redis.py` & `django_restit-4.2.9/ws4redis/redis.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/ws4redis/servers/base.py` & `django_restit-4.2.9/ws4redis/servers/base.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/ws4redis/servers/django.py` & `django_restit-4.2.9/ws4redis/servers/django.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/ws4redis/servers/uwsgi.py` & `django_restit-4.2.9/ws4redis/servers/uwsgi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/ws4redis/settings.py` & `django_restit-4.2.9/ws4redis/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/ws4redis/utf8validator.py` & `django_restit-4.2.9/ws4redis/utf8validator.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/ws4redis/websocket.py` & `django_restit-4.2.9/ws4redis/websocket.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.8/PKG-INFO` & `django_restit-4.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-restit
-Version: 4.2.8
+Version: 4.2.9
 Summary: A Rest Framework for DJANGO
 License: MIT
 Author: Ian Starnes
 Author-email: ians@311labs.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

