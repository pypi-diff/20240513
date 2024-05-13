# Comparing `tmp/pulumi_proxmoxve-6.5.1.tar.gz` & `tmp/pulumi_proxmoxve-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-6.5.1.tar", last modified: Tue May  7 07:11:04 2024, max compression
+gzip compressed data, was "pulumi_proxmoxve-6.6.0.tar", last modified: Mon May 13 07:57:16 2024, max compression
```

## Comparing `pulumi_proxmoxve-6.5.1.tar` & `pulumi_proxmoxve-6.6.0.tar`

### file list

```diff
@@ -1,109 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.014572 pulumi_proxmoxve-6.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-07 07:11:04.014572 pulumi_proxmoxve-6.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:03.998571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.002571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    53365 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.002571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.002571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37038 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    64365 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    32232 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.002571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/download/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38162 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/download/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/get_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.006571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18333 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/ha_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.006571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/get_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.006571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/get_pci.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/get_usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/pci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.010572 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    33135 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24956 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/network_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/network_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.010572 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    25681 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.010572 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.014572 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87632 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    75774 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   124005 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:04.002571 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:11:04.014572 pulumi_proxmoxve-6.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-07 07:11:03.000000 pulumi_proxmoxve-6.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.934203 pulumi_proxmoxve-6.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-13 07:57:16.934203 pulumi_proxmoxve-6.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.918203 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.922203 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/cluster/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/cluster/get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53365 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/cluster/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/cluster/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.922203 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.922203 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36258 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64491 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31452 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/dns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.922203 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38006 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/download/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/get_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.922203 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/get_ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/get_ha_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/get_ha_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/get_ha_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18177 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/ha_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.926203 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/get_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.926203 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/get_pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/get_usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.926203 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32979 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24800 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/network_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25201 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/network_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.930204 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25525 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.930204 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.930204 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16708 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/user/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.934203 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86830 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74972 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123851 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:57:16.922203 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:57:16.934203 pulumi_proxmoxve-6.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-13 07:57:16.000000 pulumi_proxmoxve-6.6.0/setup.py
```

### Comparing `pulumi_proxmoxve-6.5.1/PKG-INFO` & `pulumi_proxmoxve-6.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_proxmoxve
-Version: 6.5.1
+Version: 6.6.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.5.1/README.md` & `pulumi_proxmoxve-6.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
+from .acl import *
 from .certifi import *
 from .dns import *
 from .get_node import *
 from .hosts import *
 from .provider import *
 from .time import *
 from .vm2 import *
@@ -31,26 +32,29 @@
     hardware = __hardware
     import pulumi_proxmoxve.network as __network
     network = __network
     import pulumi_proxmoxve.permission as __permission
     permission = __permission
     import pulumi_proxmoxve.storage as __storage
     storage = __storage
+    import pulumi_proxmoxve.user as __user
+    user = __user
     import pulumi_proxmoxve.vm as __vm
     vm = __vm
 else:
     cluster = _utilities.lazy_import('pulumi_proxmoxve.cluster')
     config = _utilities.lazy_import('pulumi_proxmoxve.config')
     ct = _utilities.lazy_import('pulumi_proxmoxve.ct')
     download = _utilities.lazy_import('pulumi_proxmoxve.download')
     ha = _utilities.lazy_import('pulumi_proxmoxve.ha')
     hardware = _utilities.lazy_import('pulumi_proxmoxve.hardware')
     network = _utilities.lazy_import('pulumi_proxmoxve.network')
     permission = _utilities.lazy_import('pulumi_proxmoxve.permission')
     storage = _utilities.lazy_import('pulumi_proxmoxve.storage')
+    user = _utilities.lazy_import('pulumi_proxmoxve.user')
     vm = _utilities.lazy_import('pulumi_proxmoxve.vm')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "proxmoxve",
@@ -210,22 +214,38 @@
   "fqn": "pulumi_proxmoxve.storage",
   "classes": {
    "proxmoxve:Storage/file:File": "File"
   }
  },
  {
   "pkg": "proxmoxve",
+  "mod": "User/token",
+  "fqn": "pulumi_proxmoxve.user",
+  "classes": {
+   "proxmoxve:User/token:Token": "Token"
+  }
+ },
+ {
+  "pkg": "proxmoxve",
   "mod": "VM/virtualMachine",
   "fqn": "pulumi_proxmoxve.vm",
   "classes": {
    "proxmoxve:VM/virtualMachine:VirtualMachine": "VirtualMachine"
   }
  },
  {
   "pkg": "proxmoxve",
+  "mod": "index/acl",
+  "fqn": "pulumi_proxmoxve",
+  "classes": {
+   "proxmoxve:index/acl:Acl": "Acl"
+  }
+ },
+ {
+  "pkg": "proxmoxve",
   "mod": "index/certifi",
   "fqn": "pulumi_proxmoxve",
   "classes": {
    "proxmoxve:index/certifi:Certifi": "Certifi"
   }
  },
  {
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/_inputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/cluster/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,22 +154,20 @@
 
 def get_nodes(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNodesResult:
     """
     Retrieves information about all available nodes.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     available_nodes = proxmoxve.Cluster.get_nodes()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Cluster/getNodes:getNodes', __args__, opts=opts, typ=GetNodesResult).value
 
     return AwaitableGetNodesResult(
         cpu_counts=pulumi.get(__ret__, 'cpu_counts'),
@@ -187,17 +185,15 @@
 @_utilities.lift_output_func(get_nodes)
 def get_nodes_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNodesResult]:
     """
     Retrieves information about all available nodes.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     available_nodes = proxmoxve.Cluster.get_nodes()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/options.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/cluster/options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/cluster/outputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/cluster/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/config/vars.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ct/_inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,55 +31,55 @@
 @pulumi.input_type
 class ContainerCloneArgs:
     def __init__(__self__, *,
                  vm_id: pulumi.Input[int],
                  datastore_id: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[int] vm_id: The container identifier
-        :param pulumi.Input[str] datastore_id: The identifier for the datastore to create the
-               disk in (defaults to `local`).
-        :param pulumi.Input[str] node_name: The name of the node to assign the container to.
+        :param pulumi.Input[int] vm_id: The identifier for the source container.
+        :param pulumi.Input[str] datastore_id: The identifier for the target datastore.
+        :param pulumi.Input[str] node_name: The name of the source node (leave blank, if
+               equal to the `node_name` argument).
         """
         pulumi.set(__self__, "vm_id", vm_id)
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
 
     @property
     @pulumi.getter(name="vmId")
     def vm_id(self) -> pulumi.Input[int]:
         """
-        The container identifier
+        The identifier for the source container.
         """
         return pulumi.get(self, "vm_id")
 
     @vm_id.setter
     def vm_id(self, value: pulumi.Input[int]):
         pulumi.set(self, "vm_id", value)
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier for the datastore to create the
-        disk in (defaults to `local`).
+        The identifier for the target datastore.
         """
         return pulumi.get(self, "datastore_id")
 
     @datastore_id.setter
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the node to assign the container to.
+        The name of the source node (leave blank, if
+        equal to the `node_name` argument).
         """
         return pulumi.get(self, "node_name")
 
     @node_name.setter
     def node_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "node_name", value)
 
@@ -87,31 +87,31 @@
 @pulumi.input_type
 class ContainerConsoleArgs:
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  tty_count: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[bool] enabled: Whether to enable the network device (defaults
+        :param pulumi.Input[bool] enabled: Whether to enable the console device (defaults
                to `true`).
         :param pulumi.Input[int] tty_count: The number of available TTY (defaults to `2`).
-        :param pulumi.Input[str] type: The type (defaults to `unmanaged`).
+        :param pulumi.Input[str] type: The console mode (defaults to `tty`).
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if tty_count is not None:
             pulumi.set(__self__, "tty_count", tty_count)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether to enable the network device (defaults
+        Whether to enable the console device (defaults
         to `true`).
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
@@ -128,15 +128,15 @@
     def tty_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "tty_count", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The type (defaults to `unmanaged`).
+        The console mode (defaults to `tty`).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -200,16 +200,16 @@
 class ContainerDiskArgs:
     def __init__(__self__, *,
                  datastore_id: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[str] datastore_id: The identifier for the datastore to create the
                disk in (defaults to `local`).
-        :param pulumi.Input[int] size: Volume size (only for volume mount points).
-               Can be specified with a unit suffix (e.g. `10G`).
+        :param pulumi.Input[int] size: The size of the root filesystem in gigabytes (defaults
+               to `4`). Requires `datastore_id` to be set.
         """
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if size is not None:
             pulumi.set(__self__, "size", size)
 
     @property
@@ -225,16 +225,16 @@
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
     @property
     @pulumi.getter
     def size(self) -> Optional[pulumi.Input[int]]:
         """
-        Volume size (only for volume mount points).
-        Can be specified with a unit suffix (e.g. `10G`).
+        The size of the root filesystem in gigabytes (defaults
+        to `4`). Requires `datastore_id` to be set.
         """
         return pulumi.get(self, "size")
 
     @size.setter
     def size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "size", value)
 
@@ -392,19 +392,17 @@
 @pulumi.input_type
 class ContainerInitializationDnsArgs:
     def __init__(__self__, *,
                  domain: Optional[pulumi.Input[str]] = None,
                  server: Optional[pulumi.Input[str]] = None,
                  servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        :param pulumi.Input[str] domain: The DNS search domain.
-        :param pulumi.Input[str] server: The DNS server. The `server` attribute is
-               deprecated and will be removed in a future release. Please use
-               the `servers` attribute instead.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The list of DNS servers.
+        :param pulumi.Input[str] domain: The DNS search domain
+        :param pulumi.Input[str] server: The DNS server
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The list of DNS servers
         """
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if server is not None:
             warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
             pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
         if server is not None:
@@ -412,208 +410,198 @@
         if servers is not None:
             pulumi.set(__self__, "servers", servers)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[pulumi.Input[str]]:
         """
-        The DNS search domain.
+        The DNS search domain
         """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter
     def server(self) -> Optional[pulumi.Input[str]]:
         """
-        The DNS server. The `server` attribute is
-        deprecated and will be removed in a future release. Please use
-        the `servers` attribute instead.
+        The DNS server
         """
         warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
         pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
 
         return pulumi.get(self, "server")
 
     @server.setter
     def server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server", value)
 
     @property
     @pulumi.getter
     def servers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The list of DNS servers.
+        The list of DNS servers
         """
         return pulumi.get(self, "servers")
 
     @servers.setter
     def servers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "servers", value)
 
 
 @pulumi.input_type
 class ContainerInitializationIpConfigArgs:
     def __init__(__self__, *,
                  ipv4: Optional[pulumi.Input['ContainerInitializationIpConfigIpv4Args']] = None,
                  ipv6: Optional[pulumi.Input['ContainerInitializationIpConfigIpv6Args']] = None):
         """
-        :param pulumi.Input['ContainerInitializationIpConfigIpv4Args'] ipv4: The IPv4 configuration.
-        :param pulumi.Input['ContainerInitializationIpConfigIpv6Args'] ipv6: The IPv4 configuration.
+        :param pulumi.Input['ContainerInitializationIpConfigIpv4Args'] ipv4: The IPv4 configuration
+        :param pulumi.Input['ContainerInitializationIpConfigIpv6Args'] ipv6: The IPv6 configuration
         """
         if ipv4 is not None:
             pulumi.set(__self__, "ipv4", ipv4)
         if ipv6 is not None:
             pulumi.set(__self__, "ipv6", ipv6)
 
     @property
     @pulumi.getter
     def ipv4(self) -> Optional[pulumi.Input['ContainerInitializationIpConfigIpv4Args']]:
         """
-        The IPv4 configuration.
+        The IPv4 configuration
         """
         return pulumi.get(self, "ipv4")
 
     @ipv4.setter
     def ipv4(self, value: Optional[pulumi.Input['ContainerInitializationIpConfigIpv4Args']]):
         pulumi.set(self, "ipv4", value)
 
     @property
     @pulumi.getter
     def ipv6(self) -> Optional[pulumi.Input['ContainerInitializationIpConfigIpv6Args']]:
         """
-        The IPv4 configuration.
+        The IPv6 configuration
         """
         return pulumi.get(self, "ipv6")
 
     @ipv6.setter
     def ipv6(self, value: Optional[pulumi.Input['ContainerInitializationIpConfigIpv6Args']]):
         pulumi.set(self, "ipv6", value)
 
 
 @pulumi.input_type
 class ContainerInitializationIpConfigIpv4Args:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  gateway: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] address: The IPv6 address (use `dhcp` for
-               autodiscovery).
-        :param pulumi.Input[str] gateway: The IPv6 gateway (must be omitted
-               when `dhcp` is used as the address).
+        :param pulumi.Input[str] address: The IPv4 address
+        :param pulumi.Input[str] gateway: The IPv4 gateway
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 address (use `dhcp` for
-        autodiscovery).
+        The IPv4 address
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 gateway (must be omitted
-        when `dhcp` is used as the address).
+        The IPv4 gateway
         """
         return pulumi.get(self, "gateway")
 
     @gateway.setter
     def gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway", value)
 
 
 @pulumi.input_type
 class ContainerInitializationIpConfigIpv6Args:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  gateway: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] address: The IPv6 address (use `dhcp` for
-               autodiscovery).
-        :param pulumi.Input[str] gateway: The IPv6 gateway (must be omitted
-               when `dhcp` is used as the address).
+        :param pulumi.Input[str] address: The IPv6 address
+        :param pulumi.Input[str] gateway: The IPv6 gateway
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 address (use `dhcp` for
-        autodiscovery).
+        The IPv6 address
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 gateway (must be omitted
-        when `dhcp` is used as the address).
+        The IPv6 gateway
         """
         return pulumi.get(self, "gateway")
 
     @gateway.setter
     def gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway", value)
 
 
 @pulumi.input_type
 class ContainerInitializationUserAccountArgs:
     def __init__(__self__, *,
                  keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  password: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: The SSH keys for the root account.
-        :param pulumi.Input[str] password: The password for the root account.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: The SSH keys
+        :param pulumi.Input[str] password: The SSH password
         """
         if keys is not None:
             pulumi.set(__self__, "keys", keys)
         if password is not None:
             pulumi.set(__self__, "password", password)
 
     @property
     @pulumi.getter
     def keys(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The SSH keys for the root account.
+        The SSH keys
         """
         return pulumi.get(self, "keys")
 
     @keys.setter
     def keys(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "keys", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        The password for the root account.
+        The SSH password
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ct/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                  timeout_update: Optional[pulumi.Input[int]] = None,
                  unprivileged: Optional[pulumi.Input[bool]] = None,
                  vm_id: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a Container resource.
         :param pulumi.Input[str] node_name: The name of the node to assign the container to.
         :param pulumi.Input['ContainerCloneArgs'] clone: The cloning configuration.
-        :param pulumi.Input['ContainerConsoleArgs'] console: Console.
+        :param pulumi.Input['ContainerConsoleArgs'] console: The console configuration.
         :param pulumi.Input['ContainerCpuArgs'] cpu: The CPU configuration.
         :param pulumi.Input[str] description: The description.
         :param pulumi.Input['ContainerDiskArgs'] disk: The disk configuration.
         :param pulumi.Input['ContainerFeaturesArgs'] features: The container feature flags. Changing flags (except nesting) is only allowed for `root@pam` authenticated user.
         :param pulumi.Input[str] hook_script_file_id: The identifier for a file containing a hook script (needs to be executable).
         :param pulumi.Input['ContainerInitializationArgs'] initialization: The initialization configuration.
         :param pulumi.Input['ContainerMemoryArgs'] memory: The memory configuration.
@@ -157,15 +157,15 @@
     def clone(self, value: Optional[pulumi.Input['ContainerCloneArgs']]):
         pulumi.set(self, "clone", value)
 
     @property
     @pulumi.getter
     def console(self) -> Optional[pulumi.Input['ContainerConsoleArgs']]:
         """
-        Console.
+        The console configuration.
         """
         return pulumi.get(self, "console")
 
     @console.setter
     def console(self, value: Optional[pulumi.Input['ContainerConsoleArgs']]):
         pulumi.set(self, "console", value)
 
@@ -484,15 +484,15 @@
                  timeout_start: Optional[pulumi.Input[int]] = None,
                  timeout_update: Optional[pulumi.Input[int]] = None,
                  unprivileged: Optional[pulumi.Input[bool]] = None,
                  vm_id: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering Container resources.
         :param pulumi.Input['ContainerCloneArgs'] clone: The cloning configuration.
-        :param pulumi.Input['ContainerConsoleArgs'] console: Console.
+        :param pulumi.Input['ContainerConsoleArgs'] console: The console configuration.
         :param pulumi.Input['ContainerCpuArgs'] cpu: The CPU configuration.
         :param pulumi.Input[str] description: The description.
         :param pulumi.Input['ContainerDiskArgs'] disk: The disk configuration.
         :param pulumi.Input['ContainerFeaturesArgs'] features: The container feature flags. Changing flags (except nesting) is only allowed for `root@pam` authenticated user.
         :param pulumi.Input[str] hook_script_file_id: The identifier for a file containing a hook script (needs to be executable).
         :param pulumi.Input['ContainerInitializationArgs'] initialization: The initialization configuration.
         :param pulumi.Input['ContainerMemoryArgs'] memory: The memory configuration.
@@ -589,15 +589,15 @@
     def clone(self, value: Optional[pulumi.Input['ContainerCloneArgs']]):
         pulumi.set(self, "clone", value)
 
     @property
     @pulumi.getter
     def console(self) -> Optional[pulumi.Input['ContainerConsoleArgs']]:
         """
-        Console.
+        The console configuration.
         """
         return pulumi.get(self, "console")
 
     @console.setter
     def console(self, value: Optional[pulumi.Input['ContainerConsoleArgs']]):
         pulumi.set(self, "console", value)
 
@@ -944,15 +944,15 @@
         ```sh
         $ pulumi import proxmoxve:CT/container:Container ubuntu_container first-node/1234
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ContainerCloneArgs']] clone: The cloning configuration.
-        :param pulumi.Input[pulumi.InputType['ContainerConsoleArgs']] console: Console.
+        :param pulumi.Input[pulumi.InputType['ContainerConsoleArgs']] console: The console configuration.
         :param pulumi.Input[pulumi.InputType['ContainerCpuArgs']] cpu: The CPU configuration.
         :param pulumi.Input[str] description: The description.
         :param pulumi.Input[pulumi.InputType['ContainerDiskArgs']] disk: The disk configuration.
         :param pulumi.Input[pulumi.InputType['ContainerFeaturesArgs']] features: The container feature flags. Changing flags (except nesting) is only allowed for `root@pam` authenticated user.
         :param pulumi.Input[str] hook_script_file_id: The identifier for a file containing a hook script (needs to be executable).
         :param pulumi.Input[pulumi.InputType['ContainerInitializationArgs']] initialization: The initialization configuration.
         :param pulumi.Input[pulumi.InputType['ContainerMemoryArgs']] memory: The memory configuration.
@@ -1118,15 +1118,15 @@
         Get an existing Container resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ContainerCloneArgs']] clone: The cloning configuration.
-        :param pulumi.Input[pulumi.InputType['ContainerConsoleArgs']] console: Console.
+        :param pulumi.Input[pulumi.InputType['ContainerConsoleArgs']] console: The console configuration.
         :param pulumi.Input[pulumi.InputType['ContainerCpuArgs']] cpu: The CPU configuration.
         :param pulumi.Input[str] description: The description.
         :param pulumi.Input[pulumi.InputType['ContainerDiskArgs']] disk: The disk configuration.
         :param pulumi.Input[pulumi.InputType['ContainerFeaturesArgs']] features: The container feature flags. Changing flags (except nesting) is only allowed for `root@pam` authenticated user.
         :param pulumi.Input[str] hook_script_file_id: The identifier for a file containing a hook script (needs to be executable).
         :param pulumi.Input[pulumi.InputType['ContainerInitializationArgs']] initialization: The initialization configuration.
         :param pulumi.Input[pulumi.InputType['ContainerMemoryArgs']] memory: The memory configuration.
@@ -1195,15 +1195,15 @@
         """
         return pulumi.get(self, "clone")
 
     @property
     @pulumi.getter
     def console(self) -> pulumi.Output[Optional['outputs.ContainerConsole']]:
         """
-        Console.
+        The console configuration.
         """
         return pulumi.get(self, "console")
 
     @property
     @pulumi.getter
     def cpu(self) -> pulumi.Output[Optional['outputs.ContainerCpu']]:
         """
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ct/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,47 +53,47 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  vm_id: int,
                  datastore_id: Optional[str] = None,
                  node_name: Optional[str] = None):
         """
-        :param int vm_id: The container identifier
-        :param str datastore_id: The identifier for the datastore to create the
-               disk in (defaults to `local`).
-        :param str node_name: The name of the node to assign the container to.
+        :param int vm_id: The identifier for the source container.
+        :param str datastore_id: The identifier for the target datastore.
+        :param str node_name: The name of the source node (leave blank, if
+               equal to the `node_name` argument).
         """
         pulumi.set(__self__, "vm_id", vm_id)
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
 
     @property
     @pulumi.getter(name="vmId")
     def vm_id(self) -> int:
         """
-        The container identifier
+        The identifier for the source container.
         """
         return pulumi.get(self, "vm_id")
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[str]:
         """
-        The identifier for the datastore to create the
-        disk in (defaults to `local`).
+        The identifier for the target datastore.
         """
         return pulumi.get(self, "datastore_id")
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[str]:
         """
-        The name of the node to assign the container to.
+        The name of the source node (leave blank, if
+        equal to the `node_name` argument).
         """
         return pulumi.get(self, "node_name")
 
 
 @pulumi.output_type
 class ContainerConsole(dict):
     @staticmethod
@@ -114,31 +114,31 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  enabled: Optional[bool] = None,
                  tty_count: Optional[int] = None,
                  type: Optional[str] = None):
         """
-        :param bool enabled: Whether to enable the network device (defaults
+        :param bool enabled: Whether to enable the console device (defaults
                to `true`).
         :param int tty_count: The number of available TTY (defaults to `2`).
-        :param str type: The type (defaults to `unmanaged`).
+        :param str type: The console mode (defaults to `tty`).
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if tty_count is not None:
             pulumi.set(__self__, "tty_count", tty_count)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
-        Whether to enable the network device (defaults
+        Whether to enable the console device (defaults
         to `true`).
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="ttyCount")
     def tty_count(self) -> Optional[int]:
@@ -147,15 +147,15 @@
         """
         return pulumi.get(self, "tty_count")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        The type (defaults to `unmanaged`).
+        The console mode (defaults to `tty`).
         """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class ContainerCpu(dict):
     def __init__(__self__, *,
@@ -220,16 +220,16 @@
 
     def __init__(__self__, *,
                  datastore_id: Optional[str] = None,
                  size: Optional[int] = None):
         """
         :param str datastore_id: The identifier for the datastore to create the
                disk in (defaults to `local`).
-        :param int size: Volume size (only for volume mount points).
-               Can be specified with a unit suffix (e.g. `10G`).
+        :param int size: The size of the root filesystem in gigabytes (defaults
+               to `4`). Requires `datastore_id` to be set.
         """
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if size is not None:
             pulumi.set(__self__, "size", size)
 
     @property
@@ -241,16 +241,16 @@
         """
         return pulumi.get(self, "datastore_id")
 
     @property
     @pulumi.getter
     def size(self) -> Optional[int]:
         """
-        Volume size (only for volume mount points).
-        Can be specified with a unit suffix (e.g. `10G`).
+        The size of the root filesystem in gigabytes (defaults
+        to `4`). Requires `datastore_id` to be set.
         """
         return pulumi.get(self, "size")
 
 
 @pulumi.output_type
 class ContainerFeatures(dict):
     def __init__(__self__, *,
@@ -391,185 +391,173 @@
 @pulumi.output_type
 class ContainerInitializationDns(dict):
     def __init__(__self__, *,
                  domain: Optional[str] = None,
                  server: Optional[str] = None,
                  servers: Optional[Sequence[str]] = None):
         """
-        :param str domain: The DNS search domain.
-        :param str server: The DNS server. The `server` attribute is
-               deprecated and will be removed in a future release. Please use
-               the `servers` attribute instead.
-        :param Sequence[str] servers: The list of DNS servers.
+        :param str domain: The DNS search domain
+        :param str server: The DNS server
+        :param Sequence[str] servers: The list of DNS servers
         """
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if server is not None:
             pulumi.set(__self__, "server", server)
         if servers is not None:
             pulumi.set(__self__, "servers", servers)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[str]:
         """
-        The DNS search domain.
+        The DNS search domain
         """
         return pulumi.get(self, "domain")
 
     @property
     @pulumi.getter
     def server(self) -> Optional[str]:
         """
-        The DNS server. The `server` attribute is
-        deprecated and will be removed in a future release. Please use
-        the `servers` attribute instead.
+        The DNS server
         """
         warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
         pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
 
         return pulumi.get(self, "server")
 
     @property
     @pulumi.getter
     def servers(self) -> Optional[Sequence[str]]:
         """
-        The list of DNS servers.
+        The list of DNS servers
         """
         return pulumi.get(self, "servers")
 
 
 @pulumi.output_type
 class ContainerInitializationIpConfig(dict):
     def __init__(__self__, *,
                  ipv4: Optional['outputs.ContainerInitializationIpConfigIpv4'] = None,
                  ipv6: Optional['outputs.ContainerInitializationIpConfigIpv6'] = None):
         """
-        :param 'ContainerInitializationIpConfigIpv4Args' ipv4: The IPv4 configuration.
-        :param 'ContainerInitializationIpConfigIpv6Args' ipv6: The IPv4 configuration.
+        :param 'ContainerInitializationIpConfigIpv4Args' ipv4: The IPv4 configuration
+        :param 'ContainerInitializationIpConfigIpv6Args' ipv6: The IPv6 configuration
         """
         if ipv4 is not None:
             pulumi.set(__self__, "ipv4", ipv4)
         if ipv6 is not None:
             pulumi.set(__self__, "ipv6", ipv6)
 
     @property
     @pulumi.getter
     def ipv4(self) -> Optional['outputs.ContainerInitializationIpConfigIpv4']:
         """
-        The IPv4 configuration.
+        The IPv4 configuration
         """
         return pulumi.get(self, "ipv4")
 
     @property
     @pulumi.getter
     def ipv6(self) -> Optional['outputs.ContainerInitializationIpConfigIpv6']:
         """
-        The IPv4 configuration.
+        The IPv6 configuration
         """
         return pulumi.get(self, "ipv6")
 
 
 @pulumi.output_type
 class ContainerInitializationIpConfigIpv4(dict):
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  gateway: Optional[str] = None):
         """
-        :param str address: The IPv6 address (use `dhcp` for
-               autodiscovery).
-        :param str gateway: The IPv6 gateway (must be omitted
-               when `dhcp` is used as the address).
+        :param str address: The IPv4 address
+        :param str gateway: The IPv4 gateway
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
         """
-        The IPv6 address (use `dhcp` for
-        autodiscovery).
+        The IPv4 address
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[str]:
         """
-        The IPv6 gateway (must be omitted
-        when `dhcp` is used as the address).
+        The IPv4 gateway
         """
         return pulumi.get(self, "gateway")
 
 
 @pulumi.output_type
 class ContainerInitializationIpConfigIpv6(dict):
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  gateway: Optional[str] = None):
         """
-        :param str address: The IPv6 address (use `dhcp` for
-               autodiscovery).
-        :param str gateway: The IPv6 gateway (must be omitted
-               when `dhcp` is used as the address).
+        :param str address: The IPv6 address
+        :param str gateway: The IPv6 gateway
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
         """
-        The IPv6 address (use `dhcp` for
-        autodiscovery).
+        The IPv6 address
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[str]:
         """
-        The IPv6 gateway (must be omitted
-        when `dhcp` is used as the address).
+        The IPv6 gateway
         """
         return pulumi.get(self, "gateway")
 
 
 @pulumi.output_type
 class ContainerInitializationUserAccount(dict):
     def __init__(__self__, *,
                  keys: Optional[Sequence[str]] = None,
                  password: Optional[str] = None):
         """
-        :param Sequence[str] keys: The SSH keys for the root account.
-        :param str password: The password for the root account.
+        :param Sequence[str] keys: The SSH keys
+        :param str password: The SSH password
         """
         if keys is not None:
             pulumi.set(__self__, "keys", keys)
         if password is not None:
             pulumi.set(__self__, "password", password)
 
     @property
     @pulumi.getter
     def keys(self) -> Optional[Sequence[str]]:
         """
-        The SSH keys for the root account.
+        The SSH keys
         """
         return pulumi.get(self, "keys")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
         """
-        The password for the root account.
+        The SSH password
         """
         return pulumi.get(self, "password")
 
 
 @pulumi.output_type
 class ContainerMemory(dict):
     def __init__(__self__, *,
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/download/file.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/download/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,14 @@
                  verify: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Manages files upload using PVE download-url API. It can be fully compatible and faster replacement for image files created using `Storage.File`. Supports images for VMs (ISO images) and LXC (CT Templates).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         release20231228_debian12_bookworm_qcow2_img = proxmoxve.download.File("release20231228Debian12BookwormQcow2Img",
             checksum="d2fbcf11fb28795842e91364d8c7b69f1870db09ff299eb94e4fbbfa510eb78d141e74c1f4bf6dfa0b7e33d0c3b66e6751886feadb4e9916f778bab1776bdf1b",
             checksum_algorithm="sha512",
@@ -486,15 +485,14 @@
             url="https://cloud-images.ubuntu.com/releases/22.04/release-20231211/ubuntu-22.04-server-cloudimg-amd64-root.tar.xz")
         latest_ubuntu22_jammy_lxc_img = proxmoxve.download.File("latestUbuntu22JammyLxcImg",
             content_type="vztmpl",
             datastore_id="local",
             node_name="pve",
             url="https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-amd64.tar.gz")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] checksum: The expected checksum of the file.
         :param pulumi.Input[str] checksum_algorithm: The algorithm to calculate the checksum of the file. Must be `md5` | `sha1` | `sha224` | `sha256` | `sha384` | `sha512`.
         :param pulumi.Input[str] content_type: The file content type. Must be `iso` for VM images or `vztmpl` for LXC images.
         :param pulumi.Input[str] datastore_id: The identifier for the target datastore.
@@ -514,15 +512,14 @@
                  args: FileArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages files upload using PVE download-url API. It can be fully compatible and faster replacement for image files created using `Storage.File`. Supports images for VMs (ISO images) and LXC (CT Templates).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         release20231228_debian12_bookworm_qcow2_img = proxmoxve.download.File("release20231228Debian12BookwormQcow2Img",
             checksum="d2fbcf11fb28795842e91364d8c7b69f1870db09ff299eb94e4fbbfa510eb78d141e74c1f4bf6dfa0b7e33d0c3b66e6751886feadb4e9916f778bab1776bdf1b",
             checksum_algorithm="sha512",
@@ -558,15 +555,14 @@
             url="https://cloud-images.ubuntu.com/releases/22.04/release-20231211/ubuntu-22.04-server-cloudimg-amd64-root.tar.xz")
         latest_ubuntu22_jammy_lxc_img = proxmoxve.download.File("latestUbuntu22JammyLxcImg",
             content_type="vztmpl",
             datastore_id="local",
             node_name="pve",
             url="https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-amd64.tar.gz")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param FileArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/get_node.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/get_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,22 +140,20 @@
 def get_node(node_name: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNodeResult:
     """
     Retrieves information about node.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     node = proxmoxve.get_node()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: The node name.
     """
     __args__ = dict()
     __args__['nodeName'] = node_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -177,20 +175,18 @@
 def get_node_output(node_name: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNodeResult]:
     """
     Retrieves information about node.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     node = proxmoxve.get_node()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: The node name.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_group.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/get_ha_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,24 +107,22 @@
 def get_ha_group(group: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetHAGroupResult:
     """
     Retrieves information about a specific High Availability group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     all = proxmoxve.HA.get_ha_groups()
     example = [proxmoxve.HA.get_ha_group(group=__value) for __key, __value in all.group_ids]
     pulumi.export("proxmoxVirtualEnvironmentHagroupsFull", example)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str group: The identifier of the High Availability group to read.
     """
     __args__ = dict()
     __args__['group'] = group
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -143,22 +141,20 @@
 def get_ha_group_output(group: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetHAGroupResult]:
     """
     Retrieves information about a specific High Availability group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     all = proxmoxve.HA.get_ha_groups()
     example = [proxmoxve.HA.get_ha_group(group=__value) for __key, __value in all.group_ids]
     pulumi.export("proxmoxVirtualEnvironmentHagroupsFull", example)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str group: The identifier of the High Availability group to read.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_groups.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/get_ha_groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,23 +58,21 @@
 
 def get_ha_groups(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetHAGroupsResult:
     """
     Retrieves the list of High Availability groups.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example = proxmoxve.HA.get_ha_groups()
     pulumi.export("dataProxmoxVirtualEnvironmentHagroups", example.group_ids)
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:HA/getHAGroups:getHAGroups', __args__, opts=opts, typ=GetHAGroupsResult).value
 
     return AwaitableGetHAGroupsResult(
         group_ids=pulumi.get(__ret__, 'group_ids'),
@@ -84,18 +82,16 @@
 @_utilities.lift_output_func(get_ha_groups)
 def get_ha_groups_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetHAGroupsResult]:
     """
     Retrieves the list of High Availability groups.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example = proxmoxve.HA.get_ha_groups()
     pulumi.export("dataProxmoxVirtualEnvironmentHagroups", example.group_ids)
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_resource.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/get_ha_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,24 +131,22 @@
 def get_ha_resource(resource_id: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetHAResourceResult:
     """
     Retrieves the list of High Availability resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     all = proxmoxve.HA.get_ha_resources()
     example = [proxmoxve.HA.get_ha_resource(resource_id=__value) for __key, __value in all.resource_ids]
     pulumi.export("proxmoxVirtualEnvironmentHaresourcesFull", example)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str resource_id: The identifier of the Proxmox HA resource to read.
     """
     __args__ = dict()
     __args__['resourceId'] = resource_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -169,22 +167,20 @@
 def get_ha_resource_output(resource_id: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetHAResourceResult]:
     """
     Retrieves the list of High Availability resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     all = proxmoxve.HA.get_ha_resources()
     example = [proxmoxve.HA.get_ha_resource(resource_id=__value) for __key, __value in all.resource_ids]
     pulumi.export("proxmoxVirtualEnvironmentHaresourcesFull", example)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str resource_id: The identifier of the Proxmox HA resource to read.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/get_ha_resources.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/get_ha_resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,27 +71,25 @@
 def get_ha_resources(type: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetHAResourcesResult:
     """
     Retrieves the list of High Availability resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example_all = proxmoxve.HA.get_ha_resources()
     example_vm = proxmoxve.HA.get_ha_resources(type="vm")
     pulumi.export("dataProxmoxVirtualEnvironmentHaresources", {
         "all": example_all.resource_ids,
         "vms": example_vm.resource_ids,
     })
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str type: The type of High Availability resources to fetch (`vm` or `ct`). All resources will be fetched if this option is unset.
     """
     __args__ = dict()
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -107,25 +105,23 @@
 def get_ha_resources_output(type: Optional[pulumi.Input[Optional[str]]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetHAResourcesResult]:
     """
     Retrieves the list of High Availability resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example_all = proxmoxve.HA.get_ha_resources()
     example_vm = proxmoxve.HA.get_ha_resources(type="vm")
     pulumi.export("dataProxmoxVirtualEnvironmentHaresources", {
         "all": example_all.resource_ids,
         "vms": example_vm.resource_ids,
     })
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str type: The type of High Availability resources to fetch (`vm` or `ct`). All resources will be fetched if this option is unset.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/ha_group.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/ha_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,14 @@
                  restricted: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Manages a High Availability group in a Proxmox VE cluster.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         example = proxmoxve.ha.HAGroup("example",
             group="example",
             comment="This is a comment.",
@@ -213,15 +212,14 @@
                 "node1": None,
                 "node2": 2,
                 "node3": 1,
             },
             restricted=True,
             no_failback=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         #!/usr/bin/env sh
 
         HA groups can be imported using their name, e.g.:
 
@@ -244,15 +242,14 @@
                  args: HAGroupArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a High Availability group in a Proxmox VE cluster.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         example = proxmoxve.ha.HAGroup("example",
             group="example",
             comment="This is a comment.",
@@ -260,15 +257,14 @@
                 "node1": None,
                 "node2": 2,
                 "node3": 1,
             },
             restricted=True,
             no_failback=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         #!/usr/bin/env sh
 
         HA groups can be imported using their name, e.g.:
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/ha/ha_resource.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/ha/ha_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,27 +264,25 @@
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages Proxmox HA resources.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         example = proxmoxve.ha.HAResource("example",
             resource_id="vm:123",
             state="started",
             group="example",
             comment="Managed by Terraform",
             opts=pulumi.ResourceOptions(depends_on=[proxmox_virtual_environment_hagroup["example"]]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         #!/usr/bin/env sh
 
         HA resources can be imported using their identifiers, e.g.:
 
@@ -309,27 +307,25 @@
                  args: HAResourceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages Proxmox HA resources.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         example = proxmoxve.ha.HAResource("example",
             resource_id="vm:123",
             state="started",
             group="example",
             comment="Managed by Terraform",
             opts=pulumi.ResourceOptions(depends_on=[proxmox_virtual_environment_hagroup["example"]]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         #!/usr/bin/env sh
 
         HA resources can be imported using their identifiers, e.g.:
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/__init__.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/get_mappings.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/get_mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,27 +97,25 @@
                  type: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMappingsResult:
     """
     Retrieves a list of hardware mapping resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example_pci = proxmoxve.Hardware.get_mappings(check_node="pve",
         type="pci")
     example_usb = proxmoxve.Hardware.get_mappings(check_node="pve",
         type="usb")
     pulumi.export("dataProxmoxVirtualEnvironmentHardwareMappingsPci", example_pci)
     pulumi.export("dataProxmoxVirtualEnvironmentHardwareMappingsUsb", example_usb)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str check_node: The name of the node whose configurations should be checked for correctness.
     :param str type: The type of the hardware mappings.
     """
     __args__ = dict()
     __args__['checkNode'] = check_node
@@ -138,26 +136,24 @@
                         type: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMappingsResult]:
     """
     Retrieves a list of hardware mapping resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example_pci = proxmoxve.Hardware.get_mappings(check_node="pve",
         type="pci")
     example_usb = proxmoxve.Hardware.get_mappings(check_node="pve",
         type="usb")
     pulumi.export("dataProxmoxVirtualEnvironmentHardwareMappingsPci", example_pci)
     pulumi.export("dataProxmoxVirtualEnvironmentHardwareMappingsUsb", example_usb)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str check_node: The name of the node whose configurations should be checked for correctness.
     :param str type: The type of the hardware mappings.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/_inputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/get_pci.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/get_pci.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,23 +96,21 @@
 def get_pci(name: Optional[str] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPciResult:
     """
     Retrieves a PCI hardware mapping from a Proxmox VE cluster.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example = proxmoxve.Hardware.mapping.get_pci(name="example")
     pulumi.export("dataProxmoxVirtualEnvironmentHardwareMappingPci", example)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of this PCI hardware mapping.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -130,21 +128,19 @@
 def get_pci_output(name: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPciResult]:
     """
     Retrieves a PCI hardware mapping from a Proxmox VE cluster.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example = proxmoxve.Hardware.mapping.get_pci(name="example")
     pulumi.export("dataProxmoxVirtualEnvironmentHardwareMappingPci", example)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of this PCI hardware mapping.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/get_usb.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/get_usb.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,23 +84,21 @@
 def get_usb(name: Optional[str] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUsbResult:
     """
     Retrieves a USB hardware mapping from a Proxmox VE cluster.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example = proxmoxve.Hardware.mapping.get_usb(name="example")
     pulumi.export("dataProxmoxVirtualEnvironmentHardwareMappingUsb", example)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of this USB hardware mapping.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -117,21 +115,19 @@
 def get_usb_output(name: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUsbResult]:
     """
     Retrieves a USB hardware mapping from a Proxmox VE cluster.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example = proxmoxve.Hardware.mapping.get_usb(name="example")
     pulumi.export("dataProxmoxVirtualEnvironmentHardwareMappingUsb", example)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of this USB hardware mapping.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/outputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/pci.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/pci.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                  maps: pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]],
                  comment: Optional[pulumi.Input[str]] = None,
                  mediated_devices: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Pci resource.
         :param pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]] maps: The actual map of devices for the PCI hardware mapping.
-        :param pulumi.Input[str] comment: The comment of the mapped PCI device.
+        :param pulumi.Input[str] comment: The comment of this PCI hardware mapping.
         :param pulumi.Input[bool] mediated_devices: Indicates whether to enable mediated devices.
         :param pulumi.Input[str] name: The name of this PCI hardware mapping.
         """
         pulumi.set(__self__, "maps", maps)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if mediated_devices is not None:
@@ -47,15 +47,15 @@
     def maps(self, value: pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]]):
         pulumi.set(self, "maps", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        The comment of the mapped PCI device.
+        The comment of this PCI hardware mapping.
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -89,15 +89,15 @@
     def __init__(__self__, *,
                  comment: Optional[pulumi.Input[str]] = None,
                  maps: Optional[pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]]] = None,
                  mediated_devices: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Pci resources.
-        :param pulumi.Input[str] comment: The comment of the mapped PCI device.
+        :param pulumi.Input[str] comment: The comment of this PCI hardware mapping.
         :param pulumi.Input[Sequence[pulumi.Input['PciMapArgs']]] maps: The actual map of devices for the PCI hardware mapping.
         :param pulumi.Input[bool] mediated_devices: Indicates whether to enable mediated devices.
         :param pulumi.Input[str] name: The name of this PCI hardware mapping.
         """
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if maps is not None:
@@ -107,15 +107,15 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        The comment of the mapped PCI device.
+        The comment of this PCI hardware mapping.
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -177,15 +177,15 @@
 
         ```sh
         $ pulumi import proxmoxve:Hardware/mapping/pci:Pci example example
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] comment: The comment of the mapped PCI device.
+        :param pulumi.Input[str] comment: The comment of this PCI hardware mapping.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PciMapArgs']]]] maps: The actual map of devices for the PCI hardware mapping.
         :param pulumi.Input[bool] mediated_devices: Indicates whether to enable mediated devices.
         :param pulumi.Input[str] name: The name of this PCI hardware mapping.
         """
         ...
     @overload
     def __init__(__self__,
@@ -256,15 +256,15 @@
         """
         Get an existing Pci resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] comment: The comment of the mapped PCI device.
+        :param pulumi.Input[str] comment: The comment of this PCI hardware mapping.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PciMapArgs']]]] maps: The actual map of devices for the PCI hardware mapping.
         :param pulumi.Input[bool] mediated_devices: Indicates whether to enable mediated devices.
         :param pulumi.Input[str] name: The name of this PCI hardware mapping.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PciState.__new__(_PciState)
@@ -275,15 +275,15 @@
         __props__.__dict__["name"] = name
         return Pci(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def comment(self) -> pulumi.Output[Optional[str]]:
         """
-        The comment of the mapped PCI device.
+        The comment of this PCI hardware mapping.
         """
         return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter
     def maps(self) -> pulumi.Output[Sequence['outputs.PciMap']]:
         """
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/mapping/usb.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/mapping/usb.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(__self__, *,
                  maps: pulumi.Input[Sequence[pulumi.Input['UsbMapArgs']]],
                  comment: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Usb resource.
         :param pulumi.Input[Sequence[pulumi.Input['UsbMapArgs']]] maps: The actual map of devices for the hardware mapping.
-        :param pulumi.Input[str] comment: The comment of the mapped USB device.
+        :param pulumi.Input[str] comment: The comment of this USB hardware mapping.
         :param pulumi.Input[str] name: The name of this hardware mapping.
         """
         pulumi.set(__self__, "maps", maps)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -43,15 +43,15 @@
     def maps(self, value: pulumi.Input[Sequence[pulumi.Input['UsbMapArgs']]]):
         pulumi.set(self, "maps", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        The comment of the mapped USB device.
+        The comment of this USB hardware mapping.
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -72,30 +72,30 @@
 class _UsbState:
     def __init__(__self__, *,
                  comment: Optional[pulumi.Input[str]] = None,
                  maps: Optional[pulumi.Input[Sequence[pulumi.Input['UsbMapArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Usb resources.
-        :param pulumi.Input[str] comment: The comment of the mapped USB device.
+        :param pulumi.Input[str] comment: The comment of this USB hardware mapping.
         :param pulumi.Input[Sequence[pulumi.Input['UsbMapArgs']]] maps: The actual map of devices for the hardware mapping.
         :param pulumi.Input[str] name: The name of this hardware mapping.
         """
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if maps is not None:
             pulumi.set(__self__, "maps", maps)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        The comment of the mapped USB device.
+        The comment of this USB hardware mapping.
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -134,72 +134,68 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a USB hardware mapping in a Proxmox VE cluster.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         example = proxmoxve.hardware.mapping.Usb("example",
             comment="This is a comment",
             maps=[proxmoxve.hardware.mapping.UsbMapArgs(
                 comment="This is a device specific comment",
                 id="8087:0a2b",
                 node="pve",
                 path="1-8.2",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         #!/usr/bin/env sh
 
         A USB hardware mapping can be imported using their name, e.g.:
 
         ```sh
         $ pulumi import proxmoxve:Hardware/mapping/usb:Usb example example
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] comment: The comment of the mapped USB device.
+        :param pulumi.Input[str] comment: The comment of this USB hardware mapping.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UsbMapArgs']]]] maps: The actual map of devices for the hardware mapping.
         :param pulumi.Input[str] name: The name of this hardware mapping.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: UsbArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a USB hardware mapping in a Proxmox VE cluster.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         example = proxmoxve.hardware.mapping.Usb("example",
             comment="This is a comment",
             maps=[proxmoxve.hardware.mapping.UsbMapArgs(
                 comment="This is a device specific comment",
                 id="8087:0a2b",
                 node="pve",
                 path="1-8.2",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         #!/usr/bin/env sh
 
         A USB hardware mapping can be imported using their name, e.g.:
 
@@ -255,15 +251,15 @@
         """
         Get an existing Usb resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] comment: The comment of the mapped USB device.
+        :param pulumi.Input[str] comment: The comment of this USB hardware mapping.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UsbMapArgs']]]] maps: The actual map of devices for the hardware mapping.
         :param pulumi.Input[str] name: The name of this hardware mapping.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _UsbState.__new__(_UsbState)
 
@@ -272,15 +268,15 @@
         __props__.__dict__["name"] = name
         return Usb(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def comment(self) -> pulumi.Output[Optional[str]]:
         """
-        The comment of the mapped USB device.
+        The comment of this USB hardware mapping.
         """
         return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter
     def maps(self) -> pulumi.Output[Sequence['outputs.UsbMap']]:
         """
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hardware/outputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hardware/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/hosts.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         """
         Input properties used for looking up and filtering Hosts resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] addresses: The IP addresses.
         :param pulumi.Input[str] digest: The SHA1 digest.
         :param pulumi.Input[Sequence[pulumi.Input['HostsEntryArgs']]] entries: The host entries (conversion of `addresses` and `hostnames` into
                objects).
         :param pulumi.Input[Sequence[pulumi.Input['HostsEntryArgs']]] entry: A host entry (multiple blocks supported).
-        :param pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]] hostnames: The hostnames.
+        :param pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]] hostnames: The hostnames associated with each of the IP addresses.
         :param pulumi.Input[str] node_name: A node name.
         """
         if addresses is not None:
             pulumi.set(__self__, "addresses", addresses)
         if digest is not None:
             pulumi.set(__self__, "digest", digest)
         if entries is not None:
@@ -132,15 +132,15 @@
     def entry(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['HostsEntryArgs']]]]):
         pulumi.set(self, "entry", value)
 
     @property
     @pulumi.getter
     def hostnames(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]]]:
         """
-        The hostnames.
+        The hostnames associated with each of the IP addresses.
         """
         return pulumi.get(self, "hostnames")
 
     @hostnames.setter
     def hostnames(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]]]):
         pulumi.set(self, "hostnames", value)
 
@@ -262,15 +262,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] addresses: The IP addresses.
         :param pulumi.Input[str] digest: The SHA1 digest.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['HostsEntryArgs']]]] entries: The host entries (conversion of `addresses` and `hostnames` into
                objects).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['HostsEntryArgs']]]] entry: A host entry (multiple blocks supported).
-        :param pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]] hostnames: The hostnames.
+        :param pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]] hostnames: The hostnames associated with each of the IP addresses.
         :param pulumi.Input[str] node_name: A node name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _HostsState.__new__(_HostsState)
 
         __props__.__dict__["addresses"] = addresses
@@ -314,15 +314,15 @@
         """
         return pulumi.get(self, "entry")
 
     @property
     @pulumi.getter
     def hostnames(self) -> pulumi.Output[Sequence[Sequence[str]]]:
         """
-        The hostnames.
+        The hostnames associated with each of the IP addresses.
         """
         return pulumi.get(self, "hostnames")
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/__init__.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  enabled: Optional[pulumi.Input[bool]] = None,
                  input_policy: Optional[pulumi.Input[str]] = None,
                  log_ratelimit: Optional[pulumi.Input['FirewallLogRatelimitArgs']] = None,
                  output_policy: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Firewall resource.
         :param pulumi.Input[bool] ebtables: Enable ebtables rules cluster wide.
-        :param pulumi.Input[bool] enabled: Enable or disable the log rate limit.
+        :param pulumi.Input[bool] enabled: Enable or disable the firewall cluster wide.
         :param pulumi.Input[str] input_policy: The default input policy (`ACCEPT`, `DROP`, `REJECT`).
         :param pulumi.Input['FirewallLogRatelimitArgs'] log_ratelimit: The log rate limit.
         :param pulumi.Input[str] output_policy: The default output policy (`ACCEPT`, `DROP`, `REJECT`).
         """
         if ebtables is not None:
             pulumi.set(__self__, "ebtables", ebtables)
         if enabled is not None:
@@ -52,15 +52,15 @@
     def ebtables(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ebtables", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable or disable the log rate limit.
+        Enable or disable the firewall cluster wide.
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
@@ -108,15 +108,15 @@
                  enabled: Optional[pulumi.Input[bool]] = None,
                  input_policy: Optional[pulumi.Input[str]] = None,
                  log_ratelimit: Optional[pulumi.Input['FirewallLogRatelimitArgs']] = None,
                  output_policy: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Firewall resources.
         :param pulumi.Input[bool] ebtables: Enable ebtables rules cluster wide.
-        :param pulumi.Input[bool] enabled: Enable or disable the log rate limit.
+        :param pulumi.Input[bool] enabled: Enable or disable the firewall cluster wide.
         :param pulumi.Input[str] input_policy: The default input policy (`ACCEPT`, `DROP`, `REJECT`).
         :param pulumi.Input['FirewallLogRatelimitArgs'] log_ratelimit: The log rate limit.
         :param pulumi.Input[str] output_policy: The default output policy (`ACCEPT`, `DROP`, `REJECT`).
         """
         if ebtables is not None:
             pulumi.set(__self__, "ebtables", ebtables)
         if enabled is not None:
@@ -140,15 +140,15 @@
     def ebtables(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ebtables", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable or disable the log rate limit.
+        Enable or disable the firewall cluster wide.
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
@@ -201,15 +201,14 @@
                  output_policy: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages firewall options on the cluster level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         example = proxmoxve.network.Firewall("example",
             ebtables=False,
             enabled=False,
@@ -217,15 +216,14 @@
             log_ratelimit=proxmoxve.network.FirewallLogRatelimitArgs(
                 burst=10,
                 enabled=False,
                 rate="5/second",
             ),
             output_policy="ACCEPT")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Important Notes
 
         Be careful not to use this resource multiple times for the same node.
 
         ## Import
 
@@ -236,15 +234,15 @@
         ```sh
         $ pulumi import proxmoxve:Network/firewall:Firewall example example
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] ebtables: Enable ebtables rules cluster wide.
-        :param pulumi.Input[bool] enabled: Enable or disable the log rate limit.
+        :param pulumi.Input[bool] enabled: Enable or disable the firewall cluster wide.
         :param pulumi.Input[str] input_policy: The default input policy (`ACCEPT`, `DROP`, `REJECT`).
         :param pulumi.Input[pulumi.InputType['FirewallLogRatelimitArgs']] log_ratelimit: The log rate limit.
         :param pulumi.Input[str] output_policy: The default output policy (`ACCEPT`, `DROP`, `REJECT`).
         """
         ...
     @overload
     def __init__(__self__,
@@ -252,15 +250,14 @@
                  args: Optional[FirewallArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages firewall options on the cluster level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         example = proxmoxve.network.Firewall("example",
             ebtables=False,
             enabled=False,
@@ -268,15 +265,14 @@
             log_ratelimit=proxmoxve.network.FirewallLogRatelimitArgs(
                 burst=10,
                 enabled=False,
                 rate="5/second",
             ),
             output_policy="ACCEPT")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Important Notes
 
         Be careful not to use this resource multiple times for the same node.
 
         ## Import
 
@@ -341,15 +337,15 @@
         Get an existing Firewall resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] ebtables: Enable ebtables rules cluster wide.
-        :param pulumi.Input[bool] enabled: Enable or disable the log rate limit.
+        :param pulumi.Input[bool] enabled: Enable or disable the firewall cluster wide.
         :param pulumi.Input[str] input_policy: The default input policy (`ACCEPT`, `DROP`, `REJECT`).
         :param pulumi.Input[pulumi.InputType['FirewallLogRatelimitArgs']] log_ratelimit: The log rate limit.
         :param pulumi.Input[str] output_policy: The default output policy (`ACCEPT`, `DROP`, `REJECT`).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _FirewallState.__new__(_FirewallState)
@@ -369,15 +365,15 @@
         """
         return pulumi.get(self, "ebtables")
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Output[Optional[bool]]:
         """
-        Enable or disable the log rate limit.
+        Enable or disable the firewall cluster wide.
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="inputPolicy")
     def input_policy(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files 4% similar despite different names*

```diff
@@ -233,30 +233,28 @@
         """
         Aliases are used to see what devices or group of devices are affected by a rule.
         We can create aliases to identify an IP address or a network. Aliases can be
         created on the cluster level, on VM / Container level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         local_network = proxmoxve.network.FirewallAlias("localNetwork",
             node_name=proxmox_virtual_environment_vm["example"]["node_name"],
             vm_id=proxmox_virtual_environment_vm["example"]["vm_id"],
             cidr="192.168.0.0/23",
             comment="Managed by Terraform",
             opts=pulumi.ResourceOptions(depends_on=[proxmox_virtual_environment_vm["example"]]))
         ubuntu_vm = proxmoxve.network.FirewallAlias("ubuntuVm",
             cidr="192.168.0.1",
             comment="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cidr: Network/IP specification in CIDR format.
         :param pulumi.Input[str] comment: Alias comment.
         :param pulumi.Input[int] container_id: Container ID. Leave empty for cluster level aliases.
         :param pulumi.Input[str] name: Alias name.
@@ -272,30 +270,28 @@
         """
         Aliases are used to see what devices or group of devices are affected by a rule.
         We can create aliases to identify an IP address or a network. Aliases can be
         created on the cluster level, on VM / Container level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         local_network = proxmoxve.network.FirewallAlias("localNetwork",
             node_name=proxmox_virtual_environment_vm["example"]["node_name"],
             vm_id=proxmox_virtual_environment_vm["example"]["vm_id"],
             cidr="192.168.0.0/23",
             comment="Managed by Terraform",
             opts=pulumi.ResourceOptions(depends_on=[proxmox_virtual_environment_vm["example"]]))
         ubuntu_vm = proxmoxve.network.FirewallAlias("ubuntuVm",
             cidr="192.168.0.1",
             comment="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param FirewallAliasArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,17 @@
                  container_id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
                  vm_id: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a FirewallIPSet resource.
         :param pulumi.Input[Sequence[pulumi.Input['FirewallIPSetCidrArgs']]] cidrs: IP/CIDR block (multiple blocks supported).
-        :param pulumi.Input[str] comment: Arbitrary string annotation.
+        :param pulumi.Input[str] comment: IPSet comment.
         :param pulumi.Input[int] container_id: Container ID. Leave empty for cluster level aliases.
-        :param pulumi.Input[str] name: Network/IP specification in CIDR format.
+        :param pulumi.Input[str] name: IPSet name.
         :param pulumi.Input[str] node_name: Node name. Leave empty for cluster level aliases.
         :param pulumi.Input[int] vm_id: VM ID. Leave empty for cluster level aliases.
         """
         if cidrs is not None:
             pulumi.set(__self__, "cidrs", cidrs)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
@@ -56,15 +56,15 @@
     def cidrs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['FirewallIPSetCidrArgs']]]]):
         pulumi.set(self, "cidrs", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        Arbitrary string annotation.
+        IPSet comment.
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -80,15 +80,15 @@
     def container_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "container_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Network/IP specification in CIDR format.
+        IPSet name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -125,17 +125,17 @@
                  container_id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
                  vm_id: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering FirewallIPSet resources.
         :param pulumi.Input[Sequence[pulumi.Input['FirewallIPSetCidrArgs']]] cidrs: IP/CIDR block (multiple blocks supported).
-        :param pulumi.Input[str] comment: Arbitrary string annotation.
+        :param pulumi.Input[str] comment: IPSet comment.
         :param pulumi.Input[int] container_id: Container ID. Leave empty for cluster level aliases.
-        :param pulumi.Input[str] name: Network/IP specification in CIDR format.
+        :param pulumi.Input[str] name: IPSet name.
         :param pulumi.Input[str] node_name: Node name. Leave empty for cluster level aliases.
         :param pulumi.Input[int] vm_id: VM ID. Leave empty for cluster level aliases.
         """
         if cidrs is not None:
             pulumi.set(__self__, "cidrs", cidrs)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
@@ -160,15 +160,15 @@
     def cidrs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['FirewallIPSetCidrArgs']]]]):
         pulumi.set(self, "cidrs", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        Arbitrary string annotation.
+        IPSet comment.
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -184,15 +184,15 @@
     def container_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "container_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Network/IP specification in CIDR format.
+        IPSet name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -235,15 +235,14 @@
                  __props__=None):
         """
         An IPSet allows us to group multiple IP addresses, IP subnets and aliases. Aliases can be
         created on the cluster level, on VM / Container level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         ipset = proxmoxve.network.FirewallIPSet("ipset",
             node_name=proxmox_virtual_environment_vm["example"]["node_name"],
             vm_id=proxmox_virtual_environment_vm["example"]["vm_id"],
@@ -261,22 +260,21 @@
                 proxmoxve.network.FirewallIPSetCidrArgs(
                     name="192.168.2.1",
                     comment="Server 1",
                 ),
             ],
             opts=pulumi.ResourceOptions(depends_on=[proxmox_virtual_environment_vm["example"]]))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallIPSetCidrArgs']]]] cidrs: IP/CIDR block (multiple blocks supported).
-        :param pulumi.Input[str] comment: Arbitrary string annotation.
+        :param pulumi.Input[str] comment: IPSet comment.
         :param pulumi.Input[int] container_id: Container ID. Leave empty for cluster level aliases.
-        :param pulumi.Input[str] name: Network/IP specification in CIDR format.
+        :param pulumi.Input[str] name: IPSet name.
         :param pulumi.Input[str] node_name: Node name. Leave empty for cluster level aliases.
         :param pulumi.Input[int] vm_id: VM ID. Leave empty for cluster level aliases.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -284,15 +282,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         An IPSet allows us to group multiple IP addresses, IP subnets and aliases. Aliases can be
         created on the cluster level, on VM / Container level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         ipset = proxmoxve.network.FirewallIPSet("ipset",
             node_name=proxmox_virtual_environment_vm["example"]["node_name"],
             vm_id=proxmox_virtual_environment_vm["example"]["vm_id"],
@@ -310,15 +307,14 @@
                 proxmoxve.network.FirewallIPSetCidrArgs(
                     name="192.168.2.1",
                     comment="Server 1",
                 ),
             ],
             opts=pulumi.ResourceOptions(depends_on=[proxmox_virtual_environment_vm["example"]]))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param FirewallIPSetArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -372,17 +368,17 @@
         Get an existing FirewallIPSet resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallIPSetCidrArgs']]]] cidrs: IP/CIDR block (multiple blocks supported).
-        :param pulumi.Input[str] comment: Arbitrary string annotation.
+        :param pulumi.Input[str] comment: IPSet comment.
         :param pulumi.Input[int] container_id: Container ID. Leave empty for cluster level aliases.
-        :param pulumi.Input[str] name: Network/IP specification in CIDR format.
+        :param pulumi.Input[str] name: IPSet name.
         :param pulumi.Input[str] node_name: Node name. Leave empty for cluster level aliases.
         :param pulumi.Input[int] vm_id: VM ID. Leave empty for cluster level aliases.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _FirewallIPSetState.__new__(_FirewallIPSetState)
 
@@ -402,15 +398,15 @@
         """
         return pulumi.get(self, "cidrs")
 
     @property
     @pulumi.getter
     def comment(self) -> pulumi.Output[Optional[str]]:
         """
-        Arbitrary string annotation.
+        IPSet comment.
         """
         return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter(name="containerId")
     def container_id(self) -> pulumi.Output[Optional[int]]:
         """
@@ -418,15 +414,15 @@
         """
         return pulumi.get(self, "container_id")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Network/IP specification in CIDR format.
+        IPSet name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -502,15 +502,14 @@
                  vm_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Manages firewall options on VM / Container level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         example = proxmoxve.network.FirewallOptions("example",
             node_name=proxmox_virtual_environment_vm["example"]["node_name"],
             vm_id=proxmox_virtual_environment_vm["example"]["vm_id"],
@@ -522,15 +521,14 @@
             macfilter=False,
             ndp=True,
             input_policy="ACCEPT",
             output_policy="ACCEPT",
             radv=True,
             opts=pulumi.ResourceOptions(depends_on=[proxmox_virtual_environment_vm["example"]]))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] container_id: Container ID. Leave empty for cluster level aliases.
         :param pulumi.Input[bool] dhcp: Enable DHCP.
         :param pulumi.Input[bool] enabled: Enable or disable the firewall.
         :param pulumi.Input[str] input_policy: The default input
@@ -561,15 +559,14 @@
                  args: FirewallOptionsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages firewall options on VM / Container level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         example = proxmoxve.network.FirewallOptions("example",
             node_name=proxmox_virtual_environment_vm["example"]["node_name"],
             vm_id=proxmox_virtual_environment_vm["example"]["vm_id"],
@@ -581,15 +578,14 @@
             macfilter=False,
             ndp=True,
             input_policy="ACCEPT",
             output_policy="ACCEPT",
             radv=True,
             opts=pulumi.ResourceOptions(depends_on=[proxmox_virtual_environment_vm["example"]]))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param FirewallOptionsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,14 @@
         A security group is a collection of rules, defined at cluster level, which can
         be used in all VMs' rules. For example, you can define a group named “webserver”
         with rules to open the http and https ports. Rules can be created on the cluster
         level, on VM / Container level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         inbound = proxmoxve.network.FirewallRules("inbound",
             node_name=proxmox_virtual_environment_vm["example"]["node_name"],
             vm_id=proxmox_virtual_environment_vm["example"]["vm_id"],
@@ -220,15 +219,14 @@
                 ),
             ],
             opts=pulumi.ResourceOptions(depends_on=[
                     proxmox_virtual_environment_vm["example"],
                     proxmox_virtual_environment_cluster_firewall_security_group["example"],
                 ]))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] container_id: Container ID. Leave empty for cluster level
                rules.
         :param pulumi.Input[str] node_name: Node name. Leave empty for cluster level rules.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallRulesRuleArgs']]]] rules: Firewall rule block (multiple blocks supported).
@@ -246,15 +244,14 @@
         A security group is a collection of rules, defined at cluster level, which can
         be used in all VMs' rules. For example, you can define a group named “webserver”
         with rules to open the http and https ports. Rules can be created on the cluster
         level, on VM / Container level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         inbound = proxmoxve.network.FirewallRules("inbound",
             node_name=proxmox_virtual_environment_vm["example"]["node_name"],
             vm_id=proxmox_virtual_environment_vm["example"]["vm_id"],
@@ -284,15 +281,14 @@
                 ),
             ],
             opts=pulumi.ResourceOptions(depends_on=[
                     proxmox_virtual_environment_vm["example"],
                     proxmox_virtual_environment_cluster_firewall_security_group["example"],
                 ]))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param FirewallRulesArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                  container_id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
                  vm_id: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a FirewallSecurityGroup resource.
         :param pulumi.Input[Sequence[pulumi.Input['FirewallSecurityGroupRuleArgs']]] rules: Firewall rule block (multiple blocks supported).
-        :param pulumi.Input[str] comment: Rule comment.
+        :param pulumi.Input[str] comment: Security group comment.
         :param pulumi.Input[int] container_id: The ID of the container to manage the firewall for.
         :param pulumi.Input[str] name: Security group name.
         :param pulumi.Input[str] node_name: The name of the node.
         :param pulumi.Input[int] vm_id: The ID of the VM to manage the firewall for.
         """
         pulumi.set(__self__, "rules", rules)
         if comment is not None:
@@ -55,15 +55,15 @@
     def rules(self, value: pulumi.Input[Sequence[pulumi.Input['FirewallSecurityGroupRuleArgs']]]):
         pulumi.set(self, "rules", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        Rule comment.
+        Security group comment.
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -123,15 +123,15 @@
                  container_id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
                  rules: Optional[pulumi.Input[Sequence[pulumi.Input['FirewallSecurityGroupRuleArgs']]]] = None,
                  vm_id: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering FirewallSecurityGroup resources.
-        :param pulumi.Input[str] comment: Rule comment.
+        :param pulumi.Input[str] comment: Security group comment.
         :param pulumi.Input[int] container_id: The ID of the container to manage the firewall for.
         :param pulumi.Input[str] name: Security group name.
         :param pulumi.Input[str] node_name: The name of the node.
         :param pulumi.Input[Sequence[pulumi.Input['FirewallSecurityGroupRuleArgs']]] rules: Firewall rule block (multiple blocks supported).
         :param pulumi.Input[int] vm_id: The ID of the VM to manage the firewall for.
         """
         if comment is not None:
@@ -147,15 +147,15 @@
         if vm_id is not None:
             pulumi.set(__self__, "vm_id", vm_id)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        Rule comment.
+        Security group comment.
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -235,15 +235,14 @@
         """
         A security group is a collection of rules, defined at cluster level, which can
         be used in all VMs' rules. For example, you can define a group named “webserver”
         with rules to open the http and https ports.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         webserver = proxmoxve.network.FirewallSecurityGroup("webserver",
             comment="Managed by Terraform",
             rules=[
@@ -263,29 +262,28 @@
                     dport="443",
                     log="info",
                     proto="tcp",
                     type="in",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `name`, e.g.,
 
         bash
 
         ```sh
         $ pulumi import proxmoxve:Network/firewallSecurityGroup:FirewallSecurityGroup webserver webserver
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] comment: Rule comment.
+        :param pulumi.Input[str] comment: Security group comment.
         :param pulumi.Input[int] container_id: The ID of the container to manage the firewall for.
         :param pulumi.Input[str] name: Security group name.
         :param pulumi.Input[str] node_name: The name of the node.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallSecurityGroupRuleArgs']]]] rules: Firewall rule block (multiple blocks supported).
         :param pulumi.Input[int] vm_id: The ID of the VM to manage the firewall for.
         """
         ...
@@ -297,15 +295,14 @@
         """
         A security group is a collection of rules, defined at cluster level, which can
         be used in all VMs' rules. For example, you can define a group named “webserver”
         with rules to open the http and https ports.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         webserver = proxmoxve.network.FirewallSecurityGroup("webserver",
             comment="Managed by Terraform",
             rules=[
@@ -325,15 +322,14 @@
                     dport="443",
                     log="info",
                     proto="tcp",
                     type="in",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `name`, e.g.,
 
         bash
 
@@ -398,15 +394,15 @@
         """
         Get an existing FirewallSecurityGroup resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] comment: Rule comment.
+        :param pulumi.Input[str] comment: Security group comment.
         :param pulumi.Input[int] container_id: The ID of the container to manage the firewall for.
         :param pulumi.Input[str] name: Security group name.
         :param pulumi.Input[str] node_name: The name of the node.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallSecurityGroupRuleArgs']]]] rules: Firewall rule block (multiple blocks supported).
         :param pulumi.Input[int] vm_id: The ID of the VM to manage the firewall for.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -421,15 +417,15 @@
         __props__.__dict__["vm_id"] = vm_id
         return FirewallSecurityGroup(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def comment(self) -> pulumi.Output[Optional[str]]:
         """
-        Rule comment.
+        Security group comment.
         """
         return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter(name="containerId")
     def container_id(self) -> pulumi.Output[Optional[int]]:
         """
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_dns.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/get_dns.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,22 +80,20 @@
 def get_dns(node_name: Optional[str] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDNSResult:
     """
     Retrieves the DNS configuration for a specific node.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     first_node = proxmoxve.Network.get_dns(node_name="first-node")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: A node name.
     """
     __args__ = dict()
     __args__['nodeName'] = node_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -112,20 +110,18 @@
 def get_dns_output(node_name: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDNSResult]:
     """
     Retrieves the DNS configuration for a specific node.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     first_node = proxmoxve.Network.get_dns(node_name="first-node")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: A node name.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_hosts.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/get_hosts.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,22 +106,20 @@
 def get_hosts(node_name: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetHostsResult:
     """
     Retrieves all the host entries from a specific node.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     first_node_host_entries = proxmoxve.Network.get_hosts(node_name="first-node")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: A node name.
     """
     __args__ = dict()
     __args__['nodeName'] = node_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -140,20 +138,18 @@
 def get_hosts_output(node_name: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetHostsResult]:
     """
     Retrieves all the host entries from a specific node.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     first_node_host_entries = proxmoxve.Network.get_hosts(node_name="first-node")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: A node name.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_time.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/get_time.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,22 +92,20 @@
 def get_time(node_name: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTimeResult:
     """
     Retrieves the current time for a specific node.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     first_node_time = proxmoxve.Network.get_time(node_name="first-node")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: A node name.
     """
     __args__ = dict()
     __args__['nodeName'] = node_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -125,20 +123,18 @@
 def get_time_output(node_name: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTimeResult]:
     """
     Retrieves the current time for a specific node.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     first_node_time = proxmoxve.Network.get_time(node_name="first-node")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: A node name.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/get_version.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/get_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,27 +82,25 @@
 
 def get_version(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVersionResult:
     """
     Retrieves API version details.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example = proxmoxve.Network.get_version()
     pulumi.export("dataProxmoxVirtualEnvironmentVersion", {
         "release": example.release,
         "repository_id": example.repository_id,
         "version": example.version,
     })
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Network/getVersion:getVersion', __args__, opts=opts, typ=GetVersionResult).value
 
     return AwaitableGetVersionResult(
         id=pulumi.get(__ret__, 'id'),
@@ -114,22 +112,20 @@
 @_utilities.lift_output_func(get_version)
 def get_version_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVersionResult]:
     """
     Retrieves API version details.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     example = proxmoxve.Network.get_version()
     pulumi.export("dataProxmoxVirtualEnvironmentVersion", {
         "release": example.release,
         "repository_id": example.repository_id,
         "version": example.version,
     })
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/network_bridge.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/network_bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,27 +396,25 @@
                  vlan_aware: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Manages a Linux Bridge network interface in a Proxmox VE node.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         vmbr99 = proxmoxve.network.NetworkBridge("vmbr99",
             node_name="pve",
             address="99.99.99.99/16",
             comment="vmbr99 comment",
             ports=["ens18.99"],
             opts=pulumi.ResourceOptions(depends_on=[proxmox_virtual_environment_network_linux_vlan["vlan99"]]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         #!/usr/bin/env sh
 
         #Interfaces can be imported using the `node_name:iface` format, e.g.
 
@@ -445,27 +443,25 @@
                  args: NetworkBridgeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Linux Bridge network interface in a Proxmox VE node.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         vmbr99 = proxmoxve.network.NetworkBridge("vmbr99",
             node_name="pve",
             address="99.99.99.99/16",
             comment="vmbr99 comment",
             ports=["ens18.99"],
             opts=pulumi.ResourceOptions(depends_on=[proxmox_virtual_environment_network_linux_vlan["vlan99"]]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         #!/usr/bin/env sh
 
         #Interfaces can be imported using the `node_name:iface` format, e.g.
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/network_vlan.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/network_vlan.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,14 @@
                  vlan: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Manages a Linux VLAN network interface in a Proxmox VE node.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         # using VLAN tag
         vlan99 = proxmoxve.network.NetworkVlan("vlan99",
             comment="VLAN 99",
@@ -412,15 +411,14 @@
         # using custom network interface name
         vlan98 = proxmoxve.network.NetworkVlan("vlan98",
             comment="VLAN 98",
             interface="eno0",
             node_name="pve",
             vlan=98)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         #!/usr/bin/env sh
 
         #Interfaces can be imported using the `node_name:iface` format, e.g.
 
@@ -449,15 +447,14 @@
                  args: NetworkVlanArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Linux VLAN network interface in a Proxmox VE node.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         # using VLAN tag
         vlan99 = proxmoxve.network.NetworkVlan("vlan99",
             comment="VLAN 99",
@@ -465,15 +462,14 @@
         # using custom network interface name
         vlan98 = proxmoxve.network.NetworkVlan("vlan98",
             comment="VLAN 98",
             interface="eno0",
             node_name="pve",
             vlan=98)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         #!/usr/bin/env sh
 
         #Interfaces can be imported using the `node_name:iface` format, e.g.
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,22 +93,20 @@
 def get_group(group_id: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupResult:
     """
     Retrieves information about a specific user group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     operations_team = proxmoxve.Permission.get_group(group_id="operations-team")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str group_id: The group identifier.
     """
     __args__ = dict()
     __args__['groupId'] = group_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -126,20 +124,18 @@
 def get_group_output(group_id: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupResult]:
     """
     Retrieves information about a specific user group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     operations_team = proxmoxve.Permission.get_group(group_id="operations-team")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str group_id: The group identifier.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_groups.py`

 * *Files 13% similar despite different names*

```diff
@@ -70,22 +70,20 @@
 
 def get_groups(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupsResult:
     """
     Retrieves basic information about all available user groups.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     available_groups = proxmoxve.Permission.get_groups()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getGroups:getGroups', __args__, opts=opts, typ=GetGroupsResult).value
 
     return AwaitableGetGroupsResult(
         comments=pulumi.get(__ret__, 'comments'),
@@ -96,17 +94,15 @@
 @_utilities.lift_output_func(get_groups)
 def get_groups_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupsResult]:
     """
     Retrieves basic information about all available user groups.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     available_groups = proxmoxve.Permission.get_groups()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,22 +81,20 @@
 def get_pool(pool_id: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPoolResult:
     """
     Retrieves information about a specific resource pool.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     operations_pool = proxmoxve.Permission.get_pool(pool_id="operations")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str pool_id: The pool identifier.
     """
     __args__ = dict()
     __args__['poolId'] = pool_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -113,20 +111,18 @@
 def get_pool_output(pool_id: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPoolResult]:
     """
     Retrieves information about a specific resource pool.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     operations_pool = proxmoxve.Permission.get_pool(pool_id="operations")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str pool_id: The pool identifier.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_pools.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_pools(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPoolsResult:
     """
     Retrieves the identifiers for all the available resource pools.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     available_pools = proxmoxve.Permission.get_pools()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getPools:getPools', __args__, opts=opts, typ=GetPoolsResult).value
 
     return AwaitableGetPoolsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_pools)
 def get_pools_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPoolsResult]:
     """
     Retrieves the identifiers for all the available resource pools.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     available_pools = proxmoxve.Permission.get_pools()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_role.py`

 * *Files 13% similar despite different names*

```diff
@@ -68,22 +68,20 @@
 def get_role(role_id: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRoleResult:
     """
     Retrieves information about a specific role.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     operations_role = proxmoxve.Permission.get_role(role_id="operations")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str role_id: The role identifier.
     """
     __args__ = dict()
     __args__['roleId'] = role_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -99,20 +97,18 @@
 def get_role_output(role_id: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRoleResult]:
     """
     Retrieves information about a specific role.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     operations_role = proxmoxve.Permission.get_role(role_id="operations")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str role_id: The role identifier.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_roles.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,22 +82,20 @@
 
 def get_roles(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRolesResult:
     """
     Retrieves information about all the available roles.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     available_roles = proxmoxve.Permission.get_roles()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getRoles:getRoles', __args__, opts=opts, typ=GetRolesResult).value
 
     return AwaitableGetRolesResult(
         id=pulumi.get(__ret__, 'id'),
@@ -109,17 +107,15 @@
 @_utilities.lift_output_func(get_roles)
 def get_roles_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRolesResult]:
     """
     Retrieves information about all the available roles.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     available_roles = proxmoxve.Permission.get_roles()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,22 +165,20 @@
 def get_user(user_id: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserResult:
     """
     Retrieves information about a specific user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     operations_user = proxmoxve.Permission.get_user(user_id="operation@pam")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str user_id: The user identifier.
     """
     __args__ = dict()
     __args__['userId'] = user_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -204,20 +202,18 @@
 def get_user_output(user_id: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
     Retrieves information about a specific user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     operations_user = proxmoxve.Permission.get_user(user_id="operation@pam")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str user_id: The user identifier.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/get_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,22 +154,20 @@
 
 def get_users(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUsersResult:
     """
     Retrieves information about all the available users.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     available_users = proxmoxve.Permission.get_users()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getUsers:getUsers', __args__, opts=opts, typ=GetUsersResult).value
 
     return AwaitableGetUsersResult(
         comments=pulumi.get(__ret__, 'comments'),
@@ -187,17 +185,15 @@
 @_utilities.lift_output_func(get_users)
 def get_users_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUsersResult]:
     """
     Retrieves information about all the available users.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     available_users = proxmoxve.Permission.get_users()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,24 +150,22 @@
                  group_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a user group.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         operations_team = proxmoxve.permission.Group("operationsTeam",
             comment="Managed by Terraform",
             group_id="operations-team")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `group_id`, e.g.,
 
         bash
 
@@ -188,24 +186,22 @@
                  args: GroupArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a user group.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         operations_team = proxmoxve.permission.Group("operationsTeam",
             comment="Managed by Terraform",
             group_id="operations-team")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `group_id`, e.g.,
 
         bash
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,24 +117,22 @@
                  pool_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a resource pool.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         operations_pool = proxmoxve.permission.Pool("operationsPool",
             comment="Managed by Terraform",
             pool_id="operations-pool")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `pool_id`, e.g.,
 
         bash
 
@@ -154,24 +152,22 @@
                  args: PoolArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a resource pool.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         operations_pool = proxmoxve.permission.Pool("operationsPool",
             comment="Managed by Terraform",
             pool_id="operations-pool")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `pool_id`, e.g.,
 
         bash
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/role.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,24 +98,22 @@
                  role_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a role.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         operations_monitoring = proxmoxve.permission.Role("operationsMonitoring",
             privileges=["VM.Monitor"],
             role_id="operations-monitoring")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `role_id`, e.g.,
 
         bash
 
@@ -135,24 +133,22 @@
                  args: RoleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a role.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         operations_monitoring = proxmoxve.permission.Role("operationsMonitoring",
             privileges=["VM.Monitor"],
             role_id="operations-monitoring")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `role_id`, e.g.,
 
         bash
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/permission/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,15 +398,14 @@
                  user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a user.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         operations_monitoring = proxmoxve.permission.Role("operationsMonitoring",
             role_id="operations-monitoring",
             privileges=["VM.Monitor"])
@@ -416,15 +415,14 @@
                 propagate=True,
                 role_id=operations_monitoring.role_id,
             )],
             comment="Managed by Terraform",
             password="a-strong-password",
             user_id="operations-automation@pve")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `user_id`, e.g.,
 
         bash
 
@@ -453,15 +451,14 @@
                  args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a user.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         operations_monitoring = proxmoxve.permission.Role("operationsMonitoring",
             role_id="operations-monitoring",
             privileges=["VM.Monitor"])
@@ -471,15 +468,14 @@
                 propagate=True,
                 role_id=operations_monitoring.role_id,
             )],
             comment="Managed by Terraform",
             password="a-strong-password",
             user_id="operations-automation@pve")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `user_id`, e.g.,
 
         bash
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/storage/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,66 +353,60 @@
 
         ## Example Usage
 
         ### Backups (`dump`)
 
         > The resource with this content type uses SSH access to the node. You might need to configure the `ssh` option in the `provider` section.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         backup = proxmoxve.storage.File("backup",
             content_type="dump",
             datastore_id="local",
             node_name="pve",
             source_file=proxmoxve.storage.FileSourceFileArgs(
                 path="vzdump-lxc-100-2023_11_08-23_10_05.tar",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Images
 
         > Consider using `Download.File` resource instead. Using this resource for images is less efficient (requires to transfer uploaded image to node) though still supported.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         ubuntu_container_template = proxmoxve.storage.File("ubuntuContainerTemplate",
             content_type="iso",
             datastore_id="local",
             node_name="pve",
             source_file=proxmoxve.storage.FileSourceFileArgs(
                 path="https://cloud-images.ubuntu.com/jammy/20230929/jammy-server-cloudimg-amd64-disk-kvm.img",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Container Template (`vztmpl`)
 
         > Consider using `Download.File` resource instead. Using this resource for container images is less efficient (requires to transfer uploaded image to node) though still supported.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         ubuntu_container_template = proxmoxve.storage.File("ubuntuContainerTemplate",
             content_type="vztmpl",
             datastore_id="local",
             node_name="first-node",
             source_file=proxmoxve.storage.FileSourceFileArgs(
                 path="https://download.proxmox.com/images/system/ubuntu-20.04-standard_20.04-1_amd64.tar.gz",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Important Notes
 
         The Proxmox VE API endpoint for file uploads does not support chunked transfer
         encoding, which means that we must first store the source file as a temporary
         file locally before uploading it.
 
@@ -469,66 +463,60 @@
 
         ## Example Usage
 
         ### Backups (`dump`)
 
         > The resource with this content type uses SSH access to the node. You might need to configure the `ssh` option in the `provider` section.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         backup = proxmoxve.storage.File("backup",
             content_type="dump",
             datastore_id="local",
             node_name="pve",
             source_file=proxmoxve.storage.FileSourceFileArgs(
                 path="vzdump-lxc-100-2023_11_08-23_10_05.tar",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Images
 
         > Consider using `Download.File` resource instead. Using this resource for images is less efficient (requires to transfer uploaded image to node) though still supported.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         ubuntu_container_template = proxmoxve.storage.File("ubuntuContainerTemplate",
             content_type="iso",
             datastore_id="local",
             node_name="pve",
             source_file=proxmoxve.storage.FileSourceFileArgs(
                 path="https://cloud-images.ubuntu.com/jammy/20230929/jammy-server-cloudimg-amd64-disk-kvm.img",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Container Template (`vztmpl`)
 
         > Consider using `Download.File` resource instead. Using this resource for container images is less efficient (requires to transfer uploaded image to node) though still supported.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         ubuntu_container_template = proxmoxve.storage.File("ubuntuContainerTemplate",
             content_type="vztmpl",
             datastore_id="local",
             node_name="first-node",
             source_file=proxmoxve.storage.FileSourceFileArgs(
                 path="https://download.proxmox.com/images/system/ubuntu-20.04-standard_20.04-1_amd64.tar.gz",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Important Notes
 
         The Proxmox VE API endpoint for file uploads does not support chunked transfer
         encoding, which means that we must first store the source file as a temporary
         file locally before uploading it.
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,22 +164,20 @@
 def get_datastores(node_name: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatastoresResult:
     """
     Retrieves information about all the datastores available to a specific node.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     first_node = proxmoxve.Storage.get_datastores(node_name="first-node")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: A node name.
     """
     __args__ = dict()
     __args__['nodeName'] = node_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -203,20 +201,18 @@
 def get_datastores_output(node_name: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatastoresResult]:
     """
     Retrieves information about all the datastores available to a specific node.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     first_node = proxmoxve.Storage.get_datastores(node_name="first-node")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: A node name.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/storage/outputs.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,17 @@
                  file_name: Optional[str] = None,
                  insecure: Optional[bool] = None,
                  min_tls: Optional[str] = None):
         """
         :param str path: A path to a local file or a URL.
         :param bool changed: Whether the source file has changed since the last run
         :param str checksum: The SHA256 checksum of the source file.
-        :param str file_name: The file name.
+        :param str file_name: The file name to use instead of the source file
+               name. Useful when the source file does not have a valid file extension,
+               for example when the source file is a URL referencing a `.qcow2` image.
         :param bool insecure: Whether to skip the TLS verification step for
                HTTPS sources (defaults to `false`).
         :param str min_tls: The minimum required TLS version for HTTPS
                sources. "Supported values: `1.0|1.1|1.2|1.3` (defaults to `1.3`).
         """
         pulumi.set(__self__, "path", path)
         if changed is not None:
@@ -88,15 +90,17 @@
         """
         return pulumi.get(self, "checksum")
 
     @property
     @pulumi.getter(name="fileName")
     def file_name(self) -> Optional[str]:
         """
-        The file name.
+        The file name to use instead of the source file
+        name. Useful when the source file does not have a valid file extension,
+        for example when the source file is a URL referencing a `.qcow2` image.
         """
         return pulumi.get(self, "file_name")
 
     @property
     @pulumi.getter
     def insecure(self) -> Optional[bool]:
         """
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,24 +130,22 @@
                  time_zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages the time for a specific node.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         first_node_time = proxmoxve.Time("firstNodeTime",
             node_name="first-node",
             time_zone="UTC")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `node_name`, e.g.,
 
         bash
 
@@ -167,24 +165,22 @@
                  args: TimeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages the time for a specific node.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         first_node_time = proxmoxve.Time("firstNodeTime",
             node_name="first-node",
             time_zone="UTC")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Instances can be imported using the `node_name`, e.g.,
 
         bash
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,37 +41,37 @@
 class VirtualMachineAgentArgs:
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  timeout: Optional[pulumi.Input[str]] = None,
                  trim: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[bool] enabled: Whether to enable the VGA device (defaults
-               to `true`).
+        :param pulumi.Input[bool] enabled: Whether to enable the QEMU agent (defaults
+               to `false`).
         :param pulumi.Input[str] timeout: The maximum amount of time to wait for data from
                the QEMU agent to become available ( defaults to `15m`).
         :param pulumi.Input[bool] trim: Whether to enable the FSTRIM feature in the QEMU agent
                (defaults to `false`).
-        :param pulumi.Input[str] type: The VGA type (defaults to `std`).
+        :param pulumi.Input[str] type: The QEMU agent interface type (defaults to `virtio`).
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
         if trim is not None:
             pulumi.set(__self__, "trim", trim)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether to enable the VGA device (defaults
-        to `true`).
+        Whether to enable the QEMU agent (defaults
+        to `false`).
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
@@ -101,15 +101,15 @@
     def trim(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "trim", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The VGA type (defaults to `std`).
+        The QEMU agent interface type (defaults to `virtio`).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -117,33 +117,31 @@
 @pulumi.input_type
 class VirtualMachineAudioDeviceArgs:
     def __init__(__self__, *,
                  device: Optional[pulumi.Input[str]] = None,
                  driver: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] device: The device (defaults to `socket`).
-               - `/dev/*` - A host serial device.
+        :param pulumi.Input[str] device: The device (defaults to `intel-hda`).
         :param pulumi.Input[str] driver: The driver (defaults to `spice`).
-        :param pulumi.Input[bool] enabled: Whether to enable the VGA device (defaults
+        :param pulumi.Input[bool] enabled: Whether to enable the audio device (defaults
                to `true`).
         """
         if device is not None:
             pulumi.set(__self__, "device", device)
         if driver is not None:
             pulumi.set(__self__, "driver", driver)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def device(self) -> Optional[pulumi.Input[str]]:
         """
-        The device (defaults to `socket`).
-        - `/dev/*` - A host serial device.
+        The device (defaults to `intel-hda`).
         """
         return pulumi.get(self, "device")
 
     @device.setter
     def device(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "device", value)
 
@@ -159,15 +157,15 @@
     def driver(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "driver", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether to enable the VGA device (defaults
+        Whether to enable the audio device (defaults
         to `true`).
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
@@ -176,66 +174,62 @@
 @pulumi.input_type
 class VirtualMachineCdromArgs:
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  file_id: Optional[pulumi.Input[str]] = None,
                  interface: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[bool] enabled: Whether to enable the VGA device (defaults
-               to `true`).
-        :param pulumi.Input[str] file_id: The file ID for a disk image (experimental -
-               might cause high CPU utilization during import, especially with large
-               disk images).
-        :param pulumi.Input[str] interface: The hardware interface to connect the cloud-init
-               image to. Must be one of `ide0..3`, `sata0..5`, `scsi0..30`. Will be
-               detected if the setting is missing but a cloud-init image is present,
-               otherwise defaults to `ide2`.
+        :param pulumi.Input[bool] enabled: Whether to enable the CDROM drive (defaults
+               to `false`).
+        :param pulumi.Input[str] file_id: A file ID for an ISO file (defaults to `cdrom` as
+               in the physical drive).
+        :param pulumi.Input[str] interface: A hardware interface to connect CDROM drive to,
+               must be `ideN` (defaults to `ide3`). Note that `q35` machine type only
+               supports `ide0` and `ide2`.
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if file_id is not None:
             pulumi.set(__self__, "file_id", file_id)
         if interface is not None:
             pulumi.set(__self__, "interface", interface)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether to enable the VGA device (defaults
-        to `true`).
+        Whether to enable the CDROM drive (defaults
+        to `false`).
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter(name="fileId")
     def file_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The file ID for a disk image (experimental -
-        might cause high CPU utilization during import, especially with large
-        disk images).
+        A file ID for an ISO file (defaults to `cdrom` as
+        in the physical drive).
         """
         return pulumi.get(self, "file_id")
 
     @file_id.setter
     def file_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "file_id", value)
 
     @property
     @pulumi.getter
     def interface(self) -> Optional[pulumi.Input[str]]:
         """
-        The hardware interface to connect the cloud-init
-        image to. Must be one of `ide0..3`, `sata0..5`, `scsi0..30`. Will be
-        detected if the setting is missing but a cloud-init image is present,
-        otherwise defaults to `ide2`.
+        A hardware interface to connect CDROM drive to,
+        must be `ideN` (defaults to `ide3`). Note that `q35` machine type only
+        supports `ide0` and `ide2`.
         """
         return pulumi.get(self, "interface")
 
     @interface.setter
     def interface(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "interface", value)
 
@@ -245,20 +239,19 @@
     def __init__(__self__, *,
                  vm_id: pulumi.Input[int],
                  datastore_id: Optional[pulumi.Input[str]] = None,
                  full: Optional[pulumi.Input[bool]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
                  retries: Optional[pulumi.Input[int]] = None):
         """
-        :param pulumi.Input[int] vm_id: The VM identifier.
-        :param pulumi.Input[str] datastore_id: The identifier for the datastore to create the
-               cloud-init disk in (defaults to `local-lvm`).
+        :param pulumi.Input[int] vm_id: The identifier for the source VM.
+        :param pulumi.Input[str] datastore_id: The identifier for the target datastore.
         :param pulumi.Input[bool] full: Full or linked clone (defaults to `true`).
-        :param pulumi.Input[str] node_name: The name of the node to assign the virtual machine
-               to.
+        :param pulumi.Input[str] node_name: The name of the source node (leave blank, if
+               equal to the `node_name` argument).
         :param pulumi.Input[int] retries: Number of retries in Proxmox for clone vm.
                Sometimes Proxmox errors with timeout when creating multiple clones at
                once.
         """
         pulumi.set(__self__, "vm_id", vm_id)
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
@@ -269,28 +262,27 @@
         if retries is not None:
             pulumi.set(__self__, "retries", retries)
 
     @property
     @pulumi.getter(name="vmId")
     def vm_id(self) -> pulumi.Input[int]:
         """
-        The VM identifier.
+        The identifier for the source VM.
         """
         return pulumi.get(self, "vm_id")
 
     @vm_id.setter
     def vm_id(self, value: pulumi.Input[int]):
         pulumi.set(self, "vm_id", value)
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier for the datastore to create the
-        cloud-init disk in (defaults to `local-lvm`).
+        The identifier for the target datastore.
         """
         return pulumi.get(self, "datastore_id")
 
     @datastore_id.setter
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
@@ -306,16 +298,16 @@
     def full(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "full", value)
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the node to assign the virtual machine
-        to.
+        The name of the source node (leave blank, if
+        equal to the `node_name` argument).
         """
         return pulumi.get(self, "node_name")
 
     @node_name.setter
     def node_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "node_name", value)
 
@@ -376,17 +368,18 @@
                - `+ssbd`/`-ssbd` - Protection for "Speculative Store Bypass" for Intel
                models.
                - `+virt-ssbd`/`-virt-ssbd` - Basis for "Speculative Store Bypass"
                protection for AMD models.
         :param pulumi.Input[int] hotplugged: The number of hotplugged vCPUs (defaults
                to `0`).
         :param pulumi.Input[int] limit: Limit of CPU usage, `0...128`. (defaults to `0` -- no limit).
-        :param pulumi.Input[bool] numa: The NUMA configuration.
+        :param pulumi.Input[bool] numa: Enable/disable NUMA. (default to `false`)
         :param pulumi.Input[int] sockets: The number of CPU sockets (defaults to `1`).
-        :param pulumi.Input[str] type: The VGA type (defaults to `std`).
+        :param pulumi.Input[str] type: The emulated CPU type, it's recommended to
+               use `x86-64-v2-AES` (defaults to `qemu64`).
         :param pulumi.Input[int] units: The CPU units (defaults to `1024`).
         """
         if affinity is not None:
             pulumi.set(__self__, "affinity", affinity)
         if architecture is not None:
             pulumi.set(__self__, "architecture", architecture)
         if cores is not None:
@@ -504,15 +497,15 @@
     def limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "limit", value)
 
     @property
     @pulumi.getter
     def numa(self) -> Optional[pulumi.Input[bool]]:
         """
-        The NUMA configuration.
+        Enable/disable NUMA. (default to `false`)
         """
         return pulumi.get(self, "numa")
 
     @numa.setter
     def numa(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "numa", value)
 
@@ -528,15 +521,16 @@
     def sockets(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "sockets", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The VGA type (defaults to `std`).
+        The emulated CPU type, it's recommended to
+        use `x86-64-v2-AES` (defaults to `qemu64`).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -567,27 +561,27 @@
                  iothread: Optional[pulumi.Input[bool]] = None,
                  path_in_datastore: Optional[pulumi.Input[str]] = None,
                  replicate: Optional[pulumi.Input[bool]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  speed: Optional[pulumi.Input['VirtualMachineDiskSpeedArgs']] = None,
                  ssd: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] interface: The hardware interface to connect the cloud-init
-               image to. Must be one of `ide0..3`, `sata0..5`, `scsi0..30`. Will be
-               detected if the setting is missing but a cloud-init image is present,
-               otherwise defaults to `ide2`.
+        :param pulumi.Input[str] interface: The disk interface for Proxmox, currently `scsi`,
+               `sata` and `virtio` interfaces are supported. Append the disk index at
+               the end, for example, `virtio0` for the first virtio disk, `virtio1` for
+               the second, etc.
         :param pulumi.Input[str] aio: The disk AIO mode (defaults to `io_uring`).
         :param pulumi.Input[bool] backup: Whether the drive should be included when making backups (defaults to `true`).
         :param pulumi.Input[str] cache: The cache type (defaults to `none`).
-        :param pulumi.Input[str] datastore_id: The identifier for the datastore to create the
-               cloud-init disk in (defaults to `local-lvm`).
+        :param pulumi.Input[str] datastore_id: The identifier for the datastore to create
+               the disk in (defaults to `local-lvm`).
         :param pulumi.Input[str] discard: Whether to pass discard/trim requests to the
                underlying storage. Supported values are `on`/`ignore` (defaults
                to `ignore`).
-        :param pulumi.Input[str] file_format: The file format (defaults to `raw`).
+        :param pulumi.Input[str] file_format: The file format (defaults to `qcow2`).
         :param pulumi.Input[str] file_id: The file ID for a disk image (experimental -
                might cause high CPU utilization during import, especially with large
                disk images).
         :param pulumi.Input[bool] iothread: Whether to use iothreads for this disk (defaults
                to `false`).
         :param pulumi.Input[str] path_in_datastore: The in-datastore path to the disk image.
                ***Experimental.***Use to attach another VM's disks,
@@ -628,18 +622,18 @@
         if ssd is not None:
             pulumi.set(__self__, "ssd", ssd)
 
     @property
     @pulumi.getter
     def interface(self) -> pulumi.Input[str]:
         """
-        The hardware interface to connect the cloud-init
-        image to. Must be one of `ide0..3`, `sata0..5`, `scsi0..30`. Will be
-        detected if the setting is missing but a cloud-init image is present,
-        otherwise defaults to `ide2`.
+        The disk interface for Proxmox, currently `scsi`,
+        `sata` and `virtio` interfaces are supported. Append the disk index at
+        the end, for example, `virtio0` for the first virtio disk, `virtio1` for
+        the second, etc.
         """
         return pulumi.get(self, "interface")
 
     @interface.setter
     def interface(self, value: pulumi.Input[str]):
         pulumi.set(self, "interface", value)
 
@@ -679,16 +673,16 @@
     def cache(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cache", value)
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier for the datastore to create the
-        cloud-init disk in (defaults to `local-lvm`).
+        The identifier for the datastore to create
+        the disk in (defaults to `local-lvm`).
         """
         return pulumi.get(self, "datastore_id")
 
     @datastore_id.setter
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
@@ -706,15 +700,15 @@
     def discard(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "discard", value)
 
     @property
     @pulumi.getter(name="fileFormat")
     def file_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The file format (defaults to `raw`).
+        The file format (defaults to `qcow2`).
         """
         return pulumi.get(self, "file_format")
 
     @file_format.setter
     def file_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "file_format", value)
 
@@ -819,24 +813,22 @@
                  iops_write: Optional[pulumi.Input[int]] = None,
                  iops_write_burstable: Optional[pulumi.Input[int]] = None,
                  read: Optional[pulumi.Input[int]] = None,
                  read_burstable: Optional[pulumi.Input[int]] = None,
                  write: Optional[pulumi.Input[int]] = None,
                  write_burstable: Optional[pulumi.Input[int]] = None):
         """
-        :param pulumi.Input[int] iops_read: The maximum read I/O in operations per second.
-        :param pulumi.Input[int] iops_read_burstable: The maximum unthrottled read I/O pool in operations per second.
-        :param pulumi.Input[int] iops_write: The maximum write I/O in operations per second.
-        :param pulumi.Input[int] iops_write_burstable: The maximum unthrottled write I/O pool in operations per second.
-        :param pulumi.Input[int] read: The maximum read speed in megabytes per second.
-        :param pulumi.Input[int] read_burstable: The maximum burstable read speed in
-               megabytes per second.
-        :param pulumi.Input[int] write: The maximum write speed in megabytes per second.
-        :param pulumi.Input[int] write_burstable: The maximum burstable write speed in
-               megabytes per second.
+        :param pulumi.Input[int] iops_read: The maximum read I/O in operations per second
+        :param pulumi.Input[int] iops_read_burstable: The maximum unthrottled read I/O pool in operations per second
+        :param pulumi.Input[int] iops_write: The maximum write I/O in operations per second
+        :param pulumi.Input[int] iops_write_burstable: The maximum unthrottled write I/O pool in operations per second
+        :param pulumi.Input[int] read: The maximum read speed in megabytes per second
+        :param pulumi.Input[int] read_burstable: The maximum burstable read speed in megabytes per second
+        :param pulumi.Input[int] write: The maximum write speed in megabytes per second
+        :param pulumi.Input[int] write_burstable: The maximum burstable write speed in megabytes per second
         """
         if iops_read is not None:
             pulumi.set(__self__, "iops_read", iops_read)
         if iops_read_burstable is not None:
             pulumi.set(__self__, "iops_read_burstable", iops_read_burstable)
         if iops_write is not None:
             pulumi.set(__self__, "iops_write", iops_write)
@@ -851,101 +843,99 @@
         if write_burstable is not None:
             pulumi.set(__self__, "write_burstable", write_burstable)
 
     @property
     @pulumi.getter(name="iopsRead")
     def iops_read(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum read I/O in operations per second.
+        The maximum read I/O in operations per second
         """
         return pulumi.get(self, "iops_read")
 
     @iops_read.setter
     def iops_read(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "iops_read", value)
 
     @property
     @pulumi.getter(name="iopsReadBurstable")
     def iops_read_burstable(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum unthrottled read I/O pool in operations per second.
+        The maximum unthrottled read I/O pool in operations per second
         """
         return pulumi.get(self, "iops_read_burstable")
 
     @iops_read_burstable.setter
     def iops_read_burstable(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "iops_read_burstable", value)
 
     @property
     @pulumi.getter(name="iopsWrite")
     def iops_write(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum write I/O in operations per second.
+        The maximum write I/O in operations per second
         """
         return pulumi.get(self, "iops_write")
 
     @iops_write.setter
     def iops_write(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "iops_write", value)
 
     @property
     @pulumi.getter(name="iopsWriteBurstable")
     def iops_write_burstable(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum unthrottled write I/O pool in operations per second.
+        The maximum unthrottled write I/O pool in operations per second
         """
         return pulumi.get(self, "iops_write_burstable")
 
     @iops_write_burstable.setter
     def iops_write_burstable(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "iops_write_burstable", value)
 
     @property
     @pulumi.getter
     def read(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum read speed in megabytes per second.
+        The maximum read speed in megabytes per second
         """
         return pulumi.get(self, "read")
 
     @read.setter
     def read(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "read", value)
 
     @property
     @pulumi.getter(name="readBurstable")
     def read_burstable(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum burstable read speed in
-        megabytes per second.
+        The maximum burstable read speed in megabytes per second
         """
         return pulumi.get(self, "read_burstable")
 
     @read_burstable.setter
     def read_burstable(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "read_burstable", value)
 
     @property
     @pulumi.getter
     def write(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum write speed in megabytes per second.
+        The maximum write speed in megabytes per second
         """
         return pulumi.get(self, "write")
 
     @write.setter
     def write(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "write", value)
 
     @property
     @pulumi.getter(name="writeBurstable")
     def write_burstable(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum burstable write speed in
-        megabytes per second.
+        The maximum burstable write speed in megabytes per second
         """
         return pulumi.get(self, "write_burstable")
 
     @write_burstable.setter
     def write_burstable(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "write_burstable", value)
 
@@ -954,38 +944,41 @@
 class VirtualMachineEfiDiskArgs:
     def __init__(__self__, *,
                  datastore_id: Optional[pulumi.Input[str]] = None,
                  file_format: Optional[pulumi.Input[str]] = None,
                  pre_enrolled_keys: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] datastore_id: The identifier for the datastore to create the
-               cloud-init disk in (defaults to `local-lvm`).
+        :param pulumi.Input[str] datastore_id: The identifier for the datastore to create
+               the disk in (defaults to `local-lvm`).
         :param pulumi.Input[str] file_format: The file format (defaults to `raw`).
         :param pulumi.Input[bool] pre_enrolled_keys: Use am EFI vars template with
                distribution-specific and Microsoft Standard keys enrolled, if used with
                EFI type=`4m`. Ignored for VMs with cpu.architecture=`aarch64` (defaults
                to `false`).
-        :param pulumi.Input[str] type: The VGA type (defaults to `std`).
+        :param pulumi.Input[str] type: Size and type of the OVMF EFI disk. `4m` is newer and
+               recommended, and required for Secure Boot. For backwards compatibility
+               use `2m`. Ignored for VMs with cpu.architecture=`aarch64` (defaults
+               to `2m`).
         """
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if file_format is not None:
             pulumi.set(__self__, "file_format", file_format)
         if pre_enrolled_keys is not None:
             pulumi.set(__self__, "pre_enrolled_keys", pre_enrolled_keys)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier for the datastore to create the
-        cloud-init disk in (defaults to `local-lvm`).
+        The identifier for the datastore to create
+        the disk in (defaults to `local-lvm`).
         """
         return pulumi.get(self, "datastore_id")
 
     @datastore_id.setter
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
@@ -1016,15 +1009,18 @@
     def pre_enrolled_keys(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "pre_enrolled_keys", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The VGA type (defaults to `std`).
+        Size and type of the OVMF EFI disk. `4m` is newer and
+        recommended, and required for Secure Boot. For backwards compatibility
+        use `2m`. Ignored for VMs with cpu.architecture=`aarch64` (defaults
+        to `2m`).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -1037,21 +1033,21 @@
                  mapping: Optional[pulumi.Input[str]] = None,
                  mdev: Optional[pulumi.Input[str]] = None,
                  pcie: Optional[pulumi.Input[bool]] = None,
                  rom_file: Optional[pulumi.Input[str]] = None,
                  rombar: Optional[pulumi.Input[bool]] = None,
                  xvga: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] device: The device (defaults to `socket`).
-               - `/dev/*` - A host serial device.
+        :param pulumi.Input[str] device: The PCI device name for Proxmox, in form
+               of `hostpciX` where `X` is a sequential number from 0 to 3.
         :param pulumi.Input[str] id: The PCI device ID. This parameter is not compatible
                with `api_token` and requires the root `username` and `password`
                configured in the proxmox provider. Use either this or `mapping`.
         :param pulumi.Input[str] mapping: The resource mapping name of the device, for
-               example usbdevice. Use either this or `id`.
+               example gpu. Use either this or `id`.
         :param pulumi.Input[str] mdev: The mediated device ID to use.
         :param pulumi.Input[bool] pcie: Tells Proxmox to use a PCIe or PCI port. Some
                guests/device combination require PCIe rather than PCI. PCIe is only
                available for q35 machine types.
         :param pulumi.Input[str] rom_file: A path to a ROM file for the device to use. This
                is a relative path under `/usr/share/kvm/`.
         :param pulumi.Input[bool] rombar: Makes the firmware ROM visible for the VM (defaults
@@ -1075,16 +1071,16 @@
         if xvga is not None:
             pulumi.set(__self__, "xvga", xvga)
 
     @property
     @pulumi.getter
     def device(self) -> pulumi.Input[str]:
         """
-        The device (defaults to `socket`).
-        - `/dev/*` - A host serial device.
+        The PCI device name for Proxmox, in form
+        of `hostpciX` where `X` is a sequential number from 0 to 3.
         """
         return pulumi.get(self, "device")
 
     @device.setter
     def device(self, value: pulumi.Input[str]):
         pulumi.set(self, "device", value)
 
@@ -1103,15 +1099,15 @@
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
     def mapping(self) -> Optional[pulumi.Input[str]]:
         """
         The resource mapping name of the device, for
-        example usbdevice. Use either this or `id`.
+        example gpu. Use either this or `id`.
         """
         return pulumi.get(self, "mapping")
 
     @mapping.setter
     def mapping(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "mapping", value)
 
@@ -1206,15 +1202,15 @@
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineInitializationIpConfigArgs']]] ip_configs: The IP configuration (one block per network
                device).
         :param pulumi.Input[str] meta_data_file_id: The identifier for a file containing
                all meta data passed to the VM via cloud-init.
         :param pulumi.Input[str] network_data_file_id: The identifier for a file containing
                network configuration data passed to the VM via cloud-init (conflicts
                with `ip_config`).
-        :param pulumi.Input[str] type: The VGA type (defaults to `std`).
+        :param pulumi.Input[str] type: The cloud-init configuration format
         :param pulumi.Input[bool] upgrade: Whether to do an automatic package upgrade after the first boot (defaults to `true`).
         :param pulumi.Input['VirtualMachineInitializationUserAccountArgs'] user_account: The user account configuration (conflicts
                with `user_data_file_id`).
         :param pulumi.Input[str] user_data_file_id: The identifier for a file containing
                custom user data (conflicts with `user_account`).
         :param pulumi.Input[str] vendor_data_file_id: The identifier for a file containing
                all vendor data passed to the VM via cloud-init.
@@ -1322,15 +1318,15 @@
     def network_data_file_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_data_file_id", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The VGA type (defaults to `std`).
+        The cloud-init configuration format
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -1389,19 +1385,17 @@
 @pulumi.input_type
 class VirtualMachineInitializationDnsArgs:
     def __init__(__self__, *,
                  domain: Optional[pulumi.Input[str]] = None,
                  server: Optional[pulumi.Input[str]] = None,
                  servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        :param pulumi.Input[str] domain: The DNS search domain.
-        :param pulumi.Input[str] server: The DNS server. The `server` attribute is
-               deprecated and will be removed in a future release. Please use the
-               `servers` attribute instead.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The list of DNS servers.
+        :param pulumi.Input[str] domain: The DNS search domain
+        :param pulumi.Input[str] server: The DNS server
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The list of DNS servers
         """
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if server is not None:
             warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
             pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
         if server is not None:
@@ -1409,173 +1403,159 @@
         if servers is not None:
             pulumi.set(__self__, "servers", servers)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[pulumi.Input[str]]:
         """
-        The DNS search domain.
+        The DNS search domain
         """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter
     def server(self) -> Optional[pulumi.Input[str]]:
         """
-        The DNS server. The `server` attribute is
-        deprecated and will be removed in a future release. Please use the
-        `servers` attribute instead.
+        The DNS server
         """
         warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
         pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
 
         return pulumi.get(self, "server")
 
     @server.setter
     def server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server", value)
 
     @property
     @pulumi.getter
     def servers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The list of DNS servers.
+        The list of DNS servers
         """
         return pulumi.get(self, "servers")
 
     @servers.setter
     def servers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "servers", value)
 
 
 @pulumi.input_type
 class VirtualMachineInitializationIpConfigArgs:
     def __init__(__self__, *,
                  ipv4: Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv4Args']] = None,
                  ipv6: Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv6Args']] = None):
         """
-        :param pulumi.Input['VirtualMachineInitializationIpConfigIpv4Args'] ipv4: The IPv4 configuration.
-        :param pulumi.Input['VirtualMachineInitializationIpConfigIpv6Args'] ipv6: The IPv4 configuration.
+        :param pulumi.Input['VirtualMachineInitializationIpConfigIpv4Args'] ipv4: The IPv4 configuration
+        :param pulumi.Input['VirtualMachineInitializationIpConfigIpv6Args'] ipv6: The IPv6 configuration
         """
         if ipv4 is not None:
             pulumi.set(__self__, "ipv4", ipv4)
         if ipv6 is not None:
             pulumi.set(__self__, "ipv6", ipv6)
 
     @property
     @pulumi.getter
     def ipv4(self) -> Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv4Args']]:
         """
-        The IPv4 configuration.
+        The IPv4 configuration
         """
         return pulumi.get(self, "ipv4")
 
     @ipv4.setter
     def ipv4(self, value: Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv4Args']]):
         pulumi.set(self, "ipv4", value)
 
     @property
     @pulumi.getter
     def ipv6(self) -> Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv6Args']]:
         """
-        The IPv4 configuration.
+        The IPv6 configuration
         """
         return pulumi.get(self, "ipv6")
 
     @ipv6.setter
     def ipv6(self, value: Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv6Args']]):
         pulumi.set(self, "ipv6", value)
 
 
 @pulumi.input_type
 class VirtualMachineInitializationIpConfigIpv4Args:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  gateway: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] address: The IPv6 address in CIDR notation
-               (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
-               to `dhcp` for autodiscovery.
-        :param pulumi.Input[str] gateway: The IPv6 gateway (must be omitted
-               when `dhcp` is used as the address).
+        :param pulumi.Input[str] address: The IPv4 address
+        :param pulumi.Input[str] gateway: The IPv4 gateway
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 address in CIDR notation
-        (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
-        to `dhcp` for autodiscovery.
+        The IPv4 address
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 gateway (must be omitted
-        when `dhcp` is used as the address).
+        The IPv4 gateway
         """
         return pulumi.get(self, "gateway")
 
     @gateway.setter
     def gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway", value)
 
 
 @pulumi.input_type
 class VirtualMachineInitializationIpConfigIpv6Args:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  gateway: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] address: The IPv6 address in CIDR notation
-               (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
-               to `dhcp` for autodiscovery.
-        :param pulumi.Input[str] gateway: The IPv6 gateway (must be omitted
-               when `dhcp` is used as the address).
+        :param pulumi.Input[str] address: The IPv6 address
+        :param pulumi.Input[str] gateway: The IPv6 gateway
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 address in CIDR notation
-        (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
-        to `dhcp` for autodiscovery.
+        The IPv6 address
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 gateway (must be omitted
-        when `dhcp` is used as the address).
+        The IPv6 gateway
         """
         return pulumi.get(self, "gateway")
 
     @gateway.setter
     def gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway", value)
 
@@ -1583,54 +1563,54 @@
 @pulumi.input_type
 class VirtualMachineInitializationUserAccountArgs:
     def __init__(__self__, *,
                  keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: The SSH keys.
-        :param pulumi.Input[str] password: The SSH password.
-        :param pulumi.Input[str] username: The SSH username.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: The SSH keys
+        :param pulumi.Input[str] password: The SSH password
+        :param pulumi.Input[str] username: The SSH username
         """
         if keys is not None:
             pulumi.set(__self__, "keys", keys)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def keys(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The SSH keys.
+        The SSH keys
         """
         return pulumi.get(self, "keys")
 
     @keys.setter
     def keys(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "keys", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH password.
+        The SSH password
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH username.
+        The SSH username
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
@@ -1747,16 +1727,15 @@
                  queues: Optional[pulumi.Input[int]] = None,
                  rate_limit: Optional[pulumi.Input[float]] = None,
                  trunks: Optional[pulumi.Input[str]] = None,
                  vlan_id: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[str] bridge: The name of the network bridge (defaults to `vmbr0`).
         :param pulumi.Input[bool] disconnected: Whether to disconnect the network device from the network (defaults to `false`).
-        :param pulumi.Input[bool] enabled: Whether to enable the VGA device (defaults
-               to `true`).
+        :param pulumi.Input[bool] enabled: Whether to enable the network device (defaults to `true`).
         :param pulumi.Input[bool] firewall: Whether this interface's firewall rules should be used (defaults to `false`).
         :param pulumi.Input[str] mac_address: The MAC address.
         :param pulumi.Input[str] model: The network device model (defaults to `virtio`).
         :param pulumi.Input[int] mtu: Force MTU, for VirtIO only. Set to 1 to use the bridge MTU. Cannot be larger than the bridge MTU.
         :param pulumi.Input[int] queues: The number of queues for VirtIO (1..64).
         :param pulumi.Input[float] rate_limit: The rate limit in megabytes per second.
         :param pulumi.Input[str] trunks: String containing a `;` separated list of VLAN trunks
@@ -1811,16 +1790,15 @@
     def disconnected(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disconnected", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether to enable the VGA device (defaults
-        to `true`).
+        Whether to enable the network device (defaults to `true`).
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
@@ -1929,17 +1907,17 @@
                  cpus: pulumi.Input[str],
                  device: pulumi.Input[str],
                  memory: pulumi.Input[int],
                  hostnodes: Optional[pulumi.Input[str]] = None,
                  policy: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] cpus: The CPU cores to assign to the NUMA node (format is `0-7;16-31`).
-        :param pulumi.Input[str] device: The device (defaults to `socket`).
-               - `/dev/*` - A host serial device.
-        :param pulumi.Input[int] memory: The VGA memory in megabytes (defaults to `16`).
+        :param pulumi.Input[str] device: The NUMA device name for Proxmox, in form
+               of `numaX` where `X` is a sequential number from 0 to 7.
+        :param pulumi.Input[int] memory: The memory in megabytes to assign to the NUMA node.
         :param pulumi.Input[str] hostnodes: The NUMA host nodes.
         :param pulumi.Input[str] policy: The NUMA policy (defaults to `preferred`).
         """
         pulumi.set(__self__, "cpus", cpus)
         pulumi.set(__self__, "device", device)
         pulumi.set(__self__, "memory", memory)
         if hostnodes is not None:
@@ -1959,28 +1937,28 @@
     def cpus(self, value: pulumi.Input[str]):
         pulumi.set(self, "cpus", value)
 
     @property
     @pulumi.getter
     def device(self) -> pulumi.Input[str]:
         """
-        The device (defaults to `socket`).
-        - `/dev/*` - A host serial device.
+        The NUMA device name for Proxmox, in form
+        of `numaX` where `X` is a sequential number from 0 to 7.
         """
         return pulumi.get(self, "device")
 
     @device.setter
     def device(self, value: pulumi.Input[str]):
         pulumi.set(self, "device", value)
 
     @property
     @pulumi.getter
     def memory(self) -> pulumi.Input[int]:
         """
-        The VGA memory in megabytes (defaults to `16`).
+        The memory in megabytes to assign to the NUMA node.
         """
         return pulumi.get(self, "memory")
 
     @memory.setter
     def memory(self, value: pulumi.Input[int]):
         pulumi.set(self, "memory", value)
 
@@ -2010,24 +1988,24 @@
 
 
 @pulumi.input_type
 class VirtualMachineOperatingSystemArgs:
     def __init__(__self__, *,
                  type: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] type: The VGA type (defaults to `std`).
+        :param pulumi.Input[str] type: The type (defaults to `other`).
         """
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The VGA type (defaults to `std`).
+        The type (defaults to `other`).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -2239,41 +2217,43 @@
 
 @pulumi.input_type
 class VirtualMachineTpmStateArgs:
     def __init__(__self__, *,
                  datastore_id: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] datastore_id: The identifier for the datastore to create the
-               cloud-init disk in (defaults to `local-lvm`).
-        :param pulumi.Input[str] version: The version.
+        :param pulumi.Input[str] datastore_id: The identifier for the datastore to create
+               the disk in (defaults to `local-lvm`).
+        :param pulumi.Input[str] version: TPM state device version. Can be `v1.2` or `v2.0`.
+               (defaults to `v2.0`).
         """
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier for the datastore to create the
-        cloud-init disk in (defaults to `local-lvm`).
+        The identifier for the datastore to create
+        the disk in (defaults to `local-lvm`).
         """
         return pulumi.get(self, "datastore_id")
 
     @datastore_id.setter
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
-        The version.
+        TPM state device version. Can be `v1.2` or `v2.0`.
+        (defaults to `v2.0`).
         """
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,23 +90,21 @@
                         vm_id: Optional[int] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVirtualMachineResult:
     """
     Retrieves information about a specific VM.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     test_vm = proxmoxve.VM.get_virtual_machine(node_name="test",
         vm_id=100)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: The node name.
     :param int vm_id: The VM identifier.
     """
     __args__ = dict()
     __args__['nodeName'] = node_name
@@ -127,22 +125,20 @@
                                vm_id: Optional[pulumi.Input[int]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVirtualMachineResult]:
     """
     Retrieves information about a specific VM.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     test_vm = proxmoxve.VM.get_virtual_machine(node_name="test",
         vm_id=100)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: The node name.
     :param int vm_id: The VM identifier.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,22 +85,20 @@
                          tags: Optional[Sequence[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVirtualMachinesResult:
     """
     Retrieves information about all VMs in the Proxmox cluster.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     ubuntu_vms = proxmoxve.VM.get_virtual_machines(tags=["ubuntu"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: The node name.
     :param Sequence[str] tags: A list of tags to filter the VMs. The VM must have all
            the tags to be included in the result.
     """
     __args__ = dict()
@@ -121,22 +119,20 @@
                                 tags: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVirtualMachinesResult]:
     """
     Retrieves information about all VMs in the Proxmox cluster.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_proxmoxve as proxmoxve
 
     ubuntu_vms = proxmoxve.VM.get_virtual_machines(tags=["ubuntu"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str node_name: The node name.
     :param Sequence[str] tags: A list of tags to filter the VMs. The VM must have all
            the tags to be included in the result.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,37 +43,37 @@
 class VirtualMachineAgent(dict):
     def __init__(__self__, *,
                  enabled: Optional[bool] = None,
                  timeout: Optional[str] = None,
                  trim: Optional[bool] = None,
                  type: Optional[str] = None):
         """
-        :param bool enabled: Whether to enable the VGA device (defaults
-               to `true`).
+        :param bool enabled: Whether to enable the QEMU agent (defaults
+               to `false`).
         :param str timeout: The maximum amount of time to wait for data from
                the QEMU agent to become available ( defaults to `15m`).
         :param bool trim: Whether to enable the FSTRIM feature in the QEMU agent
                (defaults to `false`).
-        :param str type: The VGA type (defaults to `std`).
+        :param str type: The QEMU agent interface type (defaults to `virtio`).
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
         if trim is not None:
             pulumi.set(__self__, "trim", trim)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
-        Whether to enable the VGA device (defaults
-        to `true`).
+        Whether to enable the QEMU agent (defaults
+        to `false`).
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[str]:
         """
@@ -91,45 +91,43 @@
         """
         return pulumi.get(self, "trim")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        The VGA type (defaults to `std`).
+        The QEMU agent interface type (defaults to `virtio`).
         """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class VirtualMachineAudioDevice(dict):
     def __init__(__self__, *,
                  device: Optional[str] = None,
                  driver: Optional[str] = None,
                  enabled: Optional[bool] = None):
         """
-        :param str device: The device (defaults to `socket`).
-               - `/dev/*` - A host serial device.
+        :param str device: The device (defaults to `intel-hda`).
         :param str driver: The driver (defaults to `spice`).
-        :param bool enabled: Whether to enable the VGA device (defaults
+        :param bool enabled: Whether to enable the audio device (defaults
                to `true`).
         """
         if device is not None:
             pulumi.set(__self__, "device", device)
         if driver is not None:
             pulumi.set(__self__, "driver", driver)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def device(self) -> Optional[str]:
         """
-        The device (defaults to `socket`).
-        - `/dev/*` - A host serial device.
+        The device (defaults to `intel-hda`).
         """
         return pulumi.get(self, "device")
 
     @property
     @pulumi.getter
     def driver(self) -> Optional[str]:
         """
@@ -137,15 +135,15 @@
         """
         return pulumi.get(self, "driver")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
-        Whether to enable the VGA device (defaults
+        Whether to enable the audio device (defaults
         to `true`).
         """
         return pulumi.get(self, "enabled")
 
 
 @pulumi.output_type
 class VirtualMachineCdrom(dict):
@@ -167,58 +165,54 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  enabled: Optional[bool] = None,
                  file_id: Optional[str] = None,
                  interface: Optional[str] = None):
         """
-        :param bool enabled: Whether to enable the VGA device (defaults
-               to `true`).
-        :param str file_id: The file ID for a disk image (experimental -
-               might cause high CPU utilization during import, especially with large
-               disk images).
-        :param str interface: The hardware interface to connect the cloud-init
-               image to. Must be one of `ide0..3`, `sata0..5`, `scsi0..30`. Will be
-               detected if the setting is missing but a cloud-init image is present,
-               otherwise defaults to `ide2`.
+        :param bool enabled: Whether to enable the CDROM drive (defaults
+               to `false`).
+        :param str file_id: A file ID for an ISO file (defaults to `cdrom` as
+               in the physical drive).
+        :param str interface: A hardware interface to connect CDROM drive to,
+               must be `ideN` (defaults to `ide3`). Note that `q35` machine type only
+               supports `ide0` and `ide2`.
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if file_id is not None:
             pulumi.set(__self__, "file_id", file_id)
         if interface is not None:
             pulumi.set(__self__, "interface", interface)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
-        Whether to enable the VGA device (defaults
-        to `true`).
+        Whether to enable the CDROM drive (defaults
+        to `false`).
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="fileId")
     def file_id(self) -> Optional[str]:
         """
-        The file ID for a disk image (experimental -
-        might cause high CPU utilization during import, especially with large
-        disk images).
+        A file ID for an ISO file (defaults to `cdrom` as
+        in the physical drive).
         """
         return pulumi.get(self, "file_id")
 
     @property
     @pulumi.getter
     def interface(self) -> Optional[str]:
         """
-        The hardware interface to connect the cloud-init
-        image to. Must be one of `ide0..3`, `sata0..5`, `scsi0..30`. Will be
-        detected if the setting is missing but a cloud-init image is present,
-        otherwise defaults to `ide2`.
+        A hardware interface to connect CDROM drive to,
+        must be `ideN` (defaults to `ide3`). Note that `q35` machine type only
+        supports `ide0` and `ide2`.
         """
         return pulumi.get(self, "interface")
 
 
 @pulumi.output_type
 class VirtualMachineClone(dict):
     @staticmethod
@@ -245,20 +239,19 @@
     def __init__(__self__, *,
                  vm_id: int,
                  datastore_id: Optional[str] = None,
                  full: Optional[bool] = None,
                  node_name: Optional[str] = None,
                  retries: Optional[int] = None):
         """
-        :param int vm_id: The VM identifier.
-        :param str datastore_id: The identifier for the datastore to create the
-               cloud-init disk in (defaults to `local-lvm`).
+        :param int vm_id: The identifier for the source VM.
+        :param str datastore_id: The identifier for the target datastore.
         :param bool full: Full or linked clone (defaults to `true`).
-        :param str node_name: The name of the node to assign the virtual machine
-               to.
+        :param str node_name: The name of the source node (leave blank, if
+               equal to the `node_name` argument).
         :param int retries: Number of retries in Proxmox for clone vm.
                Sometimes Proxmox errors with timeout when creating multiple clones at
                once.
         """
         pulumi.set(__self__, "vm_id", vm_id)
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
@@ -269,24 +262,23 @@
         if retries is not None:
             pulumi.set(__self__, "retries", retries)
 
     @property
     @pulumi.getter(name="vmId")
     def vm_id(self) -> int:
         """
-        The VM identifier.
+        The identifier for the source VM.
         """
         return pulumi.get(self, "vm_id")
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[str]:
         """
-        The identifier for the datastore to create the
-        cloud-init disk in (defaults to `local-lvm`).
+        The identifier for the target datastore.
         """
         return pulumi.get(self, "datastore_id")
 
     @property
     @pulumi.getter
     def full(self) -> Optional[bool]:
         """
@@ -294,16 +286,16 @@
         """
         return pulumi.get(self, "full")
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[str]:
         """
-        The name of the node to assign the virtual machine
-        to.
+        The name of the source node (leave blank, if
+        equal to the `node_name` argument).
         """
         return pulumi.get(self, "node_name")
 
     @property
     @pulumi.getter
     def retries(self) -> Optional[int]:
         """
@@ -356,17 +348,18 @@
                - `+ssbd`/`-ssbd` - Protection for "Speculative Store Bypass" for Intel
                models.
                - `+virt-ssbd`/`-virt-ssbd` - Basis for "Speculative Store Bypass"
                protection for AMD models.
         :param int hotplugged: The number of hotplugged vCPUs (defaults
                to `0`).
         :param int limit: Limit of CPU usage, `0...128`. (defaults to `0` -- no limit).
-        :param bool numa: The NUMA configuration.
+        :param bool numa: Enable/disable NUMA. (default to `false`)
         :param int sockets: The number of CPU sockets (defaults to `1`).
-        :param str type: The VGA type (defaults to `std`).
+        :param str type: The emulated CPU type, it's recommended to
+               use `x86-64-v2-AES` (defaults to `qemu64`).
         :param int units: The CPU units (defaults to `1024`).
         """
         if affinity is not None:
             pulumi.set(__self__, "affinity", affinity)
         if architecture is not None:
             pulumi.set(__self__, "architecture", architecture)
         if cores is not None:
@@ -460,15 +453,15 @@
         """
         return pulumi.get(self, "limit")
 
     @property
     @pulumi.getter
     def numa(self) -> Optional[bool]:
         """
-        The NUMA configuration.
+        Enable/disable NUMA. (default to `false`)
         """
         return pulumi.get(self, "numa")
 
     @property
     @pulumi.getter
     def sockets(self) -> Optional[int]:
         """
@@ -476,15 +469,16 @@
         """
         return pulumi.get(self, "sockets")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        The VGA type (defaults to `std`).
+        The emulated CPU type, it's recommended to
+        use `x86-64-v2-AES` (defaults to `qemu64`).
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def units(self) -> Optional[int]:
         """
@@ -530,27 +524,27 @@
                  iothread: Optional[bool] = None,
                  path_in_datastore: Optional[str] = None,
                  replicate: Optional[bool] = None,
                  size: Optional[int] = None,
                  speed: Optional['outputs.VirtualMachineDiskSpeed'] = None,
                  ssd: Optional[bool] = None):
         """
-        :param str interface: The hardware interface to connect the cloud-init
-               image to. Must be one of `ide0..3`, `sata0..5`, `scsi0..30`. Will be
-               detected if the setting is missing but a cloud-init image is present,
-               otherwise defaults to `ide2`.
+        :param str interface: The disk interface for Proxmox, currently `scsi`,
+               `sata` and `virtio` interfaces are supported. Append the disk index at
+               the end, for example, `virtio0` for the first virtio disk, `virtio1` for
+               the second, etc.
         :param str aio: The disk AIO mode (defaults to `io_uring`).
         :param bool backup: Whether the drive should be included when making backups (defaults to `true`).
         :param str cache: The cache type (defaults to `none`).
-        :param str datastore_id: The identifier for the datastore to create the
-               cloud-init disk in (defaults to `local-lvm`).
+        :param str datastore_id: The identifier for the datastore to create
+               the disk in (defaults to `local-lvm`).
         :param str discard: Whether to pass discard/trim requests to the
                underlying storage. Supported values are `on`/`ignore` (defaults
                to `ignore`).
-        :param str file_format: The file format (defaults to `raw`).
+        :param str file_format: The file format (defaults to `qcow2`).
         :param str file_id: The file ID for a disk image (experimental -
                might cause high CPU utilization during import, especially with large
                disk images).
         :param bool iothread: Whether to use iothreads for this disk (defaults
                to `false`).
         :param str path_in_datastore: The in-datastore path to the disk image.
                ***Experimental.***Use to attach another VM's disks,
@@ -591,18 +585,18 @@
         if ssd is not None:
             pulumi.set(__self__, "ssd", ssd)
 
     @property
     @pulumi.getter
     def interface(self) -> str:
         """
-        The hardware interface to connect the cloud-init
-        image to. Must be one of `ide0..3`, `sata0..5`, `scsi0..30`. Will be
-        detected if the setting is missing but a cloud-init image is present,
-        otherwise defaults to `ide2`.
+        The disk interface for Proxmox, currently `scsi`,
+        `sata` and `virtio` interfaces are supported. Append the disk index at
+        the end, for example, `virtio0` for the first virtio disk, `virtio1` for
+        the second, etc.
         """
         return pulumi.get(self, "interface")
 
     @property
     @pulumi.getter
     def aio(self) -> Optional[str]:
         """
@@ -626,16 +620,16 @@
         """
         return pulumi.get(self, "cache")
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[str]:
         """
-        The identifier for the datastore to create the
-        cloud-init disk in (defaults to `local-lvm`).
+        The identifier for the datastore to create
+        the disk in (defaults to `local-lvm`).
         """
         return pulumi.get(self, "datastore_id")
 
     @property
     @pulumi.getter
     def discard(self) -> Optional[str]:
         """
@@ -645,15 +639,15 @@
         """
         return pulumi.get(self, "discard")
 
     @property
     @pulumi.getter(name="fileFormat")
     def file_format(self) -> Optional[str]:
         """
-        The file format (defaults to `raw`).
+        The file format (defaults to `qcow2`).
         """
         return pulumi.get(self, "file_format")
 
     @property
     @pulumi.getter(name="fileId")
     def file_id(self) -> Optional[str]:
         """
@@ -753,24 +747,22 @@
                  iops_write: Optional[int] = None,
                  iops_write_burstable: Optional[int] = None,
                  read: Optional[int] = None,
                  read_burstable: Optional[int] = None,
                  write: Optional[int] = None,
                  write_burstable: Optional[int] = None):
         """
-        :param int iops_read: The maximum read I/O in operations per second.
-        :param int iops_read_burstable: The maximum unthrottled read I/O pool in operations per second.
-        :param int iops_write: The maximum write I/O in operations per second.
-        :param int iops_write_burstable: The maximum unthrottled write I/O pool in operations per second.
-        :param int read: The maximum read speed in megabytes per second.
-        :param int read_burstable: The maximum burstable read speed in
-               megabytes per second.
-        :param int write: The maximum write speed in megabytes per second.
-        :param int write_burstable: The maximum burstable write speed in
-               megabytes per second.
+        :param int iops_read: The maximum read I/O in operations per second
+        :param int iops_read_burstable: The maximum unthrottled read I/O pool in operations per second
+        :param int iops_write: The maximum write I/O in operations per second
+        :param int iops_write_burstable: The maximum unthrottled write I/O pool in operations per second
+        :param int read: The maximum read speed in megabytes per second
+        :param int read_burstable: The maximum burstable read speed in megabytes per second
+        :param int write: The maximum write speed in megabytes per second
+        :param int write_burstable: The maximum burstable write speed in megabytes per second
         """
         if iops_read is not None:
             pulumi.set(__self__, "iops_read", iops_read)
         if iops_read_burstable is not None:
             pulumi.set(__self__, "iops_read_burstable", iops_read_burstable)
         if iops_write is not None:
             pulumi.set(__self__, "iops_write", iops_write)
@@ -785,73 +777,71 @@
         if write_burstable is not None:
             pulumi.set(__self__, "write_burstable", write_burstable)
 
     @property
     @pulumi.getter(name="iopsRead")
     def iops_read(self) -> Optional[int]:
         """
-        The maximum read I/O in operations per second.
+        The maximum read I/O in operations per second
         """
         return pulumi.get(self, "iops_read")
 
     @property
     @pulumi.getter(name="iopsReadBurstable")
     def iops_read_burstable(self) -> Optional[int]:
         """
-        The maximum unthrottled read I/O pool in operations per second.
+        The maximum unthrottled read I/O pool in operations per second
         """
         return pulumi.get(self, "iops_read_burstable")
 
     @property
     @pulumi.getter(name="iopsWrite")
     def iops_write(self) -> Optional[int]:
         """
-        The maximum write I/O in operations per second.
+        The maximum write I/O in operations per second
         """
         return pulumi.get(self, "iops_write")
 
     @property
     @pulumi.getter(name="iopsWriteBurstable")
     def iops_write_burstable(self) -> Optional[int]:
         """
-        The maximum unthrottled write I/O pool in operations per second.
+        The maximum unthrottled write I/O pool in operations per second
         """
         return pulumi.get(self, "iops_write_burstable")
 
     @property
     @pulumi.getter
     def read(self) -> Optional[int]:
         """
-        The maximum read speed in megabytes per second.
+        The maximum read speed in megabytes per second
         """
         return pulumi.get(self, "read")
 
     @property
     @pulumi.getter(name="readBurstable")
     def read_burstable(self) -> Optional[int]:
         """
-        The maximum burstable read speed in
-        megabytes per second.
+        The maximum burstable read speed in megabytes per second
         """
         return pulumi.get(self, "read_burstable")
 
     @property
     @pulumi.getter
     def write(self) -> Optional[int]:
         """
-        The maximum write speed in megabytes per second.
+        The maximum write speed in megabytes per second
         """
         return pulumi.get(self, "write")
 
     @property
     @pulumi.getter(name="writeBurstable")
     def write_burstable(self) -> Optional[int]:
         """
-        The maximum burstable write speed in
-        megabytes per second.
+        The maximum burstable write speed in megabytes per second
         """
         return pulumi.get(self, "write_burstable")
 
 
 @pulumi.output_type
 class VirtualMachineEfiDisk(dict):
     @staticmethod
@@ -877,38 +867,41 @@
 
     def __init__(__self__, *,
                  datastore_id: Optional[str] = None,
                  file_format: Optional[str] = None,
                  pre_enrolled_keys: Optional[bool] = None,
                  type: Optional[str] = None):
         """
-        :param str datastore_id: The identifier for the datastore to create the
-               cloud-init disk in (defaults to `local-lvm`).
+        :param str datastore_id: The identifier for the datastore to create
+               the disk in (defaults to `local-lvm`).
         :param str file_format: The file format (defaults to `raw`).
         :param bool pre_enrolled_keys: Use am EFI vars template with
                distribution-specific and Microsoft Standard keys enrolled, if used with
                EFI type=`4m`. Ignored for VMs with cpu.architecture=`aarch64` (defaults
                to `false`).
-        :param str type: The VGA type (defaults to `std`).
+        :param str type: Size and type of the OVMF EFI disk. `4m` is newer and
+               recommended, and required for Secure Boot. For backwards compatibility
+               use `2m`. Ignored for VMs with cpu.architecture=`aarch64` (defaults
+               to `2m`).
         """
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if file_format is not None:
             pulumi.set(__self__, "file_format", file_format)
         if pre_enrolled_keys is not None:
             pulumi.set(__self__, "pre_enrolled_keys", pre_enrolled_keys)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[str]:
         """
-        The identifier for the datastore to create the
-        cloud-init disk in (defaults to `local-lvm`).
+        The identifier for the datastore to create
+        the disk in (defaults to `local-lvm`).
         """
         return pulumi.get(self, "datastore_id")
 
     @property
     @pulumi.getter(name="fileFormat")
     def file_format(self) -> Optional[str]:
         """
@@ -927,15 +920,18 @@
         """
         return pulumi.get(self, "pre_enrolled_keys")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        The VGA type (defaults to `std`).
+        Size and type of the OVMF EFI disk. `4m` is newer and
+        recommended, and required for Secure Boot. For backwards compatibility
+        use `2m`. Ignored for VMs with cpu.architecture=`aarch64` (defaults
+        to `2m`).
         """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class VirtualMachineHostpci(dict):
     @staticmethod
@@ -961,21 +957,21 @@
                  mapping: Optional[str] = None,
                  mdev: Optional[str] = None,
                  pcie: Optional[bool] = None,
                  rom_file: Optional[str] = None,
                  rombar: Optional[bool] = None,
                  xvga: Optional[bool] = None):
         """
-        :param str device: The device (defaults to `socket`).
-               - `/dev/*` - A host serial device.
+        :param str device: The PCI device name for Proxmox, in form
+               of `hostpciX` where `X` is a sequential number from 0 to 3.
         :param str id: The PCI device ID. This parameter is not compatible
                with `api_token` and requires the root `username` and `password`
                configured in the proxmox provider. Use either this or `mapping`.
         :param str mapping: The resource mapping name of the device, for
-               example usbdevice. Use either this or `id`.
+               example gpu. Use either this or `id`.
         :param str mdev: The mediated device ID to use.
         :param bool pcie: Tells Proxmox to use a PCIe or PCI port. Some
                guests/device combination require PCIe rather than PCI. PCIe is only
                available for q35 machine types.
         :param str rom_file: A path to a ROM file for the device to use. This
                is a relative path under `/usr/share/kvm/`.
         :param bool rombar: Makes the firmware ROM visible for the VM (defaults
@@ -999,16 +995,16 @@
         if xvga is not None:
             pulumi.set(__self__, "xvga", xvga)
 
     @property
     @pulumi.getter
     def device(self) -> str:
         """
-        The device (defaults to `socket`).
-        - `/dev/*` - A host serial device.
+        The PCI device name for Proxmox, in form
+        of `hostpciX` where `X` is a sequential number from 0 to 3.
         """
         return pulumi.get(self, "device")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
@@ -1019,15 +1015,15 @@
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def mapping(self) -> Optional[str]:
         """
         The resource mapping name of the device, for
-        example usbdevice. Use either this or `id`.
+        example gpu. Use either this or `id`.
         """
         return pulumi.get(self, "mapping")
 
     @property
     @pulumi.getter
     def mdev(self) -> Optional[str]:
         """
@@ -1127,15 +1123,15 @@
         :param Sequence['VirtualMachineInitializationIpConfigArgs'] ip_configs: The IP configuration (one block per network
                device).
         :param str meta_data_file_id: The identifier for a file containing
                all meta data passed to the VM via cloud-init.
         :param str network_data_file_id: The identifier for a file containing
                network configuration data passed to the VM via cloud-init (conflicts
                with `ip_config`).
-        :param str type: The VGA type (defaults to `std`).
+        :param str type: The cloud-init configuration format
         :param bool upgrade: Whether to do an automatic package upgrade after the first boot (defaults to `true`).
         :param 'VirtualMachineInitializationUserAccountArgs' user_account: The user account configuration (conflicts
                with `user_data_file_id`).
         :param str user_data_file_id: The identifier for a file containing
                custom user data (conflicts with `user_account`).
         :param str vendor_data_file_id: The identifier for a file containing
                all vendor data passed to the VM via cloud-init.
@@ -1219,15 +1215,15 @@
         """
         return pulumi.get(self, "network_data_file_id")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        The VGA type (defaults to `std`).
+        The cloud-init configuration format
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def upgrade(self) -> Optional[bool]:
         """
@@ -1266,201 +1262,185 @@
 @pulumi.output_type
 class VirtualMachineInitializationDns(dict):
     def __init__(__self__, *,
                  domain: Optional[str] = None,
                  server: Optional[str] = None,
                  servers: Optional[Sequence[str]] = None):
         """
-        :param str domain: The DNS search domain.
-        :param str server: The DNS server. The `server` attribute is
-               deprecated and will be removed in a future release. Please use the
-               `servers` attribute instead.
-        :param Sequence[str] servers: The list of DNS servers.
+        :param str domain: The DNS search domain
+        :param str server: The DNS server
+        :param Sequence[str] servers: The list of DNS servers
         """
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if server is not None:
             pulumi.set(__self__, "server", server)
         if servers is not None:
             pulumi.set(__self__, "servers", servers)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[str]:
         """
-        The DNS search domain.
+        The DNS search domain
         """
         return pulumi.get(self, "domain")
 
     @property
     @pulumi.getter
     def server(self) -> Optional[str]:
         """
-        The DNS server. The `server` attribute is
-        deprecated and will be removed in a future release. Please use the
-        `servers` attribute instead.
+        The DNS server
         """
         warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
         pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
 
         return pulumi.get(self, "server")
 
     @property
     @pulumi.getter
     def servers(self) -> Optional[Sequence[str]]:
         """
-        The list of DNS servers.
+        The list of DNS servers
         """
         return pulumi.get(self, "servers")
 
 
 @pulumi.output_type
 class VirtualMachineInitializationIpConfig(dict):
     def __init__(__self__, *,
                  ipv4: Optional['outputs.VirtualMachineInitializationIpConfigIpv4'] = None,
                  ipv6: Optional['outputs.VirtualMachineInitializationIpConfigIpv6'] = None):
         """
-        :param 'VirtualMachineInitializationIpConfigIpv4Args' ipv4: The IPv4 configuration.
-        :param 'VirtualMachineInitializationIpConfigIpv6Args' ipv6: The IPv4 configuration.
+        :param 'VirtualMachineInitializationIpConfigIpv4Args' ipv4: The IPv4 configuration
+        :param 'VirtualMachineInitializationIpConfigIpv6Args' ipv6: The IPv6 configuration
         """
         if ipv4 is not None:
             pulumi.set(__self__, "ipv4", ipv4)
         if ipv6 is not None:
             pulumi.set(__self__, "ipv6", ipv6)
 
     @property
     @pulumi.getter
     def ipv4(self) -> Optional['outputs.VirtualMachineInitializationIpConfigIpv4']:
         """
-        The IPv4 configuration.
+        The IPv4 configuration
         """
         return pulumi.get(self, "ipv4")
 
     @property
     @pulumi.getter
     def ipv6(self) -> Optional['outputs.VirtualMachineInitializationIpConfigIpv6']:
         """
-        The IPv4 configuration.
+        The IPv6 configuration
         """
         return pulumi.get(self, "ipv6")
 
 
 @pulumi.output_type
 class VirtualMachineInitializationIpConfigIpv4(dict):
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  gateway: Optional[str] = None):
         """
-        :param str address: The IPv6 address in CIDR notation
-               (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
-               to `dhcp` for autodiscovery.
-        :param str gateway: The IPv6 gateway (must be omitted
-               when `dhcp` is used as the address).
+        :param str address: The IPv4 address
+        :param str gateway: The IPv4 gateway
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
         """
-        The IPv6 address in CIDR notation
-        (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
-        to `dhcp` for autodiscovery.
+        The IPv4 address
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[str]:
         """
-        The IPv6 gateway (must be omitted
-        when `dhcp` is used as the address).
+        The IPv4 gateway
         """
         return pulumi.get(self, "gateway")
 
 
 @pulumi.output_type
 class VirtualMachineInitializationIpConfigIpv6(dict):
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  gateway: Optional[str] = None):
         """
-        :param str address: The IPv6 address in CIDR notation
-               (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
-               to `dhcp` for autodiscovery.
-        :param str gateway: The IPv6 gateway (must be omitted
-               when `dhcp` is used as the address).
+        :param str address: The IPv6 address
+        :param str gateway: The IPv6 gateway
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
         """
-        The IPv6 address in CIDR notation
-        (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
-        to `dhcp` for autodiscovery.
+        The IPv6 address
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[str]:
         """
-        The IPv6 gateway (must be omitted
-        when `dhcp` is used as the address).
+        The IPv6 gateway
         """
         return pulumi.get(self, "gateway")
 
 
 @pulumi.output_type
 class VirtualMachineInitializationUserAccount(dict):
     def __init__(__self__, *,
                  keys: Optional[Sequence[str]] = None,
                  password: Optional[str] = None,
                  username: Optional[str] = None):
         """
-        :param Sequence[str] keys: The SSH keys.
-        :param str password: The SSH password.
-        :param str username: The SSH username.
+        :param Sequence[str] keys: The SSH keys
+        :param str password: The SSH password
+        :param str username: The SSH username
         """
         if keys is not None:
             pulumi.set(__self__, "keys", keys)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def keys(self) -> Optional[Sequence[str]]:
         """
-        The SSH keys.
+        The SSH keys
         """
         return pulumi.get(self, "keys")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
         """
-        The SSH password.
+        The SSH password
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
         """
-        The SSH username.
+        The SSH username
         """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class VirtualMachineMemory(dict):
     @staticmethod
@@ -1591,16 +1571,15 @@
                  queues: Optional[int] = None,
                  rate_limit: Optional[float] = None,
                  trunks: Optional[str] = None,
                  vlan_id: Optional[int] = None):
         """
         :param str bridge: The name of the network bridge (defaults to `vmbr0`).
         :param bool disconnected: Whether to disconnect the network device from the network (defaults to `false`).
-        :param bool enabled: Whether to enable the VGA device (defaults
-               to `true`).
+        :param bool enabled: Whether to enable the network device (defaults to `true`).
         :param bool firewall: Whether this interface's firewall rules should be used (defaults to `false`).
         :param str mac_address: The MAC address.
         :param str model: The network device model (defaults to `virtio`).
         :param int mtu: Force MTU, for VirtIO only. Set to 1 to use the bridge MTU. Cannot be larger than the bridge MTU.
         :param int queues: The number of queues for VirtIO (1..64).
         :param float rate_limit: The rate limit in megabytes per second.
         :param str trunks: String containing a `;` separated list of VLAN trunks
@@ -1647,16 +1626,15 @@
         """
         return pulumi.get(self, "disconnected")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
-        Whether to enable the VGA device (defaults
-        to `true`).
+        Whether to enable the network device (defaults to `true`).
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
     def firewall(self) -> Optional[bool]:
         """
@@ -1729,17 +1707,17 @@
                  cpus: str,
                  device: str,
                  memory: int,
                  hostnodes: Optional[str] = None,
                  policy: Optional[str] = None):
         """
         :param str cpus: The CPU cores to assign to the NUMA node (format is `0-7;16-31`).
-        :param str device: The device (defaults to `socket`).
-               - `/dev/*` - A host serial device.
-        :param int memory: The VGA memory in megabytes (defaults to `16`).
+        :param str device: The NUMA device name for Proxmox, in form
+               of `numaX` where `X` is a sequential number from 0 to 7.
+        :param int memory: The memory in megabytes to assign to the NUMA node.
         :param str hostnodes: The NUMA host nodes.
         :param str policy: The NUMA policy (defaults to `preferred`).
         """
         pulumi.set(__self__, "cpus", cpus)
         pulumi.set(__self__, "device", device)
         pulumi.set(__self__, "memory", memory)
         if hostnodes is not None:
@@ -1755,24 +1733,24 @@
         """
         return pulumi.get(self, "cpus")
 
     @property
     @pulumi.getter
     def device(self) -> str:
         """
-        The device (defaults to `socket`).
-        - `/dev/*` - A host serial device.
+        The NUMA device name for Proxmox, in form
+        of `numaX` where `X` is a sequential number from 0 to 7.
         """
         return pulumi.get(self, "device")
 
     @property
     @pulumi.getter
     def memory(self) -> int:
         """
-        The VGA memory in megabytes (defaults to `16`).
+        The memory in megabytes to assign to the NUMA node.
         """
         return pulumi.get(self, "memory")
 
     @property
     @pulumi.getter
     def hostnodes(self) -> Optional[str]:
         """
@@ -1790,24 +1768,24 @@
 
 
 @pulumi.output_type
 class VirtualMachineOperatingSystem(dict):
     def __init__(__self__, *,
                  type: Optional[str] = None):
         """
-        :param str type: The VGA type (defaults to `std`).
+        :param str type: The type (defaults to `other`).
         """
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        The VGA type (defaults to `std`).
+        The type (defaults to `other`).
         """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class VirtualMachineSerialDevice(dict):
     def __init__(__self__, *,
@@ -2007,37 +1985,39 @@
         VirtualMachineTpmState.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  datastore_id: Optional[str] = None,
                  version: Optional[str] = None):
         """
-        :param str datastore_id: The identifier for the datastore to create the
-               cloud-init disk in (defaults to `local-lvm`).
-        :param str version: The version.
+        :param str datastore_id: The identifier for the datastore to create
+               the disk in (defaults to `local-lvm`).
+        :param str version: TPM state device version. Can be `v1.2` or `v2.0`.
+               (defaults to `v2.0`).
         """
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[str]:
         """
-        The identifier for the datastore to create the
-        cloud-init disk in (defaults to `local-lvm`).
+        The identifier for the datastore to create
+        the disk in (defaults to `local-lvm`).
         """
         return pulumi.get(self, "datastore_id")
 
     @property
     @pulumi.getter
     def version(self) -> Optional[str]:
         """
-        The version.
+        TPM state device version. Can be `v1.2` or `v2.0`.
+        (defaults to `v2.0`).
         """
         return pulumi.get(self, "version")
 
 
 @pulumi.output_type
 class VirtualMachineUsb(dict):
     def __init__(__self__, *,
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineHostpciArgs']]] hostpcis: A host PCI device mapping (multiple blocks supported).
         :param pulumi.Input['VirtualMachineInitializationArgs'] initialization: The cloud-init configuration.
         :param pulumi.Input[str] keyboard_layout: The keyboard layout (defaults to `en-us`).
         :param pulumi.Input[str] kvm_arguments: Arbitrary arguments passed to kvm.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] mac_addresses: The MAC addresses published by the QEMU agent with fallback
                to the network device configuration, if the agent is disabled
         :param pulumi.Input[str] machine: The VM machine type (defaults to `pc`).
-        :param pulumi.Input['VirtualMachineMemoryArgs'] memory: The VGA memory in megabytes (defaults to `16`).
+        :param pulumi.Input['VirtualMachineMemoryArgs'] memory: The memory configuration.
         :param pulumi.Input[bool] migrate: Migrate the VM on node change instead of re-creating
                it (defaults to `false`).
         :param pulumi.Input[str] name: The virtual machine name.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNetworkDeviceArgs']]] network_devices: A network device (multiple blocks supported).
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNumaArgs']]] numas: The NUMA configuration.
         :param pulumi.Input[bool] on_boot: Specifies whether a VM will be started during system
                boot. (defaults to `true`)
@@ -474,15 +474,15 @@
     def machine(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "machine", value)
 
     @property
     @pulumi.getter
     def memory(self) -> Optional[pulumi.Input['VirtualMachineMemoryArgs']]:
         """
-        The VGA memory in megabytes (defaults to `16`).
+        The memory configuration.
         """
         return pulumi.get(self, "memory")
 
     @memory.setter
     def memory(self, value: Optional[pulumi.Input['VirtualMachineMemoryArgs']]):
         pulumi.set(self, "memory", value)
 
@@ -945,15 +945,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]] ipv6_addresses: The IPv6 addresses per network interface published by the
                QEMU agent (empty list when `agent.enabled` is `false`)
         :param pulumi.Input[str] keyboard_layout: The keyboard layout (defaults to `en-us`).
         :param pulumi.Input[str] kvm_arguments: Arbitrary arguments passed to kvm.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] mac_addresses: The MAC addresses published by the QEMU agent with fallback
                to the network device configuration, if the agent is disabled
         :param pulumi.Input[str] machine: The VM machine type (defaults to `pc`).
-        :param pulumi.Input['VirtualMachineMemoryArgs'] memory: The VGA memory in megabytes (defaults to `16`).
+        :param pulumi.Input['VirtualMachineMemoryArgs'] memory: The memory configuration.
         :param pulumi.Input[bool] migrate: Migrate the VM on node change instead of re-creating
                it (defaults to `false`).
         :param pulumi.Input[str] name: The virtual machine name.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNetworkDeviceArgs']]] network_devices: A network device (multiple blocks supported).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_interface_names: The network interface names published by the QEMU
                agent (empty list when `agent.enabled` is `false`)
         :param pulumi.Input[str] node_name: The name of the node to assign the virtual machine
@@ -1356,15 +1356,15 @@
     def machine(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "machine", value)
 
     @property
     @pulumi.getter
     def memory(self) -> Optional[pulumi.Input['VirtualMachineMemoryArgs']]:
         """
-        The VGA memory in megabytes (defaults to `16`).
+        The memory configuration.
         """
         return pulumi.get(self, "memory")
 
     @memory.setter
     def memory(self, value: Optional[pulumi.Input['VirtualMachineMemoryArgs']]):
         pulumi.set(self, "memory", value)
 
@@ -1864,15 +1864,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineHostpciArgs']]]] hostpcis: A host PCI device mapping (multiple blocks supported).
         :param pulumi.Input[pulumi.InputType['VirtualMachineInitializationArgs']] initialization: The cloud-init configuration.
         :param pulumi.Input[str] keyboard_layout: The keyboard layout (defaults to `en-us`).
         :param pulumi.Input[str] kvm_arguments: Arbitrary arguments passed to kvm.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] mac_addresses: The MAC addresses published by the QEMU agent with fallback
                to the network device configuration, if the agent is disabled
         :param pulumi.Input[str] machine: The VM machine type (defaults to `pc`).
-        :param pulumi.Input[pulumi.InputType['VirtualMachineMemoryArgs']] memory: The VGA memory in megabytes (defaults to `16`).
+        :param pulumi.Input[pulumi.InputType['VirtualMachineMemoryArgs']] memory: The memory configuration.
         :param pulumi.Input[bool] migrate: Migrate the VM on node change instead of re-creating
                it (defaults to `false`).
         :param pulumi.Input[str] name: The virtual machine name.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNetworkDeviceArgs']]]] network_devices: A network device (multiple blocks supported).
         :param pulumi.Input[str] node_name: The name of the node to assign the virtual machine
                to.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNumaArgs']]]] numas: The NUMA configuration.
@@ -2159,15 +2159,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]] ipv6_addresses: The IPv6 addresses per network interface published by the
                QEMU agent (empty list when `agent.enabled` is `false`)
         :param pulumi.Input[str] keyboard_layout: The keyboard layout (defaults to `en-us`).
         :param pulumi.Input[str] kvm_arguments: Arbitrary arguments passed to kvm.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] mac_addresses: The MAC addresses published by the QEMU agent with fallback
                to the network device configuration, if the agent is disabled
         :param pulumi.Input[str] machine: The VM machine type (defaults to `pc`).
-        :param pulumi.Input[pulumi.InputType['VirtualMachineMemoryArgs']] memory: The VGA memory in megabytes (defaults to `16`).
+        :param pulumi.Input[pulumi.InputType['VirtualMachineMemoryArgs']] memory: The memory configuration.
         :param pulumi.Input[bool] migrate: Migrate the VM on node change instead of re-creating
                it (defaults to `false`).
         :param pulumi.Input[str] name: The virtual machine name.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNetworkDeviceArgs']]]] network_devices: A network device (multiple blocks supported).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_interface_names: The network interface names published by the QEMU
                agent (empty list when `agent.enabled` is `false`)
         :param pulumi.Input[str] node_name: The name of the node to assign the virtual machine
@@ -2439,15 +2439,15 @@
         """
         return pulumi.get(self, "machine")
 
     @property
     @pulumi.getter
     def memory(self) -> pulumi.Output[Optional['outputs.VirtualMachineMemory']]:
         """
-        The VGA memory in megabytes (defaults to `16`).
+        The memory configuration.
         """
         return pulumi.get(self, "memory")
 
     @property
     @pulumi.getter
     def migrate(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve/vm2.py` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve/vm2.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-proxmoxve
-Version: 6.5.1
+Version: 6.6.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.5.1/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-6.6.0/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 setup.py
 pulumi_proxmoxve/__init__.py
 pulumi_proxmoxve/_inputs.py
 pulumi_proxmoxve/_utilities.py
+pulumi_proxmoxve/acl.py
 pulumi_proxmoxve/certifi.py
 pulumi_proxmoxve/dns.py
 pulumi_proxmoxve/get_node.py
 pulumi_proxmoxve/hosts.py
 pulumi_proxmoxve/outputs.py
 pulumi_proxmoxve/provider.py
 pulumi_proxmoxve/pulumi-plugin.json
@@ -81,13 +82,15 @@
 pulumi_proxmoxve/permission/role.py
 pulumi_proxmoxve/permission/user.py
 pulumi_proxmoxve/storage/__init__.py
 pulumi_proxmoxve/storage/_inputs.py
 pulumi_proxmoxve/storage/file.py
 pulumi_proxmoxve/storage/get_datastores.py
 pulumi_proxmoxve/storage/outputs.py
+pulumi_proxmoxve/user/__init__.py
+pulumi_proxmoxve/user/token.py
 pulumi_proxmoxve/vm/__init__.py
 pulumi_proxmoxve/vm/_inputs.py
 pulumi_proxmoxve/vm/get_virtual_machine.py
 pulumi_proxmoxve/vm/get_virtual_machines.py
 pulumi_proxmoxve/vm/outputs.py
 pulumi_proxmoxve/vm/virtual_machine.py
```

### Comparing `pulumi_proxmoxve-6.5.1/setup.py` & `pulumi_proxmoxve-6.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.5.1"
+VERSION = "6.6.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "proxmoxve Pulumi Package - Development Version"
```

