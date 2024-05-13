# Comparing `tmp/intunecd-2.3.3b1.tar.gz` & `tmp/intunecd-2.3.3b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intunecd-2.3.3b1.tar", last modified: Tue May  7 07:34:32 2024, max compression
+gzip compressed data, was "intunecd-2.3.3b2.tar", last modified: Mon May 13 07:50:28 2024, max compression
```

## Comparing `intunecd-2.3.3b1.tar` & `intunecd-2.3.3b2.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.420439 intunecd-2.3.3b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-07 07:34:32.420439 intunecd-2.3.3b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-07 07:34:32.424439 intunecd-2.3.3b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.400438 intunecd-2.3.3b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.400438 intunecd-2.3.3b1/src/IntuneCD/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.404438 intunecd-2.3.3b1/src/IntuneCD/backup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.404438 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/Applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/AuthenticationFlows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/AuthenticationMethods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/AuthorizationPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/B2B.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/DeviceRegistration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/Domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/ExternalIdentities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/GroupSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/RoamingSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/SSPR.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/SecurityDefaults.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Entra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.412438 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/APNs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/Activationlock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/AppConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/AppProtection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/Applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/AutopilotDevices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/Compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/CompliancePartner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ComplianceScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ConditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/CustomAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/DeviceCategories.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/DeviceCompliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/DeviceConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/DeviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/Filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ManagedGooglePlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ManagementIntents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ManagementPartner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/NotificationTemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/PowershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ProactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ReusableSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/Roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ScopeTags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/SettingsCatalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ShellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/Intune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup_entra.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/backup_intune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/document_entra.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/document_intune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.412438 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/BaseBackupModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    36408 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/BaseGraphModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/BaseUpdateModule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/IntuneCDBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/assignment_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    18214 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/get_accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/process_audit_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/intunecdlib/process_scope_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/run_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/run_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/run_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.412438 intunecd-2.3.3b1/src/IntuneCD/update/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.416438 intunecd-2.3.3b1/src/IntuneCD/update/Entra/
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/AuthenticationFlows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/AuthorizationPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/B2B.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/DeviceRegistration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/Domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/GroupSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/RoamingSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/SSPR.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/SecurityDefaults.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Entra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.420439 intunecd-2.3.3b1/src/IntuneCD/update/Intune/
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/AppConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/AppProtection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14535 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/Compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/ComplianceScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/ConditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/CustomAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/DeviceCategories.py
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/DeviceCompliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/DeviceConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/DeviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/EnrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/EnrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/Filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    23308 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/ManagementIntents.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/NotificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/PowerShellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/ProactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/ReusableSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/Roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/ScopeTags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/SettingsCatalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/ShellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/WindowsDriverUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/WindowsQualityUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/Intune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update_entra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/src/IntuneCD/update_intune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.420439 intunecd-2.3.3b1/src/IntuneCD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-07 07:34:32.000000 intunecd-2.3.3b1/src/IntuneCD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-07 07:34:32.000000 intunecd-2.3.3b1/src/IntuneCD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:34:32.000000 intunecd-2.3.3b1/src/IntuneCD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 07:34:32.000000 intunecd-2.3.3b1/src/IntuneCD.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 07:34:32.000000 intunecd-2.3.3b1/src/IntuneCD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 07:34:32.000000 intunecd-2.3.3b1/src/IntuneCD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:34:32.420439 intunecd-2.3.3b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/tests/test_documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-05-07 07:34:26.000000 intunecd-2.3.3b1/tests/test_get_authparams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.933271 intunecd-2.3.3b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-13 07:50:28.933271 intunecd-2.3.3b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-13 07:50:28.933271 intunecd-2.3.3b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.905271 intunecd-2.3.3b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.909271 intunecd-2.3.3b2/src/IntuneCD/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.913271 intunecd-2.3.3b2/src/IntuneCD/backup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.913271 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/Applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/AuthenticationFlows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/AuthenticationMethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/AuthorizationPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/B2B.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/DeviceRegistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/Domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/ExternalIdentities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/GroupSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/RoamingSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/SSPR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/SecurityDefaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Entra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.921271 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/APNs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/Activationlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/AppConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/AppProtection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/Applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/AutopilotDevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/Compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/CompliancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ComplianceScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ConditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/CustomAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/DeviceCategories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/DeviceCompliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/DeviceConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/DeviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/Filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ManagedGooglePlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ManagementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ManagementPartner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/NotificationTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/PowershellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ProactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ReusableSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/Roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ScopeTags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/SettingsCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ShellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/Intune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup_entra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/backup_intune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/document_entra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/document_intune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.921271 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/BaseBackupModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36406 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/BaseGraphModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/BaseUpdateModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/IntuneCDBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/assignment_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18214 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/get_accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/get_authparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/process_audit_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/intunecdlib/process_scope_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/run_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/run_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/run_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.925271 intunecd-2.3.3b2/src/IntuneCD/update/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.925271 intunecd-2.3.3b2/src/IntuneCD/update/Entra/
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/AuthenticationFlows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/AuthorizationPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/B2B.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/DeviceRegistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/Domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/GroupSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/RoamingSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/SSPR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/SecurityDefaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Entra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.929271 intunecd-2.3.3b2/src/IntuneCD/update/Intune/
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/AppConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/AppProtection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14535 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/Compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/ComplianceScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/ConditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/CustomAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/DeviceCategories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/DeviceCompliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/DeviceConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/DeviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/EnrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/EnrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/Filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23308 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/ManagementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/NotificationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/PowerShellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/ProactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/ReusableSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/Roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/ScopeTags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/SettingsCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/ShellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/WindowsDriverUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/WindowsQualityUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/Intune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update_entra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/src/IntuneCD/update_intune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.933271 intunecd-2.3.3b2/src/IntuneCD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-13 07:50:28.000000 intunecd-2.3.3b2/src/IntuneCD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-13 07:50:28.000000 intunecd-2.3.3b2/src/IntuneCD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:50:28.000000 intunecd-2.3.3b2/src/IntuneCD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-13 07:50:28.000000 intunecd-2.3.3b2/src/IntuneCD.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 07:50:28.000000 intunecd-2.3.3b2/src/IntuneCD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 07:50:28.000000 intunecd-2.3.3b2/src/IntuneCD.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:50:28.929271 intunecd-2.3.3b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/tests/test_documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-05-13 07:50:22.000000 intunecd-2.3.3b2/tests/test_get_authparams.py
```

### Comparing `intunecd-2.3.3b1/LICENSE` & `intunecd-2.3.3b2/LICENSE`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/PKG-INFO` & `intunecd-2.3.3b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 2.3.3b1
+Version: 2.3.3b2
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intunecd-2.3.3b1/README.md` & `intunecd-2.3.3b2/README.md`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/setup.cfg` & `intunecd-2.3.3b2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IntuneCD
-version = 2.3.3.beta1
+version = 2.3.3.beta2
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to backup and update configurations in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/IntuneCD
 project_urls =
```

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/Applications.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/Applications.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/AuthenticationFlows.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/AuthenticationFlows.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/AuthenticationMethods.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/AuthenticationMethods.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/AuthorizationPolicy.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/AuthorizationPolicy.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/B2B.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/B2B.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/DeviceRegistration.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/DeviceRegistration.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/Domains.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/Domains.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/ExternalIdentities.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/ExternalIdentities.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/GroupSettings.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/GroupSettings.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/RoamingSettings.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/RoamingSettings.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/SSPR.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/SSPR.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Entra/SecurityDefaults.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Entra/SecurityDefaults.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/APNs.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/APNs.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/Activationlock.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/Activationlock.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/AppConfiguration.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/AppConfiguration.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/AppProtection.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/AppProtection.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/Applications.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/Applications.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/AutopilotDevices.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/AutopilotDevices.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/Compliance.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/Compliance.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/CompliancePartner.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/CompliancePartner.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ComplianceScripts.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ComplianceScripts.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ConditionalAccess.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ConditionalAccess.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/CustomAttributes.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/CustomAttributes.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/DeviceCategories.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/DeviceCategories.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/DeviceCompliance.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/DeviceCompliance.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/DeviceConfigurations.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/DeviceConfigurations.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/DeviceManagementSettings.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/DeviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/Filters.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/Filters.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ManagedGooglePlay.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ManagedGooglePlay.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ManagementIntents.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ManagementIntents.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ManagementPartner.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ManagementPartner.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/NotificationTemplates.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/NotificationTemplates.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/PowershellScripts.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/PowershellScripts.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ProactiveRemediation.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ProactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ReusableSettings.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ReusableSettings.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/Roles.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/Roles.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ScopeTags.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ScopeTags.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/SettingsCatalog.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/SettingsCatalog.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/ShellScripts.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/ShellScripts.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py` & `intunecd-2.3.3b2/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup_entra.py` & `intunecd-2.3.3b2/src/IntuneCD/backup_entra.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/backup_intune.py` & `intunecd-2.3.3b2/src/IntuneCD/backup_intune.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/document_entra.py` & `intunecd-2.3.3b2/src/IntuneCD/document_entra.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/document_intune.py` & `intunecd-2.3.3b2/src/IntuneCD/document_intune.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/intunecdlib/BaseBackupModule.py` & `intunecd-2.3.3b2/src/IntuneCD/intunecdlib/BaseBackupModule.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/intunecdlib/BaseGraphModule.py` & `intunecd-2.3.3b2/src/IntuneCD/intunecdlib/BaseGraphModule.py`

 * *Files 0% similar despite different names*

```diff
@@ -857,17 +857,17 @@
                     endpoint="https://graph.microsoft.com/beta/deviceManagement/assignmentFilters",
                 )
                 for intune_filter in filters["value"]:
                     if (
                         val["target"]["deviceAndAppManagementAssignmentFilterId"]
                         == intune_filter["displayName"]
                     ):
-                        val["target"]["deviceAndAppManagementAssignmentFilterId"] = (
-                            intune_filter["id"]
-                        )
+                        val["target"][
+                            "deviceAndAppManagementAssignmentFilterId"
+                        ] = intune_filter["id"]
 
                 # If filter is None, remove keys
                 if val["target"]["deviceAndAppManagementAssignmentFilterId"] is None:
                     val["target"].pop("deviceAndAppManagementAssignmentFilterId")
                     val["target"].pop("deviceAndAppManagementAssignmentFilterType")
 
             if (
```

### Comparing `intunecd-2.3.3b1/src/IntuneCD/intunecdlib/BaseUpdateModule.py` & `intunecd-2.3.3b2/src/IntuneCD/intunecdlib/BaseUpdateModule.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/intunecdlib/IntuneCDBase.py` & `intunecd-2.3.3b2/src/IntuneCD/intunecdlib/IntuneCDBase.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/intunecdlib/archive.py` & `intunecd-2.3.3b2/src/IntuneCD/intunecdlib/archive.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/intunecdlib/assignment_report.py` & `intunecd-2.3.3b2/src/IntuneCD/intunecdlib/assignment_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                                 item["assignedTo"][payload_type] = [payload_data]
                             payload_added = True
                             break
 
                 if not payload_added:
                     group_data["assignedTo"][payload_type] = [payload_data]
                     groups.append(group_data)
-                    break
+                    # break
 
     def _collect_groups(self, path):
         exclude = set(["__archive__", "Entra"])
         groups = []
         slash = "/"
         run_os = platform.uname().system
         if run_os == "Windows":
```

### Comparing `intunecd-2.3.3b1/src/IntuneCD/intunecdlib/documentation_functions.py` & `intunecd-2.3.3b2/src/IntuneCD/intunecdlib/documentation_functions.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/intunecdlib/get_accesstoken.py` & `intunecd-2.3.3b2/src/IntuneCD/intunecdlib/get_accesstoken.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/intunecdlib/get_authparams.py` & `intunecd-2.3.3b2/src/IntuneCD/intunecdlib/get_authparams.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/intunecdlib/process_audit_data.py` & `intunecd-2.3.3b2/src/IntuneCD/intunecdlib/process_audit_data.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/intunecdlib/process_scope_tags.py` & `intunecd-2.3.3b2/src/IntuneCD/intunecdlib/process_scope_tags.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/run_backup.py` & `intunecd-2.3.3b2/src/IntuneCD/run_backup.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/run_documentation.py` & `intunecd-2.3.3b2/src/IntuneCD/run_documentation.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/run_update.py` & `intunecd-2.3.3b2/src/IntuneCD/run_update.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/AuthenticationFlows.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/AuthenticationFlows.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/AuthorizationPolicy.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/AuthorizationPolicy.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/B2B.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/B2B.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/DeviceRegistration.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/DeviceRegistration.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/Domains.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/Domains.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/GroupSettings.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/GroupSettings.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/RoamingSettings.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/RoamingSettings.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/SSPR.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/SSPR.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Entra/SecurityDefaults.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Entra/SecurityDefaults.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/AppConfiguration.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/AppConfiguration.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/AppProtection.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/AppProtection.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/Compliance.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/Compliance.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/ComplianceScripts.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/ComplianceScripts.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/ConditionalAccess.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/ConditionalAccess.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/CustomAttributes.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/CustomAttributes.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/DeviceCategories.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/DeviceCategories.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/DeviceCompliance.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/DeviceCompliance.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/DeviceConfigurations.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/DeviceConfigurations.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/DeviceManagementSettings.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/DeviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/EnrollmentConfigurations.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/EnrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/EnrollmentStatusPage.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/EnrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/Filters.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/Filters.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/ManagementIntents.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/ManagementIntents.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/NotificationTemplate.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/NotificationTemplate.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/PowerShellScripts.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/PowerShellScripts.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/ProactiveRemediation.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/ProactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/ReusableSettings.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/ReusableSettings.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/Roles.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/Roles.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/ScopeTags.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/ScopeTags.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/SettingsCatalog.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/SettingsCatalog.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/ShellScripts.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/ShellScripts.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/WindowsDriverUpdates.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/WindowsDriverUpdates.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update/Intune/WindowsQualityUpdates.py` & `intunecd-2.3.3b2/src/IntuneCD/update/Intune/WindowsQualityUpdates.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update_entra.py` & `intunecd-2.3.3b2/src/IntuneCD/update_entra.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD/update_intune.py` & `intunecd-2.3.3b2/src/IntuneCD/update_intune.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/src/IntuneCD.egg-info/PKG-INFO` & `intunecd-2.3.3b2/src/IntuneCD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 2.3.3b1
+Version: 2.3.3b2
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intunecd-2.3.3b1/src/IntuneCD.egg-info/SOURCES.txt` & `intunecd-2.3.3b2/src/IntuneCD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/tests/test_archive.py` & `intunecd-2.3.3b2/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/tests/test_documentation_functions.py` & `intunecd-2.3.3b2/tests/test_documentation_functions.py`

 * *Files identical despite different names*

### Comparing `intunecd-2.3.3b1/tests/test_get_authparams.py` & `intunecd-2.3.3b2/tests/test_get_authparams.py`

 * *Files identical despite different names*

