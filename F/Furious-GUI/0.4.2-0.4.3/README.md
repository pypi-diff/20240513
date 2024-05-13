# Comparing `tmp/Furious-GUI-0.4.2.tar.gz` & `tmp/Furious-GUI-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Furious-GUI-0.4.2.tar", last modified: Sat May 11 12:47:25 2024, max compression
+gzip compressed data, was "Furious-GUI-0.4.3.tar", last modified: Mon May 13 10:41:05 2024, max compression
```

## Comparing `Furious-GUI-0.4.2.tar` & `Furious-GUI-0.4.3.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.795924 Furious-GUI-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.743924 Furious-GUI-0.4.2/Furious/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.743924 Furious-GUI-0.4.2/Furious/Core/
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Core/CoreManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Core/Hysteria1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Core/Hysteria2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Core/Tun2socks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Core/XrayCore.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.743924 Furious-GUI-0.4.2/Furious/Data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.747924 Furious-GUI-0.4.2/Furious/Data/font/
--rw-r--r--   0 runner    (1001) docker     (127)   624892 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Data/font/CascadiaMono
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Data/font/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.751924 Furious-GUI-0.4.2/Furious/Data/hysteria/
--rw-r--r--   0 runner    (1001) docker     (127)  1974430 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Data/hysteria/bypass-Iran.acl
--rw-r--r--   0 runner    (1001) docker     (127)  1390176 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Data/hysteria/bypass-mainland-China.acl
--rw-r--r--   0 runner    (1001) docker     (127)  6444374 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Data/hysteria/country.mmdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.779924 Furious-GUI-0.4.2/Furious/Data/xray/
--rw-r--r--   0 runner    (1001) docker     (127) 10715744 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Data/xray/geoip.dat
--rw-r--r--   0 runner    (1001) docker     (127)  6057957 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Data/xray/geosite.dat
--rw-r--r--   0 runner    (1001) docker     (127)  3199463 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Data/xray/iran.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.783924 Furious-GUI-0.4.2/Furious/Externals/
--rw-r--r--   0 runner    (1001) docker     (127)    40204 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Externals/GenTranslation.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Externals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.783924 Furious-GUI-0.4.2/Furious/Interface/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Interface/Application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Interface/ConfigurationFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Interface/CoreFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Interface/Encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Interface/GuiEditorItemFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Interface/ItemUpdateProtocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Interface/Storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Interface/UserServersTableItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.783924 Furious-GUI-0.4.2/Furious/Library/
--rw-r--r--   0 runner    (1001) docker     (127)    55774 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Library/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Library/EmptyFactoryHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Library/Encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Library/Tcping.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.783924 Furious-GUI-0.4.2/Furious/PyFramework/
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/PyFramework/Ancestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/PyFramework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.787924 Furious-GUI-0.4.2/Furious/QtFramework/
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/Ancestors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/CoreProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/DNSResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/DynamicTheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/DynamicTranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/GuiEditorXXX.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/NetworkStateManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/QtGui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/QtNetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    16523 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/QtWidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/TextEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/TextEditorTheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/UpdatesManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/QtFramework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.787924 Furious-GUI-0.4.2/Furious/Storage/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Storage/UserServers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Storage/UserSubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.787924 Furious-GUI-0.4.2/Furious/TrayActions/
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/TrayActions/Connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/TrayActions/EditConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/TrayActions/Exit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/TrayActions/Import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/TrayActions/Language.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/TrayActions/Routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/TrayActions/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/TrayActions/SystemProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/TrayActions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.791924 Furious-GUI-0.4.2/Furious/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/AppMainProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)    80238 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/AppResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/AppSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/AppSettingsFn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/PySide6Legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/StartupOnBoot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/SystemProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/SystemRoutingTable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/SystemRuntime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.791924 Furious-GUI-0.4.2/Furious/Widget/
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/Application.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/ConnectProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9602 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/GuiHysteria1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/GuiHysteria2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/GuiShadowsocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/GuiTrojan.py
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/GuiVLESS.py
--rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/GuiVMess.py
--rw-r--r--   0 runner    (1001) docker     (127)    16043 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/GuiVTLS.py
--rw-r--r--   0 runner    (1001) docker     (127)    32650 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/GuiVTransport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/IndentSpinBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/SystemTrayIcon.py
--rw-r--r--   0 runner    (1001) docker     (127)    50683 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/UserServersQTableWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/UserSubsQTableWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/XrayAssetViewerQListWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.795924 Furious-GUI-0.4.2/Furious/Window/
--rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Window/AppMainWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Window/LogViewerWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Window/QRCodeWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14078 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Window/TextEditorWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Window/UserSubsWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Window/XrayAssetViewerWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/Window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/Furious/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:47:25.795924 Furious-GUI-0.4.2/Furious_GUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-11 12:47:25.000000 Furious-GUI-0.4.2/Furious_GUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-11 12:47:25.000000 Furious-GUI-0.4.2/Furious_GUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:47:25.000000 Furious-GUI-0.4.2/Furious_GUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-11 12:47:25.000000 Furious-GUI-0.4.2/Furious_GUI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-11 12:47:25.000000 Furious-GUI-0.4.2/Furious_GUI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-11 12:47:25.000000 Furious-GUI-0.4.2/Furious_GUI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-11 12:47:25.795924 Furious-GUI-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:47:25.795924 Furious-GUI-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-11 12:46:41.000000 Furious-GUI-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.688332 Furious-GUI-0.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.636331 Furious-GUI-0.4.3/Furious/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.636331 Furious-GUI-0.4.3/Furious/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Core/CoreManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Core/Hysteria1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Core/Hysteria2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Core/Tun2socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Core/XrayCore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.636331 Furious-GUI-0.4.3/Furious/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.636331 Furious-GUI-0.4.3/Furious/Data/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   624892 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Data/font/CascadiaMono
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Data/font/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.644331 Furious-GUI-0.4.3/Furious/Data/hysteria/
+-rw-r--r--   0 runner    (1001) docker     (127)  1974430 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Data/hysteria/bypass-Iran.acl
+-rw-r--r--   0 runner    (1001) docker     (127)  1390176 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Data/hysteria/bypass-mainland-China.acl
+-rw-r--r--   0 runner    (1001) docker     (127)  6444374 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Data/hysteria/country.mmdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.672332 Furious-GUI-0.4.3/Furious/Data/xray/
+-rw-r--r--   0 runner    (1001) docker     (127) 10715744 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Data/xray/geoip.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  6057957 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Data/xray/geosite.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  3199463 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Data/xray/iran.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.676332 Furious-GUI-0.4.3/Furious/Externals/
+-rw-r--r--   0 runner    (1001) docker     (127)    40204 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Externals/GenTranslation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Externals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.676332 Furious-GUI-0.4.3/Furious/Interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Interface/Application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Interface/ConfigurationFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Interface/CoreFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Interface/Encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Interface/GuiEditorItemFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Interface/ItemUpdateProtocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Interface/Storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Interface/UserServersTableItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.676332 Furious-GUI-0.4.3/Furious/Library/
+-rw-r--r--   0 runner    (1001) docker     (127)    55774 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Library/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Library/EmptyFactoryHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Library/Encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Library/Tcping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.676332 Furious-GUI-0.4.3/Furious/PyFramework/
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/PyFramework/Ancestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/PyFramework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.680332 Furious-GUI-0.4.3/Furious/QtFramework/
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/Ancestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/CoreProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/DNSResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/DynamicTheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/DynamicTranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/GuiEditorXXX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/NetworkStateManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/QtGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/QtNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16523 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/QtWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/TextEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/TextEditorTheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/UpdatesManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/QtFramework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.680332 Furious-GUI-0.4.3/Furious/Storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Storage/UserServers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Storage/UserSubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.680332 Furious-GUI-0.4.3/Furious/TrayActions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/TrayActions/Connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/TrayActions/EditConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/TrayActions/Exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/TrayActions/Import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/TrayActions/Language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/TrayActions/Routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/TrayActions/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/TrayActions/SystemProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/TrayActions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.684332 Furious-GUI-0.4.3/Furious/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/AppMainProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80238 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/AppResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/AppSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/AppSettingsFn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/PySide6Legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/StartupOnBoot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/SystemProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/SystemRoutingTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/SystemRuntime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.688332 Furious-GUI-0.4.3/Furious/Widget/
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/Application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/ConnectProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9602 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/GuiHysteria1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/GuiHysteria2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/GuiShadowsocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/GuiTrojan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/GuiVLESS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/GuiVMess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16043 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/GuiVTLS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32650 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/GuiVTransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/IndentSpinBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/SystemTrayIcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50812 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/UserServersQTableWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/UserSubsQTableWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/XrayAssetViewerQListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.688332 Furious-GUI-0.4.3/Furious/Window/
+-rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Window/AppMainWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Window/LogViewerWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Window/QRCodeWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14078 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Window/TextEditorWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Window/UserSubsWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Window/XrayAssetViewerWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/Window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/Furious/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:41:05.688332 Furious-GUI-0.4.3/Furious_GUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-13 10:41:05.000000 Furious-GUI-0.4.3/Furious_GUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-13 10:41:05.000000 Furious-GUI-0.4.3/Furious_GUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:41:05.000000 Furious-GUI-0.4.3/Furious_GUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 10:41:05.000000 Furious-GUI-0.4.3/Furious_GUI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-13 10:41:05.000000 Furious-GUI-0.4.3/Furious_GUI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 10:41:05.000000 Furious-GUI-0.4.3/Furious_GUI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-13 10:41:05.688332 Furious-GUI-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:41:05.688332 Furious-GUI-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-13 10:40:43.000000 Furious-GUI-0.4.3/setup.py
```

### Comparing `Furious-GUI-0.4.2/Furious/Core/CoreManager.py` & `Furious-GUI-0.4.3/Furious/Core/CoreManager.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Core/Hysteria1.py` & `Furious-GUI-0.4.3/Furious/Core/Hysteria1.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Core/Hysteria2.py` & `Furious-GUI-0.4.3/Furious/Core/Hysteria2.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Core/Tun2socks.py` & `Furious-GUI-0.4.3/Furious/Core/Tun2socks.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Core/XrayCore.py` & `Furious-GUI-0.4.3/Furious/Core/XrayCore.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Core/__init__.py` & `Furious-GUI-0.4.3/Furious/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Data/font/CascadiaMono` & `Furious-GUI-0.4.3/Furious/Data/font/CascadiaMono`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Data/font/LICENSE` & `Furious-GUI-0.4.3/Furious/Data/font/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Data/hysteria/bypass-Iran.acl` & `Furious-GUI-0.4.3/Furious/Data/hysteria/bypass-Iran.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Data/hysteria/bypass-mainland-China.acl` & `Furious-GUI-0.4.3/Furious/Data/hysteria/bypass-mainland-China.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Data/hysteria/country.mmdb` & `Furious-GUI-0.4.3/Furious/Data/hysteria/country.mmdb`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Data/xray/geoip.dat` & `Furious-GUI-0.4.3/Furious/Data/xray/geoip.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Data/xray/geosite.dat` & `Furious-GUI-0.4.3/Furious/Data/xray/geosite.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Data/xray/iran.dat` & `Furious-GUI-0.4.3/Furious/Data/xray/iran.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Externals/GenTranslation.py` & `Furious-GUI-0.4.3/Furious/Externals/GenTranslation.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Externals/__init__.py` & `Furious-GUI-0.4.3/Furious/Externals/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Interface/Application.py` & `Furious-GUI-0.4.3/Furious/Interface/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Interface/ConfigurationFactory.py` & `Furious-GUI-0.4.3/Furious/Interface/ConfigurationFactory.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Interface/CoreFactory.py` & `Furious-GUI-0.4.3/Furious/Interface/CoreFactory.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Interface/Encoder.py` & `Furious-GUI-0.4.3/Furious/Interface/Encoder.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Interface/GuiEditorItemFactory.py` & `Furious-GUI-0.4.3/Furious/Interface/GuiEditorItemFactory.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Interface/ItemUpdateProtocol.py` & `Furious-GUI-0.4.3/Furious/Interface/ItemUpdateProtocol.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Interface/Storage.py` & `Furious-GUI-0.4.3/Furious/Interface/Storage.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Interface/UserServersTableItem.py` & `Furious-GUI-0.4.3/Furious/Interface/UserServersTableItem.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Interface/__init__.py` & `Furious-GUI-0.4.3/Furious/Interface/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Library/Configuration.py` & `Furious-GUI-0.4.3/Furious/Library/Configuration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Library/EmptyFactoryHelper.py` & `Furious-GUI-0.4.3/Furious/Library/EmptyFactoryHelper.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Library/Encoder.py` & `Furious-GUI-0.4.3/Furious/Library/Encoder.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Library/Tcping.py` & `Furious-GUI-0.4.3/Furious/Library/Tcping.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Library/__init__.py` & `Furious-GUI-0.4.3/Furious/Library/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/PyFramework/Ancestors.py` & `Furious-GUI-0.4.3/Furious/PyFramework/Ancestors.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/PyFramework/__init__.py` & `Furious-GUI-0.4.3/Furious/PyFramework/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/Ancestors.py` & `Furious-GUI-0.4.3/Furious/QtFramework/Ancestors.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/CoreProcess.py` & `Furious-GUI-0.4.3/Furious/QtFramework/CoreProcess.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/DNSResolver.py` & `Furious-GUI-0.4.3/Furious/QtFramework/DNSResolver.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/DynamicTheme.py` & `Furious-GUI-0.4.3/Furious/QtFramework/DynamicTheme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/DynamicTranslate.py` & `Furious-GUI-0.4.3/Furious/QtFramework/DynamicTranslate.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/GuiEditorXXX.py` & `Furious-GUI-0.4.3/Furious/QtFramework/GuiEditorXXX.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,14 +354,18 @@
 
     def groupBoxSequence(self) -> Sequence[GuiEditorWidgetQGroupBox]:
         raise NotImplementedError
 
     def setTabText(self, text: str):
         self.tabWidget.setTabText(0, text)
 
+    def closeEvent(self, event):
+        self.accepted.disconnect()
+        self.rejected.disconnect()
+
     def inputToFactory(self, config: ConfigurationFactory) -> bool:
         modified = False
 
         for groupBox in self.groupBoxes:
             modified |= groupBox.inputToFactory(config)
 
         return modified
```

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/NetworkStateManager.py` & `Furious-GUI-0.4.3/Furious/QtFramework/NetworkStateManager.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/QtGui.py` & `Furious-GUI-0.4.3/Furious/QtFramework/QtGui.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/QtNetwork.py` & `Furious-GUI-0.4.3/Furious/QtFramework/QtNetwork.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/QtWidgets.py` & `Furious-GUI-0.4.3/Furious/QtFramework/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/TextEditor.py` & `Furious-GUI-0.4.3/Furious/QtFramework/TextEditor.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/TextEditorTheme.py` & `Furious-GUI-0.4.3/Furious/QtFramework/TextEditorTheme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/UpdatesManager.py` & `Furious-GUI-0.4.3/Furious/QtFramework/UpdatesManager.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/QtFramework/__init__.py` & `Furious-GUI-0.4.3/Furious/QtFramework/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Storage/UserServers.py` & `Furious-GUI-0.4.3/Furious/Storage/UserServers.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Storage/UserSubs.py` & `Furious-GUI-0.4.3/Furious/Storage/UserSubs.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Storage/__init__.py` & `Furious-GUI-0.4.3/Furious/Storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/TrayActions/Connect.py` & `Furious-GUI-0.4.3/Furious/TrayActions/Connect.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/TrayActions/EditConfiguration.py` & `Furious-GUI-0.4.3/Furious/TrayActions/EditConfiguration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/TrayActions/Exit.py` & `Furious-GUI-0.4.3/Furious/TrayActions/Exit.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/TrayActions/Import.py` & `Furious-GUI-0.4.3/Furious/TrayActions/Import.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/TrayActions/Language.py` & `Furious-GUI-0.4.3/Furious/TrayActions/Language.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/TrayActions/Routing.py` & `Furious-GUI-0.4.3/Furious/TrayActions/Routing.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/TrayActions/Settings.py` & `Furious-GUI-0.4.3/Furious/TrayActions/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/TrayActions/SystemProxy.py` & `Furious-GUI-0.4.3/Furious/TrayActions/SystemProxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/TrayActions/__init__.py` & `Furious-GUI-0.4.3/Furious/TrayActions/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/AppMainProcess.py` & `Furious-GUI-0.4.3/Furious/Utility/AppMainProcess.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/AppResources.py` & `Furious-GUI-0.4.3/Furious/Utility/AppResources.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/AppSettings.py` & `Furious-GUI-0.4.3/Furious/Utility/AppSettings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/AppSettingsFn.py` & `Furious-GUI-0.4.3/Furious/Utility/AppSettingsFn.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/Constants.py` & `Furious-GUI-0.4.3/Furious/Utility/Constants.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/PySide6Legacy.py` & `Furious-GUI-0.4.3/Furious/Utility/PySide6Legacy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/StartupOnBoot.py` & `Furious-GUI-0.4.3/Furious/Utility/StartupOnBoot.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/SystemProxy.py` & `Furious-GUI-0.4.3/Furious/Utility/SystemProxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/SystemRoutingTable.py` & `Furious-GUI-0.4.3/Furious/Utility/SystemRoutingTable.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/SystemRuntime.py` & `Furious-GUI-0.4.3/Furious/Utility/SystemRuntime.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/Utility.py` & `Furious-GUI-0.4.3/Furious/Utility/Utility.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Utility/__init__.py` & `Furious-GUI-0.4.3/Furious/Utility/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Version.py` & `Furious-GUI-0.4.3/Furious/Version.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '0.4.2'
+__version__ = '0.4.3'
```

### Comparing `Furious-GUI-0.4.2/Furious/Widget/Application.py` & `Furious-GUI-0.4.3/Furious/Widget/Application.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,14 +221,17 @@
                     lambda record: self.logViewerWindowApp_.appendLine(record)
                 ),
                 logging.StreamHandler(),
             ),
         )
         logging.raiseExceptions = False
 
+    def log(self):
+        return self.logViewerWindowApp_.plainText()
+
     def addCustomFont(self):
         fontFile = str(DATA_DIR / 'font' / 'CascadiaMono')
         fontName = 'Cascadia Mono'
 
         if QFontDatabase.addApplicationFont(fontFile) != -1:
             # Delayed
             self.customFontLoadMsg = f'custom font {fontName} load success'
```

### Comparing `Furious-GUI-0.4.2/Furious/Widget/ConnectProgressBar.py` & `Furious-GUI-0.4.3/Furious/Widget/ConnectProgressBar.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/GuiHysteria1.py` & `Furious-GUI-0.4.3/Furious/Widget/GuiHysteria1.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/GuiHysteria2.py` & `Furious-GUI-0.4.3/Furious/Widget/GuiHysteria2.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/GuiShadowsocks.py` & `Furious-GUI-0.4.3/Furious/Widget/GuiShadowsocks.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/GuiTrojan.py` & `Furious-GUI-0.4.3/Furious/Widget/GuiTrojan.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/GuiVLESS.py` & `Furious-GUI-0.4.3/Furious/Widget/GuiVLESS.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/GuiVMess.py` & `Furious-GUI-0.4.3/Furious/Widget/GuiVMess.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/GuiVTLS.py` & `Furious-GUI-0.4.3/Furious/Widget/GuiVTLS.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/GuiVTransport.py` & `Furious-GUI-0.4.3/Furious/Widget/GuiVTransport.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/IndentSpinBox.py` & `Furious-GUI-0.4.3/Furious/Widget/IndentSpinBox.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/SystemTrayIcon.py` & `Furious-GUI-0.4.3/Furious/Widget/SystemTrayIcon.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/UserServersQTableWidget.py` & `Furious-GUI-0.4.3/Furious/Widget/UserServersQTableWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
 from typing import Callable, Union, Sequence, MutableSequence
 
 import queue
 import logging
 import icmplib
 import functools
-import threading
 
 __all__ = ['UserServersQTableWidget']
 
 logger = logging.getLogger(__name__)
 
 registerAppSettings('ActivatedItemIndex')
 registerAppSettings('ServerWidgetSectionSizeTable')
@@ -809,16 +808,14 @@
         self.addActions(self.contextMenu.actions())
         self.setContextMenuPolicy(QtCore.Qt.ContextMenuPolicy.CustomContextMenu)
         self.customContextMenuRequested.connect(self.handleCustomContextMenuRequested)
 
         # Distinguish double-click and activated
         self.doubleClickedFlag = False
 
-        self.guiEditorMutex = threading.Lock()
-
         # Signals
         self.itemChanged.connect(self.handleItemChanged)
         self.itemSelectionChanged.connect(self.handleItemSelectionChanged)
         self.itemActivated.connect(self.handleItemActivated)
         self.itemDoubleClicked.connect(self.handleItemDoubleClicked)
 
         if self.activatedItem() is not None:
@@ -914,75 +911,81 @@
         else:
             guiEditor = None
 
         return guiEditor
 
     @QtCore.Slot(QTableWidgetItem)
     def handleItemDoubleClicked(self, item: QTableWidgetItem):
-        with self.guiEditorMutex:
-            self.doubleClickedFlag = True
-
-            index = item.row()
-            factory = AS_UserServers()[index]
+        self.doubleClickedFlag = True
 
-            guiEditor = self.getGuiEditorByFactory(factory, translatable=False)
+        index = item.row()
+        factory = AS_UserServers()[index]
 
-            if guiEditor is None:
-                # Unrecognized. Do nothing
-                return
+        guiEditor = self.getGuiEditorByFactory(factory, translatable=False)
 
-            # Dummy ref
-            setattr(self, '_guiEditorRef0', guiEditor)
+        if guiEditor is None:
+            # Unrecognized. Do nothing
+            return
 
-            guiEditor.setWindowTitle(f'{index + 1} - ' + factory.getExtras('remark'))
+        guiEditor.setWindowTitle(f'{index + 1} - ' + factory.getExtras('remark'))
 
-            try:
-                guiEditor.factoryToInput(factory)
-            except Exception as ex:
-                # Any non-exit exceptions
+        try:
+            guiEditor.factoryToInput(factory)
+        except Exception as ex:
+            # Any non-exit exceptions
 
-                logger.error(f'error while converting factory to input: {ex}')
+            logger.error(f'error while converting factory to input: {ex}')
 
-            guiEditor.accepted.connect(
-                functools.partial(
-                    self.handleGuiEditorAccepted,
-                    guiEditor,
-                    index,
-                    factory,
-                )
+        guiEditor.accepted.connect(
+            functools.partial(
+                self.handleGuiEditorAccepted,
+                guiEditor,
+                index,
+                factory,
+            )
+        )
+        guiEditor.rejected.connect(
+            functools.partial(
+                self.handleGuiEditorRejected,
+                guiEditor,
             )
-            guiEditor.open()
+        )
+        guiEditor.open()
 
     def handleGuiEditorAccepted(
         self,
         editor: GuiEditorWidgetQDialog,
         index: int,
         factory: ConfigurationFactory,
     ):
-        with self.guiEditorMutex:
-            logger.debug(f'guiEditor accepted with index {index}')
+        logger.debug(f'guiEditor accepted with index {index}')
 
-            modified = editor.inputToFactory(factory)
+        modified = editor.inputToFactory(factory)
 
-            # Still flush to row since remark may be modified
-            self.flushRow(index, factory)
+        # Still flush to row since remark may be modified
+        self.flushRow(index, factory)
 
-            if modified and index == AS_UserActivatedItemIndex():
-                try:
-                    if APP().isSystemTrayConnected():
-                        mbox = NewChangesNextTimeMBox()
+        if modified and index == AS_UserActivatedItemIndex():
+            try:
+                if APP().isSystemTrayConnected():
+                    mbox = NewChangesNextTimeMBox()
 
-                        # Show the MessageBox asynchronously
-                        mbox.open()
-                except Exception:
-                    # Any non-exit exceptions
+                    # Show the MessageBox asynchronously
+                    mbox.open()
+            except Exception:
+                # Any non-exit exceptions
 
-                    pass
+                pass
 
-            editor.accepted.disconnect()
+        editor.accepted.disconnect()
+        editor.rejected.disconnect()
+
+    def handleGuiEditorRejected(self, editor: GuiEditorWidgetQDialog):
+        editor.accepted.disconnect()
+        editor.rejected.disconnect()
 
     @QtCore.Slot(QtCore.QPoint)
     def handleCustomContextMenuRequested(self, point):
         self.contextMenu.exec(self.mapToGlobal(point))
 
     def customSortFn(self, clickedIndex, **kwargs):
         def keyFn(server):
@@ -1075,55 +1078,61 @@
 
     def addServerViaGui(
         self,
         protocol: str,
         windowTitle: str = APPLICATION_NAME,
         **kwargs,
     ):
-        with self.guiEditorMutex:
-            factory = getEmptyFactory(protocol)
-
-            guiEditor = self.getGuiEditorByFactory(factory, **kwargs)
+        factory = getEmptyFactory(protocol)
 
-            if guiEditor is None:
-                # Unrecognized. Do nothing
-                return
+        guiEditor = self.getGuiEditorByFactory(factory, **kwargs)
 
-            # Dummy ref
-            setattr(self, '_guiEditorRef1', guiEditor)
+        if guiEditor is None:
+            # Unrecognized. Do nothing
+            return
 
-            guiEditor.setWindowTitle(windowTitle)
+        guiEditor.setWindowTitle(windowTitle)
 
-            try:
-                guiEditor.factoryToInput(factory)
-            except Exception as ex:
-                # Any non-exit exceptions
+        try:
+            guiEditor.factoryToInput(factory)
+        except Exception as ex:
+            # Any non-exit exceptions
 
-                logger.error(f'error while converting factory to input: {ex}')
+            logger.error(f'error while converting factory to input: {ex}')
 
-            guiEditor.accepted.connect(
-                functools.partial(
-                    self.handleAddServerViaGui,
-                    guiEditor,
-                    factory,
-                )
+        guiEditor.accepted.connect(
+            functools.partial(
+                self.handleAddServerViaGuiAccepted,
+                guiEditor,
+                factory,
             )
-            guiEditor.open()
+        )
+        guiEditor.rejected.connect(
+            functools.partial(
+                self.handleAddServerViaGuiRejected,
+                guiEditor,
+            )
+        )
+        guiEditor.open()
 
-    def handleAddServerViaGui(
+    def handleAddServerViaGuiAccepted(
         self,
         editor: GuiEditorWidgetQDialog,
         factory: ConfigurationFactory,
     ):
-        with self.guiEditorMutex:
-            editor.inputToFactory(factory)
+        editor.inputToFactory(factory)
+
+        self.appendNewItemByFactory(factory)
 
-            self.appendNewItemByFactory(factory)
+        editor.accepted.disconnect()
+        editor.rejected.disconnect()
 
-            editor.accepted.disconnect()
+    def handleAddServerViaGuiRejected(self, editor: GuiEditorWidgetQDialog):
+        editor.accepted.disconnect()
+        editor.rejected.disconnect()
 
     def flushRow(self, row: int, item: ConfigurationFactory):
         for column in list(range(self.columnCount())):
             self.flushItem(row, column, item)
 
     def flushAll(self):
         if self.rowCount() == 0:
```

### Comparing `Furious-GUI-0.4.2/Furious/Widget/UserSubsQTableWidget.py` & `Furious-GUI-0.4.3/Furious/Widget/UserSubsQTableWidget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/XrayAssetViewerQListWidget.py` & `Furious-GUI-0.4.3/Furious/Widget/XrayAssetViewerQListWidget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Widget/__init__.py` & `Furious-GUI-0.4.3/Furious/Widget/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Window/AppMainWindow.py` & `Furious-GUI-0.4.3/Furious/Window/AppMainWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Window/LogViewerWindow.py` & `Furious-GUI-0.4.3/Furious/Window/LogViewerWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+from __future__ import annotations
+
 from Furious.QtFramework import *
 from Furious.QtFramework import gettext as _
 
 from PySide6 import QtCore
 from PySide6.QtWidgets import *
 
 import functools
@@ -172,12 +174,15 @@
             parent=self,
         )
 
         self.menuBar().addMenu(self._fileMenu)
         self.menuBar().addMenu(self._editMenu)
         self.menuBar().addMenu(self._viewMenu)
 
+    def plainText(self) -> str:
+        return self.textBrowser.toPlainText()
+
     def appendLine(self, line: str):
         self.textBrowser.appendLine(line)
 
     def clear(self):
         self.textBrowser.clear()
```

### Comparing `Furious-GUI-0.4.2/Furious/Window/QRCodeWindow.py` & `Furious-GUI-0.4.3/Furious/Window/QRCodeWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Window/TextEditorWindow.py` & `Furious-GUI-0.4.3/Furious/Window/TextEditorWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Window/UserSubsWindow.py` & `Furious-GUI-0.4.3/Furious/Window/UserSubsWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Window/XrayAssetViewerWindow.py` & `Furious-GUI-0.4.3/Furious/Window/XrayAssetViewerWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/Window/__init__.py` & `Furious-GUI-0.4.3/Furious/Window/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/__init__.py` & `Furious-GUI-0.4.3/Furious/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious/__main__.py` & `Furious-GUI-0.4.3/Furious/__main__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious_GUI.egg-info/PKG-INFO` & `Furious-GUI-0.4.3/Furious_GUI.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.4.2
+Version: 0.4.3
 Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Furious-GUI-0.4.2/Furious_GUI.egg-info/SOURCES.txt` & `Furious-GUI-0.4.3/Furious_GUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/Furious_GUI.egg-info/requires.txt` & `Furious-GUI-0.4.3/Furious_GUI.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/LICENSE` & `Furious-GUI-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/PKG-INFO` & `Furious-GUI-0.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.4.2
+Version: 0.4.3
 Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Furious-GUI-0.4.2/README.md` & `Furious-GUI-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.2/setup.py` & `Furious-GUI-0.4.3/setup.py`

 * *Files identical despite different names*

