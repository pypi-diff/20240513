# Comparing `tmp/PwnModules-1.6.tar.gz` & `tmp/PwnModules-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PwnModules-1.6.tar", last modified: Sat Mar 30 06:15:26 2024, max compression
+gzip compressed data, was "PwnModules-1.7.tar", last modified: Mon May 13 02:15:44 2024, max compression
```

## Comparing `PwnModules-1.6.tar` & `PwnModules-1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 06:15:26.741199 PwnModules-1.6/
--rw-rw-rw-   0        0        0     1090 2023-04-24 12:32:23.000000 PwnModules-1.6/License.txt
--rw-rw-rw-   0        0        0      772 2024-03-30 06:15:26.740188 PwnModules-1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-30 06:15:26.738216 PwnModules-1.6/PwnModules.egg-info/
--rw-rw-rw-   0        0        0      772 2024-03-30 06:15:25.000000 PwnModules-1.6/PwnModules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-03-30 06:15:26.000000 PwnModules-1.6/PwnModules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 06:15:25.000000 PwnModules-1.6/PwnModules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-30 06:15:25.000000 PwnModules-1.6/PwnModules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-30 06:15:25.000000 PwnModules-1.6/PwnModules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9349 2024-03-30 06:15:13.000000 PwnModules-1.6/PwnModules.py
--rw-rw-rw-   0        0        0       84 2023-04-24 14:25:45.000000 PwnModules-1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-03-30 06:15:26.741199 PwnModules-1.6/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-04-24 14:25:56.000000 PwnModules-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:15:44.291590 PwnModules-1.7/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 12:32:23.000000 PwnModules-1.7/License.txt
+-rw-rw-rw-   0        0        0      772 2024-05-13 02:15:44.289597 PwnModules-1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 02:15:44.287605 PwnModules-1.7/PwnModules.egg-info/
+-rw-rw-rw-   0        0        0      772 2024-05-13 02:15:43.000000 PwnModules-1.7/PwnModules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-13 02:15:44.000000 PwnModules-1.7/PwnModules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:15:43.000000 PwnModules-1.7/PwnModules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 02:15:43.000000 PwnModules-1.7/PwnModules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 02:15:43.000000 PwnModules-1.7/PwnModules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9686 2024-05-13 02:14:02.000000 PwnModules-1.7/PwnModules.py
+-rw-rw-rw-   0        0        0       84 2023-04-24 14:25:45.000000 PwnModules-1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:15:44.291590 PwnModules-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-04-24 14:25:56.000000 PwnModules-1.7/setup.py
```

### Comparing `PwnModules-1.6/License.txt` & `PwnModules-1.7/License.txt`

 * *Files identical despite different names*

### Comparing `PwnModules-1.6/PKG-INFO` & `PwnModules-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PwnModules
-Version: 1.6
+Version: 1.7
 Summary: A open-source Pwntools Extern Functions.
 Home-page: https://github.com/XKaguya/PwnModules
 Author: RedLeaves
 Author-email: rx700@vip.qq.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PwnModules-1.6/PwnModules.egg-info/PKG-INFO` & `PwnModules-1.7/PwnModules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PwnModules
-Version: 1.6
+Version: 1.7
 Summary: A open-source Pwntools Extern Functions.
 Home-page: https://github.com/XKaguya/PwnModules
 Author: RedLeaves
 Author-email: rx700@vip.qq.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PwnModules-1.6/PwnModules.py` & `PwnModules-1.7/PwnModules.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,80 +3,91 @@
 @date: 2023-4-24
 Pwntools-Extern Functions
 开源包，任何人都可以使用并修改！
 """
 
 from LibcSearcher import *
 from pwn import *
+from typing import Optional, Tuple
 import re
 
-__version__ = '1.6'
+__version__ = '1.7'
+
 
 def leak_addr(i, io_i):
     """
     获取泄露的内存地址。
 
     Args:
         i (int): 用于指定地址获取方式的参数。可以是0、1或2。0是32位，1是64位正向接收，2是64位反向接收。
         io_i: IO流。
 
     Returns:
         int: 返回获取到的内存地址。
     """
-    if i == 0:
-        address_internal = u32(io_i.recv(4))
-        return address_internal
-    if i == 1:
-        address_internal = u64(io_i.recvuntil(b'\x7f')[:6].ljust(8, b'\x00'))
-        return address_internal
-    if i == 2:
-        address_internal = u64(io_i.recvuntil(b'\x7f')[-6:].ljust(8, b'\x00'))
-        return address_internal
+    address_methods = {
+        0: lambda: u32(io_i.recv(4)),
+        1: lambda: u64(io_i.recvuntil(b'\x7f')[:6].ljust(8, b'\x00')),
+        2: lambda: u64(io_i.recvuntil(b'\x7f')[-6:].ljust(8, b'\x00'))
+    }
+
+    return address_methods[i]()
 
-def libc_remastered(func, addr_i, onlineMode=False):
+def libc_search(func, addr_i, onlineMode=False):
     """
     在没有提供Libc版本时，这个参数可以快捷的使用LibcSearcher获取常用函数地址。
 
     Args:
         func: 泄露的函数
         addr_i: 泄露的函数的地址
         onlineMode: 在线搜索还是在本地Libc库搜索
 
     Returns:
         int: libc_base, system, /bin/sh 的地址。
     """
     libc_i = LibcSearcher(func, addr_i, online=onlineMode)
     libc_base_i = addr_i - libc_i.dump(func)
-    sys_i = libc_base_i + libc_i.dump('system')
-    sh_i = libc_base_i + libc_i.dump('str_bin_sh')
-    return libc_base_i, sys_i, sh_i
+    return libc_base_i, libc_base_i + libc_i.dump('system'), libc_base_i + libc_i.dump('str_bin_sh')
 
-def debug(io):
+def debug(io, breakpoint=None):
     """
     快捷GDB Attach函数。
 
     Args:
         io: IO流
+        breakpoint: 断点地址
     """
-    gdb.attach(io)
+    if breakpoint is not None:
+        gdb.attach(io, gdbscript='b *{}'.format(breakpoint))
+    else:
+        gdb.attach(io)
     pause()
 
 def recv_int_addr(io, num):
     """
     获取泄露的Int地址，一般是格式化字符串泄露Canary等。
 
     Args:
         io: IO流
         num: 需要接收几位数字
+        format: 数字的进制，默认为十进制
 
     Returns:
         int: Int地址的十进制格式。
     """
-    return int(io.recv(num), 16)
-
+    
+    try:
+        received = io.recv(num)
+        return int(received,)
+    except ValueError:
+        if received.startswith(b'0x'):
+            return int(received, 16)
+        else:
+            raise
+    
 def show_addr(msg, *args, **kwargs):
     """
     打印地址。
 
     Args:
         msg: 在打印地址前显示的文本
         *args: 需要打印的内存地址
@@ -91,54 +102,49 @@
         print(f"{msg}{colored_text}{colored_hex_text}")
 
     for key, value in kwargs.items():
         hex_text = hex(value)
         colored_hex_text = f'\x1b[01;38;5;90m{hex_text}\x1b[0m'
         print(f"{msg}{colored_text}{key}{colored_hex_text}")
 
-def init_env(arch, loglevel='info'):
+def init_env(arch=1, loglevel='debug'):
     """
-    初始化环境，默认为 amd64 架构，info 级日志打印。
+    初始化环境，默认为 amd64, debuf 级日志打印。
 
     Args:
-        arch: 系统架构
+        arch: 系统架构，1表示64位，0表示32位
         log_level: 日志打印等级
     """
-    if (arch == 'amd64'):
+    if (arch == 1):
         context(arch='amd64', os='linux', log_level=loglevel)
     else:
         context(arch='i386', os='linux', log_level=loglevel)
 
-def get_utils(binary=None, local=True, ip=None, port=None):
+def get_utils(binary: Optional[str] = None, local: bool = True, ip: Optional[str] = None, port: Optional[int] = None) -> Tuple[Optional[tube], Optional[ELF]]:
     """
     快速获取IO流和ELF。
 
     Args:
         binary: 二进制文件
         local: 布尔值，本地模式或在线
         ip: 在线IP
         port: 在线Port
 
     Returns:
         io: IO流
         elf: ELF引用
     """
-    if binary is not None:
-        elf = ELF(binary)
-    elf = None
+    elf = ELF(binary) if binary is not None else None
 
     if not local:
         io = remote(ip, port)
-        return io, elf
-
     else:
-        if binary is not None:
-            io = process(binary)
-            return io, elf
-        return None, elf
+        io = process(binary) if binary is not None else None
+
+    return io, elf
 
 def fmt_canary(binary=None):
     """
     快速获取Canary，仅支持格式化字符串漏洞。
     本函数通过本地穷举，节省人工计算的时间。
     
     Args:
```

### Comparing `PwnModules-1.6/setup.py` & `PwnModules-1.7/setup.py`

 * *Files identical despite different names*

