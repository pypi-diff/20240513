# Comparing `tmp/networklab-1.8.2.tar.gz` & `tmp/networklab-1.8.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networklab-1.8.2.tar", last modified: Mon May 13 14:42:46 2024, max compression
+gzip compressed data, was "networklab-1.8.2.dev1.tar", last modified: Tue Apr 30 16:59:07 2024, max compression
```

## Comparing `networklab-1.8.2.tar` & `networklab-1.8.2.dev1.tar`

### file list

```diff
@@ -1,761 +1,759 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.724887 networklab-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-13 14:42:41.000000 networklab-1.8.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-13 14:42:41.000000 networklab-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-13 14:42:46.724887 networklab-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-13 14:42:41.000000 networklab-1.8.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-05-13 14:42:41.000000 networklab-1.8.2/netlab
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.620888 networklab-1.8.2/netsim/
--rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.620888 networklab-1.8.2/netsim/ansible/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/collect-configs.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)      861 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)     2469 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/create-config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)      295 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/display-neighbors.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/initial-config.ansible
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/reload-config.ansible
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.620888 networklab-1.8.2/netsim/ansible/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/create-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/create-custom-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.624888 networklab-1.8.2/netsim/ansible/tasks/deploy-config/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/linux-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/none.yml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/sonic.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-config/vyos.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-custom-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/deploy-module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.628888 networklab-1.8.2/netsim/ansible/tasks/fetch-config/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fetch-config/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.628888 networklab-1.8.2/netsim/ansible/tasks/fortinet.fortios.fortios/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.628888 networklab-1.8.2/netsim/ansible/tasks/frr/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/frr/deploy-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/frr/mpls-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/initial-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.628888 networklab-1.8.2/netsim/ansible/tasks/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/linux/dhcp.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/linux/initial-clab.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.628888 networklab-1.8.2/netsim/ansible/tasks/nxos/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/nxos/initial.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.628888 networklab-1.8.2/netsim/ansible/tasks/readiness-check/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/readiness-check/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/readiness-check/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/readiness-check/eos-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/readiness-check/iosxr-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/readiness-check/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/readiness-check/vptx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/readiness-check/vsrx.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.628888 networklab-1.8.2/netsim/ansible/tasks/vmx/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/vmx/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/tasks/wait-for-ready.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.628888 networklab-1.8.2/netsim/ansible/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.632888 networklab-1.8.2/netsim/ansible/templates/bfd/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bfd/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bfd/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bfd/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bfd/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bfd/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bfd/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bfd/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bfd/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bfd/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bfd/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bfd/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.636888 networklab-1.8.2/netsim/ansible/templates/bgp/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/arubacx.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/asa.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/dellos10.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/eos.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/ios.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/routeros.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/routeros7.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/sonic.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/bgp/vyos.macro.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.636888 networklab-1.8.2/netsim/ansible/templates/dhcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/dhcp/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/dhcp/dnsmasq.j2
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/dhcp/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/dhcp/eos.server.j2
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/dhcp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/dhcp/ios.server.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/dhcp/linux.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.636888 networklab-1.8.2/netsim/ansible/templates/eigrp/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/eigrp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/eigrp/nxos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.640888 networklab-1.8.2/netsim/ansible/templates/evpn/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/evpn/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/evpn/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/evpn/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/evpn/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/evpn/frr.evpn-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/evpn/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/evpn/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/evpn/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/evpn/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/evpn/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.640888 networklab-1.8.2/netsim/ansible/templates/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/gateway/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/gateway/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/gateway/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/gateway/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/gateway/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/gateway/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/gateway/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/gateway/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/gateway/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.648888 networklab-1.8.2/netsim/ansible/templates/initial/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/arubacx.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/arubacx.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/csr.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/dellos10.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/eos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.648888 networklab-1.8.2/netsim/ansible/templates/initial/frr/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/frr/daemons.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/ios.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/ios.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/junos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/junos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.648888 networklab-1.8.2/netsim/ansible/templates/initial/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/linux/bash_profile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/linux/hosts.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/linux/ubuntu.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/linux/vanilla.j2
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/linux-clab.j2
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/linux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/nxos.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/routeros.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/routeros.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/routeros7.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/routeros7.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/sonic.j2
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/vyos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/initial/vyos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.648888 networklab-1.8.2/netsim/ansible/templates/isis/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/isis/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/isis/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/isis/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/isis/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/isis/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/isis/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/isis/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/isis/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/isis/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/isis/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/isis/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/missing.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.652888 networklab-1.8.2/netsim/ansible/templates/mpls/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/arubacx.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/eos.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/eos.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/eos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/eos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/frr.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/frr.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/ios.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/ios.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/ios.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/ios.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/junos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/junos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/routeros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/routeros7.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/srlinux.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/sros.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/sros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/sros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/vyos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.660888 networklab-1.8.2/netsim/ansible/templates/ospf/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/eos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/eos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/frr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/frr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/ios.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/ios.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/junos.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/nxos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/nxos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/vyos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/ospf/vyos.ospfv3.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.660888 networklab-1.8.2/netsim/ansible/templates/sr/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/sr/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/sr/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/sr/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/sr/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/sr/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/sr/sros.openconfig.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.660888 networklab-1.8.2/netsim/ansible/templates/srv6/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/srv6/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.664888 networklab-1.8.2/netsim/ansible/templates/vlan/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/vmx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/vptx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/vsrx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vlan/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.672888 networklab-1.8.2/netsim/ansible/templates/vrf/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/arubacx.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/dellos10.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/eos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/eos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/eos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/eos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/frr.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/frr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/frr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/ios.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/ios.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/ios.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/ios.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/junos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/junos.ospf-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/nxos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/routeros.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/routeros7.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/vyos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.672888 networklab-1.8.2/netsim/ansible/templates/vxlan/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vxlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vxlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vxlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vxlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vxlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vxlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vxlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vxlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vxlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/ansible/templates/vxlan/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.672888 networklab-1.8.2/netsim/api/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.676888 networklab-1.8.2/netsim/augment/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/addressing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    24713 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    43060 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/augment/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.680888 networklab-1.8.2/netsim/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11583 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/_nodeset.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/alias.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/clab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.680888 networklab-1.8.2/netsim/cli/clab_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/clab_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/clab_actions/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/clab_actions/tarball.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/down.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/empty.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/external_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/libvirt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.680888 networklab-1.8.2/netsim/cli/libvirt_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/libvirt_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/libvirt_actions/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/libvirt_actions/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show-usage.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.680888 networklab-1.8.2/netsim/cli/show_commands/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show_commands/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show_commands/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show_commands/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show_commands/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show_commands/module_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show_commands/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show_commands/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show_commands/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/show_commands/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/up.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/usage.txt
--rw-r--r--   0 runner    (1001) docker     (127)    33657 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/cli/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.680888 networklab-1.8.2/netsim/daemons/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/daemons/bird.yml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/daemons/dnsmasq.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.684888 networklab-1.8.2/netsim/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/data/filemaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/data/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    30700 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/data/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28964 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/data/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.684888 networklab-1.8.2/netsim/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/defaults/addressing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/defaults/attributes.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/defaults/automation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/defaults/hints.yml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/defaults/multilab.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/defaults/paths.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/defaults/ports.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.688888 networklab-1.8.2/netsim/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/arubacx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/asav.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/asav.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/csr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/dellos10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/eos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/fortios.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/iosv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/iosv.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/junos.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/linux.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/none.yml
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/sonic.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/srlinux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/unknown.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/vmx.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/vmx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/vptx.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/vptx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/vsrx.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/vsrx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/devices/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.616888 networklab-1.8.2/netsim/extra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.688888 networklab-1.8.2/netsim/extra/bgp.domain/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.domain/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.domain/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.688888 networklab-1.8.2/netsim/extra/bgp.originate/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.originate/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.originate/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.692888 networklab-1.8.2/netsim/extra/bgp.policy/
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.policy/_route_map_aoscx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.policy/_route_map_ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.policy/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.policy/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.policy/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.policy/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.policy/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.policy/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.policy/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.policy/simple-attributes.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.policy/srlinux.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.696888 networklab-1.8.2/netsim/extra/bgp.session/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/_sample_bfd_template.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/bird.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/default-originate.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/topology.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/bgp.session/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.696888 networklab-1.8.2/netsim/extra/ebgp.multihop/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.multihop/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.multihop/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.multihop/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.multihop/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.multihop/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.multihop/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.multihop/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.multihop/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.multihop/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.696888 networklab-1.8.2/netsim/extra/ebgp.utils/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/ebgp.utils/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.696888 networklab-1.8.2/netsim/extra/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/fabric/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/fabric/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.696888 networklab-1.8.2/netsim/extra/multilab/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/multilab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.696888 networklab-1.8.2/netsim/extra/none/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/none/none.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.696888 networklab-1.8.2/netsim/extra/proxy-arp/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/proxy-arp/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/proxy-arp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/extra/proxy-arp/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.700888 networklab-1.8.2/netsim/install/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2190 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/ansible.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3699 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/containerlab.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1149 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/grpc.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.700888 networklab-1.8.2/netsim/install/libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/arubacx.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.700888 networklab-1.8.2/netsim/install/libvirt/asav/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/asav/day0-config
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/asav.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/asav.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/csr.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.704887 networklab-1.8.2/netsim/install/libvirt/dellos10/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/dellos10/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/dellos10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/eos.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/eos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/iosv.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/iosv.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/iosxr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/nxos.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/nxos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/routeros7.txt
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/sonic.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/sonic.xml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.704887 networklab-1.8.2/netsim/install/libvirt/vptx/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/vptx/juniper.conf
--rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/vptx/make-config.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/vptx/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/vptx.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/vptx.xml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.704887 networklab-1.8.2/netsim/install/libvirt/vsrx/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/vsrx/juniper.conf
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt/vsrx.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3267 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/libvirt.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2319 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/install/ubuntu.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.708887 networklab-1.8.2/netsim/modules/
--rw-r--r--   0 runner    (1001) docker     (127)    19815 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/_dataplane.py
--rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/bfd.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/bfd.yml
--rw-r--r--   0 runner    (1001) docker     (127)    25554 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/bgp.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/dhcp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/eigrp.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/eigrp.yml
--rw-r--r--   0 runner    (1001) docker     (127)    17618 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/evpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/evpn.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/gateway.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/isis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/isis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/mpls.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/mpls.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/ospf.yml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/sr.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/sr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/srv6.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/srv6.yml
--rw-r--r--   0 runner    (1001) docker     (127)    61378 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/vlan.yml
--rw-r--r--   0 runner    (1001) docker     (127)    20957 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/vrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/vrf.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/vxlan.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/modules/vxlan.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.712887 networklab-1.8.2/netsim/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/d2.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/d2.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/graph.yml
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/graphite.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/outputs/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.712887 networklab-1.8.2/netsim/providers/
--rw-r--r--   0 runner    (1001) docker     (127)    11966 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/providers/clab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/providers/clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/providers/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/providers/external.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/providers/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/providers/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/providers/virtualbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/providers/virtualbox.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.712887 networklab-1.8.2/netsim/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/ansible.cfg.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.616888 networklab-1.8.2/netsim/templates/provider/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.712887 networklab-1.8.2/netsim/templates/provider/clab/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/clab/clab.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.712887 networklab-1.8.2/netsim/templates/provider/clab/cumulus/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/clab/cumulus/hosts.j2
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/clab/cumulus/interfaces.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.712887 networklab-1.8.2/netsim/templates/provider/clab/frr/
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/clab/frr/daemons.j2
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/clab/frr/hosts.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.712887 networklab-1.8.2/netsim/templates/provider/clab/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/clab/linux/hosts.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.716887 networklab-1.8.2/netsim/templates/provider/external/
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/external/external.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.720887 networklab-1.8.2/netsim/templates/provider/libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/arubacx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/asav-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/csr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/define-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/dellos10-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/fortios-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/forwarded-ports.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/frr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/iosv-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/iosxr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/libvirt-bridge.j2
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/libvirt-tunnel.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/none-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/routeros-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/routeros7-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/sonic-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/vagrant-libvirt.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/vptx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/vsrx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/libvirt/vyos-domain.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.720887 networklab-1.8.2/netsim/templates/provider/virtualbox/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/virtualbox/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/virtualbox/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/virtualbox/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/virtualbox/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/virtualbox/frr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/virtualbox/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/virtualbox/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/virtualbox/virtualbox-network.j2
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/virtualbox/virtualbox-ports.j2
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/provider/virtualbox/vsrx-domain.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.720887 networklab-1.8.2/netsim/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/tests/clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/tests/grpc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/tests/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/templates/tests/virtualbox.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.720887 networklab-1.8.2/netsim/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/tools/graphite.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/tools/graphite.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.720887 networklab-1.8.2/netsim/tools/suzieq/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/tools/suzieq/suzieq-cfg.yml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/tools/suzieq.yml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/topology-defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.724887 networklab-1.8.2/netsim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/utils/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/utils/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/utils/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/utils/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.724887 networklab-1.8.2/netsim/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/validate/frr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-13 14:42:41.000000 networklab-1.8.2/netsim/validate/linux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.724887 networklab-1.8.2/networklab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-13 14:42:46.000000 networklab-1.8.2/networklab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25450 2024-05-13 14:42:46.000000 networklab-1.8.2/networklab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:42:46.000000 networklab-1.8.2/networklab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-13 14:42:46.000000 networklab-1.8.2/networklab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 14:42:46.000000 networklab-1.8.2/networklab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-13 14:42:41.000000 networklab-1.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:42:46.724887 networklab-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-13 14:42:41.000000 networklab-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:42:46.724887 networklab-1.8.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3377 2024-05-13 14:42:41.000000 networklab-1.8.2/tests/test_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netlab
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.167304 networklab-1.8.2.dev1/netsim/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.167304 networklab-1.8.2.dev1/netsim/ansible/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/collect-configs.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)      861 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2469 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/create-config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)      295 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/display-neighbors.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/initial-config.ansible
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/reload-config.ansible
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.167304 networklab-1.8.2.dev1/netsim/ansible/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/create-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/create-custom-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.171304 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/linux-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/none.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/sonic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/vyos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-custom-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.175304 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.175304 networklab-1.8.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.175304 networklab-1.8.2.dev1/netsim/ansible/tasks/frr/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/frr/deploy-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/frr/mpls-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/initial-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.175304 networklab-1.8.2.dev1/netsim/ansible/tasks/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/linux/dhcp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/linux/initial-clab.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.175304 networklab-1.8.2.dev1/netsim/ansible/tasks/nxos/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/nxos/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.179304 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/eos-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/iosxr-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/vptx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/vsrx.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.179304 networklab-1.8.2.dev1/netsim/ansible/tasks/vmx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/vmx/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/wait-for-ready.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.179304 networklab-1.8.2.dev1/netsim/ansible/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.179304 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.187304 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/arubacx.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/asa.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/eos.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/ios.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sonic.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/vyos.macro.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.187304 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/dnsmasq.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/eos.server.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/ios.server.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/linux.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.187304 networklab-1.8.2.dev1/netsim/ansible/templates/eigrp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/eigrp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/eigrp/nxos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.191304 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.191304 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.199304 networklab-1.8.2.dev1/netsim/ansible/templates/initial/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/arubacx.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/arubacx.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/csr.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/eos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.199304 networklab-1.8.2.dev1/netsim/ansible/templates/initial/frr/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/frr/daemons.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/ios.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/ios.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.199304 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/bash_profile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/hosts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/vanilla.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux-clab.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/nxos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros7.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/sonic.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/vyos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/vyos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.203304 networklab-1.8.2.dev1/netsim/ansible/templates/isis/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/missing.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.207305 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/arubacx.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/frr.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/junos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros7.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/srlinux.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/vyos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.215304 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/junos.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.215304 networklab-1.8.2.dev1/netsim/ansible/templates/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/sros.openconfig.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.215304 networklab-1.8.2.dev1/netsim/ansible/templates/srv6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/srv6/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.219305 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vmx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vptx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vsrx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.227305 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.ospf-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.231305 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.231305 networklab-1.8.2.dev1/netsim/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.231305 networklab-1.8.2.dev1/netsim/augment/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/addressing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24713 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42721 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.239305 networklab-1.8.2.dev1/netsim/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10608 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/_nodeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/alias.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/clab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.239305 networklab-1.8.2.dev1/netsim/cli/clab_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/clab_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/clab_actions/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/clab_actions/tarball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/down.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/empty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/external_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/libvirt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.239305 networklab-1.8.2.dev1/netsim/cli/libvirt_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/libvirt_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/libvirt_actions/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/libvirt_actions/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show-usage.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.239305 networklab-1.8.2.dev1/netsim/cli/show_commands/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/module_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/up.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/usage.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.243305 networklab-1.8.2.dev1/netsim/daemons/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/daemons/bird.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/daemons/dnsmasq.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.243305 networklab-1.8.2.dev1/netsim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/data/filemaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/data/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30700 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28964 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/data/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.243305 networklab-1.8.2.dev1/netsim/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/addressing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/attributes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/automation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/hints.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/multilab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/paths.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/ports.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.251305 networklab-1.8.2.dev1/netsim/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/arubacx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/asav.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/asav.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/csr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/eos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/iosv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/iosv.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/junos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/none.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/sonic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/unknown.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vmx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vptx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vptx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vsrx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vsrx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.163304 networklab-1.8.2.dev1/netsim/extra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.251305 networklab-1.8.2.dev1/netsim/extra/bgp.domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.domain/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.domain/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.251305 networklab-1.8.2.dev1/netsim/extra/bgp.originate/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.originate/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.originate/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.251305 networklab-1.8.2.dev1/netsim/extra/bgp.policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/_route_map_aoscx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/_route_map_ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/simple-attributes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/srlinux.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.255305 networklab-1.8.2.dev1/netsim/extra/bgp.session/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/_sample_bfd_template.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/bird.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/default-originate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/topology.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/ebgp.utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.utils/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/fabric/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/fabric/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/multilab/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/multilab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/none/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/none/none.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/proxy-arp/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/proxy-arp/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/proxy-arp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/proxy-arp/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/install/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2190 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/ansible.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3699 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/containerlab.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/grpc.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.263305 networklab-1.8.2.dev1/netsim/install/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/arubacx.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.263305 networklab-1.8.2.dev1/netsim/install/libvirt/asav/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/asav/day0-config
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/asav.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/asav.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/csr.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.263305 networklab-1.8.2.dev1/netsim/install/libvirt/dellos10/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/dellos10/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/dellos10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/eos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/eos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/iosv.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/iosv.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/iosxr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/nxos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/nxos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/routeros7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/sonic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/sonic.xml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.263305 networklab-1.8.2.dev1/netsim/install/libvirt/vptx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vptx/juniper.conf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vptx/make-config.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vptx/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vptx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vptx.xml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.263305 networklab-1.8.2.dev1/netsim/install/libvirt/vsrx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vsrx/juniper.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vsrx.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3267 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2319 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.271305 networklab-1.8.2.dev1/netsim/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)    19815 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/_dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/bfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/bfd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    25554 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/bgp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/dhcp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/eigrp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/eigrp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    17618 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/evpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/evpn.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/gateway.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/isis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/isis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/mpls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/mpls.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/ospf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/sr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/sr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/srv6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/srv6.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    61378 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vlan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20957 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vrf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vxlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vxlan.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.275305 networklab-1.8.2.dev1/netsim/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/d2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/d2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/graph.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.275305 networklab-1.8.2.dev1/netsim/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/clab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/external.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16735 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/virtualbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/virtualbox.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.275305 networklab-1.8.2.dev1/netsim/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/ansible.cfg.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.163304 networklab-1.8.2.dev1/netsim/templates/provider/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.275305 networklab-1.8.2.dev1/netsim/templates/provider/clab/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/clab.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.275305 networklab-1.8.2.dev1/netsim/templates/provider/clab/cumulus/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/cumulus/hosts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/cumulus/interfaces.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.279305 networklab-1.8.2.dev1/netsim/templates/provider/clab/frr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/frr/daemons.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/frr/hosts.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.279305 networklab-1.8.2.dev1/netsim/templates/provider/clab/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/linux/hosts.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.279305 networklab-1.8.2.dev1/netsim/templates/provider/external/
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/external/external.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.283305 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/arubacx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/asav-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/csr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/define-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/dellos10-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/fortios-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/forwarded-ports.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/iosv-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/libvirt-bridge.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/none-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/routeros-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/routeros7-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/sonic-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vptx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vyos-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.287305 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/virtualbox-network.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/vsrx-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.287305 networklab-1.8.2.dev1/netsim/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/tests/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/tests/grpc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/tests/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/tests/virtualbox.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.287305 networklab-1.8.2.dev1/netsim/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/tools/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/tools/graphite.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.287305 networklab-1.8.2.dev1/netsim/tools/suzieq/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/tools/suzieq/suzieq-cfg.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/tools/suzieq.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/topology-defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/netsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/netsim/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/validate/frr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/validate/linux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/networklab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-30 16:59:07.000000 networklab-1.8.2.dev1/networklab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25397 2024-04-30 16:59:07.000000 networklab-1.8.2.dev1/networklab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:59:07.000000 networklab-1.8.2.dev1/networklab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 16:59:07.000000 networklab-1.8.2.dev1/networklab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 16:59:07.000000 networklab-1.8.2.dev1/networklab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3377 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/tests/test_transformation.py
```

### Comparing `networklab-1.8.2/LICENSE.md` & `networklab-1.8.2.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/PKG-INFO` & `networklab-1.8.2.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.8.2
+Version: 1.8.2.dev1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.8.2](https://github.com/ipspace/netlab/releases/tag/release_1.8.2), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.1-post1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1-post1) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
+The latest release is [release 1.8.1-post1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1-post1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
 
 <!--
 If you encounter bugs using release 1.7.x, please downgrade to [1.6.4](https://github.com/ipspace/netlab/releases/tag/release_1.6.4) and [open a GitHub issue](https://github.com/ipspace/netlab/issues).
 -->
 
 ## An Overview of CLI Commands
```

### Comparing `networklab-1.8.2/README.md` & `networklab-1.8.2.dev1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.8.2](https://github.com/ipspace/netlab/releases/tag/release_1.8.2), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.1-post1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1-post1) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
+The latest release is [release 1.8.1-post1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1-post1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
 
 <!--
 If you encounter bugs using release 1.7.x, please downgrade to [1.6.4](https://github.com/ipspace/netlab/releases/tag/release_1.6.4) and [open a GitHub issue](https://github.com/ipspace/netlab/issues).
 -->
 
 ## An Overview of CLI Commands
```

### Comparing `networklab-1.8.2/netsim/ansible/collect-configs.ansible` & `networklab-1.8.2.dev1/netsim/ansible/collect-configs.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/config.ansible` & `networklab-1.8.2.dev1/netsim/ansible/config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/create-config.ansible` & `networklab-1.8.2.dev1/netsim/ansible/create-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/initial-config.ansible` & `networklab-1.8.2.dev1/netsim/ansible/initial-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/reload-config.ansible` & `networklab-1.8.2.dev1/netsim/ansible/reload-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/create-config.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/create-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/create-custom-config.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/create-custom-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-config/arubacx.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-config/cumulus.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-config/frr.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-config/linux-clab.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/linux-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-config/routeros.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-config/sonic.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/sonic.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-config/srlinux.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-config/sros.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-config/vyos.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-custom-config.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-custom-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/deploy-module.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-module.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/fetch-config/cumulus.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/fetch-config/srlinux.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 - name: Backup SR Linux node config user={{ ansible_user }}
   vars:
    ansible_connection: nokia.grpc.gnmi
    ansible_port: "{{ srlinux_grpc_port }}" # Uses gNMI over TLS to this port
    clab_base: "{{ hostname|replace('-'+inventory_hostname,'') }}"
    clab_ca_dir: "{{ inventory_dir }}/{{ clab_base }}/ca"
-   ansible_root_certificates_file: '{{ inventory_dir }}/clab-{{ netlab_name }}/.tls/ca/ca.pem'
+   ansible_root_certificates_file: '{{ clab_ca_dir }}/root/root-ca.pem'
    ansible_certificate_chain_file: ''
 
   nokia.grpc.gnmi_config:
    backup: yes
    backup_options:
     dir_path: "{{ config_dir }}"
     filename: "{{ inventory_hostname+'.config' }}"
```

### Comparing `networklab-1.8.2/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/frr/deploy-config.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/frr/deploy-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/linux/dhcp.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/linux/dhcp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/linux/initial-clab.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/linux/initial-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/readiness-check/vptx.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/vptx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/tasks/vmx/initial.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/vmx/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bfd/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bfd/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bfd/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bfd/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bfd/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bfd/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/arubacx.j2`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 {% import "arubacx.macro.j2" as bgpcfg %}
 !
 !
 router bgp {{ bgp.as }}
   bgp log-neighbor-changes
-  timers bgp connect-retry 10
 {% if bgp.router_id|ipv4 %}
   bgp router-id {{ bgp.router_id }}
 {% endif %}
 {% if bgp.rr|default(False) and bgp.rr_cluster_id|default(False) %}
   bgp cluster-id {{ bgp.rr_cluster_id }}
 {% endif %}
 {#
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/arubacx.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/arubacx.macro.j2`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 {% endif %}
 {%- endmacro %}
 {#
    Address family BGP neighbor definition
 #}
 {% macro neighbor_af(n,ip,bgp) %}
     neighbor {{ ip }} activate
-    neighbor {{ ip }} advertisement-interval 1
 {% if 'ibgp' in n.type %}
 {%   if bgp.community.ibgp|default([]) %}
     neighbor {{ ip }} send-community {{ community(bgp.community.ibgp) }}
 {%   endif %}
 {%   if bgp.next_hop_self is defined and bgp.next_hop_self %}
     neighbor {{ ip }} next-hop-self
 {%   endif %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/asa.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/asa.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/asa.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/cumulus_nvue.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/dellos10.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/ios.j2`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-{% import "dellos10.macro.j2" as bgpcfg %}
+{% import "ios.macro.j2" as bgpcfg %}
+!
+ip bgp-community new-format
 !
 router bgp {{ bgp.as }}
-  log-neighbor-changes
-
-! define a generic unnumbered template to be used for eBGP unnumbered...
-! additionally, need to define link-local-only-nexthop as per Dell suggested "Cumulus workaround"
-! WTF Dell...
-  template unnumbered_ebgp
-    link-local-only-nexthop
-    exit
-
+  no bgp default ipv4-unicast
+  bgp update-delay 5
+  bgp nopeerup-delay cold-boot 1
+  bgp nopeerup-delay user-initiated 1
 {% if bgp.router_id|ipv4 %}
-  router-id {{ bgp.router_id }}
+  bgp router-id {{ bgp.router_id }}
 {% endif %}
 {% if bgp.rr|default(False) and bgp.rr_cluster_id|default(False) %}
-  cluster-id {{ bgp.rr_cluster_id }}
-{% endif %}
-{% if bgp.rr|default('') %}
-  client-to-client reflection
+  bgp cluster-id {{ bgp.rr_cluster_id }}
 {% endif %}
+{#
+    Configure IPv4 and IPv6 BGP neighbors
+#}
 {% for n in bgp.neighbors %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined %}
-{{     bgpcfg.neighbor(n,n[af],bgp,af) }}
+{{     bgpcfg.neighbor_global(n,n[af]) }}
 {%   endfor %}
 {% endfor %}
 !
-{% for af in ['ipv4','ipv6'] %}
-{%   if bgp[af] is defined %}
+{# Configure BGP address families #}
+{% for af in ['ipv4','ipv6'] if bgp[af] is defined %}
+ address-family {{ af }}
+  bgp scan-time 5
 !
- address-family {{ af }} unicast
+{%   if loopback[af] is defined and bgp.advertise_loopback %}
+{{     bgpcfg.bgp_network(af,loopback[af]) }}
+{%   endif %}
 !
-{%     if loopback[af] is defined and bgp.advertise_loopback %}
-  network {{ loopback[af]|ipaddr('0') }}
-{%     endif %}
-!
-{%     for l in interfaces|default([]) if l.bgp.advertise|default("") and l[af] is defined and not 'vrf' in l %}
-  network {{ l[af]|ipaddr('0') }}
-{%     endfor %}
-!
-{%     for pfx in bgp.originate|default([]) if af == 'ipv4' %}
-  network {{ pfx|ipaddr('0') }}
-{%     endfor %}
+{%   for l in interfaces|default([]) if l.bgp.advertise|default("") and l[af] is defined and not 'vrf' in l %}
+{{     bgpcfg.bgp_network(af,l[af]) }}
+{%   endfor %}
+{%   for pfx in bgp.originate|default([]) if af == 'ipv4' %}
+{{     bgpcfg.bgp_network(af,pfx) }}
+{%   endfor %}
 !
-{%   endif %}
+{%   for n in bgp.neighbors if n[af] is defined and n.activate[af] is defined and n.activate[af] %}
+{{     bgpcfg.neighbor_af(n,n[af],bgp) }}
+{%   endfor %}
 {% endfor %}
 !
+{#
+  Add extra IPv4 prefixes
+#}
 {% for pfx in bgp.originate|default([]) %}
-ip route {{ pfx|ipaddr('0') }} interface null 0
+ip route {{ pfx|ipaddr('network') }} {{ pfx|ipaddr('netmask') }} null 0
 {% endfor %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/dellos10.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2`

 * *Files 12% similar despite different names*

```diff
@@ -33,28 +33,26 @@
 {%         endfor %}
 {%       endif %}
 
 {%       if bgp.rr|default('') and not n.rr|default('') %}
     route-reflector-client
 {%       endif %}
 {%       if bgp.community.ibgp|default([]) %}
-{%         if "standard" in bgp.community.ibgp|default([]) %}
-    send-community standard
-{%         endif %}
 {%         if "extended" in bgp.community.ibgp|default([]) %}
     send-community extended
+{%         else %}
+    send-community standard
 {%         endif %}
 {%       endif %}
 {%   else %}
 {%       if bgp.community.ebgp|default([]) %}
-{%         if "standard" in bgp.community.ebgp|default([]) %}
-    send-community standard
-{%         endif %}
 {%         if "extended" in bgp.community.ebgp|default([]) %}
     send-community extended
+{%         else %}
+    send-community standard
 {%         endif %}
 {%       endif %}
 {%     endif %}
 
 {% for af in ['ipv4','ipv6'] if bgp[af] is defined and n.activate[af] is defined and n.activate[af] %}
 !
  address-family {{ af }} unicast
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/eos.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/eos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/ios.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/ios.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/iosxr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/junos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/routeros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/routeros.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/routeros7.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros7.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 {% import "routeros7.macro.j2" as bgpcfg %}
 
 /routing/bgp/template add name=main as={{ bgp.as }} output.network=bgp-networks
 
 {% if bgp.router_id|ipv4 %}
 /routing/bgp/template set main router-id={{ bgp.router_id }}
 {% endif %}
-{% if bgp.rr|default(False) and bgp.rr_cluster_id|default(False) %}
-/routing/bgp/template set main cluster-id={{ bgp.rr_cluster_id }}
-{% endif %}
 
 {% for n in bgp.neighbors %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined %}
 {{     bgpcfg.neighbor(n,n[af],bgp,'main') }}
 {%   endfor %}
 {% endfor %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/routeros7.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/srlinux.cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/srlinux.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,96 @@
+{% macro bgp_policy(vrf,is_import,communities,vrf_context) %}
+{% set name = vrf + "_ebgp_" + ('import' if is_import else 'export') %}
+
+{% macro accept() %}
+{% if is_import or not communities %}
+      policy-result: "accept"
+{% else %}
+      policy-result: "accept"
+      # bgp:
+      #  communities:
+      #   add: "{{ name }}"
+{% endif %}
+{% endmacro %}
+
+- path: routing-policy/prefix-set[name={{vrf}}_export]
+  val:
+   prefix: [] # Make sure it exists
+
+- path: routing-policy/policy[name={{name}}]
+  val:
+   default-action:
+    policy-result: "reject"
+   statement:
+{% if is_import %}
+{%  for c in communities|default([]) %}
+   - name: {{ 10 + loop.index }}
+     match:
+      bgp:
+       community-set: "C{{ c|replace(':','_') }}"
+     action:
+{{    accept() }}
+{%  endfor %}
+{% else %}
+   - name: 5
+     match:
+      protocol: bgp
+      _annotate_protocol: "Accept and propagate prefixes received via BGP"
+     action:
+{{    accept() }}
+   - name: 10
+     match:
+      prefix-set: "{{ vrf }}_export"
+     action:
+{{    accept() }}
+{% endif %}
+{% endmacro %}
+
 {% macro bgp_export_prefix(vrf,prefix) %}
 - path: routing-policy/prefix-set[name={{vrf}}_export]
   val:
    prefix:
    - ip-prefix: {{ prefix }}
      mask-length-range: exact
 {% endmacro %}
 
 {% macro bgp_config(vrf,_as,router_id,vrf_bgp,vrf_context) %}
+
+{% if 'import' in vrf_context %}
+{% set import_policy = vrf + "_ebgp_import" %}
+{{ bgp_policy(vrf,1,vrf_context.import,vrf_context) }}
+{% else %}
+{% set import_policy = "accept_all" %}
+{% endif -%}
+
+{% set export_policy = vrf + "_ebgp_export" %}
+{{ bgp_policy(vrf,0,vrf_context.export|default({}),vrf_context) }}
+
 - path: network-instance[name={{vrf}}]/protocols/bgp
   val:
    admin-state: enable
    autonomous-system: {{ _as }}
    router-id: {{ router_id }}
    ebgp-default-policy:
     export-reject-all: False
     import-reject-all: False
-   import-policy: "accept_all"  # Set eBGP policy globally, override for iBGP
-   export-policy: "accept_all"
+   import-policy: {{ import_policy }}  # Set eBGP policy globally, override for iBGP
+   export-policy: {{ export_policy }}
 
 {# Configure BGP address families globally #}
 {% for af in ['ipv4','ipv6'] if af in vrf_context.af and vrf_context.af[af] %}
    afi-safi:
    - afi-safi-name: {{ af }}-unicast
      admin-state: enable
      multipath:
       max-paths-level-1: 64
       max-paths-level-2: 64 # indirect nexthops
 {% endfor %}
 
 {# Create route export policies #}
-- path: routing-policy/prefix-set[name={{vrf}}_export]
-  val:
-   prefix: [] # Make sure it exists
-
 {% for af in ['ipv4','ipv6'] if af in vrf_context.af and vrf_context.af[af] %}
 {% if loopback[af] is defined and bgp.advertise_loopback and vrf=='default' %}
 {{ bgp_export_prefix(vrf,loopback[af]|ipaddr('address')|ipaddr('host')) }}
 {% endif %}
 
 {% for l in interfaces|default([]) if l.bgp.advertise|default(0) and l[af]|default(False) is string and l.vrf|default('default')==vrf %}
 {{ bgp_export_prefix(vrf,l[af]|ipaddr('subnet')) }}
@@ -47,22 +101,22 @@
 {% endfor %}
 {% endfor %}
 
 {% macro bgp_families(neighbor,ipv4=True,ipv6=True) %}
 {% set activate = neighbor.activate|default( {'ipv4': True,'ipv6': True } ) %}
    afi-safi:
    - afi-safi-name: ipv4-unicast
-     admin-state: {{ 'enable' if activate.ipv4|default(False) else 'disable' }}
+     admin-state: {{ 'enable' if activate.ipv4|default(False) and ipv4 else 'disable' }}
 {% if neighbor.ipv4_rfc8950|default(False) %}
      ipv4-unicast:
       advertise-ipv6-next-hops: True
       receive-ipv6-next-hops: True
 {% endif %}
    - afi-safi-name: ipv6-unicast
-     admin-state: {{ 'enable' if activate.ipv6|default(False) else 'disable' }}
+     admin-state: {{ 'enable' if activate.ipv6|default(False) and ipv6 else 'disable' }}
 {% if 'evpn' in neighbor and neighbor.evpn %}
    - afi-safi-name: evpn
      admin-state: enable # Must have at least 1 address family enabled
 {% endif %}
 {% endmacro %}
 
 {% macro bgp_peer_group(name,type,neighbor,transport_ip) %}
@@ -129,15 +183,15 @@
 {% endif %}
 {% if n.local_as is defined %}
      local-as:
       as-number: {{ n.local_as }}
       prepend-global-as: {{ not n.replace_global_as|default(True) }} # Don't include iBGP global AS in eBGP advertisements
 {% endif %}
 
-{% elif n[af]==True %}
+{% elif n[af]==True and af=='ipv6' %}
 {# BGP unnumbered for IPv6 LLA, not supported in combination with evpn #}
 {% if 'evpn' in n %}
 {{ raise_error | mandatory( 'EVPN not supported for BGP unnumbered peers' ) }}
 {% endif %}
 
 {% set peer_group = n.type + "-unnumbered" + (('-' + n.local_as|string()) if n.local_as is defined else '') %}
 {{ bgp_peer_group(peer_group,n.type,n,None) }}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/sros.gnmi.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/sros.md-cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/sros.openconfig.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/bgp/vyos.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/vyos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/dhcp/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/dhcp/dnsmasq.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/dnsmasq.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/dhcp/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/dhcp/eos.server.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/eos.server.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/dhcp/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/dhcp/ios.server.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/ios.server.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/eigrp/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/eigrp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/eigrp/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/eigrp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/evpn/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/evpn/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/evpn/dellos10.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/evpn/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/evpn/frr.evpn-config.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/evpn/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/evpn/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/evpn/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/evpn/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/gateway/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/gateway/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/gateway/dellos10.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/gateway/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/gateway/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/gateway/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/gateway/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/gateway/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/gateway/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/arcos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/arcos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/asa.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/cumulus_nvue.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/dellos10.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/ios.j2`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,91 @@
-hostname {{ inventory_hostname.replace("_","-") }}
+hostname {{ inventory_hostname }}
 !
-lldp enable
+no ip domain lookup
 !
-{% if vrfs is defined %}
-{% include 'dellos10.vrf.j2' %}
-{% endif %}
+lldp run
 !
-{% for k,v in hostvars.items() if k != inventory_hostname and v.af.ipv4|default(False) and v.loopback.ipv4 is defined %}
-ip host {{ k|replace('_','') }} {{ v.loopback.ipv4|ipaddr('address') }}
+{% for hname,hdata in hosts.items() if hname != inventory_hostname %}
+{%   set addr_list = hdata.ipv4|default([]) + hdata.ipv6|default([]) %}
+ip host {{ hname }} {{ addr_list|join (' ') }}
 {% endfor %}
 !
-{% if mtu is defined %}
+{% if af.ipv6|default(False) %}
+ipv6 unicast-routing
 !
-{# Dell wanted the MTU to be supplied as IP MTU + 32 #}
-default mtu {{ mtu + 32 }}
 {% endif %}
+{% if vrfs is defined %}
+{% include 'ios.vrf.j2' +%}
 !
-interface loopback0
-{% if 'ipv4' in loopback %}
- ip address {{ loopback.ipv4 }}
 {% endif %}
-{% if 'ipv6' in loopback %}
- ipv6 address {{ loopback.ipv6 }}
+{% if vlans is defined %}
+{% include netlab_device_type ~ '.vlan.j2' +%}
+!
 {% endif %}
 !
-interface {{ mgmt.ifname|default('mgmt1/1/1') }}
+{% if loopback is defined %}
+interface {{ loopback.ifname }}
+{%   if 'ipv4' in loopback %}
+ ip address {{ loopback.ipv4|ipaddr('address') }} {{ loopback.ipv4|ipaddr('netmask') }}
+{%   endif %}
+{%   if 'ipv6' in loopback %}
+ ipv6 address {{ loopback.ipv6|upper }}
+{%   endif %}
+{% endif %}
+!
+interface {{ mgmt.ifname|default('GigabitEthernet0/0') }}
  no lldp transmit
  no lldp receive
 !
 {% for l in interfaces|default([]) %}
 interface {{ l.ifname }}
  no shutdown
-{%   if l.virtual_interface is not defined %}
- no switchport
-{%   endif %}
-{% if l.vrf is defined %}
- ip vrf forwarding {{ l.vrf }}
+{% if l.type == 'vlan_member' and l.vlan.access_id is defined %}
+ encapsulation dot1Q {{ l.vlan.access_id }}
 {% endif %}
-{% if l.mtu is defined %}
- mtu {{ l.mtu + 32 }}
+{% if l.vrf is defined %}
+ vrf forwarding {{ l.vrf }}
 {% endif %}
 {% if l.name is defined %}
- description "{{ l.name | replace(",", "\\\\,") }}{{ " ["+l.role+"]" if l.role is defined else "" }}"
+ description {{ l.name }}{{ " ["+l.role+"]" if l.role is defined else "" }}
 {% elif l.type|default("") == "stub" %}
- description "Stub interface"
+ description Stub interface
+{% endif %}
+{% if l.bandwidth is defined %}
+ bandwidth {{ l.bandwidth  }}
+{% endif %}
+{% if l.mtu is defined %}
+{%   if min_mtu is defined and min_mtu > l.mtu %}
+ ip mtu {{ l.mtu }}
+{%   else %}
+ mtu {{ l.mtu }}
+{%   endif %}
 {% endif %}
 {#
-    Set interface IPv4 addresses
+    Set interface addresses: IPv4
 #}
 {% if 'ipv4' in l %}
-{%   if l.ipv4|ipv4 %}
- ip address {{ l.ipv4 }}
+{%   if l.ipv4 == True %}
+ ip unnumbered {{ l._parent_intf }} poll
+{%   elif l.ipv4|ipv4 %}
+ ip address {{ l.ipv4|ipaddr('address') }} {{ l.ipv4|ipaddr('netmask') }}
 {%   else %}
 ! Invalid IPv4 address {{ l.ipv4 }}
 {%   endif %}
 {% endif %}
 {#
-    Set interface IPv6 addresses
+    Set interface addresses: IPv6
 #}
 {% if 'ipv6' in l %}
-{# do not set nd on loopback interfaces #}
-{%   if l.type|default('') != 'loopback' %}
- ipv6 nd max-ra-interval 4
- ipv6 nd min-ra-interval 3
- ipv6 nd send-ra
-{%   endif %}
 {%   if l.ipv6 == True %}
  ipv6 enable
 {%   elif l.ipv6|ipv6 %}
- ipv6 address {{ l.ipv6 }}
+ ipv6 address {{ l.ipv6|upper }}
 {%   else %}
 ! Invalid IPv6 address {{ l.ipv6 }}
 {%   endif %}
 {% endif %}
 !
 {% endfor %}
+no banner exec
+no banner login
+no banner incoming
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/dellos10.vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/frr.j2`

 * *Files 13% similar despite different names*

```diff
@@ -44,36 +44,14 @@
   echo "FRR already installed, skipping installation"
 else
   curl -s https://deb.frrouting.org/frr/keys.asc | apt-key add -
   FRRVER="frr-stable"
   echo deb https://deb.frrouting.org/frr $(lsb_release -s -c) $FRRVER > /etc/apt/sources.list.d/frr.list
   apt-get update -qq && apt-get install -qq frr frr-pythontools
 fi
-{% else %}
-{%   if netlab_mgmt_vrf|default(False) %}
-#
-# Get the current next hop for the default route
-#
-def_nh=$(ip route list default|awk '{ print $3 }')
-#
-# Create the management VRF and add eth0 to it
-#
-if [ ! -e /sys/devices/virtual/net/mgmt ]; then
-  ip link add mgmt type vrf table 42
-fi
-ip link set mgmt up
-sysctl -qw net.ipv6.conf.eth0.keep_addr_on_down=1
-ip link set eth0 master mgmt
-#
-# Reinstall the default route if we had it before
-#
-if [[ -n "$def_nh" ]]; then
-  ip route add 0.0.0.0/0 vrf mgmt via $def_nh
-fi
-{%   endif %}
 {% endif %}
 #
 # Enable FRR modules (if not using containerlab bind-mounted /etc/frr/daemons)
 #
 {% if clab is not defined or clab.binds|default({})=={} %}
 {% set modlist = {'bfd':'bfdd','bgp':'bgpd','ospf':['ospfd','ospf6d'],'isis':'isisd','vrf':'bgpd','mpls':'ldpd'} %}
 {% for m in module|default([]) if modlist[m] is defined %}
@@ -120,19 +98,14 @@
 {% endfor %}
 #
 # Rest of initial configuration done through VTYSH
 #
 cat >/tmp/config <<CONFIG
 hostname {{ inventory_hostname }}
 !
-{% if clab is defined %}
-vrf mgmt
- exit-vrf
-!
-{% endif %}
 {% if 'ipv6' in af %}
 ipv6 forwarding
 {% endif %}
 {% set frr_defaults = netlab_frr_defaults|default('datacenter') %}
 frr defaults {{ frr_defaults }}
 !
 {% for l in netlab_interfaces %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/nxos.j2`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,76 @@
-hostname {{ inventory_hostname }}
-!
-no ip domain lookup
+{#
+  NXOS hates single-character hostnames. Prepend 'nxos-' to hostname if it's too short
+#}
+hostname {{ 'nxos-' if inventory_hostname|length == 1 else '' }}{{ inventory_hostname }}
 !
-lldp run
+no ip domain-lookup
 !
-{% for hname,hdata in hosts.items() if hname != inventory_hostname %}
-{%   set addr_list = hdata.ipv4|default([]) + hdata.ipv6|default([]) %}
-ip host {{ hname }} {{ addr_list|join (' ') }}
-{% endfor %}
+feature lldp
 !
-{% if af.ipv6|default(False) %}
-ipv6 unicast-routing
+username vagrant password vagrant
 !
-{% endif %}
-{% if vrfs is defined %}
-{% include 'ios.vrf.j2' +%}
+{% for hname,hdata in hosts.items() if 'ipv4' in hdata and hname != inventory_hostname %}
+ip host {{ hname }} {{ hdata.ipv4[0] }}
+{% endfor %}
 !
-{% endif %}
 {% if vlans is defined %}
-{% include netlab_device_type ~ '.vlan.j2' +%}
-!
+feature interface-vlan
 {% endif %}
+{% if vrfs is defined %}
+{% include 'nxos.vrf.j2' %}
 !
-{% if loopback is defined %}
-interface {{ loopback.ifname }}
-{%   if 'ipv4' in loopback %}
- ip address {{ loopback.ipv4|ipaddr('address') }} {{ loopback.ipv4|ipaddr('netmask') }}
-{%   endif %}
-{%   if 'ipv6' in loopback %}
- ipv6 address {{ loopback.ipv6|upper }}
-{%   endif %}
 {% endif %}
 !
 interface {{ mgmt.ifname|default('GigabitEthernet0/0') }}
  no lldp transmit
  no lldp receive
 !
-{% for l in interfaces|default([]) %}
+{% for l in netlab_interfaces %}
 interface {{ l.ifname }}
  no shutdown
-{% if l.type == 'vlan_member' and l.vlan.access_id is defined %}
- encapsulation dot1Q {{ l.vlan.access_id }}
+{% if l.virtual_interface is not defined %}
+ no switchport
+ mac-address {{ '52dc.cafe.%02d%02d' % ( id,l.ifindex ) }}
 {% endif %}
 {% if l.vrf is defined %}
- vrf forwarding {{ l.vrf }}
+  vrf member {{ l.vrf }}
 {% endif %}
 {% if l.name is defined %}
  description {{ l.name }}{{ " ["+l.role+"]" if l.role is defined else "" }}
 {% elif l.type|default("") == "stub" %}
  description Stub interface
 {% endif %}
 {% if l.bandwidth is defined %}
  bandwidth {{ l.bandwidth  }}
 {% endif %}
 {% if l.mtu is defined %}
-{%   if min_mtu is defined and min_mtu > l.mtu %}
- ip mtu {{ l.mtu }}
-{%   else %}
  mtu {{ l.mtu }}
-{%   endif %}
 {% endif %}
 {#
-    Set interface addresses: IPv4
+    IPv4 addresses
 #}
 {% if 'ipv4' in l %}
 {%   if l.ipv4 == True %}
- ip unnumbered {{ l._parent_intf }} poll
+ medium p2p
+ ip unnumbered loopback0
 {%   elif l.ipv4|ipv4 %}
- ip address {{ l.ipv4|ipaddr('address') }} {{ l.ipv4|ipaddr('netmask') }}
+ ip address {{ l.ipv4 }}
 {%   else %}
 ! Invalid IPv4 address {{ l.ipv4 }}
 {%   endif %}
 {% endif %}
 {#
-    Set interface addresses: IPv6
+    IPv6 addresses
 #}
 {% if 'ipv6' in l %}
 {%   if l.ipv6 == True %}
- ipv6 enable
+ ipv6 address use-link-local-only
 {%   elif l.ipv6|ipv6 %}
- ipv6 address {{ l.ipv6|upper }}
+ ipv6 address {{ l.ipv6 }}
 {%   else %}
 ! Invalid IPv6 address {{ l.ipv6 }}
 {%   endif %}
+ ipv6 nd ra-interval 5 min 3
 {% endif %}
 !
 {% endfor %}
-no banner exec
-no banner login
-no banner incoming
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/iosxr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/junos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/junos.vlan.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/junos.vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/linux/hosts.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/linux/ubuntu.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/linux/vanilla.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/vanilla.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/dellos10.j2`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,74 @@
-{#
-  NXOS hates single-character hostnames. Prepend 'nxos-' to hostname if it's too short
-#}
-hostname {{ 'nxos-' if inventory_hostname|length == 1 else '' }}{{ inventory_hostname }}
+hostname {{ inventory_hostname.replace("_","-") }}
 !
-no ip domain-lookup
+lldp enable
 !
-feature lldp
-!
-username vagrant password vagrant
+{% if vrfs is defined %}
+{% include 'dellos10.vrf.j2' %}
+{% endif %}
 !
-{% for hname,hdata in hosts.items() if 'ipv4' in hdata and hname != inventory_hostname %}
-ip host {{ hname }} {{ hdata.ipv4[0] }}
+{% for k,v in hostvars.items() if k != inventory_hostname and v.af.ipv4|default(False) and v.loopback.ipv4 is defined %}
+ip host {{ k|replace('_','') }} {{ v.loopback.ipv4|ipaddr('address') }}
 {% endfor %}
 !
-{% if vlans is defined %}
-feature interface-vlan
+{% if mtu is defined %}
+!
+{# Dell wanted the MTU to be supplied as IP MTU + 32 #}
+default mtu {{ mtu + 32 }}
 {% endif %}
-{% if vrfs is defined %}
-{% include 'nxos.vrf.j2' %}
 !
+interface loopback0
+{% if 'ipv4' in loopback %}
+ ip address {{ loopback.ipv4 }}
+{% endif %}
+{% if 'ipv6' in loopback %}
+ ipv6 address {{ loopback.ipv6 }}
 {% endif %}
 !
-interface {{ mgmt.ifname|default('GigabitEthernet0/0') }}
+interface {{ mgmt.ifname|default('mgmt1/1/1') }}
  no lldp transmit
  no lldp receive
 !
-{% for l in netlab_interfaces %}
+{% for l in interfaces|default([]) %}
 interface {{ l.ifname }}
  no shutdown
-{% if l.virtual_interface is not defined %}
+{%   if l.virtual_interface is not defined %}
  no switchport
- mac-address {{ '52dc.cafe.%02d%02d' % ( id,l.ifindex ) }}
-{% endif %}
+{%   endif %}
 {% if l.vrf is defined %}
-  vrf member {{ l.vrf }}
+ ip vrf forwarding {{ l.vrf }}
+{% endif %}
+{% if l.mtu is defined %}
+ mtu {{ l.mtu + 32 }}
 {% endif %}
 {% if l.name is defined %}
- description {{ l.name }}{{ " ["+l.role+"]" if l.role is defined else "" }}
+ description "{{ l.name | replace(",", "\\\\,") }}{{ " ["+l.role+"]" if l.role is defined else "" }}"
 {% elif l.type|default("") == "stub" %}
- description Stub interface
-{% endif %}
-{% if l.bandwidth is defined %}
- bandwidth {{ l.bandwidth  }}
-{% endif %}
-{% if l.mtu is defined %}
- mtu {{ l.mtu }}
+ description "Stub interface"
 {% endif %}
 {#
-    IPv4 addresses
+    Set interface IPv4 addresses
 #}
 {% if 'ipv4' in l %}
-{%   if l.ipv4 == True %}
- medium p2p
- ip unnumbered loopback0
-{%   elif l.ipv4|ipv4 %}
+{%   if l.ipv4|ipv4 %}
  ip address {{ l.ipv4 }}
 {%   else %}
 ! Invalid IPv4 address {{ l.ipv4 }}
 {%   endif %}
 {% endif %}
 {#
-    IPv6 addresses
+    Set interface IPv6 addresses
 #}
 {% if 'ipv6' in l %}
+ ipv6 nd max-ra-interval 4
+ ipv6 nd min-ra-interval 3
+ ipv6 nd send-ra
 {%   if l.ipv6 == True %}
- ipv6 address use-link-local-only
+ ipv6 enable
 {%   elif l.ipv6|ipv6 %}
  ipv6 address {{ l.ipv6 }}
 {%   else %}
 ! Invalid IPv6 address {{ l.ipv6 }}
 {%   endif %}
- ipv6 nd ra-interval 5 min 3
 {% endif %}
 !
 {% endfor %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/routeros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/routeros.vlan.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/routeros7.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/routeros7.vlan.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/sonic.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/sonic.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/srlinux.cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/srlinux.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 {% macro ip_addresses(name,index,intf,ipv6_ra=True,is_system=False) %}
 - path: interface[name={{name}}]/subinterface[index={{index}}]
   val:
    description: "{{ intf.name | default( 'No description' )|replace('->','~')|regex_replace('[\\[\\]]','') }}"
-{% if 'ipv4' in intf %}
+{% if 'ipv4' in intf and intf.ipv4 is string %}
    ipv4:
     admin-state: enable
-{%   if intf.ipv4|bool %}
-    unnumbered:
-      admin-state: enable
-      interface: "system0.0"
-{%   else %}
     address:
     - ip-prefix: "{{ intf.ipv4 }}"
-{%     if not is_system %}
+{% if not is_system %}
       primary: [null]
-{%     endif %}
-{%   endif %}
+{% endif %}
 {% endif %}
 {% if 'ipv6' in intf %}
    ipv6:
     admin-state: enable
 {%   if intf.ipv6 is string %}
     address:
     - ip-prefix: "{{ intf.ipv6 }}"
@@ -36,34 +30,32 @@
 {% endif %}
 {% endif %}
 {% endmacro %}
 
 updates:
 {% if mtu is defined %}
 {% if (clab.type in ['ixr6','ixr10'] and (mtu+14)>9486)
-   or (clab.type in ['ixrd1','ixrd2','ixrd3','ixrh1','ixrh2','ixrh3','ixrd2l','ixrd3l'] and (mtu+14)>9398) %}
+   or (clab.type in ['ixrd1','ixrd2','ixrd3','ixrh1','ixrh2'] and (mtu+14)>9398) %}
 {{ mtu_too_large | mandatory( 'IP MTU '+str(mtu)+' too large for given hardware platform: ' + clab.type ) }}
 {% else %}
 - path: system/mtu
   val:
    default-port-mtu: {{ [mtu + 14,1500]|max }}
-{%  if 'ixrh' not in clab.type %}
    default-l2-mtu: {{ [mtu + 14,1500]|max }}
-{%  endif %}
    default-ip-mtu: {{ mtu }}
    _annotate_default-ip-mtu: "Custom system wide setting, overrides default 1500"
 {% endif %}
 {% endif %}
 
 {{  ip_addresses('system0',0,loopback,False,True)  }}
 
 {% for l in interfaces|default([]) if l.vlan is not defined and l.subif_index is not defined %}
 {% set if_name_index = l.ifname.split('.') %}
-{% set if_name = if_name_index[0] %}
-{% set if_index = if_name_index[1] if if_name_index|length > 1 else '0' %}
+{% set if_name = if_name_index[0] if l.type!='stub' else "lo0" %}
+{% set if_index = if_name_index[1] if if_name_index|length > 1 else l.ifindex if l.type=='stub' else '0' %}
 {% set if_desc = l.name|default( l.ifname )|replace('->','~')|regex_replace('[\\[\\]]','') %}
 - path: interface[name={{ if_name }}]
   val:
 {% if l.mtu is defined and l.type!='loopback' %} # min 1500; max 9412 for 7220, 9500 for 7250 platforms
    mtu: {{ [l.mtu + 14,1500]|max }}
 {% endif %}
    subinterface:
@@ -75,16 +67,16 @@
 
 {{ ip_addresses(if_name,if_index,l) }}
 {% endfor %}
 
 {% macro list_interfaces(vrf) %}
 {% for l in interfaces|default([]) if l.vlan is not defined and l.subif_index is not defined and l.vrf|default('default')==vrf %}
 {% set if_name_index = l.ifname.split('.') %}
-{% set if_name = if_name_index[0] %}
-{% set if_index = if_name_index[1] if if_name_index|length > 1 else '0' %}
+{% set if_name = if_name_index[0] if l.type!='stub' else "lo0" %}
+{% set if_index = if_name_index[1] if if_name_index|length > 1 else l.ifindex if l.type=='stub' else '0' %}
 - path: network-instance[name={{ vrf }}]
   val:
    type: {{ 'default' if vrf=='default' else 'ip-vrf' }}
    interface:
    - name: {{ if_name }}.{{ if_index }}
 {% endfor %}
 {% endmacro %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/sros.md-cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/sros.openconfig.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/initial/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/vyos.j2`

 * *Files 5% similar despite different names*

```diff
@@ -96,9 +96,7 @@
 
 # Commit, save and exit from subshell
 
 commit
 save
 exit
 
-# Restart FRR to pick up the new hostname
-sudo service frr restart
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/isis/asa.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/isis/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/isis/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/frr.j2`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 {% endif %}
 !
 router isis Gandalf
   log-adjacency-changes
   hostname dynamic
   is-type {{ isis.type }}
   metric-style wide
-  lsp-timers gen-interval 1 refresh-interval 900 max-lifetime 1800
 {% if isis.net is defined %}
   net {{ isis.net }}
 {% elif isis.area is defined %}
   net {{ "%s.0000.0000.%04d.00" % (isis.area,id) }}
 {% endif %}
 {% if isis.af.ipv6 is defined %}
   topology ipv6-unicast
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/isis/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/ios.j2`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 {% if 'ipv6' in isis.af %}
 ipv6 unicast-routing
 {% endif %}
 !
+router isis Gandalf
+  log-adjacency-changes
+  hostname dynamic
+  is-type {{ isis.type }}
+  metric-style wide
+{% if isis.net is defined %}
+  net {{ isis.net }}
+{% elif isis.area is defined %}
+  net {{ "%s.0000.0000.%04d.00" % (isis.area,id) }}
+{% endif %}
+{% for l in interfaces|default([]) if 'isis' in l and l.isis.passive %}
+  passive-interface {{ l.ifname }}
+{% endfor %}
+{% if isis.af.ipv6 is defined %}
+  address-family ipv6
+    multi-topology
+{% endif %}
+!
 interface Loopback0
 {% if 'ipv4' in loopback and 'ipv4' in isis.af %}
   ip router isis Gandalf
 {% endif %}
 {% if 'ipv6' in loopback and 'ipv6' in isis.af %}
   ipv6 router isis Gandalf
 {% endif %}
@@ -32,25 +50,7 @@
   isis bfd
 {%   endif %}
 {%   if l.isis.bfd.ipv6|default(False) %}
   isis ipv6 bfd
 {%   endif %}
 !
 {% endfor %}
-!
-router isis Gandalf
-  log-adjacency-changes
-  hostname dynamic
-  is-type {{ isis.type }}
-  metric-style wide
-{% if isis.net is defined %}
-  net {{ isis.net }}
-{% elif isis.area is defined %}
-  net {{ "%s.0000.0000.%04d.00" % (isis.area,id) }}
-{% endif %}
-{% for l in interfaces|default([]) if 'isis' in l and l.isis.passive %}
-  passive-interface {{ l.ifname }}
-{% endfor %}
-{% if isis.af.ipv6 is defined %}
-  address-family ipv6
-    multi-topology
-{% endif %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/isis/iosxr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/isis/junos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/isis/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/isis/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/srlinux.j2`

 * *Files 4% similar despite different names*

```diff
@@ -29,28 +29,28 @@
 {%    set ifname = l.ifname if '.' in l.ifname else l.ifname|replace('vlan','irb0.') if l.type=='svi' else (l.ifname+'.0') %}
 {%    if "isis" not in l %}
      # IS-IS not configured on external interface {{ ifname }}
 {%    else %}
      - interface-name: {{ ifname }}
        circuit-type: {{ l.isis.network_type|default("broadcast") }}
        passive: {{ l.isis.passive }}
+{%     if 'ipv4' in l and 'ipv4' in isis.af %}
        ipv4-unicast:
-        admin-state: {{ 'enable' if 'ipv4' in l and 'ipv4' in isis.af else 'disable' }}
+        admin-state: enable
         enable-bfd: {{ l.isis.bfd.ipv4|default(False) }}
+{%     endif %}
 {%     if 'ipv6' in l and 'ipv6' in isis.af  %}
        ipv6-unicast:
         admin-state: enable
         enable-bfd: {{ l.isis.bfd.ipv6|default(False) }}
 {%     endif %}
 {%     if l.isis.metric is defined or l.isis.cost is defined %}
        level:
-{%      if isis.type!='level-2' %}
        - level-number: 1
+         metric-style: wide
          metric: {{ l.isis.metric|default(l.isis.cost) }}
-{%      endif %}
-{%      if isis.type!='level-1' %}
        - level-number: 2
+         metric-style: wide
          metric: {{ l.isis.metric|default(l.isis.cost) }}
-{%      endif %}
 {%     endif %}
 {%    endif %}
 {%   endfor %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/isis/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/isis/sros.openconfig.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/isis/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/eos.6pe.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.6pe.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/eos.bgp-lu.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/frr.ldp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/frr.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/ios.bgp-lu.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/junos.ldp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/junos.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/junos.mplsvpn.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/srlinux.ldp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/srlinux.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/sros.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/sros.ldp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/sros.mplsvpn.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/mpls/vyos.mplsvpn.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/arubacx.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/arubacx.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/cumulus.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/cumulus.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/cumulus_nvue.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/dellos10.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/dellos10.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/eos.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/eos.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/frr.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/frr.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/ios.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/ios.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 {%   endif %}
 {% endif %}
 !
 {% for l in intf_data if 'ospf' in l and ('ipv6' in l or 'ipv6' in l.dhcp.client|default({})) %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
  ospfv3 {{ ospf_pid }} ipv6 area {{ l.ospf.area }}
-{%   if l.ospf.network_type is defined %}
+{%   if l.type == 'loopback' %}
+ ospfv3 network point-to-point
+{%   elif l.ospf.network_type is defined %}
  ospfv3 network {{ l.ospf.network_type }}
 {%   endif %}
 {%   if l.ospf.cost is defined %}
  ospfv3 cost {{ l.ospf.cost }}
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
  ospfv3 bfd
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/iosxr.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/iosxr.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/junos.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/junos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/nxos.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/nxos.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 !
 {% for l in netlab_interfaces if 'ospf' in l and 'ipv6' in l %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
  ipv6 router ospfv3 {{ pid }} area {{ l.ospf.area }}
 {%   if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
  ospfv3 network {{ l.ospf.network_type }}
+{%   elif l.type == 'loopback' %}
+ ospfv3 network point-to-point
 {%   endif %}
 {%   if l.ospf.cost is defined %}
  ospfv3 cost {{ l.ospf.cost }}
 {%   endif %}
 {%   if l.ospf.passive|default(False) %}
  ospfv3 passive-interface
 {%   endif %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/routeros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/routeros7.ospf-include.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/srlinux.cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/srlinux.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-{% macro format_area(a) -%}
-{{ '0.0.0.0' if not a else a | ipv4 }}
-{%- endmacro %}
-
 {% macro ospf_config(pid,af,vrf,ospf,vrf_interfaces) %}
 - path: network-instance[name={{ vrf|default('default') }}]
   val:
    router-id: {{ ospf.router_id }}
    protocols:
     ospf:
      instance:
@@ -20,27 +16,27 @@
        ldp-synchronization: { }
 {% endif %}
 {%     if ospf.reference_bandwidth is defined %}
        reference-bandwidth: {{ ospf.reference_bandwidth * 1000 }} # in kbps
 {%     endif %}
        area:
 {%     if vrf=='default' %}
-       - area-id: {{ format_area(ospf.area) }}
+       - area-id: {{ ospf.area }}
          interface:
          - interface-name: system0.0
            passive: True
 {%     endif %}
 {%     for l in vrf_interfaces if (l.vlan is not defined or l.vlan.mode|default('irb')!='bridge') and l.subif_index is not defined %}
 {%      set if_name_index = l.ifname.split('.') %}
 {%      set if_name = if_name_index[0] if l.type!='stub' else "lo0" %}
 {%      set if_index = if_name_index[1] if if_name_index|length > 1 else l.ifindex if l.type=='stub' else '0' %}
 {%      if 'ospf' not in l %}
        # OSPF not configured on external interface {{ if_name }}
 {%      else %}
-       - area-id: {{ format_area(l.ospf.area) }}
+       - area-id: {{ l.ospf.area }}
          interface:
          - interface-name: {{ if_name }}.{{ if_index }}
 {%         if l.ospf.passive | default(False) %}
            passive: True
 {%         endif %}
 {%         if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
            interface-type: "{{ l.ospf.network_type }}"
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.j2`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 {% macro ospf_interface(l) %}
 {{ declare_router(l,sub_path="/"+ospfv+"[ospf-instance="+pid|string + "]") }}
   val:
 {%  if ospf.reference_bandwidth is defined %}
    reference-bandwidth: {{ ospf.reference_bandwidth * 1000 }} # in kbps
 {%  endif %}
    admin-state: enable
-   router-id: {{ ospf.router_id }}
    area:
    - area-id: "{{ l.ospf.area }}"
      interface:
      - interface-name: "{{ if_name(l,l.ifname) }}"
 {%  if l.ospf.passive|default(False) %}
        passive: True
 {%  endif %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/sros.md-cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/sros.openconfig.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/vyos.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/ospf/vyos.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/sr/junos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/sr/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/sr/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/sr/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/sr/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/sr/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/sr/sros.openconfig.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/sr/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/srv6/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/srv6/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/csr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/dellos10.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/routeros7.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/vmx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vmx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/vptx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vptx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vlan/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 {% endif %}
 {%- endmacro %}
 {#
    Address family BGP neighbor definition
 #}
 {% macro neighbor_af(n,ip,bgp) %}
     neighbor {{ ip }} activate
-    neighbor {{ ip }} advertisement-interval 1
 {% if 'ibgp' in n.type %}
 {%   if bgp.community.ibgp|default([]) %}
     neighbor {{ ip }} send-community {{ community(bgp.community.ibgp) }}
 {%   endif %}
 {%   if bgp.next_hop_self is defined and bgp.next_hop_self %}
     neighbor {{ ip }} next-hop-self
 {%   endif %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/arubacx.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2`

 * *Files 12% similar despite different names*

```diff
@@ -33,28 +33,26 @@
 {%         endfor %}
 {%       endif %}
 
 {%       if bgp.rr|default('') and not n.rr|default('') %}
     route-reflector-client
 {%       endif %}
 {%       if bgp.community.ibgp|default([]) %}
-{%         if "standard" in bgp.community.ibgp|default([]) %}
-    send-community standard
-{%         endif %}
 {%         if "extended" in bgp.community.ibgp|default([]) %}
     send-community extended
+{%         else %}
+    send-community standard
 {%         endif %}
 {%       endif %}
 {%   else %}
 {%       if bgp.community.ebgp|default([]) %}
-{%         if "standard" in bgp.community.ebgp|default([]) %}
-    send-community standard
-{%         endif %}
 {%         if "extended" in bgp.community.ebgp|default([]) %}
     send-community extended
+{%         else %}
+    send-community standard
 {%         endif %}
 {%       endif %}
 {%     endif %}
 
 {% for af in ['ipv4','ipv6'] if bgp[af] is defined and n.activate[af] is defined and n.activate[af] %}
 !
  address-family {{ af }} unicast
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/dellos10.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 {% import "dellos10.bgp-macro.j2" as bgpcfg %}
 !
 router bgp {{ bgp.as }}
 {% for vname,vdata in vrfs.items() %}
 !
  vrf {{ vname }}
   router-id {{ bgp.router_id }}
-! need to define unnumbered template also at vrf-level
-  template unnumbered_ebgp
-    link-local-only-nexthop
-    exit
-
 
 {%   for n in vdata.bgp.neighbors|default([]) %}
 {%     for af in ['ipv4','ipv6'] if n[af] is defined %}
 {{       bgpcfg.neighbor(n,n[af],bgp,af) }}
 {%     endfor %}
 {%   endfor %}
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/eos.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/eos.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/eos.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/eos.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/frr.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/frr.frr-config.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.frr-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/frr.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/frr.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/ios.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/ios.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/ios.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/ios.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv3.j2`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 {%   endif %}
 {% endif %}
 !
 {% for l in intf_data if 'ospf' in l and ('ipv6' in l or 'ipv6' in l.dhcp.client|default({})) %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
  ospfv3 {{ ospf_pid }} ipv6 area {{ l.ospf.area }}
-{%   if l.ospf.network_type is defined %}
+{%   if l.type == 'loopback' %}
+ ospfv3 network point-to-point
+{%   elif l.ospf.network_type is defined %}
  ospfv3 network {{ l.ospf.network_type }}
 {%   endif %}
 {%   if l.ospf.cost is defined %}
  ospfv3 cost {{ l.ospf.cost }}
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
  ospfv3 bfd
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/junos.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/junos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/junos.ospf-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.ospf-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/nxos.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/routeros.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/routeros.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/routeros7.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% import "routeros7.bgp-macro.j2" as bgpcfg %}
 
 {% for vname,vdata in vrfs.items() %}
 {#
     First of all, need to add the vrf to the default instance (for VPNv4)
 #}
-/routing/bgp/vpn add label-allocation-policy=per-vrf vrf={{ vname }} route-distinguisher={{ vdata.rd }} import.route-targets={{ vdata.import|join(',') }} export.route-targets={{ vdata.export|join(',') }} export.redistribute=bgp,connected,ospf,static,vpn
+/routing/bgp/vpn add label-allocation-policy=per-vrf vrf={{ vname }} route-distinguisher={{ vdata.rd }} import-route-targets={{ vdata.import|join(',') }} export-route-targets={{ vdata.export|join(',') }}
 
 {#
     Create BGP template/instance
 #}
-/routing/bgp/template add name=vrf_{{ vname }} as={{ bgp.as }} output.network=bgp-networks-{{ vname }} vrf={{ vname }} routing-table={{ vname }} output.redistribute=connected,bgp,bgp-mpls-vpn,vpn
+/routing/bgp/template add name=vrf_{{ vname }} as={{ bgp.as }} output.network=bgp-networks-{{ vname }} vrf={{ vname }} routing-table={{ vname }} output.redistribute=connected,bgp,copy
 
 {% if bgp.router_id|ipv4 %}
 /routing/bgp/template set vrf_{{ vname }} router-id={{ bgp.router_id }}
 {% endif %}
 
 {% if 'ospf' in vdata %}
 /routing/bgp/template set vrf_{{ vname }} output.redistribute=([get vrf_{{ vname }} output.redistribute],"ospf")
```

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/routeros7.ospf-include.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/vyos.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/vyos.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vxlan/csr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vxlan/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vxlan/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vxlan/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vxlan/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vxlan/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/ansible/templates/vxlan/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/api/__init__.py` & `networklab-1.8.2.dev1/netsim/api/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/augment/addressing.py` & `networklab-1.8.2.dev1/netsim/augment/addressing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/augment/components.py` & `networklab-1.8.2.dev1/netsim/augment/components.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/augment/config.py` & `networklab-1.8.2.dev1/netsim/augment/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/augment/devices.py` & `networklab-1.8.2.dev1/netsim/augment/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/augment/groups.py` & `networklab-1.8.2.dev1/netsim/augment/groups.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/augment/links.py` & `networklab-1.8.2.dev1/netsim/augment/links.py`

 * *Files 1% similar despite different names*

```diff
@@ -741,27 +741,25 @@
       ifdata.neighbors.append(ngh_data)
 
 def set_link_loopback_type(link: Box, nodes: Box, defaults: Box) -> None:
   node = link.interfaces[0].node
   ndata = nodes[node]
   features = devices.get_device_features(ndata,defaults)
 
-  # If we don't know how to create loopbacks on this device, it makes no sense to proceed
-  #
   lb_name = devices.get_device_attribute(ndata,'loopback_interface_name',defaults)
   if not lb_name:
     return
 
-  # Check the device feature first, then the system default. Set the link type if the first
-  # one you get is True. Also note that a True feature gets translated into Box({}) early
-  # in the transformation process (don't ask).
-  #
-  make_loopback = features.get('stub_loopback',defaults.get('links.stub_loopback',None))
-  if make_loopback or isinstance(make_loopback,Box):
-    link.type = 'loopback'
+  if features.stub_loopback is False:
+    return
+
+  if not defaults.links.stub_loopback and not features.stub_loopback:
+    return
+
+  link.type = 'loopback'
 
 def set_link_type_role(link: Box, pools: Box, nodes: Box, defaults: Box) -> None:
   node_cnt = len(link.interfaces)   # Set the number of attached nodes (used in many places further on)
   link['node_count'] = node_cnt
 
   host_count = 0                    # Count the number of hosts attached to the link
   for ifdata in link.interfaces:
```

### Comparing `networklab-1.8.2/netsim/augment/main.py` & `networklab-1.8.2.dev1/netsim/augment/main.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/augment/nodes.py` & `networklab-1.8.2.dev1/netsim/augment/nodes.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/augment/plugin.py` & `networklab-1.8.2.dev1/netsim/augment/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/augment/tools.py` & `networklab-1.8.2.dev1/netsim/augment/tools.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/augment/topology.py` & `networklab-1.8.2.dev1/netsim/augment/topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/augment/validate.py` & `networklab-1.8.2.dev1/netsim/augment/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/__init__.py` & `networklab-1.8.2.dev1/netsim/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,24 +49,14 @@
   parser.add_argument('--raise_on_error', dest='raise_on_error', action='store_true',help=argparse.SUPPRESS)
   parser_add_verbose(parser)
   if debugging:
     parser_add_debug(parser)
 
   return parser
 
-def parser_add_snapshot(parser: argparse.ArgumentParser, hide: bool = False) -> None:
-  parser.add_argument(
-    '--snapshot',
-    dest='snapshot',
-    action='store',
-    nargs='?',
-    default='netlab.snapshot.yml',
-    const='netlab.snapshot.yml',
-    help=argparse.SUPPRESS if hide else 'Transformed topology snapshot file')
-
 def topology_parse_args() -> argparse.ArgumentParser:
   parser = argparse.ArgumentParser(description='Common topology arguments',add_help=False)
   parser.add_argument('--defaults', dest='defaults', action='store',nargs='*',
                   help='Local topology defaults file')
   parser.add_argument('-d','--device', dest='device', action='store', help='Default device type')
   parser.add_argument('-p','--provider', dest='provider', action='store',help='Override virtualization provider')
   parser.add_argument('--plugin',dest='plugin',action='append',help='Additional plugin(s)')
@@ -123,68 +113,47 @@
   if args.settings or args.device or args.provider or args.plugin:
     topology.nodes = augment.nodes.create_node_dict(topology.nodes)
     _read.add_cli_args(topology,args)
 
   log.exit_on_error()
   return topology
 
-# Snapshot loading code -- loads the specified snapshot file and checks its modification date
-#
+# Snapshot-or-topology loader (used by down)
+
 def load_snapshot(args: typing.Union[argparse.Namespace,Box]) -> Box:
   if not os.path.isfile(args.snapshot):
     print(f"The topology snapshot file {args.snapshot} does not exist.\n"+
           "Looks like no lab was started from this directory")
     sys.exit(1)
 
   topology = _read.read_yaml(filename=args.snapshot)
   if topology is None:
     print(f"Cannot read the topology snapshot file {args.snapshot}")
     sys.exit(1)
 
   global_vars.init(topology)
-  check_modified_source(args.snapshot,topology)
   return topology
 
-def check_modified_source(snapshot: str, topology: typing.Optional[Box] = None) -> None:
-  if topology is None:
-    return
-
-  snap_time = os.path.getmtime(snapshot)
-
-  for infile in topology.get('input',[]):
-    if not os.path.exists(infile):
-      continue
-    in_time = os.path.getmtime(infile)
-    if in_time <= snap_time:
-      continue
-
-    log.error(
-      text=f'Lab topology source file {infile} has been modified',
-      more_data=f'after the snapshot {snapshot} has been created',
-      category=Warning,
-      module='cli',
-      hint='recreate')
-
-# Load snapshot or topology -- used by 'netlab initial'
-#
 def load_snapshot_or_topology(args: typing.Union[argparse.Namespace,Box]) -> typing.Optional[Box]:
   log.set_logging_flags(args)
   if args.device or args.provider or args.settings:     # If we have -d, -p or -s flag
     if not args.topology:                               # ... then the user wants to use the topology file
       args.topology = 'topology.yml'                    # ... so let's set the default value if needed
 
   topology = None
   if args.topology:
     topology = load_topology(args)
     augment.main.transform(topology)
     log.exit_on_error()
   else:
     args.snapshot = args.snapshot or 'netlab.snapshot.yml'
-    return load_snapshot(args)
+    topology = _read.read_yaml(filename=args.snapshot)
 
+  if topology:
+    global_vars.init(topology)
   return topology
 
 # get_message: get action-specific message from topology file
 #
 
 def get_message(topology: Box, action: str, default_message: bool = False) -> typing.Optional[str]:
   global DRY_RUN
```

### Comparing `networklab-1.8.2/netsim/cli/_nodeset.py` & `networklab-1.8.2.dev1/netsim/cli/_nodeset.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/ansible.py` & `networklab-1.8.2.dev1/netsim/cli/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/clab.py` & `networklab-1.8.2.dev1/netsim/cli/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/clab_actions/build.py` & `networklab-1.8.2.dev1/netsim/cli/clab_actions/build.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/clab_actions/tarball.py` & `networklab-1.8.2.dev1/netsim/cli/clab_actions/tarball.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/collect.py` & `networklab-1.8.2.dev1/netsim/cli/collect.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 import typing
 import os
 import argparse
 import shutil
 import subprocess
 
-from . import fs_cleanup,parser_add_snapshot,load_snapshot
+from . import common_parse_args,fs_cleanup
 from . import ansible
 from . import external_commands
 from ..utils import log
 
 #
 # CLI parser for 'netlab collect' command
 #
@@ -46,29 +46,25 @@
     action='store',
     help='Create configuration tarball')
   parser.add_argument(
     '--cleanup',
     dest='cleanup',
     action='store_true',
     help='Clean up config directory and modified configuration file after creating tarball')
-  parser_add_snapshot(parser,hide=True)
-
   return parser.parse_known_args(args)
 
 def get_tarball_file(tarball: str) -> str:
   if not '.tar' in tarball:
     tarball = tarball + '.tar.gz'
   return tarball
 
 def run(cli_args: typing.List[str]) -> None:
   (args,rest) = initial_config_parse(cli_args)
   log.set_logging_flags(args)
 
-  topology = load_snapshot(args)
-
   fs_cleanup([ args.output ])
   try:
     os.mkdir(args.output)
   except Exception as ex:
     log.fatal(f"Cannot create output directory {args.output}: {ex}")
 
   if args.verbose:
@@ -97,9 +93,7 @@
       log.fatal(f"Cannot start tar: {ex}")
 
     if args.cleanup:
       if not args.quiet:
         external_commands.print_step(3,"Cleanup config directory",spacing = True)
       fs_cleanup([ args.output ],args.verbose)
       print("... done")
-
-  log.repeat_warnings('netlab collect')
```

### Comparing `networklab-1.8.2/netsim/cli/config.py` & `networklab-1.8.2.dev1/netsim/cli/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Deploy custom configuration template to network devices
 #
 import typing
 import argparse
 import os
 import glob
 
-from . import parser_add_verbose,parser_add_snapshot,load_snapshot
+from . import parser_add_verbose
 from .external_commands import set_ansible_flags
 from . import ansible
 from ..utils import log
 
 #
 # CLI parser for 'netlab config' command
 #
@@ -25,35 +25,30 @@
     '-r','--reload',
     dest='reload',
     action='store_true',
     help='Reload saved device configurations')
   parser.add_argument(
     dest='template', action='store',
     help='Configuration template or a directory with templates')
-  parser_add_snapshot(parser,hide=True)
   parser_add_verbose(parser)
 
   return parser.parse_known_args(args)
 
 def run(cli_args: typing.List[str]) -> None:
   (args,rest) = custom_config_parse(cli_args)
   log.set_logging_flags(args)
   set_ansible_flags(rest)
 
-  topology = load_snapshot(args)
-
   if args.template != '-':
     if os.path.exists(args.template) or \
        os.path.exists(args.template+'.j2') or \
        glob.glob(args.template+'.*.j2'):
       rest = ['-e','config='+args.template] + rest
     else:
       log.fatal(f'Cannot find specified Jinja2 template or configuration directory { args.template }','config')
 
   if args.verbose:
     print(f'Ansible playbook args: { rest }')
   if args.reload:
     ansible.playbook('reload-config.ansible',rest)
   else:
     ansible.playbook('config.ansible',rest)
-
-  log.repeat_warnings('netlab initial')
```

### Comparing `networklab-1.8.2/netsim/cli/connect.py` & `networklab-1.8.2.dev1/netsim/cli/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,14 @@
   elif args.verbose:
     return LogLevel.ARGS
   else:
     return LogLevel.INFO
 
 def run(cli_args: typing.List[str]) -> None:
   (args,rest) = connect_parse(cli_args)
-  log.set_logging_flags(args)
   log_level = get_log_level(args)
   set_dry_run(args)
 
   rest = quote_list(rest)     # Quote arguments with whitespaces
   topology = load_snapshot(args)
   host = args.host
```

### Comparing `networklab-1.8.2/netsim/cli/create.py` & `networklab-1.8.2.dev1/netsim/cli/create.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/down.py` & `networklab-1.8.2.dev1/netsim/cli/down.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import typing
 import textwrap
 import os
 import sys
 from box import Box
 
 from . import external_commands, set_dry_run, is_dry_run
-from . import lab_status_change,fs_cleanup,load_snapshot,parser_add_snapshot
+from . import lab_status_change,fs_cleanup,load_snapshot
 from .. import providers
 from ..utils import status,strings,log
 from .up import provider_probes
 #
 # CLI parser for 'netlab down' command
 #
 def down_parse(args: typing.List[str]) -> argparse.Namespace:
@@ -42,15 +42,22 @@
     action='store_true',
     help='Print the commands that would be executed, but do not execute them')
   parser.add_argument(
     '--force',
     dest='force',
     action='count', default = 0,
     help='Force shutdown or cleanup (use at your own risk)')
-  parser_add_snapshot(parser,hide=True)
+  parser.add_argument(
+    '--snapshot',
+    dest='snapshot',
+    action='store',
+    nargs='?',
+    default='netlab.snapshot.yml',
+    const='netlab.snapshot.yml',
+    help='Transformed topology snapshot file')
 
   return parser.parse_args(args)
 
 #
 # Cleanup common configuration files
 #
 def down_cleanup(topology: Box, verbose: bool = False) -> None:
```

### Comparing `networklab-1.8.2/netsim/cli/external_commands.py` & `networklab-1.8.2.dev1/netsim/cli/external_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,27 +64,23 @@
   cmd_text = cmd if isinstance(cmd,str) else ' '.join(cmd)
   lab_status_log(topology,f'{status}: {cmd_text}')
 
 def run_command(
     cmd : typing.Union[str,list],
     check_result : bool = False,
     ignore_errors: bool = False,
-    return_stdout: bool = False,
-    run_always: bool = False) -> typing.Union[bool,str]:
+    return_stdout: bool = False) -> typing.Union[bool,str]:
 
   if log.debug_active('cli'):
     print(f"Not running: {cmd}")
     return True
 
   if is_dry_run():
-    if run_always:
-      print(f"RUNNING: {cmd}")
-    else:
-      print(f"DRY RUN: {cmd}")
-      return True
+    print(f"DRY RUN: {cmd}")
+    return True
 
   if log.VERBOSE or log.debug_active('external'):
     print(f"run_command executing: {cmd}")
 
   add_netlab_path()
   if isinstance(cmd,str):
     cmd = [ arg for arg in cmd.split(" ") if arg not in (""," ") ]
```

### Comparing `networklab-1.8.2/netsim/cli/graph.py` & `networklab-1.8.2.dev1/netsim/cli/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/initial.py` & `networklab-1.8.2.dev1/netsim/cli/initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 #
 # Deploys initial device configurations
 #
 import typing
 import os
 import argparse
 
-from . import common_parse_args,get_message,load_snapshot,lab_status_change,parser_add_snapshot
+from . import common_parse_args,get_message,load_snapshot_or_topology,lab_status_change
 from . import external_commands
 from . import ansible
-from ..utils import log,status as _status
-from .. import devices
+from ..utils import status as _status
 from box import Box
 
 #
 # CLI parser for 'netlab initial' command
 #
 def initial_config_parse(args: typing.List[str]) -> typing.Tuple[argparse.Namespace, typing.List[str]]:
   parser = argparse.ArgumentParser(
@@ -44,23 +43,19 @@
     '-o','--output',
     dest='output', action='store',nargs='?',const='config',
     help='Create a directory with initial configurations instead of deploying them (default output directory: config)')
   parser.add_argument(
     '--no-message',
     dest='no_message', action='store_true',
     help=argparse.SUPPRESS)
-  parser_add_snapshot(parser,hide=True)
-
   return parser.parse_known_args(args)
 
 def run(cli_args: typing.List[str]) -> None:
   (args,rest) = initial_config_parse(cli_args)
 
-  topology = load_snapshot(args)
-
   deploy_parts = []
   if args.verbose:
     rest = ['-' + 'v' * args.verbose] + rest
 
   if args.initial:
     rest = ['-t','initial'] + rest
     deploy_parts.append("initial configuration")
@@ -90,23 +85,22 @@
     print("Ansible playbook args: %s" % rest)
 
   if args.output:
     ansible.playbook('create-config.ansible',rest)
     print("\nInitial configurations have been created in the %s directory" % args.output)
   else:
     external_commands.LOG_COMMANDS = True
+
+    topology = load_snapshot_or_topology(Box({},default_box=True,box_dots=True))
     deploy_text = ', '.join(deploy_parts) or 'complete configuration'
-    if topology is not None:
-      devices.process_config_sw_check(topology)
+    if not topology is None:
       lab_status_change(topology,f'deploying configuration: {deploy_text}')
 
     ansible.playbook('initial-config.ansible',rest)
     if topology and not args.no_message:
       message = get_message(topology,'initial',True)
       if message:
         print(f"\n\n{message}")
       lab_status_change(topology,f'configuration deployment complete')
 
   if _status.is_directory_locked():                   # If we're using the lock file, touch it after we're done
     _status.lock_directory()                          # .. to have a timestamp of when the lab was started
-
-  log.repeat_warnings('netlab initial')
```

### Comparing `networklab-1.8.2/netsim/cli/inspect.py` & `networklab-1.8.2.dev1/netsim/cli/inspect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/install.py` & `networklab-1.8.2.dev1/netsim/cli/install.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/libvirt.py` & `networklab-1.8.2.dev1/netsim/cli/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/libvirt_actions/config.py` & `networklab-1.8.2.dev1/netsim/cli/libvirt_actions/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/libvirt_actions/package.py` & `networklab-1.8.2.dev1/netsim/cli/libvirt_actions/package.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/read.py` & `networklab-1.8.2.dev1/netsim/cli/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/report.py` & `networklab-1.8.2.dev1/netsim/cli/report.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/restart.py` & `networklab-1.8.2.dev1/netsim/cli/restart.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show-usage.txt` & `networklab-1.8.2.dev1/netsim/cli/show-usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show.py` & `networklab-1.8.2.dev1/netsim/cli/show.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show_commands/__init__.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show_commands/attributes.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/attributes.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show_commands/defaults.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/defaults.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show_commands/devices.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show_commands/images.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/images.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show_commands/module_support.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/module_support.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show_commands/modules.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/modules.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show_commands/outputs.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/outputs.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show_commands/providers.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/providers.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/show_commands/reports.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/reports.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/status.py` & `networklab-1.8.2.dev1/netsim/cli/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,15 @@
   if args.verbose:
     print(f'netlab status file: {status.get_status_filename(topology)}\n')
 
   print("Active lab instance(s)\n")
   heading = [ 'id', 'directory', 'status', 'providers' ]
   rows = []
   for id,lab_state in lab_states.items():
-    line = [str(id),lab_state.dir,lab_state.status or 'Unknown',",".join(lab_state.providers)]
-    rows.append(line)
+    rows.append([str(id),lab_state.dir,lab_state.status,",".join(lab_state.providers)])
 
   strings.print_table(heading,rows)
 
 def show_lab_instance(iid: Lab_Instance_ID, lab_state: Box) -> None:
   print(f'Lab {iid} in {lab_state.dir}')
   print(f'  status: {lab_state.status}')
   print(f'  provider(s): {",".join(lab_state.providers)}')
```

### Comparing `networklab-1.8.2/netsim/cli/test.py` & `networklab-1.8.2.dev1/netsim/cli/test.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/up.py` & `networklab-1.8.2.dev1/netsim/cli/up.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from . import create
 from . import external_commands, set_dry_run, is_dry_run
 from . import common_parse_args, get_message
 from . import lab_status_update, lab_status_change
 from .. import providers
 from ..utils import log,strings,status as _status, read as _read
 from ..data import global_vars
-from ..devices import process_config_sw_check
 
 #
 # Extra arguments for 'netlab up' command
 #
 def up_parse_args(standalone: bool) -> argparse.ArgumentParser:
   parse_parents = [ common_parse_args() ] if standalone else []
   parser = argparse.ArgumentParser(
@@ -309,16 +308,14 @@
 
   settings = topology.defaults
   if log.QUIET:
     os.environ["ANSIBLE_STDOUT_CALLBACK"] = "selective"
 
   external_commands.LOG_COMMANDS = True
   provider_probes(topology)
-  if not args.no_config:
-    process_config_sw_check(topology)
 
   p_provider = topology.provider
   p_module = providers.get_provider_module(topology,p_provider)
   providers.mark_providers(topology)
   p_module.call('pre_output_transform',topology)
 
   providers.validate_images(topology)
```

### Comparing `networklab-1.8.2/netsim/cli/usage.txt` & `networklab-1.8.2.dev1/netsim/cli/usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/cli/validate.py` & `networklab-1.8.2.dev1/netsim/cli/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,33 +113,24 @@
     return
 
   p_status(v_entry.name,"bright_cyan",topology)
   print(h_text)
 
 # Print generic "test failed" message
 #
-def log_failure(
-      msg: str,
-      topology: Box,
-      f_status: str = 'FAIL',
-      more_data: typing.Optional[str] = None) -> None:
-
+def log_failure(msg: str, topology: Box, f_status: str = 'FAIL') -> None:
   global TEST_HEADER,ERROR_ONLY
   if TEST_HEADER:
     print(file=sys.stderr)
     p_status(TEST_HEADER['name'],'red',topology,stderr=True)
     print(TEST_HEADER['text'],file=sys.stderr)
     TEST_HEADER = {}
 
-  o_file = sys.stderr if ERROR_ONLY else sys.stdout
   p_status(f_status,'bright_red',topology,stderr=ERROR_ONLY)
-  print(msg,file=o_file)
-  if more_data:
-    p_status('MORE','bright_black',topology,stderr=ERROR_ONLY)
-    print(more_data,file=o_file)
+  print(msg,file=sys.stderr if ERROR_ONLY else sys.stdout)
 
 # Print generic "making progress" message
 #
 def log_progress(msg: str, topology: Box, f_status: str = 'PASS') -> None:
   global ERROR_ONLY
   if ERROR_ONLY:
     return
@@ -209,37 +200,29 @@
         module='')
     return
 
 '''
 load_plugin: try to load the validation plugin for the specified device
 '''
 
-PLUGIN_ERROR: dict = {}
-
 def load_plugin(device: str) -> typing.Any:
-  global PLUGIN_ERROR
   topology = global_vars.get_topology()
   if topology is None:                                                # Abort if we can't get a point to the topology
     return None
 
   v_path = topology.defaults.paths.validate or ['topology:validate']  # Get validation plugin path
   v_base = os.path.dirname(topology.input[0])                         # Get base (topology) directory
   v_path = _files.absolute_search_path(v_path,v_base)                 # Get the absolute search path
   if log.VERBOSE >= 2:
     print(f'Searching for {device} plugin in {v_path}')
   for v_entry in v_path:                                              # Iterate over the seach path
     v_file = f'{v_entry}/{device}.py'                                 # ... trying to find the device-specific plugin
     if os.path.exists(v_file):                                        # Got it?
       return _files.load_python_module(f'validate_{device}',v_file)   # ... cool, try to load the Python module
 
-  err_key = f'plugin_{device}'
-  if err_key not in PLUGIN_ERROR:
-    log.error('Cannot find validation plugin for device {device}',category=log.MissingDependency,module='validate')
-    PLUGIN_ERROR[err_key] = True
-
   return None
 
 '''
 find_plugin -- find the validation plugin
 
 The plugin could have been already loaded, in which case we'll find it in the global
 _validation_plugin dictionary, or we have to load it, in which case we'll save it in
@@ -259,35 +242,26 @@
 '''
 find_plugin_action -- find the action (show/exec) from the plugin
 
 Figure out whether the validation plugin for the device under test providers the
 desired functionality (show_ or exec_ function). If not, the test is skipped.
 '''
 def find_plugin_action(v_entry: Box, node: Box) -> typing.Optional[str]:
-  global PLUGIN_ERROR
-
   if 'plugin' not in v_entry:
     return None
 
   plugin = find_plugin(node.device)
   if not plugin:
     return None
 
   func_name = v_entry.plugin.split('(')[0]
   for kw in ('show','exec'):
     if getattr(plugin,f'{kw}_{func_name}',None):
       return kw
 
-  err_key = 'action_{node.device}_{func_name}'
-
-  if err_key not in PLUGIN_ERROR:
-    log.error(
-      f"Validation plugin for device {node.device} has no action for test '{func_name}'",
-      category=log.MissingDependency,
-      module='validate')
   return None
 
 class PluginEvalError(Exception):     # Exception class used to raise plugin evaluation exceptions
   pass
 
 '''
 Execute the plugin function specified by 'action' variable and 'plugin' v_entry value
@@ -388,47 +362,14 @@
     return v_cmd
   elif isinstance(v_cmd,str):
     return v_cmd.split(' ')
 
   return []
 
 '''
-Try to parse the results returned from a lab device as a JSON
-
-* Cleanup the returned text
-* If the cleaned-up text starts with [ we have a list: create a bogus
-  wrapper JSON, parse it, and return the inside list
-* Otherwise, try to parse the returned text as JSON object
-
-Cleanup part:
-* Remove the leading and trailing whitespace
-* Find the first [ or { and skip everything in front of it (might be
-  an error message mixed with the JSON data)
-'''
-def parse_JSON(result: str) -> typing.Union[Box,Exception]:
-  result = result.strip()
-  low_idx = len(result)
-  for s_char in ('[','{'):
-    p_char = result.find(s_char,0,low_idx)
-    if p_char >= 0 and p_char < low_idx:
-      low_idx = p_char
-
-  if low_idx < len(result):
-    result = result[low_idx:]
-
-  try:
-    if result.startswith('['):
-      result = f'{{ "rx": {result} }}'
-      return Box.from_json(result).rx
-    else:
-      return Box.from_json(result)
-  except Exception as ex:
-    return ex
-
-'''
 Execute a 'show' command. The return value is expected to be parseable JSON
 '''
 def get_parsed_result(v_entry: Box, n_name: str, topology: Box, verbosity: int) -> Box:
   node = topology.nodes[n_name]                             # Get the node data
   v_cmd = get_exec_list(v_entry,'show',node,topology)       # ... and the 'show' action for the current node
   err_value = data.get_box({'_error': True})                # Assume an error
 
@@ -457,24 +398,22 @@
     log_failure(
       f'Failed to execute show command "{" ".join(v_cmd)}" on {n_name} (device {node.device})',
       topology=topology)
     return err_value
 
   # Try to parse the results we got back as JSON data
   #
-  j_result = parse_JSON(result)
-  if isinstance(j_result,Exception):
+  try:
+    return Box.from_json(result)
+  except:
     log_failure(
       f'Failed to parse result output of "{" ".join(v_cmd)}" on {n_name} (device {node.device}) as JSON',
-      more_data = str(j_result),
       topology=topology)
     return err_value
 
-  return j_result
-
 '''
 Execute a command on the device and return stdout
 '''
 def get_result_string(
       v_entry: Box,
       n_name: str,
       topology: Box,
@@ -727,27 +666,24 @@
         return (True, False)                    # Return (processed, failed)
 
   OK = None
   if 'valid' in v_entry:                        # Do we have a validation expression in the test entry?
     OK = execute_validation_expression(v_entry,node,topology,result,args.verbose,report_error)
   elif 'plugin' in v_entry:                     # If not, try to call the plugin function
     OK = execute_validation_plugin(v_entry,node,topology,result,args.verbose,report_error)
-  elif 'pass' in v_entry:
-    log_progress(f"{node.name}: {v_entry['pass']}",topology)
 
   if OK is False:                               # Validation failed...
     if not report_error:                        # ... but we still don't have to report it?
       return (False, None)                      # ... return (not processed, unknown)
     if 'result' in args.dump:                   # Do we have to dump the result for further troubleshooting?
-      if isinstance(result,Box):                # If the result is a Box, clean it first
-        for kw in ['re']:                       # ... remove extra keys first
-          result.pop(kw,None)
-        # ... and remove the 'result' key if it's not needed
-        if 'result' in result and isinstance(result.result,Box):
-          result.pop('result',None)
+      for kw in ['re']:                         # ... remove extra keys first
+        result.pop(kw,None)
+      # ... and remove the 'result' key if it's not needed
+      if 'result' in result and isinstance(result.result,Box):
+        result.pop('result',None)
       print(f'Returned result\n{"=" * 80}\n{result.to_yaml()}')
   return (True, OK)                             # ... otherwise return (processed, validation result)
 
 '''
 Execute a single validation test on all specified nodes
 '''
 def execute_validation_test(
```

### Comparing `networklab-1.8.2/netsim/common.py` & `networklab-1.8.2.dev1/netsim/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/daemons/bird.yml` & `networklab-1.8.2.dev1/netsim/daemons/bird.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/data/__init__.py` & `networklab-1.8.2.dev1/netsim/data/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/data/filemaps.py` & `networklab-1.8.2.dev1/netsim/data/filemaps.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/data/global_vars.py` & `networklab-1.8.2.dev1/netsim/data/global_vars.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/data/types.py` & `networklab-1.8.2.dev1/netsim/data/types.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/data/validate.py` & `networklab-1.8.2.dev1/netsim/data/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/defaults/attributes.yml` & `networklab-1.8.2.dev1/netsim/defaults/attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/defaults/paths.yml` & `networklab-1.8.2.dev1/netsim/defaults/paths.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/arubacx.py` & `networklab-1.8.2.dev1/netsim/devices/arubacx.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # # 
 # # OSPF Process ID can only be 1-63.
 # # When using VRFs, the process ID is taken from the vrfidx, which usually is > 100.
 # # Here we are mapping every VRF to a specific ospfidx
 #
 from box import Box
 
-from . import _Quirks,need_ansible_collection
+from . import _Quirks
 from ..augment import devices
 from ..utils import log
 
 class ARUBACX(_Quirks):
 
   @classmethod
   def device_quirks(self, node: Box, topology: Box) -> None:
@@ -23,10 +23,7 @@
                 log.error(
                     f'Too many VRFs with OSPF in ({node.name}).\n',
                     log.IncorrectType,
                     'quirks')
                 return
             node.vrfs[vrf]['ospfidx'] = ospfidx
             ospfidx = ospfidx + 1
-
-  def check_config_sw(self, node: Box, topology: Box) -> None:
-    need_ansible_collection(node,'arubanetworks.aoscx')
```

### Comparing `networklab-1.8.2/netsim/devices/arubacx.yml` & `networklab-1.8.2.dev1/netsim/devices/arubacx.yml`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   ansible_ssh_pass: admin
   netlab_device_type: arubacx
 features:
   bfd: true
   bgp:
     activate_af: true
     local_as: true
-    local_as_ibgp: false
+    local_as_ibgp: true
     vrf_local_as: true
   evpn:
     asymmetrical_irb: true
     irb: true
   gateway:
     protocol: [ anycast, vrrp ]
   mpls:
```

### Comparing `networklab-1.8.2/netsim/devices/asav.py` & `networklab-1.8.2.dev1/netsim/devices/asav.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/asav.yml` & `networklab-1.8.2.dev1/netsim/devices/asav.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/csr.yml` & `networklab-1.8.2.dev1/netsim/devices/csr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/cumulus.yml` & `networklab-1.8.2.dev1/netsim/devices/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/cumulus_nvue.yml` & `networklab-1.8.2.dev1/netsim/devices/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/dellos10.yml` & `networklab-1.8.2.dev1/netsim/devices/dellos10.yml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 loopback_interface_name: loopback{ifindex}
 features:
   initial:
     ipv4:
       unnumbered: true
     ipv6:
       lla: true
-    delay: 30
   bgp:
     activate_af: true
     ipv6_lla: true
     local_as: true
     rfc8950: true
     vrf_local_as: true
   evpn:
```

### Comparing `networklab-1.8.2/netsim/devices/eos.py` & `networklab-1.8.2.dev1/netsim/devices/eos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/eos.yml` & `networklab-1.8.2.dev1/netsim/devices/eos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/fortios.yml` & `networklab-1.8.2.dev1/netsim/devices/fortios.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/frr.yml` & `networklab-1.8.2.dev1/netsim/devices/frr.yml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
   netlab_initial: always
 clab:
   # image: frrouting/frr:v7.5.0
   group_vars:
     ansible_connection: docker
     ansible_user: root
     netlab_show_command: [ vtysh, -c, 'show $@' ]
-    netlab_mgmt_vrf: True
   image: quay.io/frrouting/frr:9.1.0
   mtu: 1500
   node:
     kind: linux
     config_templates:
       daemons: /etc/frr/daemons
       hosts: /etc/hosts
```

### Comparing `networklab-1.8.2/netsim/devices/iosv.py` & `networklab-1.8.2.dev1/netsim/devices/iosv.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/iosv.yml` & `networklab-1.8.2.dev1/netsim/devices/iosv.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/iosxr.yml` & `networklab-1.8.2.dev1/netsim/devices/iosxr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/junos.py` & `networklab-1.8.2.dev1/netsim/devices/junos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/junos.yml` & `networklab-1.8.2.dev1/netsim/devices/junos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/linux.py` & `networklab-1.8.2.dev1/netsim/devices/linux.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/linux.yml` & `networklab-1.8.2.dev1/netsim/devices/linux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/none.yml` & `networklab-1.8.2.dev1/netsim/devices/none.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/nxos.yml` & `networklab-1.8.2.dev1/netsim/devices/nxos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/routeros.yml` & `networklab-1.8.2.dev1/netsim/devices/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/routeros7.yml` & `networklab-1.8.2.dev1/netsim/devices/routeros7.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/sonic.yml` & `networklab-1.8.2.dev1/netsim/devices/sonic.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/srlinux.yml` & `networklab-1.8.2.dev1/netsim/devices/srlinux.yml`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   srgb_range_start: 500000
   srgb_range_size: 1000
   ipv6_sid_offset: 100
 bfd:                                    # SR Linux supports lower BFD timers than the global default
   min_tx: 100
   min_rx: 100
 clab:
-  image: ghcr.io/nokia/srlinux:24.3.2
+  image: ghcr.io/nokia/srlinux:23.3.1   # latest version, changes YANG model
   node:
     kind: srl
     type: ixrd2
   interface:
     name: e1-{ifindex}
   group_vars:
     srlinux_grpc_port: 57400
@@ -47,24 +47,23 @@
     rfc8950: True
   vxlan:
     requires: [ evpn ]                  # vrf for l3 vxlan
   evpn:
     irb: True
     asymmetrical_irb: True
   ospf:
-    unnumbered: True
+    unnumbered: False
   isis:
     unnumbered:
-      ipv4: True
+      ipv4: False
       ipv6: True
-      network: True
+      network: False
   vrf:
     keep_module: True
     ospfv2: True
-    ospfv3: True
     bgp: True
   gateway:
     protocol: [ anycast ]
   sr: True
   mpls:
     ldp: True                           # on 7250 IXR only
 external:
```

### Comparing `networklab-1.8.2/netsim/devices/sros.yml` & `networklab-1.8.2.dev1/netsim/devices/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/unknown.py` & `networklab-1.8.2.dev1/netsim/devices/unknown.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/vmx.py` & `networklab-1.8.2.dev1/netsim/devices/vmx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/vptx.py` & `networklab-1.8.2.dev1/netsim/devices/vptx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/vptx.yml` & `networklab-1.8.2.dev1/netsim/devices/vptx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/vsrx.py` & `networklab-1.8.2.dev1/netsim/devices/vsrx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/vsrx.yml` & `networklab-1.8.2.dev1/netsim/devices/vsrx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/devices/vyos.yml` & `networklab-1.8.2.dev1/netsim/devices/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.domain/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/bgp.domain/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.originate/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/bgp.originate/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.policy/_route_map_aoscx.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/_route_map_aoscx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.policy/_route_map_ios.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/_route_map_ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.policy/arubacx.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.policy/cumulus.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.policy/defaults.yml` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.policy/eos.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.policy/frr.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.policy/ios.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.policy/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.policy/simple-attributes.yml` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/simple-attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.policy/srlinux.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/_sample_bfd_template.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/_sample_bfd_template.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/arubacx.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/arubacx.j2`

 * *Files 3% similar despite different names*

```diff
@@ -58,10 +58,7 @@
 {%       endif %}
 {{       ebgp_neighbor(n,af) -}}
 {%     endfor %}
 {%   endfor %}
 {% endfor %}
 {% endif %}
 !
-{% for ngb in bgp._session_clear|default([]) %}
-do clear bgp {{ ngb }}
-{% endfor %}
```

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/cumulus.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/default-originate.yml` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/default-originate.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/defaults.yml` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/defaults.yml`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     passive: True
     timers: True
   routeros7.features.bgp:
     default_originate: True
     allowas_in: True
     as_override: True
     password: True
-    remove_private_as: True
   srlinux.features.bgp:
     default_originate: True
     allowas_in: True
     as_override: True
     password: True
     tcp_ao: False
     timers: True
@@ -109,15 +108,14 @@
     password: True
     tcp_ao: True
   vyos.features.bgp:
     default_originate: True
     allowas_in: True
     as_override: True
     password: True
-    remove_private_as: True
   arubacx.features.bgp:
     allowas_in: True
     bfd: True
     default_originate: True
     gtsm: True
     password: True
     remove_private_as: True
```

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/eos.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/frr.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/ios.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/junos.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/nxos.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,20 +40,14 @@
     if not attr_value:                                  # Attribute not defined in node or interface, move on
       continue
 
     # Check that the node(device) supports the desired attribute
     OK = OK and _bgp.check_device_attribute_support(attr,node,ngb,topology,_config_name)
     ngb[attr] = attr_value                              # Set neighbor attribute from interface/node value
     api.node_config(node,_config_name)                  # And remember that we have to do extra configuration
-    if not node.bgp._session_clear:
-      node.bgp._session_clear = []
-
-    for af in ('ipv4','ipv6'):
-      if af in ngb and ngb[af] not in node.bgp._session_clear:
-        node.bgp._session_clear.append(ngb[af])
 
   return OK
 
 '''
 Copy local session attributes to BGP neighbors because we need
 them there in the configuration templates
 '''
```

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/routeros7.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/routeros7.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AllowAS-IN
 {% for n in bgp.neighbors if n.allowas_in is defined %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined %}
-/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates=main] input.allow-as={{ n.allowas_in }}
+/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates=default] input.allow-as={{ n.allowas_in }}
 {%   endfor %}
 {% endfor %}
 
 {% if vrfs is defined %}
 {% for vname,vdata in vrfs.items() if vdata.bgp is defined %}
 {%   for n in vdata.bgp.neighbors|default([]) if n.allowas_in is defined %}
 {%     for af in ['ipv4','ipv6'] if n[af] is defined and n.allowas_in %}
@@ -14,32 +14,32 @@
 {%   endfor %}
 {% endfor %}
 {% endif %}
 
 # AS-Override
 {% for n in bgp.neighbors if n.as_override is defined %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined %}
-/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates=main] output.as-override=yes
+/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates=default] as-override=yes
 {%   endfor %}
 {% endfor %}
 
 {% if vrfs is defined %}
 {% for vname,vdata in vrfs.items() if vdata.bgp is defined %}
 {%   for n in vdata.bgp.neighbors|default([]) if n.as_override is defined %}
 {%     for af in ['ipv4','ipv6'] if n[af] is defined and n.as_override %}
-/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates={{vname}}] output.as-override=yes
+/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates={{vname}}] as-override=yes
 {%     endfor %}
 {%   endfor %}
 {% endfor %}
 {% endif %}
 
 # Default Originate
 {% for n in bgp.neighbors if n.default_originate is defined %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined and n.default_originate %}
-/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates=main] output.default-originate=always
+/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates=default] output.default-originate=always
 {%   endfor %}
 {% endfor %}
 
 {% if vrfs is defined %}
 {% for vname,vdata in vrfs.items() if vdata.bgp is defined %}
 {%   for n in vdata.bgp.neighbors|default([]) if n.default_originate is defined %}
 {%     for af in ['ipv4','ipv6'] if n[af] is defined and n.default_originate %}
@@ -48,37 +48,20 @@
 {%   endfor %}
 {% endfor %}
 {% endif %}
 
 # Password
 {% for n in bgp.neighbors if n.password is defined %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined %}
-/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates=main] tcp-md5-key={{ n.password }}
+/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates=default] tcp-md5-key={{ n.password }}
 {%   endfor %}
 {% endfor %}
 
 {% if vrfs is defined %}
 {% for vname,vdata in vrfs.items() if vdata.bgp is defined %}
 {%   for n in vdata.bgp.neighbors|default([]) if n.password is defined %}
 {%     for af in ['ipv4','ipv6'] if n[af] is defined and n.password %}
 /routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates={{vname}}] tcp-md5-key={{ n.password }}
 {%     endfor %}
 {%   endfor %}
 {% endfor %}
-{% endif %}
-
-# Remove Private AS
-{% for n in bgp.neighbors if n.remove_private_as|default([]) %}
-{%   for af in ['ipv4','ipv6'] if n[af] is defined and n.remove_private_as %}
-/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates=main] output.remove-private-as=yes
-{%   endfor %}
-{% endfor %}
-
-{% if vrfs is defined %}
-{% for vname,vdata in vrfs.items() if vdata.bgp is defined %}
-{%   for n in vdata.bgp.neighbors|default([]) if n.remove_private_as|default([]) %}
-{%     for af in ['ipv4','ipv6'] if n[af] is defined and n.remove_private_as %}
-/routing/bgp/connection set [/routing/bgp/connection find remote.address={{ n[af] }} and templates={{vname}}] output.remove-private-as=yes
-{%     endfor %}
-{%   endfor %}
-{% endfor %}
-{% endif %}
+{% endif %}
```

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/srlinux.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/sros.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/bgp.session/vyos.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/vyos.j2`

 * *Files 22% similar despite different names*

```diff
@@ -5,83 +5,81 @@
     exec sg vyattacfg -c "/bin/vbash $(readlink -f $0) $@"
 fi
 
 # Configuration items start here
 
 configure
 
-# Catch all config stuff on the same loop (and avoid multiple loopings)
-
-# main routing table
-{% for n in bgp.neighbors %}
+# AllowAS-IN
+{% for n in bgp.neighbors if n.allowas_in is defined %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined %}
-{%     set peer = n[af] if n[af] is string else n.local_if|default('?') %}
+set protocols bgp neighbor {{ n[af] }} address-family {{ af }}-unicast allowas-in number {{ n.allowas_in }}
+{%   endfor %}
+{% endfor %}
 
-# AllowAS-IN
-{%     if n.allowas_in is defined %}
-set protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast allowas-in number {{ n.allowas_in }}
-{%     endif %}
+{% if vrfs is defined %}
+{% for vname,vdata in vrfs.items() if vdata.bgp is defined %}
+{%   for n in vdata.bgp.neighbors|default([]) if n.allowas_in is defined %}
+{%     for af in ['ipv4','ipv6'] if n[af] is defined and n.allowas_in %}
+set vrf name {{ vname }} protocols bgp neighbor {{ n[af] }} address-family {{ af }}-unicast allowas-in number {{ n.allowas_in }}
+{%     endfor %}
+{%   endfor %}
+{% endfor %}
+{% endif %}
 
 # AS-Override
-{%     if n.as_override is defined %}
-set protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast as-override
-{%     endif %}
-
-# Default Originate
-{%     if n.default_originate is defined %}
-set protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast default-originate
-{%     endif %}
-
-# Password
-{%     if n.password is defined %}
-set protocols bgp neighbor {{ peer }} password {{ n.password }}
-{%     endif %}
-
-# Remote Private AS
-{%     if n.remove_private_as is defined %}
-set protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast remove-private-as
-{%     endif %}
-
+{% for n in bgp.neighbors if n.as_override is defined %}
+{%   for af in ['ipv4','ipv6'] if n[af] is defined %}
+set protocols bgp neighbor {{ n[af] }} address-family {{ af }}-unicast as-override
 {%   endfor %}
 {% endfor %}
 
-# Specific VRFs
-{% for vname,vdata in (vrfs|default({})).items() if vdata.bgp is defined %}
-{%   for n in vdata.bgp.neighbors|default([]) %}
-{%     for af in ['ipv4','ipv6'] if n[af] is defined %}
-{%       set peer = n[af] if n[af] is string else n.local_if|default('?') %}
-
-# AllowAS-IN
-{%       if n.allowas_in is defined %}
-set vrf name {{ vname }} protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast allowas-in number {{ n.allowas_in }}
-{%       endif %}
-
-# AS-Override
-{%       if n.as_override is defined %}
-set vrf name {{ vname }} protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast as-override
-{%       endif %}
+{% if vrfs is defined %}
+{% for vname,vdata in vrfs.items() if vdata.bgp is defined %}
+{%   for n in vdata.bgp.neighbors|default([]) if n.as_override is defined %}
+{%     for af in ['ipv4','ipv6'] if n[af] is defined and n.as_override %}
+set vrf name {{ vname }} protocols bgp neighbor {{ n[af] }} address-family {{ af }}-unicast as-override
+{%     endfor %}
+{%   endfor %}
+{% endfor %}
+{% endif %}
 
 # Default Originate
-{%       if n.default_originate is defined %}
-set vrf name {{ vname }} protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast default-originate
-{%       endif %}
+{% for n in bgp.neighbors if n.default_originate is defined %}
+{%   for af in ['ipv4','ipv6'] if n[af] is defined and n.default_originate %}
+set protocols bgp neighbor {{ n[af] }} address-family {{ af }}-unicast default-originate
+{%   endfor %}
+{% endfor %}
+
+{% if vrfs is defined %}
+{% for vname,vdata in vrfs.items() if vdata.bgp is defined %}
+{%   for n in vdata.bgp.neighbors|default([]) if n.default_originate is defined %}
+{%     for af in ['ipv4','ipv6'] if n[af] is defined and n.default_originate %}
+set vrf name {{ vname }} protocols bgp neighbor {{ n[af] }} address-family {{ af }}-unicast default-originate
+{%     endfor %}
+{%   endfor %}
+{% endfor %}
+{% endif %}
 
 # Password
-{%       if n.password is defined %}
-set vrf name {{ vname }} protocols bgp neighbor {{ peer }} password {{ n.password }}
-{%       endif %}
-
-# Remote Private AS
-{%       if n.remove_private_as is defined %}
-set vrf name {{ vname }} protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast remove-private-as
-{%       endif %}
+{% for n in bgp.neighbors if n.password is defined %}
+{%   for af in ['ipv4','ipv6'] if n[af] is defined %}
+set protocols bgp neighbor {{ n[af] }} password {{ n.password }}
+{%   endfor %}
+{% endfor %}
 
+{% if vrfs is defined %}
+{% for vname,vdata in vrfs.items() if vdata.bgp is defined %}
+{%   for n in vdata.bgp.neighbors|default([]) if n.password is defined %}
+{%     for af in ['ipv4','ipv6'] if n[af] is defined and n.password %}
+set vrf name {{ vname }} protocols bgp neighbor {{ n[af] }} password {{ n.password }}
 {%     endfor %}
 {%   endfor %}
 {% endfor %}
+{% endif %}
 
 # Commit, save and exit from subshell
 
 commit
 save
 exit
```

### Comparing `networklab-1.8.2/netsim/extra/ebgp.multihop/arubacx.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/ebgp.multihop/defaults.yml` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/ebgp.multihop/eos.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/ebgp.multihop/frr.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/ebgp.multihop/ios.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/ebgp.multihop/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/ebgp.multihop/srlinux.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/ebgp.multihop/sros.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/fabric/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/fabric/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/multilab/__init__.py` & `networklab-1.8.2.dev1/netsim/extra/multilab/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/proxy-arp/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/proxy-arp/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/proxy-arp/srlinux.j2` & `networklab-1.8.2.dev1/netsim/extra/proxy-arp/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/extra/proxy-arp/sros.j2` & `networklab-1.8.2.dev1/netsim/extra/proxy-arp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/ansible.sh` & `networklab-1.8.2.dev1/netsim/install/ansible.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/containerlab.sh` & `networklab-1.8.2.dev1/netsim/install/containerlab.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/grpc.sh` & `networklab-1.8.2.dev1/netsim/install/grpc.sh`

 * *Files 13% similar despite different names*

```diff
@@ -27,16 +27,15 @@
   fi
   FLAG_YES="Y"
 fi
 
 # Install Ansible grpc plug-in and its dependencies from github repo
 ansible-galaxy collection install 'git+https://github.com/nokia/ansible-networking-collections.git#/grpc/'
 
-echo "We have to upgrade Ansible to release 9.5.1 or greater or it will break"
-echo "Alternatively, you can manually downgrade it to release 4.10.0 or earlier"
-echo
-sudo python3 -m pip install --upgrade 'ansible>=9.5.1'
+# The last version of Ansible working with Nokia Ansible collection is 4.10.0
+#
+sudo python3 -m pip install --upgrade ansible==4.10.0
 
 # grpc sources contain generated pb2 file which is not compatible with newer versions of protobuf
 python3 -m pip install grpcio protobuf==3.20.1 --upgrade
 
 exit $?
```

### Comparing `networklab-1.8.2/netsim/install/libvirt/arubacx.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/arubacx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/asav/day0-config` & `networklab-1.8.2.dev1/netsim/install/libvirt/asav/day0-config`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/asav.xml.j2` & `networklab-1.8.2.dev1/netsim/install/libvirt/asav.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/csr.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/csr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/dellos10/run.sh` & `networklab-1.8.2.dev1/netsim/install/libvirt/dellos10/run.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/dellos10.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/dellos10.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Creating initial configuration for Dell OS10
 =============================================
 
 * Wait for the 'login' prompt, and then wait again some more minutes
 * Login as 'admin' (password: 'admin')
 * Disable zero-touch ('ztd cancel')
-* Save configuration ('write memory') and reload the box ('reload')
-* Login as 'admin' (password: 'admin')
 * Enter configuration mode ('configure')
 * Copy-paste the following configuration
 
 NOTE: the management traffic is isolated in a dedicated management VRF (management).
 
+===============
+*** WARNING ***
+===============
+To disable zero-touch (ZTD) a full reload is required after the first configuration.
+
 =============================================
 !
 interface mgmt1/1/1
   no ip address dhcp
   no ipv6 address
   exit
 !
@@ -28,12 +31,17 @@
   exit
 !
 service simple-password
 username vagrant password vagrant role sysadmin priv-lvl 15
 username vagrant sshkey "ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEA6NF8iallvQVp22WDkTkyrtvp9eWW6A8YVr+kz4TjGYe7gHzIw+niNltGEFHzD8+v1I2YJ6oXevct1YeS0o9HZyN1Q9qgCgzUFtdOKLv6IedplqoPkcmF0aYet2PkEDo3MlTBckFXPITAMzF8dJSIFo9D8HfdOV0IAdx4O7PtixWKn5y2hMNG0zQPyUecp4pzC6kivAIhyfHilFR61RGL+GPXQ2MWZWFYbAGjyiYJnAmCP3NOTd0jMZEnDkbUvxhMmBYSdETk1rRgm+R4LOzFUGaHqHDLKLX+FIPKcF96hrucXzcWyLbIbEgE98OHlnVYCzRdK8jlqm8tehUc9c9WhQ== vagrant insecure public key"
 !
 end
+write memory
+!
+! reload cycle is required to disable ZTD
+!
+reload
+!
 =============================================
 
-* Save configuration ('write memory') and reload the box ('reload')
 * Wait until the reload is completed
 * Disconnect from console (ctrl-] usually works).
```

### Comparing `networklab-1.8.2/netsim/install/libvirt/eos.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/eos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/eos.xml.j2` & `networklab-1.8.2.dev1/netsim/install/libvirt/eos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/iosv.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/iosv.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/iosv.xml.j2` & `networklab-1.8.2.dev1/netsim/install/libvirt/iosv.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/iosxr.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/iosxr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/nxos.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/nxos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/nxos.xml.j2` & `networklab-1.8.2.dev1/netsim/install/libvirt/nxos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/routeros7.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/routeros7.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/sonic.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/sonic.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/sonic.xml.j2` & `networklab-1.8.2.dev1/netsim/install/libvirt/sonic.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/vptx/juniper.conf` & `networklab-1.8.2.dev1/netsim/install/libvirt/vptx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/vptx/make-config.sh` & `networklab-1.8.2.dev1/netsim/install/libvirt/vptx/make-config.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/vptx.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/vptx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/vptx.xml.j2` & `networklab-1.8.2.dev1/netsim/install/libvirt/vptx.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/vsrx/juniper.conf` & `networklab-1.8.2.dev1/netsim/install/libvirt/vsrx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt/vsrx.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/vsrx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/libvirt.sh` & `networklab-1.8.2.dev1/netsim/install/libvirt.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/install/ubuntu.sh` & `networklab-1.8.2.dev1/netsim/install/ubuntu.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/__init__.py` & `networklab-1.8.2.dev1/netsim/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/_dataplane.py` & `networklab-1.8.2.dev1/netsim/modules/_dataplane.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/_routing.py` & `networklab-1.8.2.dev1/netsim/modules/_routing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/bfd.py` & `networklab-1.8.2.dev1/netsim/modules/bfd.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/bfd.yml` & `networklab-1.8.2.dev1/netsim/modules/bfd.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/bgp.py` & `networklab-1.8.2.dev1/netsim/modules/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/bgp.yml` & `networklab-1.8.2.dev1/netsim/modules/bgp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/dhcp.py` & `networklab-1.8.2.dev1/netsim/modules/dhcp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/dhcp.yml` & `networklab-1.8.2.dev1/netsim/modules/dhcp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/eigrp.py` & `networklab-1.8.2.dev1/netsim/modules/eigrp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/evpn.py` & `networklab-1.8.2.dev1/netsim/modules/evpn.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/evpn.yml` & `networklab-1.8.2.dev1/netsim/modules/evpn.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/gateway.py` & `networklab-1.8.2.dev1/netsim/modules/gateway.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/gateway.yml` & `networklab-1.8.2.dev1/netsim/modules/gateway.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/isis.py` & `networklab-1.8.2.dev1/netsim/modules/isis.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/isis.yml` & `networklab-1.8.2.dev1/netsim/modules/isis.yml`

 * *Files 7% similar despite different names*

```diff
@@ -28,18 +28,15 @@
     metric: { type: int, min_value: 1, max_value: 16777215 }
     cost: { type: int, min_value: 1, max_value: 16777215 }
     type: { type: str, valid_values: [ level-1, level-2, level-1-2 ] }
     bfd:
       ipv4: bool
       ipv6: bool
       _alt_types: [ bool ]
-    network_type:
-      type: str
-      valid_values: [ point-to-point ]
-      _alt_types: [ bool ]
+    network_type: { type: str, valid_values: [ point-to-point ] }
     passive: bool
 features:
   unnumbered:
     ipv4: IPv4 unnumbered interfaces
     ipv6: IPv6 unnumbered interfaces
     network: multi-access unnumbered links
 warnings:
```

### Comparing `networklab-1.8.2/netsim/modules/mpls.py` & `networklab-1.8.2.dev1/netsim/modules/mpls.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/mpls.yml` & `networklab-1.8.2.dev1/netsim/modules/mpls.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/ospf.py` & `networklab-1.8.2.dev1/netsim/modules/ospf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/ospf.yml` & `networklab-1.8.2.dev1/netsim/modules/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/srv6.py` & `networklab-1.8.2.dev1/netsim/modules/srv6.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/vlan.py` & `networklab-1.8.2.dev1/netsim/modules/vlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/vlan.yml` & `networklab-1.8.2.dev1/netsim/modules/vlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/vrf.py` & `networklab-1.8.2.dev1/netsim/modules/vrf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/vrf.yml` & `networklab-1.8.2.dev1/netsim/modules/vrf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/vxlan.py` & `networklab-1.8.2.dev1/netsim/modules/vxlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/modules/vxlan.yml` & `networklab-1.8.2.dev1/netsim/modules/vxlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/outputs/__init__.py` & `networklab-1.8.2.dev1/netsim/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/outputs/ansible.py` & `networklab-1.8.2.dev1/netsim/outputs/ansible.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from . import _TopologyOutput,check_writeable
 from ..augment import nodes
 from ..augment import devices
 from ..augment import plugin
 from ..utils import templates,strings,log
 from ..utils import files as _files
-from ..data import global_vars
 
 forwarded_port_name = { 'ssh': 'ansible_port', }
 
 def copy_provider_inventory(host: Box, p_data: Box) -> None:
   if 'inventory' in p_data:
     for k,v in p_data.inventory.items():
       host[k] = v
@@ -65,46 +64,33 @@
     if not k in topo_to_host_skip:
       host[k] = v
 
   provider_inventory_settings(host,node,topology)
   return host
 
 """
-Create a 'hosts' dictionary listing usable IPv4 and IPv6 addresses of all lab devices.
+Create a 'hosts' dictionary as an 'all' group variable listing usable IPv4 and
+IPv6 addresses of all lab devices.
 """
-def get_host_addresses(topology: Box) -> Box:
-  hosts = global_vars.get('hosts')                          # Try to use a cached version
-  if hosts:
-    return hosts
-
+def add_host_addresses(topology: Box, inventory: Box) -> None:
   for name,node in topology.nodes.items():
     intf_list = node.interfaces
     if 'loopback' in node:                                  # Create a list of all usable interfaces
       intf_list = [ node.loopback ] + node.interfaces       # ... starting with loopback
 
     for intf in intf_list:                                  # Now iterate over interfaces
-      h_name = f'{name}-{intf.vrf}' if 'vrf' in intf else name
       for af in ('ipv4','ipv6'):                            # ... and collect IPv4 and IPv6 addresses
         if not isinstance(intf.get(af,False),str):          # Is the IP address a string (= usable IP address)?
           continue
       
-        if not af in hosts[h_name]:                         # Edge case: first interface
-          hosts[h_name][af] = []                            # ... have to start with an empty list
+        if not af in inventory.all.vars.hosts[name]:        # Edge case: first interface
+          inventory.all.vars.hosts[name][af] = []           # ... have to start with an empty list
 
         addr = str(netaddr.IPNetwork(intf[af]).ip)          # Extract IP address from the CIDR prefix
-        hosts[h_name][af].append(addr)                      # ... and append it to the list of usable IP addresses
-
-  global_vars.set('hosts',hosts)                            # Cache the hosts dictionary
-  return hosts
-
-"""
-Add the hosts dictionary to Ansible inventory as an 'all' group variable 
-"""
-def add_host_addresses(topology: Box, inventory: Box) -> None:
-  inventory.all.vars.hosts = get_host_addresses(topology)
+        inventory.all.vars.hosts[name][af].append(addr)     # ... and append it to the list of usable IP addresses
 
 """
 Copy defaults.paths dictionary into ALL group. Create separate variables
 from individual customizable paths to prevent dependencies on too many
 variables that might not be set (example: only 'paths.custom' values should
 depend on 'custom_config' variable)
 """
```

### Comparing `networklab-1.8.2/netsim/outputs/common.py` & `networklab-1.8.2.dev1/netsim/outputs/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/outputs/d2.py` & `networklab-1.8.2.dev1/netsim/outputs/d2.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/outputs/d2.yml` & `networklab-1.8.2.dev1/netsim/outputs/d2.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/outputs/devices.py` & `networklab-1.8.2.dev1/netsim/outputs/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/outputs/graph.py` & `networklab-1.8.2.dev1/netsim/outputs/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/outputs/graphite.py` & `networklab-1.8.2.dev1/netsim/outputs/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/outputs/provider.py` & `networklab-1.8.2.dev1/netsim/outputs/provider.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/outputs/report.py` & `networklab-1.8.2.dev1/netsim/outputs/report.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/outputs/tools.py` & `networklab-1.8.2.dev1/netsim/outputs/tools.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/outputs/yaml.py` & `networklab-1.8.2.dev1/netsim/outputs/yaml.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/providers/__init__.py` & `networklab-1.8.2.dev1/netsim/providers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from box import Box
 
 from ..utils.callback import Callback
 from ..augment import devices,links
 from ..data import get_box,get_empty_box,filemaps
 from ..utils import files as _files
 from ..utils import templates,log,strings
-from ..outputs.ansible import get_host_addresses
 
 class _Provider(Callback):
   def __init__(self, provider: str, data: Box) -> None:
     self.provider = provider
     if 'template' in data:
       self._default_template_name = data.template
 
@@ -156,15 +155,15 @@
     bind_dict = filemaps.mapping_to_dict(binds)
     for file,mapping in bind_dict.items():
       if not out_folder in file:                  # Skip files that are not mapped into the temporary provider folder
         continue
       file_name = file.replace(out_folder+"/","")
       template_name = self.find_extra_template(node,file_name,topology)
       if template_name:
-        node_data = node + { 'hostvars': topology.nodes, 'hosts': get_host_addresses(topology) }
+        node_data = node + { 'hostvars': topology.nodes }
         if '/' in file_name:                      # Create subdirectory in out_folder if needed
           pathlib.Path(f"{out_folder}/{os.path.dirname(file_name)}").mkdir(parents=True,exist_ok=True)
         try:
           templates.write_template(
             in_folder=os.path.dirname(template_name),
             j2=os.path.basename(template_name),
             data=node_data.to_dict(),
```

### Comparing `networklab-1.8.2/netsim/providers/clab.py` & `networklab-1.8.2.dev1/netsim/providers/clab.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,16 +136,15 @@
 
   def get_lab_status(self) -> Box:
     try:
       status = external_commands.run_command(
                   'docker ps --format json',
                   check_result=True,
                   ignore_errors=True,
-                  return_stdout=True,
-                  run_always=True)
+                  return_stdout=True)
       
       stat_box = get_empty_box()
       if not isinstance(status,str):
         return stat_box
       try:
         for line in status.split('\n'):
           if not line.startswith('{'):
```

### Comparing `networklab-1.8.2/netsim/providers/clab.yml` & `networklab-1.8.2.dev1/netsim/providers/clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/providers/external.py` & `networklab-1.8.2.dev1/netsim/providers/external.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/providers/libvirt.py` & `networklab-1.8.2.dev1/netsim/providers/libvirt.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,15 +360,15 @@
     return f'{ topology.name.split(".")[0] }_{ node }'
 
   def validate_node_image(self, node: Box, topology: Box) -> None:
     box_list = getattr(self,'box_list',None)
     if not box_list:                                        # Create an box cache on first call
       box_list = external_commands.run_command(             # Get the list of Vagrant boxes
                       ['vagrant', 'box', 'list'],
-                      check_result=True, ignore_errors=True, return_stdout=True, run_always=True)
+                      check_result=True, ignore_errors=True, return_stdout=True)
       box_list = box_list if isinstance(box_list,str) else ''
       self.box_list = box_list.split('\n')
 
     log.print_verbose(f'libvirt: validating node {node.name} image {node.box}')
     box_specs = node.box.split(':')
     box_name = box_specs[0]
     box_version = box_specs[1] if len(box_specs) > 1 else ''
```

### Comparing `networklab-1.8.2/netsim/providers/libvirt.yml` & `networklab-1.8.2.dev1/netsim/providers/libvirt.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/clab/clab.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/clab/clab.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/clab/frr/daemons.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/clab/frr/daemons.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/external/external.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/external/external.j2`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {%   if loop.last %}
 |-----------------|---------------|-------------|--------------------|------------------|
 {%   endif %}
 {% endfor %}
 
 {% set row_count = [] %}
 {% for node_name, n in nodes.items() %}
-{%   for l in n.interfaces if l.type=='lan' and 'neighbors' in l and l.neighbors|length > 1 %}
+{%   for l in n.interfaces if l.type=='lan' and l.neighbors|length > 1 %}
 {%     if not row_count %}
 LAN LINKS:
 
 |---------------|-------------|-----------------|----------------------|
 | Origin Device | Origin Port | Link Name (NET) | Description          |
 |---------------|-------------|-----------------|----------------------|
 {%     endif %}
@@ -33,15 +33,15 @@
 {% endfor %}
 {% if row_count %}
 |---------------|-------------|-----------------|----------------------|
 {% endif %}
 
 {% set row_count = [] %}
 {% for node_name, n in nodes.items() %}
-{%   for l in n.interfaces if l.type in ['lan','stub'] and not l.neighbors|default([]) %}
+{%   for l in n.interfaces if l.type in ['lan','stub'] and l.neighbors|length == 0 %}
 {%     if not row_count %}
 STUB LINKS:
 
 |---------------|-------------|----------------------|
 | Origin Device | Origin Port | Description          |
 |---------------|-------------|----------------------|
 {%     endif %}
```

### Comparing `networklab-1.8.2/netsim/templates/provider/libvirt/Vagrantfile.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/libvirt/define-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/define-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/libvirt/iosxr-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/libvirt/libvirt-bridge.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/libvirt-bridge.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/libvirt/libvirt-tunnel.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/libvirt/nxos-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/nxos-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/libvirt/vagrant-libvirt.xml` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/libvirt/vptx-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vptx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/libvirt/vsrx-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/templates/provider/virtualbox/Vagrantfile.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/tools/__init__.py` & `networklab-1.8.2.dev1/netsim/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/tools/graphite.py` & `networklab-1.8.2.dev1/netsim/tools/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/tools/graphite.yml` & `networklab-1.8.2.dev1/netsim/tools/graphite.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/tools/suzieq.yml` & `networklab-1.8.2.dev1/netsim/tools/suzieq.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/topology-defaults.yml` & `networklab-1.8.2.dev1/netsim/topology-defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/utils/bgp.py` & `networklab-1.8.2.dev1/netsim/utils/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/utils/callback.py` & `networklab-1.8.2.dev1/netsim/utils/callback.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/utils/files.py` & `networklab-1.8.2.dev1/netsim/utils/files.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/utils/log.py` & `networklab-1.8.2.dev1/netsim/utils/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,15 @@
   from .strings import extra_data_printout
 
   topology = get_topology()
   if topology is None:                                              # No valid topology ==> no static hints
     return
 
   mod_hints = topology.defaults.hints[module]                       # Get static hints for current module
+
   if mod_hints[hint]:                                               # Do we know what to do?
     hint_printout = extra_data_printout(mod_hints[hint],width=90)   # Format the hint for traditional printout
     if category is not Warning:
       _ERROR_LOG.extend(hint_printout.split("\n"))
     if strings.rich_err_color:
       l_width = min(strings.rich_err_width-10,100)
       hint_lines = strings.wrap_text_into_lines(mod_hints[hint],width=l_width)
```

### Comparing `networklab-1.8.2/netsim/utils/read.py` & `networklab-1.8.2.dev1/netsim/utils/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/utils/sort.py` & `networklab-1.8.2.dev1/netsim/utils/sort.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/utils/status.py` & `networklab-1.8.2.dev1/netsim/utils/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/utils/strings.py` & `networklab-1.8.2.dev1/netsim/utils/strings.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/utils/templates.py` & `networklab-1.8.2.dev1/netsim/utils/templates.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/utils/versioning.py` & `networklab-1.8.2.dev1/netsim/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/netsim/validate/linux.py` & `networklab-1.8.2.dev1/netsim/validate/linux.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/networklab.egg-info/PKG-INFO` & `networklab-1.8.2.dev1/networklab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.8.2
+Version: 1.8.2.dev1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.8.2](https://github.com/ipspace/netlab/releases/tag/release_1.8.2), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.1-post1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1-post1) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
+The latest release is [release 1.8.1-post1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1-post1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
 
 <!--
 If you encounter bugs using release 1.7.x, please downgrade to [1.6.4](https://github.com/ipspace/netlab/releases/tag/release_1.6.4) and [open a GitHub issue](https://github.com/ipspace/netlab/issues).
 -->
 
 ## An Overview of CLI Commands
```

### Comparing `networklab-1.8.2/networklab.egg-info/SOURCES.txt` & `networklab-1.8.2.dev1/networklab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,14 @@
 netsim/devices/arubacx.py
 netsim/devices/arubacx.yml
 netsim/devices/asav.py
 netsim/devices/asav.yml
 netsim/devices/csr.yml
 netsim/devices/cumulus.yml
 netsim/devices/cumulus_nvue.yml
-netsim/devices/dellos10.py
 netsim/devices/dellos10.yml
 netsim/devices/eos.py
 netsim/devices/eos.yml
 netsim/devices/fortios.yml
 netsim/devices/frr.yml
 netsim/devices/iosv.py
 netsim/devices/iosv.yml
@@ -454,15 +453,14 @@
 netsim/devices/linux.py
 netsim/devices/linux.yml
 netsim/devices/none.yml
 netsim/devices/nxos.yml
 netsim/devices/routeros.yml
 netsim/devices/routeros7.yml
 netsim/devices/sonic.yml
-netsim/devices/srlinux.py
 netsim/devices/srlinux.yml
 netsim/devices/sros.yml
 netsim/devices/unknown.py
 netsim/devices/unknown.yml
 netsim/devices/vmx.py
 netsim/devices/vmx.yml
 netsim/devices/vptx.py
```

### Comparing `networklab-1.8.2/setup.py` & `networklab-1.8.2.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.2/tests/test_transformation.py` & `networklab-1.8.2.dev1/tests/test_transformation.py`

 * *Files identical despite different names*

