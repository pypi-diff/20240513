# Comparing `tmp/fbs-1.2.1.tar.gz` & `tmp/fbs-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbs-1.2.1.tar", last modified: Tue Apr  4 10:02:34 2023, max compression
+gzip compressed data, was "fbs-1.2.2.tar", last modified: Mon May 13 05:53:02 2024, max compression
```

## Comparing `fbs-1.2.1.tar` & `fbs-1.2.2.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/
--rw-r--r--   0 michael   (1000) michael   (1000)     1137 2023-04-04 10:02:34.376550 fbs-1.2.1/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      174 2021-04-08 14:16:17.000000 fbs-1.2.1/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/
--rw-r--r--   0 michael   (1000) michael   (1000)     2394 2022-11-29 05:33:21.000000 fbs-1.2.1/fbs/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1706 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1053 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_aws.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/_defaults/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/_defaults/requirements/
--rw-r--r--   0 michael   (1000) michael   (1000)      135 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/requirements/arch.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-04-04 10:01:23.000000 fbs-1.2.1/fbs/_defaults/requirements/base.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/requirements/fedora.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       11 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/requirements/linux.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/requirements/ubuntu.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/_defaults/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/_defaults/src/build/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/_defaults/src/build/docker/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/_defaults/src/build/docker/arch/
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2021-07-29 07:58:53.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/arch/.bashrc
--rw-r--r--   0 michael   (1000) michael   (1000)     1645 2021-07-29 11:27:59.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/arch/Dockerfile
--rw-r--r--   0 michael   (1000) michael   (1000)      103 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/arch/gpg-agent.conf
--rw-r--r--   0 michael   (1000) michael   (1000)      388 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/arch/motd
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/_defaults/src/build/docker/fedora/
--rw-r--r--   0 michael   (1000) michael   (1000)       95 2021-07-29 07:58:53.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/fedora/.bashrc
--rw-r--r--   0 michael   (1000) michael   (1000)       84 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/fedora/.rpmmacros
--rw-r--r--   0 michael   (1000) michael   (1000)     1845 2022-11-29 05:33:33.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/fedora/Dockerfile
--rw-r--r--   0 michael   (1000) michael   (1000)      103 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/fedora/gpg-agent.conf
--rw-r--r--   0 michael   (1000) michael   (1000)      392 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/fedora/motd
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/_defaults/src/build/docker/ubuntu/
--rw-r--r--   0 michael   (1000) michael   (1000)       95 2021-07-27 07:23:25.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/ubuntu/.bashrc
--rw-r--r--   0 michael   (1000) michael   (1000)     1753 2023-04-04 06:48:37.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/ubuntu/Dockerfile
--rw-r--r--   0 michael   (1000) michael   (1000)      103 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/ubuntu/gpg-agent.conf
--rw-r--r--   0 michael   (1000) michael   (1000)      362 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/ubuntu/gpg.conf
--rw-r--r--   0 michael   (1000) michael   (1000)      392 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/docker/ubuntu/motd
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/_defaults/src/build/settings/
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/settings/arch.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1209 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/settings/base.json
--rw-r--r--   0 michael   (1000) michael   (1000)      279 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/settings/fedora.json
--rw-r--r--   0 michael   (1000) michael   (1000)      291 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/settings/linux.json
--rw-r--r--   0 michael   (1000) michael   (1000)      226 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/settings/mac.json
--rw-r--r--   0 michael   (1000) michael   (1000)       56 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/settings/release.json
--rw-r--r--   0 michael   (1000) michael   (1000)      134 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/settings/ubuntu.json
--rw-r--r--   0 michael   (1000) michael   (1000)      216 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/build/settings/windows.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/_defaults/src/freeze/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/_defaults/src/freeze/mac/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/_defaults/src/freeze/mac/Contents/
--rw-r--r--   0 michael   (1000) michael   (1000)      969 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/freeze/mac/Contents/Info.plist
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/_defaults/src/freeze/windows/
--rw-r--r--   0 michael   (1000) michael   (1000)     1781 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/freeze/windows/version_info.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/_defaults/src/installer/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/_defaults/src/installer/linux/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/_defaults/src/installer/linux/usr/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/_defaults/src/installer/linux/usr/share/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/_defaults/src/installer/linux/usr/share/applications/
--rw-r--r--   0 michael   (1000) michael   (1000)      168 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/installer/linux/usr/share/applications/AppName.desktop
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/_defaults/src/installer/windows/
--rw-r--r--   0 michael   (1000) michael   (1000)     3398 2021-10-08 06:32:42.000000 fbs-1.2.1/fbs/_defaults/src/installer/windows/Installer.nsi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/_defaults/src/repo/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/_defaults/src/repo/fedora/
--rw-r--r--   0 michael   (1000) michael   (1000)       92 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/repo/fedora/AppName.repo
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/_defaults/src/repo/ubuntu/
--rw-r--r--   0 michael   (1000) michael   (1000)      143 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_defaults/src/repo/ubuntu/distributions
--rw-r--r--   0 michael   (1000) michael   (1000)     2070 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_gpg.py
--rw-r--r--   0 michael   (1000) michael   (1000)      764 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_server.py
--rw-r--r--   0 michael   (1000) michael   (1000)      578 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/_state.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/builtin_commands/
--rw-r--r--   0 michael   (1000) michael   (1000)    19413 2021-08-31 07:09:39.000000 fbs-1.2.1/fbs/builtin_commands/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1268 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/_account.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3572 2021-07-29 07:30:24.000000 fbs-1.2.1/fbs/builtin_commands/_docker.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/builtin_commands/_gpg/
--rw-r--r--   0 michael   (1000) michael   (1000)      280 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/_gpg/Dockerfile
--rw-r--r--   0 michael   (1000) michael   (1000)     2890 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/_gpg/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      425 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/_gpg/genkey.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      143 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/_gpg/gpg-agent.conf
--rw-r--r--   0 michael   (1000) michael   (1000)     2191 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/_licensing.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2682 2021-08-02 09:12:09.000000 fbs-1.2.1/fbs/builtin_commands/_util.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/builtin_commands/project_template/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/builtin_commands/project_template/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/builtin_commands/project_template/src/build/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/builtin_commands/project_template/src/build/settings/
--rw-r--r--   0 michael   (1000) michael   (1000)      130 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/build/settings/base.json
--rw-r--r--   0 michael   (1000) michael   (1000)       94 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/build/settings/linux.json
--rw-r--r--   0 michael   (1000) michael   (1000)       59 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/build/settings/mac.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.368550 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/
--rw-r--r--   0 michael   (1000) michael   (1000)   168229 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/Icon.ico
--rw-r--r--   0 michael   (1000) michael   (1000)      558 2022-05-20 05:24:02.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/base/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      544 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/base/16.png
--rwxr-xr-x   0 michael   (1000) michael   (1000)      783 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/base/24.png
--rwxr-xr-x   0 michael   (1000) michael   (1000)      912 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/base/32.png
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1497 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/base/48.png
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1657 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/base/64.png
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/linux/
--rwxr-xr-x   0 michael   (1000) michael   (1000)    26841 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/linux/1024.png
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3177 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/linux/128.png
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5641 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/linux/256.png
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11653 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/linux/512.png
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/mac/
--rw-r--r--   0 michael   (1000) michael   (1000)    47311 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/mac/1024.png
--rw-r--r--   0 michael   (1000) michael   (1000)     4978 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/mac/128.png
--rw-r--r--   0 michael   (1000) michael   (1000)    10278 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/mac/256.png
--rw-r--r--   0 michael   (1000) michael   (1000)    21699 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/mac/512.png
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/python/
--rw-r--r--   0 michael   (1000) michael   (1000)      421 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/builtin_commands/project_template/src/main/python/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3147 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/cmdline.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs/freeze/
--rw-r--r--   0 michael   (1000) michael   (1000)     3376 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/freeze/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)       96 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/freeze/arch.py
--rw-r--r--   0 michael   (1000) michael   (1000)      748 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/freeze/fedora.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs/freeze/hooks/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/freeze/hooks/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1243 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/freeze/hooks/hook-PySide2.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1088 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/freeze/hooks/hook-shiboken2.py
--rw-r--r--   0 michael   (1000) michael   (1000)      996 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/freeze/linux.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2281 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/freeze/mac.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/freeze/ubuntu.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3913 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/freeze/windows.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs/installer/
--rw-r--r--   0 michael   (1000) michael   (1000)      312 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      341 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/arch.py
--rw-r--r--   0 michael   (1000) michael   (1000)      147 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/fedora.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3198 2022-05-20 05:24:02.000000 fbs-1.2.1/fbs/installer/linux.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs/installer/mac/
--rw-r--r--   0 michael   (1000) michael   (1000)     1118 2021-07-01 07:28:01.000000 fbs-1.2.1/fbs/installer/mac/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs/installer/mac/create-dmg/
--rw-r--r--   0 michael   (1000) michael   (1000)     1088 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/mac/create-dmg/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     3488 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/mac/create-dmg/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs/installer/mac/create-dmg/builder/
--rw-r--r--   0 michael   (1000) michael   (1000)      516 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/mac/create-dmg/builder/create-dmg.builder
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11681 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/mac/create-dmg/create-dmg
--rwxr-xr-x   0 michael   (1000) michael   (1000)      506 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/mac/create-dmg/sample
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs/installer/mac/create-dmg/support/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      697 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/mac/create-dmg/support/brew-me.sh
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6279 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/mac/create-dmg/support/dmg-license.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1828 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/mac/create-dmg/support/template.applescript
--rw-r--r--   0 michael   (1000) michael   (1000)      147 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/ubuntu.py
--rw-r--r--   0 michael   (1000) michael   (1000)      571 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/installer/windows.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs/repo/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/repo/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1071 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/repo/arch.py
--rw-r--r--   0 michael   (1000) michael   (1000)      962 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/repo/fedora.py
--rw-r--r--   0 michael   (1000) michael   (1000)      915 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/repo/ubuntu.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4523 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/resources.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs/sign/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/sign/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3916 2022-05-20 05:24:02.000000 fbs-1.2.1/fbs/sign/windows.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs/sign_installer/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/sign_installer/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      461 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/sign_installer/arch.py
--rw-r--r--   0 michael   (1000) michael   (1000)      329 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/sign_installer/fedora.py
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/sign_installer/windows.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1658 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs/upload.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.372550 fbs-1.2.1/fbs.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1137 2023-04-04 10:02:34.000000 fbs-1.2.1/fbs.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     4867 2023-04-04 10:02:34.000000 fbs-1.2.1/fbs.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-04 10:02:34.000000 fbs-1.2.1/fbs.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       44 2023-04-04 10:02:34.000000 fbs-1.2.1/fbs.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       85 2023-04-04 10:02:34.000000 fbs-1.2.1/fbs.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       16 2023-04-04 10:02:34.000000 fbs-1.2.1/fbs.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs_runtime/
--rw-r--r--   0 michael   (1000) michael   (1000)       35 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      934 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/_fbs.py
--rw-r--r--   0 michael   (1000) michael   (1000)      537 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/_frozen.py
--rw-r--r--   0 michael   (1000) michael   (1000)      500 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/_resources.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1854 2021-09-30 14:55:20.000000 fbs-1.2.1/fbs_runtime/_settings.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2633 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/_signal.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1924 2022-05-20 05:24:02.000000 fbs-1.2.1/fbs_runtime/_source.py
--rw-r--r--   0 michael   (1000) michael   (1000)      640 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/_state.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs_runtime/application_context/
--rw-r--r--   0 michael   (1000) michael   (1000)     1226 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/application_context/PyQt5.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1232 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/application_context/PySide2.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5794 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/application_context/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 10:02:34.376550 fbs-1.2.1/fbs_runtime/excepthook/
--rw-r--r--   0 michael   (1000) michael   (1000)     5234 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/excepthook/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      596 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/excepthook/_util.py
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2022-09-14 07:25:54.000000 fbs-1.2.1/fbs_runtime/excepthook/sentry.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3127 2021-04-08 14:16:17.000000 fbs-1.2.1/fbs_runtime/licensing.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2458 2022-05-20 05:24:02.000000 fbs-1.2.1/fbs_runtime/platform.py
--rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-04-04 10:02:34.376550 fbs-1.2.1/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2429 2023-04-04 10:01:23.000000 fbs-1.2.1/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.581895 fbs-1.2.2/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1137 2024-05-13 05:53:02.581895 fbs-1.2.2/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      174 2021-04-08 14:16:17.000000 fbs-1.2.2/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2394 2022-11-29 05:33:21.000000 fbs-1.2.2/fbs/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1706 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1053 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_aws.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.561894 fbs-1.2.2/fbs/_defaults/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/_defaults/requirements/
+-rw-r--r--   0 michael   (1000) michael   (1000)      135 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/requirements/arch.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       10 2024-05-13 05:51:55.000000 fbs-1.2.2/fbs/_defaults/requirements/base.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/requirements/fedora.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       11 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/requirements/linux.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/requirements/ubuntu.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/_defaults/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.561894 fbs-1.2.2/fbs/_defaults/src/build/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.561894 fbs-1.2.2/fbs/_defaults/src/build/docker/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/_defaults/src/build/docker/arch/
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2021-07-29 07:58:53.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/arch/.bashrc
+-rw-r--r--   0 michael   (1000) michael   (1000)     1645 2021-07-29 11:27:59.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/arch/Dockerfile
+-rw-r--r--   0 michael   (1000) michael   (1000)      103 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/arch/gpg-agent.conf
+-rw-r--r--   0 michael   (1000) michael   (1000)      388 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/arch/motd
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/_defaults/src/build/docker/fedora/
+-rw-r--r--   0 michael   (1000) michael   (1000)       95 2021-07-29 07:58:53.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/fedora/.bashrc
+-rw-r--r--   0 michael   (1000) michael   (1000)       84 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/fedora/.rpmmacros
+-rw-r--r--   0 michael   (1000) michael   (1000)     1845 2022-11-29 05:33:33.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/fedora/Dockerfile
+-rw-r--r--   0 michael   (1000) michael   (1000)      103 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/fedora/gpg-agent.conf
+-rw-r--r--   0 michael   (1000) michael   (1000)      392 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/fedora/motd
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/_defaults/src/build/docker/ubuntu/
+-rw-r--r--   0 michael   (1000) michael   (1000)       95 2021-07-27 07:23:25.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/ubuntu/.bashrc
+-rw-r--r--   0 michael   (1000) michael   (1000)     1753 2023-04-04 06:48:37.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/ubuntu/Dockerfile
+-rw-r--r--   0 michael   (1000) michael   (1000)      103 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/ubuntu/gpg-agent.conf
+-rw-r--r--   0 michael   (1000) michael   (1000)      362 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/ubuntu/gpg.conf
+-rw-r--r--   0 michael   (1000) michael   (1000)      392 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/docker/ubuntu/motd
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/_defaults/src/build/settings/
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/settings/arch.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1209 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/settings/base.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      279 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/settings/fedora.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      291 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/settings/linux.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      226 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/settings/mac.json
+-rw-r--r--   0 michael   (1000) michael   (1000)       56 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/settings/release.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      134 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/settings/ubuntu.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      216 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/build/settings/windows.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/_defaults/src/freeze/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/_defaults/src/freeze/mac/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/_defaults/src/freeze/mac/Contents/
+-rw-r--r--   0 michael   (1000) michael   (1000)      969 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/freeze/mac/Contents/Info.plist
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/_defaults/src/freeze/windows/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1781 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/freeze/windows/version_info.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/_defaults/src/installer/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/_defaults/src/installer/linux/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/_defaults/src/installer/linux/usr/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/_defaults/src/installer/linux/usr/share/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/_defaults/src/installer/linux/usr/share/applications/
+-rw-r--r--   0 michael   (1000) michael   (1000)      168 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/installer/linux/usr/share/applications/AppName.desktop
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/_defaults/src/installer/windows/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3398 2021-10-08 06:32:42.000000 fbs-1.2.2/fbs/_defaults/src/installer/windows/Installer.nsi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/_defaults/src/repo/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/_defaults/src/repo/fedora/
+-rw-r--r--   0 michael   (1000) michael   (1000)       92 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/repo/fedora/AppName.repo
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/_defaults/src/repo/ubuntu/
+-rw-r--r--   0 michael   (1000) michael   (1000)      143 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_defaults/src/repo/ubuntu/distributions
+-rw-r--r--   0 michael   (1000) michael   (1000)     2070 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_gpg.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      764 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_server.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      578 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/_state.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/builtin_commands/
+-rw-r--r--   0 michael   (1000) michael   (1000)    19413 2021-08-31 07:09:39.000000 fbs-1.2.2/fbs/builtin_commands/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1268 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/_account.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3572 2021-07-29 07:30:24.000000 fbs-1.2.2/fbs/builtin_commands/_docker.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/builtin_commands/_gpg/
+-rw-r--r--   0 michael   (1000) michael   (1000)      280 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/_gpg/Dockerfile
+-rw-r--r--   0 michael   (1000) michael   (1000)     2890 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/_gpg/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      425 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/_gpg/genkey.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      143 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/_gpg/gpg-agent.conf
+-rw-r--r--   0 michael   (1000) michael   (1000)     2191 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/_licensing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2682 2021-08-02 09:12:09.000000 fbs-1.2.2/fbs/builtin_commands/_util.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/builtin_commands/project_template/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/builtin_commands/project_template/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/builtin_commands/project_template/src/build/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.569894 fbs-1.2.2/fbs/builtin_commands/project_template/src/build/settings/
+-rw-r--r--   0 michael   (1000) michael   (1000)      130 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/build/settings/base.json
+-rw-r--r--   0 michael   (1000) michael   (1000)       94 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/build/settings/linux.json
+-rw-r--r--   0 michael   (1000) michael   (1000)       59 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/build/settings/mac.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.573895 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/
+-rw-r--r--   0 michael   (1000) michael   (1000)   168229 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/Icon.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)      558 2022-05-20 05:24:02.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.573895 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/base/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      544 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/base/16.png
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      783 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/base/24.png
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      912 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/base/32.png
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1497 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/base/48.png
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1657 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/base/64.png
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.573895 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/linux/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    26841 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/linux/1024.png
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3177 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/linux/128.png
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5641 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/linux/256.png
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11653 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/linux/512.png
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.573895 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/mac/
+-rw-r--r--   0 michael   (1000) michael   (1000)    47311 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/mac/1024.png
+-rw-r--r--   0 michael   (1000) michael   (1000)     4978 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/mac/128.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    10278 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/mac/256.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    21699 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/mac/512.png
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.573895 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/python/
+-rw-r--r--   0 michael   (1000) michael   (1000)      421 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/builtin_commands/project_template/src/main/python/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3147 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/cmdline.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.573895 fbs-1.2.2/fbs/freeze/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3376 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/freeze/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       96 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/freeze/arch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      748 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/freeze/fedora.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.573895 fbs-1.2.2/fbs/freeze/hooks/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/freeze/hooks/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1243 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/freeze/hooks/hook-PySide2.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1088 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/freeze/hooks/hook-shiboken2.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      996 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/freeze/linux.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2281 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/freeze/mac.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/freeze/ubuntu.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3913 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/freeze/windows.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.573895 fbs-1.2.2/fbs/installer/
+-rw-r--r--   0 michael   (1000) michael   (1000)      312 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      341 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/arch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      147 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/fedora.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3198 2022-05-20 05:24:02.000000 fbs-1.2.2/fbs/installer/linux.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.573895 fbs-1.2.2/fbs/installer/mac/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1118 2021-07-01 07:28:01.000000 fbs-1.2.2/fbs/installer/mac/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.577895 fbs-1.2.2/fbs/installer/mac/create-dmg/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1088 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/mac/create-dmg/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     3488 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/mac/create-dmg/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.577895 fbs-1.2.2/fbs/installer/mac/create-dmg/builder/
+-rw-r--r--   0 michael   (1000) michael   (1000)      516 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/mac/create-dmg/builder/create-dmg.builder
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11681 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/mac/create-dmg/create-dmg
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      506 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/mac/create-dmg/sample
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.577895 fbs-1.2.2/fbs/installer/mac/create-dmg/support/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      697 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/mac/create-dmg/support/brew-me.sh
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6279 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/mac/create-dmg/support/dmg-license.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1828 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/mac/create-dmg/support/template.applescript
+-rw-r--r--   0 michael   (1000) michael   (1000)      147 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/ubuntu.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      571 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/installer/windows.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.577895 fbs-1.2.2/fbs/repo/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/repo/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1071 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/repo/arch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      962 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/repo/fedora.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      915 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/repo/ubuntu.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4523 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/resources.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.577895 fbs-1.2.2/fbs/sign/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/sign/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3916 2022-05-20 05:24:02.000000 fbs-1.2.2/fbs/sign/windows.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.577895 fbs-1.2.2/fbs/sign_installer/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/sign_installer/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      461 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/sign_installer/arch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      329 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/sign_installer/fedora.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/sign_installer/windows.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1658 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs/upload.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.565894 fbs-1.2.2/fbs.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1137 2024-05-13 05:53:02.000000 fbs-1.2.2/fbs.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     4867 2024-05-13 05:53:02.000000 fbs-1.2.2/fbs.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-05-13 05:53:02.000000 fbs-1.2.2/fbs.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       44 2024-05-13 05:53:02.000000 fbs-1.2.2/fbs.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       85 2024-05-13 05:53:02.000000 fbs-1.2.2/fbs.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       16 2024-05-13 05:53:02.000000 fbs-1.2.2/fbs.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.581895 fbs-1.2.2/fbs_runtime/
+-rw-r--r--   0 michael   (1000) michael   (1000)       35 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      934 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/_fbs.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      537 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/_frozen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      500 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/_resources.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1854 2021-09-30 14:55:20.000000 fbs-1.2.2/fbs_runtime/_settings.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2633 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/_signal.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1924 2022-05-20 05:24:02.000000 fbs-1.2.2/fbs_runtime/_source.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      640 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/_state.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.581895 fbs-1.2.2/fbs_runtime/application_context/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1226 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/application_context/PyQt5.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1232 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/application_context/PySide2.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5794 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/application_context/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 05:53:02.581895 fbs-1.2.2/fbs_runtime/excepthook/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5234 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/excepthook/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      596 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/excepthook/_util.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2022-09-14 07:25:54.000000 fbs-1.2.2/fbs_runtime/excepthook/sentry.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3127 2021-04-08 14:16:17.000000 fbs-1.2.2/fbs_runtime/licensing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2458 2022-05-20 05:24:02.000000 fbs-1.2.2/fbs_runtime/platform.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       79 2024-05-13 05:53:02.581895 fbs-1.2.2/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2429 2024-05-13 05:52:03.000000 fbs-1.2.2/setup.py
```

### Comparing `fbs-1.2.1/PKG-INFO` & `fbs-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbs
-Version: 1.2.1
+Version: 1.2.2
 Summary: Create cross-platform desktop applications with Python and Qt
 Home-page: https://build-system.fman.io
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 License: GPLv3 or later
 Description: Create cross-platform desktop applications with Python and Qt
```

### Comparing `fbs-1.2.1/fbs/__init__.py` & `fbs-1.2.2/fbs/__init__.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/__main__.py` & `fbs-1.2.2/fbs/__main__.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/_aws.py` & `fbs-1.2.2/fbs/_aws.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/_defaults/src/build/docker/arch/Dockerfile` & `fbs-1.2.2/fbs/_defaults/src/build/docker/arch/Dockerfile`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/_defaults/src/build/docker/fedora/Dockerfile` & `fbs-1.2.2/fbs/_defaults/src/build/docker/fedora/Dockerfile`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/_defaults/src/build/docker/ubuntu/Dockerfile` & `fbs-1.2.2/fbs/_defaults/src/build/docker/ubuntu/Dockerfile`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/_defaults/src/build/settings/base.json` & `fbs-1.2.2/fbs/_defaults/src/build/settings/base.json`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/_defaults/src/freeze/mac/Contents/Info.plist` & `fbs-1.2.2/fbs/_defaults/src/freeze/mac/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/_defaults/src/freeze/windows/version_info.py` & `fbs-1.2.2/fbs/_defaults/src/freeze/windows/version_info.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/_defaults/src/installer/windows/Installer.nsi` & `fbs-1.2.2/fbs/_defaults/src/installer/windows/Installer.nsi`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/_gpg.py` & `fbs-1.2.2/fbs/_gpg.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/_server.py` & `fbs-1.2.2/fbs/_server.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/_state.py` & `fbs-1.2.2/fbs/_state.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/__init__.py` & `fbs-1.2.2/fbs/builtin_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/_account.py` & `fbs-1.2.2/fbs/builtin_commands/_account.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/_docker.py` & `fbs-1.2.2/fbs/builtin_commands/_docker.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/_gpg/__init__.py` & `fbs-1.2.2/fbs/builtin_commands/_gpg/__init__.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/_licensing.py` & `fbs-1.2.2/fbs/builtin_commands/_licensing.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/_util.py` & `fbs-1.2.2/fbs/builtin_commands/_util.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/Icon.ico` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/Icon.ico`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/README.md` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/README.md`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/base/16.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/base/16.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/base/24.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/base/24.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/base/32.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/base/32.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/base/48.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/base/48.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/base/64.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/base/64.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/linux/1024.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/linux/1024.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/linux/128.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/linux/128.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/linux/256.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/linux/256.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/linux/512.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/linux/512.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/mac/1024.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/mac/1024.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/mac/128.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/mac/128.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/mac/256.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/mac/256.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/builtin_commands/project_template/src/main/icons/mac/512.png` & `fbs-1.2.2/fbs/builtin_commands/project_template/src/main/icons/mac/512.png`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/cmdline.py` & `fbs-1.2.2/fbs/cmdline.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/freeze/__init__.py` & `fbs-1.2.2/fbs/freeze/__init__.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/freeze/fedora.py` & `fbs-1.2.2/fbs/freeze/fedora.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/freeze/hooks/hook-PySide2.py` & `fbs-1.2.2/fbs/freeze/hooks/hook-PySide2.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/freeze/hooks/hook-shiboken2.py` & `fbs-1.2.2/fbs/freeze/hooks/hook-shiboken2.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/freeze/linux.py` & `fbs-1.2.2/fbs/freeze/linux.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/freeze/mac.py` & `fbs-1.2.2/fbs/freeze/mac.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/freeze/ubuntu.py` & `fbs-1.2.2/fbs/freeze/ubuntu.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/freeze/windows.py` & `fbs-1.2.2/fbs/freeze/windows.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/installer/linux.py` & `fbs-1.2.2/fbs/installer/linux.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/installer/mac/__init__.py` & `fbs-1.2.2/fbs/installer/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/installer/mac/create-dmg/LICENSE` & `fbs-1.2.2/fbs/installer/mac/create-dmg/LICENSE`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/installer/mac/create-dmg/README.md` & `fbs-1.2.2/fbs/installer/mac/create-dmg/README.md`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/installer/mac/create-dmg/builder/create-dmg.builder` & `fbs-1.2.2/fbs/installer/mac/create-dmg/builder/create-dmg.builder`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/installer/mac/create-dmg/create-dmg` & `fbs-1.2.2/fbs/installer/mac/create-dmg/create-dmg`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/installer/mac/create-dmg/support/brew-me.sh` & `fbs-1.2.2/fbs/installer/mac/create-dmg/support/brew-me.sh`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/installer/mac/create-dmg/support/dmg-license.py` & `fbs-1.2.2/fbs/installer/mac/create-dmg/support/dmg-license.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/installer/mac/create-dmg/support/template.applescript` & `fbs-1.2.2/fbs/installer/mac/create-dmg/support/template.applescript`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/installer/windows.py` & `fbs-1.2.2/fbs/installer/windows.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/repo/arch.py` & `fbs-1.2.2/fbs/repo/arch.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/repo/fedora.py` & `fbs-1.2.2/fbs/repo/fedora.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/repo/ubuntu.py` & `fbs-1.2.2/fbs/repo/ubuntu.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/resources.py` & `fbs-1.2.2/fbs/resources.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/sign/windows.py` & `fbs-1.2.2/fbs/sign/windows.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs/upload.py` & `fbs-1.2.2/fbs/upload.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs.egg-info/PKG-INFO` & `fbs-1.2.2/fbs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbs
-Version: 1.2.1
+Version: 1.2.2
 Summary: Create cross-platform desktop applications with Python and Qt
 Home-page: https://build-system.fman.io
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 License: GPLv3 or later
 Description: Create cross-platform desktop applications with Python and Qt
```

### Comparing `fbs-1.2.1/fbs.egg-info/SOURCES.txt` & `fbs-1.2.2/fbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/_fbs.py` & `fbs-1.2.2/fbs_runtime/_fbs.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/_frozen.py` & `fbs-1.2.2/fbs_runtime/_frozen.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/_settings.py` & `fbs-1.2.2/fbs_runtime/_settings.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/_signal.py` & `fbs-1.2.2/fbs_runtime/_signal.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/_source.py` & `fbs-1.2.2/fbs_runtime/_source.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/_state.py` & `fbs-1.2.2/fbs_runtime/_state.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/application_context/PyQt5.py` & `fbs-1.2.2/fbs_runtime/application_context/PyQt5.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/application_context/PySide2.py` & `fbs-1.2.2/fbs_runtime/application_context/PySide2.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/application_context/__init__.py` & `fbs-1.2.2/fbs_runtime/application_context/__init__.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/excepthook/__init__.py` & `fbs-1.2.2/fbs_runtime/excepthook/__init__.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/excepthook/_util.py` & `fbs-1.2.2/fbs_runtime/excepthook/_util.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/licensing.py` & `fbs-1.2.2/fbs_runtime/licensing.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/fbs_runtime/platform.py` & `fbs-1.2.2/fbs_runtime/platform.py`

 * *Files identical despite different names*

### Comparing `fbs-1.2.1/setup.py` & `fbs-1.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             result.append(relpath(filepath, pkg_dir))
     return result
 
 description = 'Create cross-platform desktop applications with Python and Qt'
 setup(
     name='fbs',
     # Also update fbs/_defaults/requirements/base.txt when you change this:
-    version='1.2.1',
+    version='1.2.2',
     description=description,
     long_description=
         description + '\n\nHome page: https://build-system.fman.io',
     author='Michael Herrmann',
     author_email='michael+removethisifyouarehuman@herrmann.io',
     url='https://build-system.fman.io',
     packages=find_packages(exclude=('tests', 'tests.*')),
```

