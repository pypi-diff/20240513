# Comparing `tmp/rabbit_library-0.0.3.tar.gz` & `tmp/rabbit_library-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbit_library-0.0.3.tar", max compression
+gzip compressed data, was "rabbit_library-1.0.4.tar", max compression
```

## Comparing `rabbit_library-0.0.3.tar` & `rabbit_library-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1112 2023-10-26 21:52:21.915249 rabbit_library-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       26 2023-07-03 17:14:02.867213 rabbit_library-0.0.3/rabbit_library/__init__.py
--rw-r--r--   0        0        0     9548 2023-10-26 11:42:11.137212 rabbit_library-0.0.3/rabbit_library/Rabbit.py
--rw-r--r--   0        0        0     3448 2023-10-26 20:38:03.049544 rabbit_library-0.0.3/README.md
--rw-r--r--   0        0        0     4058 1970-01-01 00:00:00.000000 rabbit_library-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1130 2024-05-13 16:48:34.469873 rabbit_library-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-07-03 17:14:02.867213 rabbit_library-1.0.4/rabbit_library/__init__.py
+-rw-r--r--   0        0        0     9327 2024-05-13 16:46:57.259220 rabbit_library-1.0.4/rabbit_library/Rabbit.py
+-rw-r--r--   0        0        0     3448 2023-10-26 20:38:03.049544 rabbit_library-1.0.4/README.md
+-rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 rabbit_library-1.0.4/PKG-INFO
```

### Comparing `rabbit_library-0.0.3/pyproject.toml` & `rabbit_library-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "rabbit-library"
-version = "0.0.3"
+version = "1.0.4"
 description = "Biblioteca para se conectar ao rabbit e possibilitar trabalhar com o serviço de mensageria"
 license = "MIT"
-authors = ["Your Name <you@example.com>"]
+authors = ["Eliézer Schwartz <eliezer.mail090@gmail.com>"]
 readme = "README.md"
 packages = [{include = "rabbit_library"}]
 classifiers = [    
     "Environment :: Console",
     "Natural Language :: Portuguese (Brazilian)",
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3.11",
```

### Comparing `rabbit_library-0.0.3/rabbit_library/Rabbit.py` & `rabbit_library-1.0.4/rabbit_library/Rabbit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pika
 import threading
 import typing
 import logging
-import os,signal
+import os
+import signal
 import time
 
+
 class Rabbit():
     def __init__(self, host: str, port: int, virtualhost: str, username: str, password: str, reconnect: bool = False, reconnect_delay: int = 300, continue_execution: bool = False):
         '''
         Metodo de comunicação com o rabbit nele pode ser encontrado métodos como:
             getMessages(Capturar as mensagens de uma fila )
             postMessage(Enviar mensagem para uma fila)
             close_connection(Metodo utilizado para fechar a conexão)
@@ -29,83 +31,87 @@
         self.channel = None
         self.consume_thread = None
         self.SelectConn = None
         self.confirmed_messages = set()
         self.reconnect: bool = reconnect
         self.reconnect_delay_client: int = reconnect_delay
         self.reconnect_delay_system: int = reconnect_delay
-        self.qtd_reconnects:int = 0
-        self.continue_execution:bool = continue_execution
+        self.qtd_reconnects: int = 0
+        self.continue_execution: bool = continue_execution
 
     def getMessages(self, queue: str, exchange: str, message_handler: typing.Callable, limit_get_messages: int) -> None:
         '''
             Get messages the queue!
             Recived: 
                 queue - queue to get messages
                 message_handler - method executed after having each message
                 limit_get_messages - number of messages that will be taken from the queue
         '''
-        while(True):
+        while (True):
             if not callable(message_handler):
                 raise TypeError(
                     "Necessary implemention the message_handler must be a callable function")
 
             if not queue:
                 raise ValueError("Queue parameter is mandatory")
-            
+
             try:
                 if exchange is None or exchange.strip() == '':
                     exchange = self.virtualhost
 
                 if not self.__is_connected():
                     self.__connect()
 
                 if not bool(limit_get_messages):
                     limit_get_messages = 1
-                self.__receive_message(queue, exchange, message_handler, limit_get_messages)
-                
+                self.__receive_message(
+                    queue, exchange, message_handler, limit_get_messages)
+
                 if self.continue_execution:
                     break
             except pika.exceptions.AMQPConnectionError:
                 logging.error("Connection was closed, retrying...")
                 continue
             except pika.exceptions.StreamLostError:
                 logging.error("The stream was lost, retrying...")
                 continue
             except ConnectionResetError:
                 logging.error("Connection was reset, retrying...")
                 continue
             except pika.exceptions.AMQPChannelError as err:
-                logging.error("Caught a channel error: {}, stopping...".format(err))
+                logging.error(
+                    "Caught a channel error: {}, stopping...".format(err))
                 self.reconnect = False
                 break
-            except KeyboardInterrupt:                
+            except KeyboardInterrupt:
                 self.reconnect = False
                 break
             except Exception as e:
                 logging.error(
-                    f"Error receiving message from rabbit: {str(e)} ", stack_info=True)
+                    "Error receiving message from rabbit: {} ".format(e).encode('ascii', 'ignore'), stack_info=True)
                 self.reconnect = False
                 break
             finally:
                 if not self.continue_execution:
                     if self.reconnect:
-                        if self.qtd_reconnects > 10:
+                        if self.qtd_reconnects >= 10 and self.qtd_reconnects < 30:
                             self.reconnect_delay_system = 3600
-                        elif self.qtd_reconnects > 30:
+                        elif self.qtd_reconnects >= 30 and self.qtd_reconnects <= 50:
                             self.reconnect_delay_system = 7200
-                        elif self.qtd_reconnects > 50:
+                        else:
                             self.reconnect = False
 
-                        if self.qtd_reconnects > 10:
-                            logging.info(f'Passou de {self.qtd_reconnects} reconexões, irá aguardar {str(self.reconnect_delay_system)} segundos para tentar uma nova reconexão!')
-                            
+                        if self.qtd_reconnects >= 10:
+                            logging.info(
+                                f'Passou de {self.qtd_reconnects} reconexões, irá aguardar {str(self.reconnect_delay_system)} segundos para tentar uma nova reconexão!')
+
                         time.sleep(self.reconnect_delay_system)
                         self.qtd_reconnects += 1
-                        print(f'Quantidade de reconexões: {str(self.qtd_reconnects)}')
+                        print(
+                            f'Quantidade de reconexões: {str(self.qtd_reconnects)}')
                     else:
                         self.channel.stop_consuming()
                         if self.SelectConn.is_open:
                             self.SelectConn.close()
                         os.kill(os.getpid(), signal.SIGINT)
                         break
 
@@ -145,14 +151,15 @@
         # Create a SelectConnection with the provided parameters and a callback method to handle the established connection
         self.SelectConn = pika.BlockingConnection(parameters)
         # Start the connection's I/O loop in a separate thread
         self.channel = self.SelectConn.channel()
         if not self.channel.is_closed and self.qtd_reconnects > 0:
             self.qtd_reconnects = 0
             self.reconnect_delay_system = self.reconnect_delay_client
+
     def __send_message(self, queue: str, exchange: str, message: str) -> bool:
         '''
             Send messages the rabbit
         '''
         if not queue:
             raise ValueError("Queue parameter is mandatory")
         try:
@@ -178,31 +185,25 @@
         '''
         def callback(ch, method, properties, body):
             message_handler(ch, method, properties, body)
 
         self.channel.basic_qos(prefetch_count=limit_get_messages)
         self.channel.queue_declare(queue=queue, durable=True)
         self.channel.queue_bind(
-            queue=queue, exchange=exchange, routing_key=queue)            
+            queue=queue, exchange=exchange, routing_key=queue)
         self.channel.basic_consume(
             queue=queue, on_message_callback=callback, auto_ack=False)
-        
+
         if self.continue_execution:
             self.consume_thread = threading.Thread(
                 target=self.channel.start_consuming)
             self.consume_thread.start()
         else:
             self.channel.start_consuming()
 
-        '''
-            Caso deseja que o fluxo continue executando após conectar  pode ser colocado para uma Thread o contexto de execução,
-                o que irá mudar é que no reconnect pode dae duplicidade de Threads. Deixado para fins de utilização futura caso precisar.
-            
-        '''
-
     def close_connection(self):
         try:
             if self.channel and not self.channel.is_closed:
                 self.channel.close()
         except Exception as e:
             logging.error(
                 f"Error closing connection: {str(e)} ", stack_info=True)
```

### Comparing `rabbit_library-0.0.3/README.md` & `rabbit_library-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rabbit_library-0.0.3/PKG-INFO` & `rabbit_library-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: rabbit-library
-Version: 0.0.3
+Version: 1.0.4
 Summary: Biblioteca para se conectar ao rabbit e possibilitar trabalhar com o serviço de mensageria
 License: MIT
-Author: Your Name
-Author-email: you@example.com
+Author: Eliézer Schwartz
+Author-email: eliezer.mail090@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

