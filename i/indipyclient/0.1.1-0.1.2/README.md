# Comparing `tmp/indipyclient-0.1.1.tar.gz` & `tmp/indipyclient-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.1.1.tar` & `indipyclient-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.1/LICENSE
--rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.1/README.md
--rw-r--r--   0        0        0      416 2024-05-05 14:31:43.000000 indipyclient-0.1.1/indipyclient/__init__.py
--rw-r--r--   0        0        0     3245 2024-05-02 10:21:26.000000 indipyclient-0.1.1/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.1/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    21417 2024-05-05 09:36:44.000000 indipyclient-0.1.1/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.1/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.1/indipyclient/console/windows.py
--rw-r--r--   0        0        0    26738 2024-05-03 13:06:57.000000 indipyclient-0.1.1/indipyclient/events.py
--rw-r--r--   0        0        0    32617 2024-05-05 09:46:34.000000 indipyclient-0.1.1/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    16279 2024-05-03 09:59:43.000000 indipyclient-0.1.1/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    27626 2024-05-03 10:01:46.000000 indipyclient-0.1.1/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-05-05 14:31:16.000000 indipyclient-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.2/README.md
+-rw-r--r--   0        0        0      416 2024-05-13 19:28:53.000000 indipyclient-0.1.2/indipyclient/__init__.py
+-rw-r--r--   0        0        0     4030 2024-05-09 13:19:51.000000 indipyclient-0.1.2/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.2/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    22033 2024-05-13 16:45:57.000000 indipyclient-0.1.2/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.2/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.2/indipyclient/console/windows.py
+-rw-r--r--   0        0        0    26738 2024-05-03 13:06:57.000000 indipyclient-0.1.2/indipyclient/events.py
+-rw-r--r--   0        0        0    33660 2024-05-13 11:23:49.000000 indipyclient-0.1.2/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    16279 2024-05-03 09:59:43.000000 indipyclient-0.1.2/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27626 2024-05-03 10:01:46.000000 indipyclient-0.1.2/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-05-13 19:28:14.000000 indipyclient-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.2/PKG-INFO
```

### Comparing `indipyclient-0.1.1/LICENSE` & `indipyclient-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.1/README.md` & `indipyclient-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.1/indipyclient/__main__.py` & `indipyclient-0.1.2/indipyclient/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 
-"""Usage is
+"""Creates a terminal client
 
-python3 -m indipyclient
+Try
 
+python3 -m indipyclient --help
+
+For a description of options
 """
 
 
-import os, sys, argparse, asyncio, collections, contextlib, pathlib
+import sys, argparse, asyncio, pathlib
+
+import logging
+logger = logging.getLogger('indipyclient')
 
 from . import version
 
 from .console.consoleclient import ConsoleClient, ConsoleControl
 
 
 async def runclient(client, control):
+    "Run the client.asyncrun() and control.asyncrun() coroutines"
     t1 = asyncio.create_task(client.asyncrun())
     t2 = asyncio.create_task(control.asyncrun())
-    await asyncio.gather(t1, t2)
-    # wait for tasks to be done
-    while (not t1.done()) and (not t2.done()):
-        await asyncio.sleep(0)
+    try:
+        await asyncio.gather(t1, t2)
+    except Exception:
+        # one task has raised an exception, shutdown and wait for the
+        # remaining task to shutdown
+        logger.exception("Exception report from  __main__.runclient coroutine")
+        # set flags in these classes requesting them to stop
+        client.shutdown()
+        control.shutdown()
+        while not t1.done():
+            await asyncio.sleep(0)
+        while not t2.done():
+            await asyncio.sleep(0)
+
 
 
 def main():
-    """The main routine."""
+    """The commandline entry point to run the terminal client."""
 
     parser = argparse.ArgumentParser(usage="indipyclient [options]",
                                      formatter_class=argparse.RawDescriptionHelpFormatter,
                                      description="Terminal client to communicate to an INDI service.",
                                      epilog="""The BLOB's folder can also be set from within the session.
 Setting loglevel and logfile should only be used for brief
 diagnostic purposes, the logfile could grow very big.
@@ -41,33 +58,36 @@
     parser.add_argument("-b", "--blobs", help="Optional folder where BLOB's will be saved.")
     parser.add_argument("--loglevel", help="Enables logging, value 1, 2, 3 or 4.")
     parser.add_argument("--logfile", help="File where logs will be saved")
 
     parser.add_argument("--version", action="version", version=version)
     args = parser.parse_args()
 
-    eventque = collections.deque(maxlen=4)
-
     if args.blobs:
         try:
             blobfolder = pathlib.Path(args.blobs).expanduser().resolve()
         except Exception:
             print("Error: If given, the BLOB's folder should be an existing directory")
             return 1
         else:
             if not blobfolder.is_dir():
                 print("Error: If given, the BLOB's folder should be an existing directory")
                 return 1
     else:
         blobfolder = None
 
+    # ConsoleClient is a subclass of IPyClient, with its rxevent(event) method created
+    # to add events to a queue. First a queue is created and passed into ConsoleClient
+    eventque = asyncio.Queue(maxsize=4)
+
     # On receiving an event, the client appends it into eventque
     client = ConsoleClient(indihost=args.host, indiport=args.port, eventque=eventque)
 
     # Monitors eventque and acts on the events, creates the console screens
+    # and calls the send vector methods of client to transmit data
     control = ConsoleControl(client, blobfolder=blobfolder)
 
     if args.loglevel and args.logfile:
         try:
             loglevel = int(args.loglevel)
             if loglevel not in (1,2,3,4):
                 print("Error: If given, the loglevel should be 1, 2, 3 or 4")
```

### Comparing `indipyclient-0.1.1/indipyclient/console/consoleclient.py` & `indipyclient-0.1.2/indipyclient/console/consoleclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     """Overrides IPyClient
        On receiving an event, appends it into eventque
        Which will pass the received event into ConsoleControl"""
 
     async def rxevent(self, event):
         """Add event to eventque"""
-        self.clientdata['eventque'].appendleft(event)
+        await self.clientdata['eventque'].put(event)
 
 
 class ConsoleControl:
 
     def __init__(self, client, blobfolder=None):
         """client is an instance of ConsoleClient
            If given, blobfolder will be the folder where BLOBs will be saved"""
@@ -158,17 +158,15 @@
             await asyncio.sleep(0)
         # so either shutdown has been requested or the ipyclient has stopped for some reason
         self._shutdown = True
         if not self.client.stopped:
             # client is still running, shut it down
             self.client.report("Shutting down client - please wait")
             self.client.shutdown()
-            while not self.client.stopped:
-                await asyncio.sleep(0)
-        # so ipyclient has stopped now stop console co-routines
+        # Now stop console co-routines
         self.stop = True
         while (not self.updatescreenstopped) and (not self.getinputstopped):
             await asyncio.sleep(0)
         # async tasks finished, clear up the terminal
         curses.nocbreak()
         self.stdscr.keypad(False)
         curses.curs_set(1)
@@ -188,19 +186,20 @@
                         # set disconnected status and focus on the quit button
                         if not self.screen.disconnectionflag:
                             self.devicenames.clear()
                             self.screen.showunconnected() # sets disconnectionflag
                     else:
                         # when not connected, show messages screen
                         self.screen.close("Messages")
-                    continue
+                        continue
                 # act when an event is received
                 try:
-                    event = self.eventque.pop()
-                except IndexError:
+                    event = self.eventque.get_nowait()
+                    self.eventque.task_done()
+                except asyncio.QueueEmpty:
                     # no event received, so do not update screen
                     continue
                 if isinstance(event, VectorTimeOut) and (event.devicename == self.screen.devicename):
                     if isinstance(self.screen, windows.ChooseVectorScreen):
                         self.screen.timeout(event)
                         continue
                     if isinstance(self.screen, windows.VectorScreen) and (self.screen.vectorname == event.vectorname):
@@ -271,20 +270,19 @@
                 # so its not a delete property
                 if isinstance(self.screen, windows.ChooseVectorScreen):
                     self.screen.update(event)
                     continue
                 if isinstance(self.screen, windows.VectorScreen) and (self.screen.vectorname == event.vectorname):
                     # The event refers to this vector
                     self.screen.update(event)
-
         except asyncio.CancelledError:
             self.shutdown()
             raise
         except Exception:
-            logger.exception("Error in updatescreen")
+            logger.exception("Exception report from ConsoleControl.updatescreen")
             self.shutdown()
         finally:
             self.updatescreenstopped = True
 
 
     async def getinput(self):
         try:
@@ -446,34 +444,50 @@
                         self.screen.show()
                         continue
 
         except asyncio.CancelledError:
             self.shutdown()
             raise
         except Exception:
-            logger.exception("Error in getinput")
+            logger.exception("Exception report from ConsoleControl.getinput")
             self.shutdown()
         finally:
             self.getinputstopped = True
 
 
     def send_enableBLOB(self):
         "Sends Also to enable blobs for all devices"
         if not self.blobenabled:
             return
         for devicename,device in self.client.items():
             if device.enable:
                 self.client.send_enableBLOB('Also', devicename)
 
+
     def send_disableBLOB(self):
         "Sends Never to disable blobs for all devices"
         if self.blobenabled:
             return
         for devicename,device in self.client.items():
             if device.enable:
                 self.client.send_enableBLOB('Never', devicename)
 
 
     async def asyncrun(self):
         """Gathers tasks to be run simultaneously"""
         self.stop = False
-        await asyncio.gather(self.updatescreen(), self.getinput(), self._checkshutdown())
+        t1 = asyncio.create_task(self.updatescreen())
+        t2 = asyncio.create_task(self.getinput())
+        t3 = asyncio.create_task(self._checkshutdown())
+        try:
+            await asyncio.gather(t1, t2, t3)
+        except Exception:
+            # one task has raised an exception, shutdown and wait for the
+            # remaining task to shutdown
+            logger.exception("Exception report from  ConsoleControl.asyncrun coroutine")
+            self.stop = True
+            while not t1.done():
+                await asyncio.sleep(0)
+            while not t2.done():
+                await asyncio.sleep(0)
+            while not t3.done():
+                await asyncio.sleep(0)
```

### Comparing `indipyclient-0.1.1/indipyclient/console/widgets.py` & `indipyclient-0.1.2/indipyclient/console/widgets.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.1/indipyclient/console/windows.py` & `indipyclient-0.1.2/indipyclient/console/windows.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.1/indipyclient/events.py` & `indipyclient-0.1.2/indipyclient/events.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.1/indipyclient/ipyclient.py` & `indipyclient-0.1.2/indipyclient/ipyclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         self.stopped = False
 
         # Indicates how verbose the debug xml logs will be when created.
         self._verbose = 1
 
 
     def debug_verbosity(self, verbose):
-        """Indicate how verbose the debug xml logs will be when created.
+        """Set how verbose the debug xml logs will be when created.
            1 for transmitted/received vector tags only,
            2 for transmitted/received vectors, members and contents (apart from BLOBs)
            3 for all transmitted/received data including BLOBs."""
         if verbose not in (1,2,3):
             raise ValueError
         self._verbose = verbose
 
@@ -198,40 +198,52 @@
 
     async def _comms(self):
         "Create a connection to an INDI port"
         try:
             while not self._stop:
                 self.tx_timer = None
                 self.idle_timer = time.time()
+                t1 = None
+                t2 = None
+                t3 = None
                 try:
                     # start by openning a connection
-                    # clear messages
-                    self.messages.clear()
                     self.report("Attempting to connect")
                     reader, writer = await asyncio.open_connection(self.indihost, self.indiport)
                     self.connected = True
                     self.messages.clear()
+                    # clear devices etc
+                    self.clear()
                     self.report(f"Connected to {self.indihost}:{self.indiport}")
-                    await asyncio.gather(self._run_tx(writer),
-                                         self._run_rx(reader),
-                                         self._check_alive(writer)
-                                         )
+                    t1 = asyncio.create_task(self._run_tx(writer))
+                    t2 = asyncio.create_task(self._run_rx(reader))
+                    t3 = asyncio.create_task(self._check_alive(writer))
+                    await asyncio.gather(t1, t2, t3)
                 except ConnectionRefusedError:
                     self.report(f"Error: Connection refused on {self.indihost}:{self.indiport}")
                 except ConnectionResetError:
                     self.report("Error: Connection Lost")
                 except Exception:
                     logger.exception("Connection Error")
                     self.report("Error: Connection failed")
                 self._clear_connection()
+                # connection has failed, ensure all tasks are done
+                if t1:
+                    while not t1.done():
+                        await asyncio.sleep(0)
+                if t2:
+                    while not t2.done():
+                        await asyncio.sleep(0)
+                if t3:
+                    while not t3.done():
+                        await asyncio.sleep(0)
                 if self._stop:
                     break
                 else:
                     self.report(f"Connection failed, re-trying...")
-
                 # wait five seconds before re-trying, but keep checking
                 # that self._stop has not been set
                 count = 0
                 while not self._stop:
                     await asyncio.sleep(0.5)
                     count += 1
                     if count >= 10:
@@ -239,29 +251,19 @@
         except Exception:
             logger.exception("Error in IPyClient._comms method")
         finally:
             self.shutdown()
 
 
     def _clear_connection(self):
-        "On a connection closing down, clears queues"
+        "On a connection closing down, clears devices"
         self.connected = False
         self.tx_timer = None
-        # clear devices etc
-        self.clear()
         # clear the writerque
         self.writerque.clear()
-        if not self.readerque.empty():
-            # empty the queue
-            while True:
-                try:
-                    xmldata = self.readerque.get_nowait()
-                    self.readerque.task_done()
-                except asyncio.QueueEmpty:
-                    break
 
 
 
     def send(self, xmldata):
         """Transmits xmldata, this is an internal method, not normally called by a user.
            xmldata is an xml.etree.ElementTree object"""
         if self.connected:
@@ -319,15 +321,18 @@
         try:
             while self.connected and (not self._stop):
                 await asyncio.sleep(0)
                 try:
                     txdata = self.writerque.popleft()
                 except IndexError:
                     continue
-
+                if not self.connected:
+                    break
+                if self._stop:
+                    break
                 if txdata.tag == "newBLOBVector" and len(txdata):
                     # txdata is a newBLOBVector containing blobs
                     # the generator blob_xml_bytes yields bytes
                     for binarydata in blob_xml_bytes(txdata):
                         # Send to the port
                         writer.write(binarydata)
                         await writer.drain()
@@ -341,14 +346,16 @@
                 # data has been transmitted set timers going, do not set timer
                 # for enableBLOB as no answer is expected for that
                 if (self.tx_timer is None) and (txdata.tag != "enableBLOB"):
                     self.tx_timer = time.time()
                 self.idle_timer = time.time()
                 if logger.isEnabledFor(logging.DEBUG):
                     self._logtx(txdata)
+            # stop writing data, so clear writerque
+            self.writerque.clear()
         except KeyboardInterrupt:
             self.shutdown()
 
     def _logrx(self, rxdata):
         "log rx data to file"
         startlog = "RX:: "
         if self._verbose == 3:
@@ -370,52 +377,57 @@
             binarydata = ET.tostring(data, short_empty_elements=False).split(b">")
             logger.debug(startlog + binarydata[0].decode() + ">")
 
 
     async def _run_rx(self, reader):
         "pass xml.etree.ElementTree data to readerque"
         try:
+            # get block of xml.etree.ElementTree data
+            # from source and append it to  readerque
             source = self._datasource(reader)
-            while self.connected and (not self._stop):
-                await asyncio.sleep(0)
-                # get block of xml.etree.ElementTree data
-                # from source and append it to  readerque
-                rxdata = await anext(source)
-                if rxdata is not None:
-                    # and place rxdata into readerque
+            async for rxdata in source:
+                # and place rxdata into readerque
+                while self.connected and (not self._stop):
+                    await asyncio.sleep(0)
                     try:
                         self.readerque.put_nowait(rxdata)
                     except asyncio.QueueFull:
-                        # The queue is full, something may be wrong
-                        # discard this data and continue
-                        pass
-                    else:
-                        if logger.isEnabledFor(logging.DEBUG):
-                            self._logrx(rxdata)
+                        # The queue is full
+                        continue
+                    # rxdata is now in readerque
+                    break
+                if logger.isEnabledFor(logging.DEBUG):
+                    self._logrx(rxdata)
+                if (not self.connected) or self._stop:
+                    break
         except RuntimeError:
             # catches StopAsyncIteration and stops this coroutine
             pass
+        except StopAsyncIteration:
+            # catches StopAsyncIteration and stops this coroutine
+            pass
         except KeyboardInterrupt:
             self.shutdown()
         except Exception:
             logger.exception("Error in _run_rx")
             self.shutdown()
 
 
 
     async def _datasource(self, reader):
         "get received data, parse it, and yield it as xml.etree.ElementTree object"
         data_in = self._datainput(reader)
         message = b''
         messagetagnumber = None
         try:
-            while self.connected and (not self._stop):
-                await asyncio.sleep(0)
-                # get blocks of data from _datainput
-                data = await anext(data_in)
+            async for data in data_in:
+                if not self.connected:
+                    return
+                if self._stop:
+                    return
                 if not data:
                     continue
                 if not message:
                     # data is expected to start with <tag, first strip any newlines
                     data = data.strip()
                     for index, st in enumerate(_STARTTAGS):
                         if data.startswith(st):
@@ -508,19 +520,19 @@
             raise
 
 
     async def _rxhandler(self):
         """Populates the events using data from self.readerque"""
         try:
             while not self._stop:
-                # get block of data from the self.readerque
                 await asyncio.sleep(0)
+                # get block of data from the self.readerque
                 try:
-                    root = self.readerque.get_nowait()
-                except asyncio.QueueEmpty:
+                    root = await asyncio.wait_for(self.readerque.get(), timeout=0.5)
+                except asyncio.TimeoutError:
                     # nothing to read, continue while loop which re-checks the _stop flag
                     continue
                 devicename = root.get("device")
                 # block any other thread from accessing data until update is done
                 try:
                     with threading.Lock():
                         if devicename is None:
@@ -655,15 +667,15 @@
                             self.report("getProperties sent")
                         count += 1
                         if count >= 10:
                             count = 0
         except asyncio.CancelledError:
              raise
         except Exception:
-            logger.exception("Error in IPyClient._timeout_monitor method")
+            logger.exception("Exception report from IPyClient._timeout_monitor method")
         finally:
             self.shutdown()
 
 
     def send_getProperties(self, devicename=None, vectorname=None):
         """Sends a getProperties request. On startup the IPyClient object
            will automatically send getProperties, so typically you will
@@ -700,15 +712,30 @@
            event is an object with attributes according to the data received."""
         pass
 
 
     async def asyncrun(self):
         "Await this method to run the client."
         self._stop = False
-        await asyncio.gather(self._comms(), self._rxhandler(), self._timeout_monitor(), return_exceptions=True)
+        t1 = asyncio.create_task(self._comms())
+        t2 = asyncio.create_task(self._rxhandler())
+        t3 = asyncio.create_task(self._timeout_monitor())
+        try:
+            await asyncio.gather(t1, t2, t3)
+        except Exception:
+            # one task has raised an exception, wait for the
+            # remaining tasks to stop
+            self._stop = True
+            logger.exception("Exception report from IPyClient.asyncrun coroutine")
+            while not t1.done():
+                await asyncio.sleep(0)
+            while not t2.done():
+                await asyncio.sleep(0)
+            while not t3.done():
+                await asyncio.sleep(0)
         self.stopped = True
 
 
 class Device(collections.UserDict):
 
     "Each device is a mapping of vector name to vector object."
```

### Comparing `indipyclient-0.1.1/indipyclient/propertymembers.py` & `indipyclient-0.1.2/indipyclient/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.1/indipyclient/propertyvectors.py` & `indipyclient-0.1.2/indipyclient/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.1/pyproject.toml` & `indipyclient-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.1.1"
+version = "0.1.2"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.1.1/PKG-INFO` & `indipyclient-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

