# Comparing `tmp/opentera-1.2.5.tar.gz` & `tmp/opentera-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentera-1.2.5.tar", last modified: Tue Mar  5 19:30:13 2024, max compression
+gzip compressed data, was "opentera-1.2.6.tar", last modified: Mon May 13 12:46:51 2024, max compression
```

## Comparing `opentera-1.2.5.tar` & `opentera-1.2.6.tar`

### file list

```diff
@@ -1,155 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.201575 opentera-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-05 19:28:48.000000 opentera-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-05 19:28:48.000000 opentera-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-03-05 19:30:13.201575 opentera-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-05 19:28:48.000000 opentera-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.181575 opentera-1.2.5/opentera/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-05 19:29:31.000000 opentera-1.2.5/opentera/OpenTeraServerVersion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       17 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.185575 opentera-1.2.5/opentera/config/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4321 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/config/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.185575 opentera-1.2.5/opentera/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/crypto/crypto_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.185575 opentera-1.2.5/opentera/db/
--rwxr-xr-x   0 runner    (1001) docker     (127)    13227 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/Base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16845 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/SoftDeleteMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/SoftDeleteQueryRewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/SoftInsertMixin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       17 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.189575 opentera-1.2.5/opentera/db/models/
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraAsset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12062 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraDevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraDeviceParticipant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraDeviceProject.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraDeviceSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraDeviceSubType.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraDeviceType.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraParticipant.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraParticipantGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraProject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraServerSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraService.py
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraServiceAccess.py
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraServiceConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraServiceConfigSpecific.py
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraServiceProject.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraServiceRole.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraServiceSite.py
--rw-r--r--   0 runner    (1001) docker     (127)    23930 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraSession.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraSessionDevices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraSessionEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraSessionParticipants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraSessionType.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraSessionTypeProject.py
--rw-r--r--   0 runner    (1001) docker     (127)     9960 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraSessionTypeSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraSessionUsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraTestType.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraTestTypeProject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraTestTypeSite.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17338 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraUserGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraUserPreference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/TeraUserUserGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/db/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.189575 opentera-1.2.5/opentera/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.193575 opentera-1.2.5/opentera/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraDeviceForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraDeviceSubTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraDeviceTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraParticipantForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraParticipantGroupForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraProjectForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraServiceConfigForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraServiceForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraSessionForm.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraSessionTypeConfigForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraSessionTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraSiteForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraTestTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraUserForm.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraUserGroupForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/TeraVersionsForm.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.193575 opentera-1.2.5/opentera/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/logging/LoggingClient.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.193575 opentera-1.2.5/opentera/messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.197575 opentera-1.2.5/opentera/messages/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/CreateSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/DatabaseEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/DeviceEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/JoinSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/JoinSessionReplyEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/LeaveSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/LogEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/LoginEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/ParticipantEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/RPCMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/Result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/ServerCommand_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/StopSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/TeraEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/TeraMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/TeraModuleMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/UserEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-05 19:30:07.000000 opentera-1.2.5/opentera/messages/python/UserRegisterToEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/messages/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.197575 opentera-1.2.5/opentera/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/modules/BaseModule.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.197575 opentera-1.2.5/opentera/redis/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5734 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/redis/RedisClient.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3143 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/redis/RedisProtocolFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/redis/RedisRPCClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/redis/RedisVars.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.201575 opentera-1.2.5/opentera/services/
--rw-r--r--   0 runner    (1001) docker     (127)    38393 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/BaseWebRTCService.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/DisabledTokenStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)    22790 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/ServiceAccessManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/ServiceConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/ServiceOpenTera.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/ServiceOpenTeraWithAssets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/ServiceOpenTeraWithTests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/TeraDeviceClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/TeraParticipantClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/TeraServiceClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/TeraUserClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.201575 opentera-1.2.5/opentera/services/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/modules/WebRTCModule.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/services/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.201575 opentera-1.2.5/opentera/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/utils/Metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/utils/TeraVersions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/utils/UserAgentParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.201575 opentera-1.2.5/opentera/utils/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/utils/assets/AssetFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/utils/assets/AssetVideoFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/utils/assets/BaseAsset.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 19:28:48.000000 opentera-1.2.5/opentera/utils/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.201575 opentera-1.2.5/opentera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-03-05 19:30:13.000000 opentera-1.2.5/opentera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-05 19:30:13.000000 opentera-1.2.5/opentera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 19:30:13.000000 opentera-1.2.5/opentera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-05 19:30:13.000000 opentera-1.2.5/opentera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-05 19:30:13.000000 opentera-1.2.5/opentera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 19:30:13.201575 opentera-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-05 19:28:48.000000 opentera-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.181575 opentera-1.2.5/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.181575 opentera-1.2.5/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.201575 opentera-1.2.5/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-05 19:30:09.000000 opentera-1.2.5/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    80958 2024-03-05 19:28:48.000000 opentera-1.2.5/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.181575 opentera-1.2.5/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:30:13.201575 opentera-1.2.5/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    40248 2024-03-05 19:30:09.000000 opentera-1.2.5/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    98901 2024-03-05 19:28:48.000000 opentera-1.2.5/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.271237 opentera-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-13 12:45:47.000000 opentera-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 12:45:47.000000 opentera-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-13 12:46:51.271237 opentera-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-13 12:45:47.000000 opentera-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.251237 opentera-1.2.6/opentera/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-13 12:46:12.000000 opentera-1.2.6/opentera/OpenTeraServerVersion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       17 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.251237 opentera-1.2.6/opentera/config/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4321 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/config/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.251237 opentera-1.2.6/opentera/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/crypto/crypto_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.255237 opentera-1.2.6/opentera/db/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13227 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16845 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/SoftDeleteMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/SoftDeleteQueryRewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/SoftInsertMixin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       17 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.259237 opentera-1.2.6/opentera/db/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraAsset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12062 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraDevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraDeviceParticipant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraDeviceProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraDeviceSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraDeviceSubType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraDeviceType.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraParticipant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraParticipantGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraServerSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraService.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraServiceAccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraServiceConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraServiceConfigSpecific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraServiceProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraServiceRole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraServiceSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23944 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraSession.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraSessionDevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraSessionEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraSessionParticipants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraSessionType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraSessionTypeProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9960 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraSessionTypeSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraSessionUsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraTestType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraTestTypeProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraTestTypeSite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17338 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraUserGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraUserPreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/TeraUserUserGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/db/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.259237 opentera-1.2.6/opentera/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.263237 opentera-1.2.6/opentera/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraDeviceForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraDeviceSubTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraDeviceTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraParticipantForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraParticipantGroupForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraProjectForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraServiceConfigForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraServiceForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraSessionForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraSessionTypeConfigForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraSessionTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraSiteForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraTestTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraUserForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraUserGroupForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/TeraVersionsForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.263237 opentera-1.2.6/opentera/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/logging/LoggingClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.263237 opentera-1.2.6/opentera/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.267237 opentera-1.2.6/opentera/messages/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/ArchiveEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/CreateSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/DatabaseEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/DeviceEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/JoinSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/JoinSessionReplyEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/LeaveSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/LogEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/LoginEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/ParticipantEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/RPCMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/Result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/ServerCommand_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/StopSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/TeraEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/TeraMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/TeraModuleMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/UserEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-13 12:46:45.000000 opentera-1.2.6/opentera/messages/python/UserRegisterToEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/messages/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.267237 opentera-1.2.6/opentera/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/modules/BaseModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.267237 opentera-1.2.6/opentera/redis/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5734 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/redis/RedisClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3143 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/redis/RedisProtocolFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/redis/RedisRPCClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/redis/RedisVars.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.267237 opentera-1.2.6/opentera/services/
+-rw-r--r--   0 runner    (1001) docker     (127)    38393 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/BaseWebRTCService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/DisabledTokenStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22790 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/ServiceAccessManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/ServiceConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/ServiceOpenTera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/ServiceOpenTeraWithAssets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/ServiceOpenTeraWithTests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/TeraDeviceClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/TeraParticipantClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/TeraServiceClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/TeraUserClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.267237 opentera-1.2.6/opentera/services/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/modules/WebRTCModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/services/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.267237 opentera-1.2.6/opentera/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/utils/Metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/utils/TeraVersions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/utils/UserAgentParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.271237 opentera-1.2.6/opentera/utils/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/utils/assets/AssetFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/utils/assets/AssetVideoFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/utils/assets/BaseAsset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/opentera/utils/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.271237 opentera-1.2.6/opentera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-13 12:46:51.000000 opentera-1.2.6/opentera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-13 12:46:51.000000 opentera-1.2.6/opentera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:46:51.000000 opentera-1.2.6/opentera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-13 12:46:51.000000 opentera-1.2.6/opentera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 12:46:51.000000 opentera-1.2.6/opentera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:46:51.271237 opentera-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-13 12:45:47.000000 opentera-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.251237 opentera-1.2.6/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.251237 opentera-1.2.6/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.271237 opentera-1.2.6/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-13 12:46:47.000000 opentera-1.2.6/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    80958 2024-05-13 12:45:47.000000 opentera-1.2.6/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.251237 opentera-1.2.6/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.271237 opentera-1.2.6/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    40248 2024-05-13 12:46:47.000000 opentera-1.2.6/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    98901 2024-05-13 12:45:47.000000 opentera-1.2.6/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:46:51.271237 opentera-1.2.6/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-13 12:45:47.000000 opentera-1.2.6/workers/AssetsArchiveWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:45:47.000000 opentera-1.2.6/workers/__init__.py
```

### Comparing `opentera-1.2.5/LICENSE` & `opentera-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/PKG-INFO` & `opentera-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentera
-Version: 1.2.5
+Version: 1.2.6
 Summary: OpenTera base package
 Home-page: https://github.com/introlab/opentera
 Author: Dominic Létourneau, Simon Brière
 Author-email: dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opentera-1.2.5/README.md` & `opentera-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/config/ConfigManager.py` & `opentera-1.2.6/opentera/config/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/crypto/crypto_utils.py` & `opentera-1.2.6/opentera/crypto/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/Base.py` & `opentera-1.2.6/opentera/db/Base.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/SoftDeleteMixin.py` & `opentera-1.2.6/opentera/db/SoftDeleteMixin.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/SoftDeleteQueryRewriter.py` & `opentera-1.2.6/opentera/db/SoftDeleteQueryRewriter.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/SoftInsertMixin.py` & `opentera-1.2.6/opentera/db/SoftInsertMixin.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraAsset.py` & `opentera-1.2.6/opentera/db/models/TeraAsset.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     # Put a description of the asset here
     asset_name = Column(String, nullable=False)
 
     asset_uuid = Column(String(36), nullable=False, unique=True)
     asset_service_uuid = Column(String(36), ForeignKey("t_services.service_uuid", ondelete='cascade'), nullable=False)
     asset_type = Column(String, nullable=False)  # MIME Type
     asset_datetime = Column(TIMESTAMP(timezone=True), nullable=True)
+    asset_expiration_datetime = Column(TIMESTAMP(timezone=True), nullable=True)
 
     asset_session = relationship("TeraSession", back_populates='session_assets')
     asset_device = relationship("TeraDevice", back_populates='device_assets')
     asset_user = relationship("TeraUser", back_populates='user_assets')
     asset_participant = relationship("TeraParticipant", back_populates='participant_assets')
     asset_service = relationship("TeraService", foreign_keys="TeraAsset.id_service")
     asset_service_owner = relationship("TeraService", foreign_keys="TeraAsset.asset_service_uuid")
@@ -103,14 +104,26 @@
             new_asset.asset_device = asset_device
             new_asset.asset_uuid = str(uuid.uuid4())
             new_asset.asset_service_uuid = '00000000-0000-0000-0000-000000000001'
             new_asset.asset_type = 'video/mpeg'
             new_asset.id_service = 1
             TeraAsset.insert(new_asset)
 
+            device_session = TeraSession.get_session_by_name('Séance #9')
+            for i in range(3):
+                new_asset = TeraAsset()
+                new_asset.asset_name = "Device Asset"
+                new_asset.asset_session = device_session
+                new_asset.asset_device = asset_device
+                new_asset.asset_uuid = str(uuid.uuid4())
+                new_asset.asset_service_uuid = '00000000-0000-0000-0000-000000000001'
+                new_asset.asset_type = 'video/mpeg'
+                new_asset.id_service = 1
+                TeraAsset.insert(new_asset)
+
     @staticmethod
     def get_asset_by_id(asset_id: int, with_deleted: bool = False):
         return TeraAsset.query.filter_by(id_asset=asset_id).execution_options(include_deleted=with_deleted).first()
 
     @staticmethod
     def get_asset_by_uuid(asset_uuid: str, with_deleted: bool = False):
         return TeraAsset.query.filter_by(asset_uuid=asset_uuid).execution_options(include_deleted=with_deleted).first()
```

### Comparing `opentera-1.2.5/opentera/db/models/TeraDevice.py` & `opentera-1.2.6/opentera/db/models/TeraDevice.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraDeviceParticipant.py` & `opentera-1.2.6/opentera/db/models/TeraDeviceParticipant.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraDeviceProject.py` & `opentera-1.2.6/opentera/db/models/TeraDeviceProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraDeviceSite.py` & `opentera-1.2.6/opentera/db/models/TeraDeviceSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraDeviceSubType.py` & `opentera-1.2.6/opentera/db/models/TeraDeviceSubType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraDeviceType.py` & `opentera-1.2.6/opentera/db/models/TeraDeviceType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraParticipant.py` & `opentera-1.2.6/opentera/db/models/TeraParticipant.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraParticipantGroup.py` & `opentera-1.2.6/opentera/db/models/TeraParticipantGroup.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraProject.py` & `opentera-1.2.6/opentera/db/models/TeraProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraServerSettings.py` & `opentera-1.2.6/opentera/db/models/TeraServerSettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from opentera.db.Base import BaseModel
-from sqlalchemy import Column, ForeignKey, Integer, String, Sequence, Boolean, TIMESTAMP
-from sqlalchemy.orm import relationship
+from sqlalchemy import Column, Integer, String, Sequence
 import string
 from string import digits, ascii_lowercase, ascii_uppercase
-import random
+import secrets
 import uuid
 
 
 class TeraServerSettings(BaseModel):
     __tablename__ = 't_server_settings'
     id_server_settings = Column(Integer, Sequence('id_server_settings_sequence'), primary_key=True, autoincrement=True)
     server_settings_name = Column(String, nullable=False, unique=True)
@@ -36,15 +35,15 @@
         # Unique server id
         server_uuid = str(uuid.uuid4())
         TeraServerSettings.set_server_setting(TeraServerSettings.ServerUUID, server_uuid)
 
     @staticmethod
     def generate_token_key(length: int) -> str:
         token_symbols = digits + ascii_uppercase + ascii_lowercase
-        token_key = ''.join(random.choice(token_symbols) for i in range(length))  # Key length = 32 chars
+        token_key = ''.join(secrets.choice(token_symbols) for i in range(length))  # Key length = 32 chars
         return token_key
 
     @staticmethod
     def get_server_setting_value(setting_name: string):
         current_setting = TeraServerSettings.get_server_setting(setting_name=setting_name)
         if current_setting:
             return current_setting.server_settings_value
```

### Comparing `opentera-1.2.5/opentera/db/models/TeraService.py` & `opentera-1.2.6/opentera/db/models/TeraService.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraServiceAccess.py` & `opentera-1.2.6/opentera/db/models/TeraServiceAccess.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraServiceConfig.py` & `opentera-1.2.6/opentera/db/models/TeraServiceConfig.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraServiceConfigSpecific.py` & `opentera-1.2.6/opentera/db/models/TeraServiceConfigSpecific.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraServiceProject.py` & `opentera-1.2.6/opentera/db/models/TeraServiceProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraServiceRole.py` & `opentera-1.2.6/opentera/db/models/TeraServiceRole.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraServiceSite.py` & `opentera-1.2.6/opentera/db/models/TeraServiceSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraSession.py` & `opentera-1.2.6/opentera/db/models/TeraSession.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
             # Create device sessions
             for i in range(8):
                 base_session = TeraSession()
                 base_session.session_creator_device = TeraDevice.get_device_by_id(1)
                 ses_type = random.randint(1, 3)
                 base_session.session_session_type = TeraSessionType.get_session_type_by_id(ses_type)
-                base_session.session_name = "Séance #" + str(i + 1)
+                base_session.session_name = "Séance #" + str(i + 1 + 8)
                 base_session.session_start_datetime = datetime.now() - timedelta(days=i)
                 base_session.session_duration = random.randint(60, 4800)
                 # ses_status = random.randint(0, 4)
                 ses_status = default_status[i]
                 base_session.session_status = ses_status
                 if i < 7:
                     base_session.session_participants = [session_part]
@@ -195,15 +195,15 @@
 
             # Create participant sessions
             for i in range(8):
                 base_session = TeraSession()
                 base_session.session_creator_participant = TeraParticipant.get_participant_by_id(1)
                 ses_type = random.randint(1, 3)
                 base_session.session_session_type = TeraSessionType.get_session_type_by_id(ses_type)
-                base_session.session_name = "Séance #" + str(i + 1)
+                base_session.session_name = "Séance #" + str(i + 1 + 16)
                 base_session.session_start_datetime = datetime.now() - timedelta(days=i)
                 base_session.session_duration = random.randint(60, 4800)
                 # ses_status = random.randint(0, 4)
                 ses_status = default_status[i]
                 base_session.session_status = ses_status
                 base_session.session_participants = [base_session.session_creator_participant]
                 base_session.session_uuid = str(uuid.uuid4())
@@ -223,15 +223,15 @@
 
             # Create service sessions
             for i in range(4):
                 base_session = TeraSession()
                 base_session.session_creator_service = session_service
                 ses_type = random.randint(1, 3)
                 base_session.session_session_type = TeraSessionType.get_session_type_by_id(ses_type)
-                base_session.session_name = "Séance #" + str(i + 1)
+                base_session.session_name = "Séance #" + str(i + 1 + 24)
                 base_session.session_start_datetime = datetime.now() - timedelta(days=i)
                 base_session.session_duration = random.randint(60, 4800)
                 # ses_status = random.randint(0, 4)
                 ses_status = default_status[i]
                 base_session.session_status = ses_status
                 if i < 3:
                     base_session.session_participants = [session_part]
```

### Comparing `opentera-1.2.5/opentera/db/models/TeraSessionDevices.py` & `opentera-1.2.6/opentera/db/models/TeraSessionDevices.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraSessionEvent.py` & `opentera-1.2.6/opentera/db/models/TeraSessionEvent.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraSessionParticipants.py` & `opentera-1.2.6/opentera/db/models/TeraSessionParticipants.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraSessionType.py` & `opentera-1.2.6/opentera/db/models/TeraSessionType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraSessionTypeProject.py` & `opentera-1.2.6/opentera/db/models/TeraSessionTypeProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraSessionTypeSite.py` & `opentera-1.2.6/opentera/db/models/TeraSessionTypeSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraSessionUsers.py` & `opentera-1.2.6/opentera/db/models/TeraSessionUsers.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraSite.py` & `opentera-1.2.6/opentera/db/models/TeraSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraTest.py` & `opentera-1.2.6/opentera/db/models/TeraTest.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraTestType.py` & `opentera-1.2.6/opentera/db/models/TeraTestType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraTestTypeProject.py` & `opentera-1.2.6/opentera/db/models/TeraTestTypeProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraTestTypeSite.py` & `opentera-1.2.6/opentera/db/models/TeraTestTypeSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraUser.py` & `opentera-1.2.6/opentera/db/models/TeraUser.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraUserGroup.py` & `opentera-1.2.6/opentera/db/models/TeraUserGroup.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraUserPreference.py` & `opentera-1.2.6/opentera/db/models/TeraUserPreference.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/TeraUserUserGroup.py` & `opentera-1.2.6/opentera/db/models/TeraUserUserGroup.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/db/models/__init__.py` & `opentera-1.2.6/opentera/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraDeviceForm.py` & `opentera-1.2.6/opentera/forms/TeraDeviceForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraDeviceSubTypeForm.py` & `opentera-1.2.6/opentera/forms/TeraDeviceSubTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraDeviceTypeForm.py` & `opentera-1.2.6/opentera/forms/TeraDeviceTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraForm.py` & `opentera-1.2.6/opentera/forms/TeraForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraParticipantForm.py` & `opentera-1.2.6/opentera/forms/TeraParticipantForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraParticipantGroupForm.py` & `opentera-1.2.6/opentera/forms/TeraParticipantGroupForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraProjectForm.py` & `opentera-1.2.6/opentera/forms/TeraProjectForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraServiceConfigForm.py` & `opentera-1.2.6/opentera/forms/TeraServiceConfigForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraServiceForm.py` & `opentera-1.2.6/opentera/forms/TeraServiceForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraSessionForm.py` & `opentera-1.2.6/opentera/forms/TeraSessionForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraSessionTypeForm.py` & `opentera-1.2.6/opentera/forms/TeraSessionTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraSiteForm.py` & `opentera-1.2.6/opentera/forms/TeraSiteForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraTestTypeForm.py` & `opentera-1.2.6/opentera/forms/TeraTestTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraUserForm.py` & `opentera-1.2.6/opentera/forms/TeraUserForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraUserGroupForm.py` & `opentera-1.2.6/opentera/forms/TeraUserGroupForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/forms/TeraVersionsForm.py` & `opentera-1.2.6/opentera/forms/TeraVersionsForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/logging/LoggingClient.py` & `opentera-1.2.6/opentera/logging/LoggingClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/CreateSession_pb2.py` & `opentera-1.2.6/opentera/messages/python/CreateSession_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/DatabaseEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/DatabaseEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/DeviceEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/DeviceEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/JoinSessionEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/JoinSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/JoinSessionReplyEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/JoinSessionReplyEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/LeaveSessionEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/LeaveSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/LogEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/LogEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/LoginEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/LoginEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/ParticipantEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/ParticipantEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/RPCMessage_pb2.py` & `opentera-1.2.6/opentera/messages/python/RPCMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/Result_pb2.py` & `opentera-1.2.6/opentera/messages/python/Result_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/ServerCommand_pb2.py` & `opentera-1.2.6/opentera/messages/python/ServerCommand_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/StopSessionEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/StopSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/TeraEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/TeraEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/TeraMessage_pb2.py` & `opentera-1.2.6/opentera/messages/python/TeraMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/TeraModuleMessage_pb2.py` & `opentera-1.2.6/opentera/messages/python/TeraModuleMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/UserEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/UserEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/UserRegisterToEvent_pb2.py` & `opentera-1.2.6/opentera/messages/python/UserRegisterToEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/messages/python/__init__.py` & `opentera-1.2.6/opentera/messages/python/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,24 @@
 from .UserEvent_pb2 import UserEvent
 from .UserRegisterToEvent_pb2 import UserRegisterToEvent
 from .JoinSessionReplyEvent_pb2 import JoinSessionReplyEvent
 from .LeaveSessionEvent_pb2 import LeaveSessionEvent
 from .LogEvent_pb2 import LogEvent
 from .LeaveSessionEvent_pb2 import LeaveSessionEvent
 from .LoginEvent_pb2 import LoginEvent
+from .ArchiveEvent_pb2 import ArchiveEvent
 
 from google.protobuf.any_pb2 import Any
 
 
 
 
 # All exported symbols
-__all__ = ['CreateSession',
+__all__ = ['ArchiveEvent',
+           'CreateSession',
            'DatabaseEvent',
            'DeviceEvent',
            'JoinSessionEvent',
            'JoinSessionReplyEvent',
            'LeaveSessionEvent',
            'LogEvent',
            'ParticipantEvent',
```

### Comparing `opentera-1.2.5/opentera/modules/BaseModule.py` & `opentera-1.2.6/opentera/modules/BaseModule.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/redis/RedisClient.py` & `opentera-1.2.6/opentera/redis/RedisClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/redis/RedisProtocolFactory.py` & `opentera-1.2.6/opentera/redis/RedisProtocolFactory.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/redis/RedisRPCClient.py` & `opentera-1.2.6/opentera/redis/RedisRPCClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/redis/RedisVars.py` & `opentera-1.2.6/opentera/redis/RedisVars.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,7 +31,12 @@
     @classmethod
     def build_service_rpc_topic(cls, service_key) -> str:
         return cls.RedisVar_ServicePrefixKey + service_key + '.rpc'
 
     @classmethod
     def build_service_message_topic(cls, service_key) -> str:
         return cls.RedisVar_ServicePrefixKey + service_key + '.messages'
+
+    @classmethod
+    def build_service_event_topic(cls, service_key) -> str:
+        """ Build service event topic from service key, used to subscribe events to a specific service. """
+        return cls.RedisVar_ServicePrefixKey + service_key + '.events'
```

### Comparing `opentera-1.2.5/opentera/services/BaseWebRTCService.py` & `opentera-1.2.6/opentera/services/BaseWebRTCService.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/services/DisabledTokenStorage.py` & `opentera-1.2.6/opentera/services/DisabledTokenStorage.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/services/ServiceAccessManager.py` & `opentera-1.2.6/opentera/services/ServiceAccessManager.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/services/ServiceConfigManager.py` & `opentera-1.2.6/opentera/services/ServiceConfigManager.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/services/ServiceOpenTera.py` & `opentera-1.2.6/opentera/services/ServiceOpenTera.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,31 +67,29 @@
     def notify_service_messages(self, pattern, channel, message):
         pass
 
     @defer.inlineCallbacks
     def build_interface(self):
         # TODO not sure of the interface using UUID or name here...
         # Will do  both!
-        ret1 = yield self.subscribe_pattern_with_callback(
+        yield self.subscribe_pattern_with_callback(
             RedisVars.build_service_message_topic( self.service_info['service_uuid']), self.notify_service_messages)
 
-        ret2 = yield self.subscribe_pattern_with_callback(
+        yield self.subscribe_pattern_with_callback(
             RedisVars.build_service_message_topic(self.service_info['service_key']), self.notify_service_messages)
 
-        ret3 = yield self.subscribe_pattern_with_callback(
+        yield self.subscribe_pattern_with_callback(
             RedisVars.build_service_rpc_topic(self.service_info['service_uuid']), self.notify_service_rpc)
 
-        ret4 = yield self.subscribe_pattern_with_callback(
+        yield self.subscribe_pattern_with_callback(
             RedisVars.build_service_rpc_topic(self.service_info['service_key']), self.notify_service_rpc)
 
-        print(ret1, ret2, ret3, ret4)
-
     def notify_service_rpc(self, pattern, channel, message):
-        import threading
-        print('ServiceOpenTera - Received rpc', self, pattern, channel, message, ' thread:', threading.current_thread())
+        # import threading
+        # print('ServiceOpenTera - Received rpc', self, pattern, channel, message, ' thread:', threading.current_thread())
 
         rpc_message = messages.RPCMessage()
 
         try:
             # Look for a RPCMessage
             rpc_message.ParseFromString(message)
 
@@ -168,14 +166,18 @@
     def send_event_message(self, event, topic: str):
         message = self.create_event_message(topic)
         any_message = messages.Any()
         any_message.Pack(event)
         message.events.extend([any_message])
         return self.publish(message.header.topic, message.SerializeToString())
 
+    def send_service_event_message(self, event):
+        topic = RedisVars.build_service_event_topic(self.service_info['service_key'])
+        self.send_event_message(event, topic)
+
     def create_event_message(self, topic):
         event_message = messages.TeraEvent()
         event_message.header.version = 1
         event_message.header.time = datetime.datetime.now().timestamp()
         event_message.header.topic = topic
         return event_message
```

### Comparing `opentera-1.2.5/opentera/services/ServiceOpenTeraWithAssets.py` & `opentera-1.2.6/opentera/services/ServiceOpenTeraWithAssets.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/services/ServiceOpenTeraWithTests.py` & `opentera-1.2.6/opentera/services/ServiceOpenTeraWithTests.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/services/TeraDeviceClient.py` & `opentera-1.2.6/opentera/services/TeraDeviceClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/services/TeraParticipantClient.py` & `opentera-1.2.6/opentera/services/TeraParticipantClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/services/TeraServiceClient.py` & `opentera-1.2.6/opentera/services/TeraServiceClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/services/TeraUserClient.py` & `opentera-1.2.6/opentera/services/TeraUserClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/services/modules/WebRTCModule.py` & `opentera-1.2.6/opentera/services/modules/WebRTCModule.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/utils/Metrics.py` & `opentera-1.2.6/opentera/utils/Metrics.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/utils/TeraVersions.py` & `opentera-1.2.6/opentera/utils/TeraVersions.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/utils/UserAgentParser.py` & `opentera-1.2.6/opentera/utils/UserAgentParser.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera/utils/assets/BaseAsset.py` & `opentera-1.2.6/opentera/utils/assets/BaseAsset.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/opentera.egg-info/PKG-INFO` & `opentera-1.2.6/opentera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentera
-Version: 1.2.5
+Version: 1.2.6
 Summary: OpenTera base package
 Home-page: https://github.com/introlab/opentera
 Author: Dominic Létourneau, Simon Brière
 Author-email: dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opentera-1.2.5/opentera.egg-info/SOURCES.txt` & `opentera-1.2.6/opentera.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 opentera/forms/TeraUserForm.py
 opentera/forms/TeraUserGroupForm.py
 opentera/forms/TeraVersionsForm.py
 opentera/forms/__init__.py
 opentera/logging/LoggingClient.py
 opentera/logging/__init__.py
 opentera/messages/__init__.py
+opentera/messages/python/ArchiveEvent_pb2.py
 opentera/messages/python/CreateSession_pb2.py
 opentera/messages/python/DatabaseEvent_pb2.py
 opentera/messages/python/DeviceEvent_pb2.py
 opentera/messages/python/JoinSessionEvent_pb2.py
 opentera/messages/python/JoinSessionReplyEvent_pb2.py
 opentera/messages/python/LeaveSessionEvent_pb2.py
 opentera/messages/python/LogEvent_pb2.py
@@ -123,8 +124,10 @@
 opentera/utils/assets/AssetFile.py
 opentera/utils/assets/AssetVideoFile.py
 opentera/utils/assets/BaseAsset.py
 opentera/utils/assets/__init__.py
 translations/en/LC_MESSAGES/messages.mo
 translations/en/LC_MESSAGES/messages.po
 translations/fr/LC_MESSAGES/messages.mo
-translations/fr/LC_MESSAGES/messages.po
+translations/fr/LC_MESSAGES/messages.po
+workers/AssetsArchiveWorker.py
+workers/__init__.py
```

### Comparing `opentera-1.2.5/opentera.egg-info/requires.txt` & `opentera-1.2.6/opentera.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/setup.py` & `opentera-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("env/requirements.txt", "r", encoding="utf-8") as f:
     requirements = f.readlines()
     requirements.append('protobuf==3.20.3')
 
 setuptools.setup(
     name="opentera",
-    version="1.2.5",
+    version="1.2.6",
     author="Dominic Létourneau, Simon Brière",
     author_email="dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca",
     description="OpenTera base package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/introlab/opentera",
     packages=setuptools.find_packages(),
```

### Comparing `opentera-1.2.5/translations/en/LC_MESSAGES/messages.po` & `opentera-1.2.6/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `opentera-1.2.5/translations/fr/LC_MESSAGES/messages.mo` & `opentera-1.2.6/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: \n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "A new usergroup must have at least one service access"
 msgstr ""
 "Un nouveau groupe utilisateur doit avoir au moins un accès à un service"
 
 msgid "Access Token"
 msgstr "Jeton d'accès"
```

### Comparing `opentera-1.2.5/translations/fr/LC_MESSAGES/messages.po` & `opentera-1.2.6/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

