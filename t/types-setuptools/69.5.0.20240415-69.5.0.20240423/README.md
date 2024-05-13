# Comparing `tmp/types-setuptools-69.5.0.20240415.tar.gz` & `tmp/types-setuptools-69.5.0.20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-setuptools-69.5.0.20240415.tar", last modified: Mon Apr 15 04:04:26 2024, max compression
+gzip compressed data, was "types-setuptools-69.5.0.20240423.tar", last modified: Tue Apr 23 02:19:00 2024, max compression
```

## Comparing `types-setuptools-69.5.0.20240415.tar` & `types-setuptools-69.5.0.20240423.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.236409 types-setuptools-69.5.0.20240415/
--rw-r--r--   0 runner    (1001) docker     (127)    17378 2024-04-15 04:04:25.000000 types-setuptools-69.5.0.20240415/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 04:04:25.000000 types-setuptools-69.5.0.20240415/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-15 04:04:26.236409 types-setuptools-69.5.0.20240415/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.220409 types-setuptools-69.5.0.20240415/distutils-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 04:04:25.000000 types-setuptools-69.5.0.20240415/distutils-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/_modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/ccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.220409 types-setuptools-69.5.0.20240415/distutils-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/bdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/command/upload.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.224409 types-setuptools-69.5.0.20240415/distutils-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:25.000000 types-setuptools-69.5.0.20240415/distutils-stubs/compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/sysconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/distutils-stubs/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.224409 types-setuptools-69.5.0.20240415/pkg_resources-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 04:04:25.000000 types-setuptools-69.5.0.20240415/pkg_resources-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    19842 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/pkg_resources-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.224409 types-setuptools-69.5.0.20240415/pkg_resources-stubs/_vendored_packaging/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/pkg_resources-stubs/_vendored_packaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/pkg_resources-stubs/_vendored_packaging/markers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/pkg_resources-stubs/_vendored_packaging/requirements.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/pkg_resources-stubs/_vendored_packaging/specifiers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/pkg_resources-stubs/_vendored_packaging/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.224409 types-setuptools-69.5.0.20240415/pkg_resources-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/pkg_resources-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:25.000000 types-setuptools-69.5.0.20240415/pkg_resources-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 04:04:26.236409 types-setuptools-69.5.0.20240415/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-15 04:04:25.000000 types-setuptools-69.5.0.20240415/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.228409 types-setuptools-69.5.0.20240415/setuptools-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 04:04:25.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.228409 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/_modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/ccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.232409 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/bdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/upload.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.232409 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/sysconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/build_meta.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.232409 types-setuptools-69.5.0.20240415/setuptools-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/alias.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/bdist_egg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/develop.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/dist_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/easy_install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/editable_wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/install_egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/rotate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/saveopts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/setopt.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/test.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/command/upload_docs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.236409 types-setuptools-69.5.0.20240415/setuptools-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/compat/py310.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/compat/py311.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/compat/py39.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.236409 types-setuptools-69.5.0.20240415/setuptools-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/config/expand.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/config/pyprojecttoml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/config/setupcfg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/depends.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/discovery.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.236409 types-setuptools-69.5.0.20240415/setuptools-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/installer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/launch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/logging.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/monkey.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/msvc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/namespaces.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/package_index.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:25.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/sandbox.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/unicode_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 04:04:15.000000 types-setuptools-69.5.0.20240415/setuptools-stubs/windows_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:26.236409 types-setuptools-69.5.0.20240415/types_setuptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-15 04:04:26.000000 types-setuptools-69.5.0.20240415/types_setuptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-15 04:04:26.000000 types-setuptools-69.5.0.20240415/types_setuptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:04:26.000000 types-setuptools-69.5.0.20240415/types_setuptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 04:04:26.000000 types-setuptools-69.5.0.20240415/types_setuptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.512423 types-setuptools-69.5.0.20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)    17585 2024-04-23 02:18:59.000000 types-setuptools-69.5.0.20240423/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 02:18:59.000000 types-setuptools-69.5.0.20240423/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-23 02:19:00.512423 types-setuptools-69.5.0.20240423/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.496423 types-setuptools-69.5.0.20240423/distutils-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-23 02:18:59.000000 types-setuptools-69.5.0.20240423/distutils-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/_modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/ccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.496423 types-setuptools-69.5.0.20240423/distutils-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/bdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/command/upload.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.496423 types-setuptools-69.5.0.20240423/distutils-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:59.000000 types-setuptools-69.5.0.20240423/distutils-stubs/compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/sysconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/distutils-stubs/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.496423 types-setuptools-69.5.0.20240423/pkg_resources-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-23 02:18:59.000000 types-setuptools-69.5.0.20240423/pkg_resources-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    19842 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/pkg_resources-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.500423 types-setuptools-69.5.0.20240423/pkg_resources-stubs/_vendored_packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/pkg_resources-stubs/_vendored_packaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/pkg_resources-stubs/_vendored_packaging/markers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/pkg_resources-stubs/_vendored_packaging/requirements.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/pkg_resources-stubs/_vendored_packaging/specifiers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/pkg_resources-stubs/_vendored_packaging/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.500423 types-setuptools-69.5.0.20240423/pkg_resources-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/pkg_resources-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:59.000000 types-setuptools-69.5.0.20240423/pkg_resources-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:19:00.512423 types-setuptools-69.5.0.20240423/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-23 02:18:59.000000 types-setuptools-69.5.0.20240423/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.504423 types-setuptools-69.5.0.20240423/setuptools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-23 02:18:59.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.504423 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/_modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/ccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.504423 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/bdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/upload.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.504423 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/sysconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/build_meta.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.508423 types-setuptools-69.5.0.20240423/setuptools-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/alias.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/bdist_egg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/develop.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/dist_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/easy_install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/editable_wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/install_egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/rotate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/saveopts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/setopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/command/upload_docs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.512423 types-setuptools-69.5.0.20240423/setuptools-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/compat/py310.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/compat/py311.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/compat/py39.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.512423 types-setuptools-69.5.0.20240423/setuptools-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/config/expand.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/config/pyprojecttoml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/config/setupcfg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/depends.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.512423 types-setuptools-69.5.0.20240423/setuptools-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/installer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/launch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/logging.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/monkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/msvc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/namespaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/package_index.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:59.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/sandbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/unicode_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 02:18:48.000000 types-setuptools-69.5.0.20240423/setuptools-stubs/windows_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:00.512423 types-setuptools-69.5.0.20240423/types_setuptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-23 02:19:00.000000 types-setuptools-69.5.0.20240423/types_setuptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-23 02:19:00.000000 types-setuptools-69.5.0.20240423/types_setuptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:19:00.000000 types-setuptools-69.5.0.20240423/types_setuptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 02:19:00.000000 types-setuptools-69.5.0.20240423/types_setuptools.egg-info/top_level.txt
```

### Comparing `types-setuptools-69.5.0.20240415/CHANGELOG.md` & `types-setuptools-69.5.0.20240423/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 69.5.0.20240423 (2024-04-23)
+
+Add precise values for enum members where possible (#11299)
+
+Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
+Co-authored-by: Alex Waygood <alex.waygood@gmail.com>
+
 ## 69.5.0.20240415 (2024-04-15)
 
 Ensure that distutils and setuptools._distutils stay consistent (#11758)
 
 Update setuptools to 69.5.* (#11756)
 
 ## 69.2.0.20240317 (2024-03-17)
```

### Comparing `types-setuptools-69.5.0.20240415/PKG-INFO` & `types-setuptools-69.5.0.20240423/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 69.5.0.20240415
+Version: 69.5.0.20240423
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-setuptools` aims to provide accurate annotations
 for `setuptools==69.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7c8e82fe483a40ec4cb0a2505cfdb0f3e7cc81d9` and was tested
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-setuptools-69.5.0.20240415/pkg_resources-stubs/__init__.pyi` & `types-setuptools-69.5.0.20240423/pkg_resources-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/pkg_resources-stubs/_vendored_packaging/markers.pyi` & `types-setuptools-69.5.0.20240423/pkg_resources-stubs/_vendored_packaging/markers.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/pkg_resources-stubs/_vendored_packaging/specifiers.pyi` & `types-setuptools-69.5.0.20240423/pkg_resources-stubs/_vendored_packaging/specifiers.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/pkg_resources-stubs/_vendored_packaging/version.pyi` & `types-setuptools-69.5.0.20240423/pkg_resources-stubs/_vendored_packaging/version.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/pkg_resources-stubs/extern/__init__.pyi` & `types-setuptools-69.5.0.20240423/pkg_resources-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setup.py` & `types-setuptools-69.5.0.20240423/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-setuptools` aims to provide accurate annotations
 for `setuptools==69.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7c8e82fe483a40ec4cb0a2505cfdb0f3e7cc81d9` and was tested
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="69.5.0.20240415",
+      version="69.5.0.20240423",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
-      packages=['distutils-stubs', 'setuptools-stubs', 'pkg_resources-stubs'],
-      package_data={'distutils-stubs': ['_modified.pyi', 'archive_util.pyi', 'ccompiler.pyi', 'cmd.pyi', 'command/bdist.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/install.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/sdist.pyi', 'command/upload.pyi', 'compat/__init__.pyi', 'config.pyi', 'dep_util.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'filelist.pyi', 'sysconfig.pyi', 'util.pyi', 'METADATA.toml', 'compat/py.typed'], 'setuptools-stubs': ['__init__.pyi', '_distutils/_modified.pyi', '_distutils/archive_util.pyi', '_distutils/ccompiler.pyi', '_distutils/cmd.pyi', '_distutils/command/bdist.pyi', '_distutils/command/bdist_rpm.pyi', '_distutils/command/build.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/compat/__init__.pyi', '_distutils/config.pyi', '_distutils/dep_util.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', '_distutils/sysconfig.pyi', '_distutils/util.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/bdist_egg.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/editable_wheel.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'compat/__init__.pyi', 'compat/py310.pyi', 'compat/py311.pyi', 'compat/py39.pyi', 'config/__init__.pyi', 'config/expand.pyi', 'config/pyprojecttoml.pyi', 'config/setupcfg.pyi', 'dep_util.pyi', 'depends.pyi', 'discovery.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'logging.pyi', 'modified.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'warnings.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml', 'py.typed'], 'pkg_resources-stubs': ['__init__.pyi', '_vendored_packaging/__init__.pyi', '_vendored_packaging/markers.pyi', '_vendored_packaging/requirements.pyi', '_vendored_packaging/specifiers.pyi', '_vendored_packaging/version.pyi', 'extern/__init__.pyi', 'METADATA.toml', 'py.typed']},
+      packages=['setuptools-stubs', 'distutils-stubs', 'pkg_resources-stubs'],
+      package_data={'setuptools-stubs': ['__init__.pyi', '_distutils/_modified.pyi', '_distutils/archive_util.pyi', '_distutils/ccompiler.pyi', '_distutils/cmd.pyi', '_distutils/command/bdist.pyi', '_distutils/command/bdist_rpm.pyi', '_distutils/command/build.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/compat/__init__.pyi', '_distutils/config.pyi', '_distutils/dep_util.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', '_distutils/sysconfig.pyi', '_distutils/util.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/bdist_egg.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/editable_wheel.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'compat/__init__.pyi', 'compat/py310.pyi', 'compat/py311.pyi', 'compat/py39.pyi', 'config/__init__.pyi', 'config/expand.pyi', 'config/pyprojecttoml.pyi', 'config/setupcfg.pyi', 'dep_util.pyi', 'depends.pyi', 'discovery.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'logging.pyi', 'modified.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'warnings.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml', 'py.typed'], 'distutils-stubs': ['_modified.pyi', 'archive_util.pyi', 'ccompiler.pyi', 'cmd.pyi', 'command/bdist.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/install.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/sdist.pyi', 'command/upload.pyi', 'compat/__init__.pyi', 'config.pyi', 'dep_util.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'filelist.pyi', 'sysconfig.pyi', 'util.pyi', 'METADATA.toml', 'compat/py.typed'], 'pkg_resources-stubs': ['__init__.pyi', '_vendored_packaging/__init__.pyi', '_vendored_packaging/markers.pyi', '_vendored_packaging/requirements.pyi', '_vendored_packaging/specifiers.pyi', '_vendored_packaging/version.pyi', 'extern/__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/__init__.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/archive_util.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/ccompiler.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/ccompiler.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/cmd.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/cmd.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/bdist.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/bdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/bdist_rpm.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/bdist_rpm.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/build.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/build.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/build_clib.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/build_clib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/build_ext.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/build_py.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/install.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/install_lib.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/install_lib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/register.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/register.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/sdist.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/command/upload.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/command/upload.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/dist.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/errors.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/extension.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/filelist.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/filelist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/sysconfig.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/sysconfig.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/_distutils/util.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/_distutils/util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/archive_util.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/build_meta.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/build_meta.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/command/bdist_egg.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/command/bdist_egg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/command/build_ext.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/command/build_py.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/command/develop.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/command/develop.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/command/easy_install.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/command/easy_install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/command/editable_wheel.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/command/editable_wheel.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from ..dist import Distribution
 from ..warnings import SetuptoolsWarning
 
 # Actually from wheel.wheelfile import WheelFile
 _WheelFile: TypeAlias = Incomplete
 
 class _EditableMode(Enum):
-    STRICT: str
-    LENIENT: str
-    COMPAT: str
+    STRICT = "strict"
+    LENIENT = "lenient"
+    COMPAT = "compat"
     @classmethod
     def convert(cls, mode: str | None) -> _EditableMode: ...
 
 class editable_wheel(Command):
     description: str
     user_options: Incomplete
     dist_dir: Incomplete
```

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/command/egg_info.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/command/egg_info.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/command/sdist.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/command/setopt.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/command/setopt.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/command/test.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/command/test.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/command/upload_docs.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/command/upload_docs.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/config/expand.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/config/expand.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/config/pyprojecttoml.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/config/pyprojecttoml.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/config/setupcfg.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/config/setupcfg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/depends.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/depends.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/discovery.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/discovery.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/dist.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/errors.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/extension.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/extern/__init__.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/msvc.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/msvc.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/package_index.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/package_index.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/setuptools-stubs/sandbox.pyi` & `types-setuptools-69.5.0.20240423/setuptools-stubs/sandbox.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240415/types_setuptools.egg-info/PKG-INFO` & `types-setuptools-69.5.0.20240423/types_setuptools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 69.5.0.20240415
+Version: 69.5.0.20240423
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-setuptools` aims to provide accurate annotations
 for `setuptools==69.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7c8e82fe483a40ec4cb0a2505cfdb0f3e7cc81d9` and was tested
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-setuptools-69.5.0.20240415/types_setuptools.egg-info/SOURCES.txt` & `types-setuptools-69.5.0.20240423/types_setuptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

