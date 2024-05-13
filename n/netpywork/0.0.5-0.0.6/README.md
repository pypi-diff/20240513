# Comparing `tmp/netpywork-0.0.5.tar.gz` & `tmp/netpywork-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpywork-0.0.5.tar", last modified: Thu Apr 18 17:15:04 2024, max compression
+gzip compressed data, was "netpywork-0.0.6.tar", last modified: Mon May 13 16:01:43 2024, max compression
```

## Comparing `netpywork-0.0.5.tar` & `netpywork-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 17:15:04.760164 netpywork-0.0.5/
--rw-rw-rw-   0        0        0     1063 2024-04-18 17:15:04.759167 netpywork-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      503 2024-04-10 14:09:29.000000 netpywork-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 17:15:04.744212 netpywork-0.0.5/netpywork/
--rw-rw-rw-   0        0        0      201 2024-04-14 13:18:43.000000 netpywork-0.0.5/netpywork/__init__.py
--rw-rw-rw-   0        0        0     5475 2024-04-18 17:12:32.000000 netpywork-0.0.5/netpywork/client.py
--rw-rw-rw-   0        0        0      153 2024-04-18 17:13:40.000000 netpywork-0.0.5/netpywork/constants.py
--rw-rw-rw-   0        0        0       93 2024-04-08 12:13:40.000000 netpywork-0.0.5/netpywork/protocol.py
--rw-rw-rw-   0        0        0     2451 2024-04-14 09:08:08.000000 netpywork-0.0.5/netpywork/sequence_manager.py
--rw-rw-rw-   0        0        0     7378 2024-04-18 17:13:12.000000 netpywork-0.0.5/netpywork/server.py
--rw-rw-rw-   0        0        0     3841 2024-04-14 09:09:30.000000 netpywork-0.0.5/netpywork/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-18 17:15:04.756175 netpywork-0.0.5/netpywork.egg-info/
--rw-rw-rw-   0        0        0     1063 2024-04-18 17:15:04.000000 netpywork-0.0.5/netpywork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-18 17:15:04.000000 netpywork-0.0.5/netpywork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 17:15:04.000000 netpywork-0.0.5/netpywork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 17:15:04.000000 netpywork-0.0.5/netpywork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 17:15:04.761161 netpywork-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-04-08 13:45:44.000000 netpywork-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:01:43.636564 netpywork-0.0.6/
+-rw-rw-rw-   0        0        0     1221 2024-05-13 16:01:43.634569 netpywork-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2024-04-18 20:13:57.000000 netpywork-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 16:01:43.615621 netpywork-0.0.6/netpywork/
+-rw-rw-rw-   0        0        0      257 2024-05-13 15:53:38.000000 netpywork-0.0.6/netpywork/__init__.py
+-rw-rw-rw-   0        0        0     5555 2024-04-19 12:31:19.000000 netpywork-0.0.6/netpywork/client.py
+-rw-rw-rw-   0        0        0      187 2024-05-13 15:59:37.000000 netpywork-0.0.6/netpywork/constants.py
+-rw-rw-rw-   0        0        0       93 2024-04-08 12:13:40.000000 netpywork-0.0.6/netpywork/protocol.py
+-rw-rw-rw-   0        0        0     2451 2024-04-14 09:08:08.000000 netpywork-0.0.6/netpywork/sequence_manager.py
+-rw-rw-rw-   0        0        0     7496 2024-04-19 12:28:13.000000 netpywork-0.0.6/netpywork/server.py
+-rw-rw-rw-   0        0        0     3860 2024-04-19 12:44:01.000000 netpywork-0.0.6/netpywork/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:01:43.630583 netpywork-0.0.6/netpywork.egg-info/
+-rw-rw-rw-   0        0        0     1221 2024-05-13 16:01:43.000000 netpywork-0.0.6/netpywork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-13 16:01:43.000000 netpywork-0.0.6/netpywork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 16:01:43.000000 netpywork-0.0.6/netpywork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-13 16:01:43.000000 netpywork-0.0.6/netpywork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 16:01:43.636564 netpywork-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-04-08 13:45:44.000000 netpywork-0.0.6/setup.py
```

### Comparing `netpywork-0.0.5/PKG-INFO` & `netpywork-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: netpywork
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library that simplifies UDP and TCP server and client
 Home-page: https://github.com/MurkyYT/netpywork
 Author: Murky
 Author-email: shooterkingof@gmail.com
 License: UNKNOWN
-Description: # netpywork
+Description: 
+        # *netpywork* 
+        
+        ![PYPI Version](https://img.shields.io/pypi/v/netpywork?style=for-the-badge&logo=python&logoColor=orange)
+        
+        
         **netpywork** is a library that makes using tcp and udp server and client easier
         
         # Features
         - Creating a server and client which uses `TCP` and `UDP`
         - Callbacks for `On Receive`, `On Connect` and `On Disconnect` for server
         - Callbacks for `On Receive` and `On Connect` for client
         - Sending messages from server to client both with tcp and udp by specifing the address to send to (see examples [here](https://github.com/MurkyYT/netpywork/tree/main))
```

### Comparing `netpywork-0.0.5/netpywork/client.py` & `netpywork-0.0.6/netpywork/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import socket
+import netpywork
 from threading import Thread
 from .sequence_manager import sequence_manager
 from .utils import *
 from .utils import _utils
 from .protocol import *
 from .constants import *
 
@@ -30,30 +31,30 @@
         self.__is_running = False
     def connect(self):
         self.__is_running = True
         self.__tcp_thread = Thread(target=self.__run_tcp)
         self.__tcp_socket.connect((self.ip,self.port))
         self.__tcp_thread.start()
         self.address = self.__tcp_socket.getsockname()
-        server_address = self.__tcp_socket.getpeername()
-        self.__seq_manager.add_addr(server_address)
+        self.server_address = self.__tcp_socket.getpeername()
+        self.__seq_manager.add_addr(self.server_address)
 
         self.__udp_thread = Thread(target=self.__run_udp)
         self.__udp_socket.bind(self.address)
         self.__udp_socket.settimeout(UDP_TIMEOUT)
+        self.__udp_socket.setsockopt(socket.SOL_SOCKET,socket.SO_RCVBUF,netpywork.udp_buffer_size)
         self.__udp_thread.start()
         if(self.on_connect):
-            self.on_connect(server_address,self)
+            self.on_connect(self.server_address,self)
     def close(self):
         self.__is_running = False
-        server_address = self.__tcp_socket.getpeername()
         self.__tcp_socket.shutdown(socket.SHUT_RDWR)
         self.__tcp_socket.close()
         self.__tcp_thread.join()
-        self.__seq_manager.delete_addr(server_address)
+        self.__seq_manager.delete_addr(self.server_address)
 
         self.__udp_thread.join()
         self.__udp_socket.shutdown(socket.SHUT_RDWR)
         self.__udp_socket.close()
 
         self.__seq_manager.stop()
     def has_tcp_messages(self) -> bool:
```

### Comparing `netpywork-0.0.5/netpywork/sequence_manager.py` & `netpywork-0.0.6/netpywork/sequence_manager.py`

 * *Files identical despite different names*

### Comparing `netpywork-0.0.5/netpywork/server.py` & `netpywork-0.0.6/netpywork/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import socket
 import select
+import netpywork
 from threading import Thread
 from .protocol import *
 from .sequence_manager import sequence_manager
 from .utils import *
 from .utils import _utils
 from .constants import *
 
@@ -38,14 +39,15 @@
         self.__is_running = True
         self.__tcp_thread = Thread(target=self.__run_tcp)
         self.__tcp_socket.listen()
         self.__tcp_thread.start()
 
         self.__udp_thread = Thread(target=self.__run_udp)
         self.__udp_socket.settimeout(UDP_TIMEOUT)
+        self.__udp_socket.setsockopt(socket.SOL_SOCKET,socket.SO_RCVBUF,netpywork.udp_buffer_size)
         self.__udp_thread.start()
     def close(self):
         self.__is_running = False
         self.__tcp_socket.close()
         self.__tcp_thread.join()
         for client in self.__clients:
             self.__seq_manager.delete_addr(client.getpeername())
```

### Comparing `netpywork-0.0.5/netpywork/utils.py` & `netpywork-0.0.6/netpywork/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import socket
+import netpywork
+
 class udp_msg:
     """
     UDP Message header:
 
     Length 4 bytes
 
     Port 2 bytes
@@ -78,15 +80,15 @@
         udp_message.seq_no = seqno
         udp_message.seq_id = seqid
         return udp_message
     def read_tcp_msg(socket: socket.socket):
         length = socket.recv(4)
         length = int.from_bytes(length,"big")
         buffer = socket.recv(length)
-        # TCP not always reads the entire message, read byte by byte untill length is correct
+        # TCP not always reads the entire message, read byte by byte until length is correct
         while len(buffer) < length:
             buffer += socket.recv(1)
         buffer = bytearray(buffer)
         close_con = int.from_bytes(_utils.read_message(buffer,1),"big") == 1
         result = _utils.read_message(buffer)
         address = socket.getpeername()
         tcp_message = tcp_msg()
```

### Comparing `netpywork-0.0.5/netpywork.egg-info/PKG-INFO` & `netpywork-0.0.6/netpywork.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: netpywork
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library that simplifies UDP and TCP server and client
 Home-page: https://github.com/MurkyYT/netpywork
 Author: Murky
 Author-email: shooterkingof@gmail.com
 License: UNKNOWN
-Description: # netpywork
+Description: 
+        # *netpywork* 
+        
+        ![PYPI Version](https://img.shields.io/pypi/v/netpywork?style=for-the-badge&logo=python&logoColor=orange)
+        
+        
         **netpywork** is a library that makes using tcp and udp server and client easier
         
         # Features
         - Creating a server and client which uses `TCP` and `UDP`
         - Callbacks for `On Receive`, `On Connect` and `On Disconnect` for server
         - Callbacks for `On Receive` and `On Connect` for client
         - Sending messages from server to client both with tcp and udp by specifing the address to send to (see examples [here](https://github.com/MurkyYT/netpywork/tree/main))
```

### Comparing `netpywork-0.0.5/setup.py` & `netpywork-0.0.6/setup.py`

 * *Files identical despite different names*

