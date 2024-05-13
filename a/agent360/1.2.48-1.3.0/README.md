# Comparing `tmp/agent360-1.2.48.tar.gz` & `tmp/agent360-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent360-1.2.48.tar", last modified: Fri Apr  5 15:39:44 2024, max compression
+gzip compressed data, was "agent360-1.3.0.tar", last modified: Mon May 13 10:45:22 2024, max compression
```

## Comparing `agent360-1.2.48.tar` & `agent360-1.3.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:44.140929 agent360-1.2.48/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-05 15:39:38.000000 agent360-1.2.48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 15:39:38.000000 agent360-1.2.48/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-05 15:39:44.140929 agent360-1.2.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-05 15:39:38.000000 agent360-1.2.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:44.132929 agent360-1.2.48/agent360/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27744 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/agent360.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:44.140929 agent360-1.2.48/agent360/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/apt-updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/asterisk.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/bird.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/bitninja.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/cloudlinux-dbgov.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/cloudlinux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/cpanel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2020 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/cpu_freq.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/dirsize.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/diskinodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/diskstatus-nvme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/diskstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4140 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/diskusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/dovecot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/exim.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/fail2ban.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/haproxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/httpd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5227 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/iostat.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/janus.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/kamailio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/litespeed.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      332 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/loadavg.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/loggedin.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/mailq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/mdstat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/megacli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/memcached.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      932 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/minecraft.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/nginx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/openvpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/phpfpm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3165 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/ping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6330 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/plesk-cgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/postfix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/powerdns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/proftpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/redis_stat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/sleeper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/swap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/tcpports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/unbound.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/vms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/wp-toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/yum-updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360-example.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:44.140929 agent360-1.2.48/agent360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:39:44.140929 agent360-1.2.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-05 15:39:38.000000 agent360-1.2.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:45:22.269319 agent360-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-13 10:45:18.000000 agent360-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 10:45:18.000000 agent360-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-13 10:45:22.269319 agent360-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-13 10:45:18.000000 agent360-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:45:22.257319 agent360-1.3.0/agent360/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28595 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/agent360.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:45:22.269319 agent360-1.3.0/agent360/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/apt-updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/asterisk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/bird.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/bitninja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/cloudlinux-dbgov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/cloudlinux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/cpanel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2020 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/cpu_freq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/dirsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/diskinodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/diskstatus-nvme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/diskstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4140 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/diskusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/dovecot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/exim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/fail2ban.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/haproxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/httpd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5227 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/iostat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/janus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/kamailio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/litespeed.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      332 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/loadavg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/loggedin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/mailq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/mdstat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/megacli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/memcached.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      932 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/minecraft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/openvpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/phpfpm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3165 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6330 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/plesk-cgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/postfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/powerdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/proftpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/redis_stat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/sleeper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/tcpports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/unbound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/vms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/wp-toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360/plugins/yum-updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-13 10:45:18.000000 agent360-1.3.0/agent360-example.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:45:22.269319 agent360-1.3.0/agent360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-13 10:45:22.000000 agent360-1.3.0/agent360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-13 10:45:22.000000 agent360-1.3.0/agent360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:45:22.000000 agent360-1.3.0/agent360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 10:45:22.000000 agent360-1.3.0/agent360.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 10:45:22.000000 agent360-1.3.0/agent360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 10:45:22.000000 agent360-1.3.0/agent360.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:45:22.269319 agent360-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-13 10:45:18.000000 agent360-1.3.0/setup.py
```

### Comparing `agent360-1.2.48/LICENSE` & `agent360-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/PKG-INFO` & `agent360-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent360
-Version: 1.2.48
+Version: 1.3.0
 Summary: 360 agent
 Home-page: https://github.com/plesk/agent360
 Author: 360
 Author-email: 360support@webpros.com
 Maintainer: 360
 Maintainer-email: 360support@webpros.com
 License: BSD-3-Clause
```

### Comparing `agent360-1.2.48/README.md` & `agent360-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/agent360.py` & `agent360-1.3.0/agent360/agent360.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,20 @@
     import io
 else:
     import ConfigParser
     import httplib
     import StringIO
     from Queue import Queue, Empty
 
+if sys.version_info >= (3,4):
+    import importlib.util
+else:
+    import imp
+
 import glob
-import imp
 import certifi
 import ssl
 
 try:
     import json
 except ImportError:
     import simplejson as json
@@ -44,15 +48,15 @@
     from urllib.request import urlopen, Request
     from urllib.error import HTTPError
 except ImportError:
     from urlparse import urlparse
     from urllib import urlencode
     from urllib2 import urlopen, Request, HTTPError
 
-__version__ = '1.2.48'
+__version__ = '1.3.0'
 __FILEABSDIRNAME__ = os.path.dirname(os.path.abspath(__file__))
 
 ini_files = (
     os.path.join('/etc', 'agent360.ini'),
     os.path.join('/etc', 'agent360-custom.ini'),
     os.path.join('/etc', 'agent360-token.ini'),
     os.path.join(os.path.dirname(__FILEABSDIRNAME__), 'agent360.ini'),
@@ -242,28 +246,36 @@
         plugins = agent._get_plugins(state='enabled')
         print('Check all enabled plugins: %s' % ', '.join(plugins))
 
     for plugin_name in plugins:
         print('%s:' % plugin_name)
 
         try:
-            fp, pathname, description = imp.find_module(plugin_name)
+            if sys.version_info >= (3,4):
+                spec = importlib.util.find_spec(plugin_name)
+            else:
+                fp, pathname, description = imp.find_module(plugin_name)
         except Exception as e:
             print('Find error:', e)
             continue
 
         try:
-            module = imp.load_module(plugin_name, fp, pathname, description)
+            if sys.version_info >= (3,4):
+                module = importlib.util.module_from_spec(spec)
+                spec.loader.exec_module(module)
+            else:
+                module = imp.load_module(plugin_name, fp, pathname, description)
         except Exception as e:
             print('Load error:', e)
             continue
         finally:
-            # Since we may exit via an exception, close fp explicitly.
-            if fp:
-                fp.close()
+            if sys.version_info < (3,4):
+                # Since we may exit via an exception, close fp explicitly.
+                if fp:
+                    fp.close()
 
         try:
             payload = module.Plugin().run(agent.config)
             print(json.dumps(payload, indent=4, sort_keys=True))
         except Exception as e:
             print('Execution error:', e)
 
@@ -395,24 +407,34 @@
             if name == 'plugins':
                 continue
             self._config_section_create(name)
             if self.config.getboolean(name, 'enabled'):
                 if self.config.getboolean(name, 'subprocess'):
                     self.schedule[filename] = 0
                 else:
-                    fp, pathname, description = imp.find_module(name)
+                    if sys.version_info >= (3,4):
+                        spec = importlib.util.find_spec(name)
+                    else:
+                        fp, pathname, description = imp.find_module(name)
+
                     try:
-                        module = imp.load_module(name, fp, pathname, description)
+                        if sys.version_info >= (3,4):
+                            module = importlib.util.module_from_spec(spec)
+                            spec.loader.exec_module(module)
+                        else:
+                            module = imp.load_module(name, fp, pathname, description)
                     except Exception:
                         module = None
                         logging.error('import_plugin_exception:%s', str(sys.exc_info()[0]))
                     finally:
-                        # Since we may exit via an exception, close fp explicitly.
-                        if fp:
-                            fp.close()
+                        if sys.version_info < (3,4):
+                            # Since we may exit via an exception, close fp explicitly.
+                            if fp:
+                                fp.close()
+
                     if module:
                         self.schedule[module] = 0
                     else:
                         logging.error('import_plugin:%s', name)
 
     def _subprocess_execution(self, task):
         '''
```

### Comparing `agent360-1.2.48/agent360/plugins/apt-updates.py` & `agent360-1.3.0/agent360/plugins/apt-updates.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/asterisk.py` & `agent360-1.3.0/agent360/plugins/asterisk.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/bind.py` & `agent360-1.3.0/agent360/plugins/bind.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/bird.py` & `agent360-1.3.0/agent360/plugins/bird.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/bitninja.py` & `agent360-1.3.0/agent360/plugins/bitninja.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/cloudlinux-dbgov.py` & `agent360-1.3.0/agent360/plugins/cloudlinux-dbgov.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/cloudlinux.py` & `agent360-1.3.0/agent360/plugins/cloudlinux.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/cpanel.py` & `agent360-1.3.0/agent360/plugins/cpanel.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/cpu.py` & `agent360-1.3.0/agent360/plugins/cpu.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/cpu_freq.py` & `agent360-1.3.0/agent360/plugins/cpu_freq.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/dirsize.py` & `agent360-1.3.0/agent360/plugins/dirsize.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/diskinodes.py` & `agent360-1.3.0/agent360/plugins/diskinodes.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/diskstatus-nvme.py` & `agent360-1.3.0/agent360/plugins/diskstatus-nvme.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/diskstatus.py` & `agent360-1.3.0/agent360/plugins/diskstatus.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/diskusage.py` & `agent360-1.3.0/agent360/plugins/diskusage.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/docker.py` & `agent360-1.3.0/agent360/plugins/docker.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/dovecot.py` & `agent360-1.3.0/agent360/plugins/dovecot.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/elasticsearch.py` & `agent360-1.3.0/agent360/plugins/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/fail2ban.py` & `agent360-1.3.0/agent360/plugins/fail2ban.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/gpu.py` & `agent360-1.3.0/agent360/plugins/gpu.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/haproxy.py` & `agent360-1.3.0/agent360/plugins/haproxy.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/httpd.py` & `agent360-1.3.0/agent360/plugins/httpd.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/iostat.py` & `agent360-1.3.0/agent360/plugins/iostat.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/janus.py` & `agent360-1.3.0/agent360/plugins/janus.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/kamailio.py` & `agent360-1.3.0/agent360/plugins/kamailio.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/litespeed.py` & `agent360-1.3.0/agent360/plugins/litespeed.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/mailq.py` & `agent360-1.3.0/agent360/plugins/mailq.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/mdstat.py` & `agent360-1.3.0/agent360/plugins/mdstat.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/megacli.py` & `agent360-1.3.0/agent360/plugins/megacli.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/memcached.py` & `agent360-1.3.0/agent360/plugins/memcached.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/memory.py` & `agent360-1.3.0/agent360/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/minecraft.py` & `agent360-1.3.0/agent360/plugins/minecraft.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/mongodb.py` & `agent360-1.3.0/agent360/plugins/mongodb.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/mysql.py` & `agent360-1.3.0/agent360/plugins/mysql.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/network.py` & `agent360-1.3.0/agent360/plugins/network.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/nginx.py` & `agent360-1.3.0/agent360/plugins/nginx.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/openvpn.py` & `agent360-1.3.0/agent360/plugins/openvpn.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/phpfpm.py` & `agent360-1.3.0/agent360/plugins/phpfpm.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/ping.py` & `agent360-1.3.0/agent360/plugins/ping.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/plesk-cgroups.py` & `agent360-1.3.0/agent360/plugins/plesk-cgroups.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/plugins.py` & `agent360-1.3.0/agent360/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/postfix.py` & `agent360-1.3.0/agent360/plugins/postfix.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/powerdns.py` & `agent360-1.3.0/agent360/plugins/powerdns.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/process.py` & `agent360-1.3.0/agent360/plugins/process.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/proftpd.py` & `agent360-1.3.0/agent360/plugins/proftpd.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/rabbitmq.py` & `agent360-1.3.0/agent360/plugins/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/redis_stat.py` & `agent360-1.3.0/agent360/plugins/redis_stat.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/system.py` & `agent360-1.3.0/agent360/plugins/system.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/tcpports.py` & `agent360-1.3.0/agent360/plugins/tcpports.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/temp.py` & `agent360-1.3.0/agent360/plugins/temp.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/unbound.py` & `agent360-1.3.0/agent360/plugins/unbound.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/vms.py` & `agent360-1.3.0/agent360/plugins/vms.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/wp-toolkit.py` & `agent360-1.3.0/agent360/plugins/wp-toolkit.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360/plugins/yum-updates.py` & `agent360-1.3.0/agent360/plugins/yum-updates.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360-example.ini` & `agent360-1.3.0/agent360-example.ini`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/agent360.egg-info/PKG-INFO` & `agent360-1.3.0/agent360.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent360
-Version: 1.2.48
+Version: 1.3.0
 Summary: 360 agent
 Home-page: https://github.com/plesk/agent360
 Author: 360
 Author-email: 360support@webpros.com
 Maintainer: 360
 Maintainer-email: 360support@webpros.com
 License: BSD-3-Clause
```

### Comparing `agent360-1.2.48/agent360.egg-info/SOURCES.txt` & `agent360-1.3.0/agent360.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agent360-1.2.48/setup.py` & `agent360-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     install_requires = ['psutil==5.6.7', 'netifaces', 'configparser==3.5.0', 'future', 'certifi']
 else:
     install_requires = ['psutil', 'netifaces', 'configparser', 'future', 'certifi']
 
 
 setuptools.setup(
     name='agent360',
-    version='1.2.48',
+    version='1.3.0',
     description='360 agent',
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/plesk/agent360',
     author='360',
     author_email='360support@webpros.com',
     maintainer='360',
```

