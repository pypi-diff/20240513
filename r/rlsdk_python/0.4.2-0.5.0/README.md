# Comparing `tmp/rlsdk_python-0.4.2.tar.gz` & `tmp/rlsdk_python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlsdk_python-0.4.2.tar", max compression
+gzip compressed data, was "rlsdk_python-0.5.0.tar", max compression
```

## Comparing `rlsdk_python-0.4.2.tar` & `rlsdk_python-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      357 2024-05-06 00:11:43.618389 rlsdk_python-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1640 2024-04-21 20:56:20.206780 rlsdk_python-0.4.2/README.md
--rw-r--r--   0        0        0      121 2024-04-28 17:35:36.468385 rlsdk_python-0.4.2/rlsdk_python/__init__.py
--rw-r--r--   0        0        0     1812 2024-04-18 23:00:20.787805 rlsdk_python-0.4.2/rlsdk_python/event_handling.py
--rw-r--r--   0        0        0     1814 2024-04-18 21:23:06.061748 rlsdk_python-0.4.2/rlsdk_python/events.py
--rw-r--r--   0        0        0     4065 2024-04-26 18:56:51.985326 rlsdk_python-0.4.2/rlsdk_python/frida_script.py
--rw-r--r--   0        0        0    31126 2024-05-06 00:07:22.328055 rlsdk_python-0.4.2/rlsdk_python/game_objects.py
--rw-r--r--   0        0        0    22132 2024-05-06 00:10:23.291759 rlsdk_python-0.4.2/rlsdk_python/sdk.py
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 rlsdk_python-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      378 2024-05-13 07:58:38.910785 rlsdk_python-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1640 2024-04-21 20:56:20.206780 rlsdk_python-0.5.0/README.md
+-rw-r--r--   0        0        0      121 2024-04-28 17:35:36.468385 rlsdk_python-0.5.0/rlsdk_python/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-18 23:00:20.787805 rlsdk_python-0.5.0/rlsdk_python/event_handling.py
+-rw-r--r--   0        0        0     2165 2024-05-10 12:17:36.935543 rlsdk_python-0.5.0/rlsdk_python/events.py
+-rw-r--r--   0        0        0     9026 2024-05-11 22:26:21.652222 rlsdk_python-0.5.0/rlsdk_python/frida_script.py
+-rw-r--r--   0        0        0    32605 2024-05-10 11:48:32.834382 rlsdk_python-0.5.0/rlsdk_python/game_objects.py
+-rw-r--r--   0        0        0    27050 2024-05-11 22:23:03.827502 rlsdk_python-0.5.0/rlsdk_python/sdk.py
+-rw-r--r--   0        0        0     2103 1970-01-01 00:00:00.000000 rlsdk_python-0.5.0/PKG-INFO
```

### Comparing `rlsdk_python-0.4.2/README.md` & `rlsdk_python-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.4.2/rlsdk_python/event_handling.py` & `rlsdk_python-0.5.0/rlsdk_python/event_handling.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.4.2/rlsdk_python/events.py` & `rlsdk_python-0.5.0/rlsdk_python/events.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .game_objects import Car, UFunction, FName, BoostPad
+from .game_objects import Car, UFunction, FName, BoostPad, PlayerController
 from typing import Any
 from .event_handling import EventData
 
 
 
 class EventBoostPadChanged(EventData):
     def __init__(self, boostpad: BoostPad):
@@ -29,15 +29,22 @@
 class EventGameEventStarted(EventData):
     def __init__(self):
         pass
 
 class EventGameEventDestroyed(EventData):
     def __init__(self):
         pass
-
+    
+class EventChatMessage(EventData):
+    def __init__(self, player_controller: PlayerController, message: str, channel: int, preset: bool):
+        self.channel = channel
+        self.player_controller = player_controller
+        self.message = message
+        
+        
 class EventKeyPressed(EventData):
 
     types = {
         0: "pressed",
         1: "released",
         2: "repeat",
         3: "doubleclick",
@@ -50,16 +57,16 @@
         self.controller_id = int.from_bytes(bytes[0:4], byteorder='little')
         self.return_value = bytes[24] & 0x01
         self.key = key 
         self.type = self.types[int.from_bytes(bytes[12:13], byteorder='little')]
 
 
 class EventTypes:
-    ON_HOOKED_FUNCTION = "on_hooked_function"
+    ON_HOOKED_FUNCTION_CALLED = "on_hooked_function_called"
     ON_PLAYER_TICK = "on_player_tick"
     ON_ROUND_ACTIVE_STATE_CHANGED = "on_round_active_state_changed" 
     ON_RESET_PICKUPS = "on_reset_pickups"
     ON_GAME_EVENT_STARTED = "on_game_event_started"
     ON_KEY_PRESSED = "on_key_pressed"
     ON_BOOSTPAD_CHANGED = "on_boostpad_changed"
     ON_GAME_EVENT_DESTROYED = "on_game_event_destroyed"
-
+    ON_CHAT_MESSAGE = "on_chat_message"
```

### Comparing `rlsdk_python-0.4.2/rlsdk_python/game_objects.py` & `rlsdk_python-0.5.0/rlsdk_python/game_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         for i in range(array_count - 1):  # -1 car il y a souvent un caractère null de terminaison
             char = self.sdk.pm.read_ushort(array_data_address + (i * 2))  # lire 2 octets à la fois
             result += chr(char)
 
         return result
     
 
-class PlayerReplicationInfo(Pointer):
+class PlayerReplicationInfo(Actor):
     size = 0x0410
 
     def get_player_name(self):
         player_name_address = self.address + 0x0288
         return FString(player_name_address, sdk=self.sdk).get_string()
     
     def get_team_info(self):
@@ -601,31 +601,59 @@
 class Team(TeamInfo):
     size = 0x0468
 
     def get_members(self):
         members_address = self.address + 0x0318
         return TArray(members_address, PRI, sdk=self.sdk).get_items()
 
-class Controller(Pointer):
+class Controller(Actor):
     size = 0x0474
 
     def get_player_num(self):
         return self.sdk.pm.read_int(self.address + 0x0290)
 
 class PlayerController(Controller):
     size = 0x0D00
+    
+    def __init__(self, address, *, sdk=None):
+        super().__init__(address, sdk=sdk)
+        
+        self.chat_message = self.sdk.create_callable_function(
+            "Function TAGame.PlayerController_TA.ChatMessage_TA",
+            arg_types={
+                "InPRI": "pointer",
+                "Message": "fstring",  # La taille sera ajustée dynamiquement
+                "ChatChannel": "uint32",
+                "bPreset": "uint32"
+                
+            }
+        )
+    
+    
+    def chat(self, message, channel=0, preset=0):  
+        self.chat_message(self, InPRI=self.get_pri(), Message=message, ChatChannel=channel, bPreset=0)
+        
+        
  
     def get_pri(self):
         pri_address = self.sdk.pm.read_ulonglong(self.address + 0x0988)
         return PRI(pri_address, sdk=self.sdk)
 
     def get_car(self):
         car_address = self.sdk.pm.read_ulonglong(self.address + 0x0980)
         return Car(car_address, sdk=self.sdk)
     
+    def get_hud(self):
+        hud_address = self.sdk.pm.read_ulonglong(self.address + 0x04F8)
+        return HUD(hud_address, sdk=self.sdk)
+    
+    def get_secondary_hud(self):
+        secondary_hud_address = self.sdk.pm.read_ulonglong(self.address + 0x0500)
+        return HUD(secondary_hud_address, sdk=self.sdk)
+    
 
 class VehicleInputs(Pointer):
     size = 0x0020
 
     def __init__ (self, address, sdk=None):
         super().__init__(address, sdk=sdk)
 
@@ -790,14 +818,31 @@
     size = 0x03C0
 
     def get_game_event(self):
         game_event_address = self.sdk.pm.read_ulonglong(self.address + 0x02E8)
         return GameEvent(game_event_address, sdk=self.sdk)
 
     
+class Canvas(UObject):
+     size = 0x00C8
+     
+
+class HUD(UObject):
+    size = 0x0308
+    
+    def get_player_owner(self):
+        player_controller_address = self.sdk.pm.read_ulonglong(self.address + 0x0278)
+        return PlayerController(player_controller_address, sdk=self.sdk)
+    
+    def get_canvas(self):
+        canvas_address = self.sdk.pm.read_ulonglong(self.address + 0x0280)
+        return Canvas(canvas_address, sdk=self.sdk)
+
+
+
 # Following classes are not pointing to any memory address, they are just data containers
     
 
 
 
 
 class BoostPad():
@@ -903,15 +948,19 @@
     
     def update_boostpad_from_pickup(self, pad: BoostPad, pickup: VehiclePickupBoost):
         x,y,z = pickup.get_location().get_xyz()
         pad.location.x = x
         pad.location.y = y
         pad.location.z = z
         
-        
+
+
+
+
+
 
 # struct UGameViewportClient_TA_execHandleKeyPress_Params
 # {
 # 	int32_t                                            ControllerId;                                     		// 0x0000 (0x0004) [0x0000000000000080] (CPF_Parm)    
 # 	struct FName                                       Key;                                              		// 0x0004 (0x0008) [0x0000000000000080] (CPF_Parm)    
 # 	uint8_t                                            EventType;                                        		// 0x000C (0x0001) [0x0000000000000080] (CPF_Parm)    
 # 	float                                              AmountDepressed;                                  		// 0x0010 (0x0004) [0x0000000000000080] (CPF_Parm)
```

### Comparing `rlsdk_python-0.4.2/rlsdk_python/sdk.py` & `rlsdk_python-0.5.0/rlsdk_python/sdk.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,422 +2,537 @@
 import pymem.pattern
 import ctypes
 import frida
 import time
 import threading
 from typing import Callable, Any, Protocol
 from .event_handling import Event
-from .events import EventFunctionHooked, EventBoostPadChanged, EventTypes, EventPlayerTick, EventRoundActiveStateChanged, EventResetPickups, EventGameEventStarted, EventKeyPressed, EventGameEventDestroyed
-from .game_objects import UClass, UFunction, GameEvent, TArray, UObject, FNameEntry, FName, Field, VehiclePickupBoost, GameViewportClient
+from .events import (
+    EventFunctionHooked,
+    EventBoostPadChanged,
+    EventTypes,
+    EventPlayerTick,
+    EventRoundActiveStateChanged,
+    EventResetPickups,
+    EventGameEventStarted,
+    EventKeyPressed,
+    EventGameEventDestroyed,
+    EventChatMessage
+)
+from .game_objects import (
+    UClass,
+    UFunction,
+    GameEvent,
+    TArray,
+    UObject,
+    FNameEntry,
+    FName,
+    Field,
+    VehiclePickupBoost,
+    GameViewportClient,
+    PlayerController
+)
 from .frida_script import frida_script
 from colorama import Fore, Back, Style, just_fix_windows_console
 from tqdm import tqdm
 import json
+from tabulate import tabulate
 
 PROCESS_NAME = "RocketLeague.exe"
 
 FUNCTION_PICKED_UP = "Function TAGame.VehiclePickup_TA.OnPickUp"
 FUNCTION_PLAYER_TICK = "Function Engine.PlayerController.PlayerTick"
 FUNCTION_KEY_PRESS = "Function TAGame.GameViewportClient_TA.HandleKeyPress"
-FUNCTION_BALL_CAR_TOUCH= "Function TAGame.Ball_TA.EventCarTouch"
+FUNCTION_BALL_CAR_TOUCH = "Function TAGame.Ball_TA.EventCarTouch"
 FUNCTION_SET_VEHICLE_INPUT = "Function TAGame.Car_TA.SetVehicleInput"
 FUNCTION_PICKUP_TOUCH = "Function TAGame.VehiclePickup_TA.Touch"
 FUNCTION_BALL_ON_RIGID_BODY_COLLISION = "Function TAGame.Ball_TA.OnRigidBodyCollision"
 FUNCTION_BOOST_PICKED_UP = "Function TAGame.VehiclePickup_Boost_TA.Idle.EndState"
 FUNCTION_BOOST_RESPAWN = "Function TAGame.VehiclePickup_Boost_TA.Idle.BeginState"
 FUNCTION_ROUND_ACTIVE_BEGIN = "Function TAGame.GameEvent_Soccar_TA.Active.BeginState"
 FUNCTION_ROUND_ACTIVE_END = "Function TAGame.GameEvent_Soccar_TA.Active.EndState"
 FUNCTION_RESET_PICKUPS = "Function TAGame.GameEvent_TA.ResetPickups"
 FUNCTION_GAMEEVENT_BEGIN_PLAY = "Function TAGame.GameEvent_Soccar_TA.PostBeginPlay"
 FUNCTION_GAME_EVENT_ACTIVE_TICK = "Function TAGame.GameEvent_Soccar_TA.Active.Tick"
 FUNCTION_GAME_VIEWPORT_CLIENT_TICK = "Function Engine.GameViewportClient.Tick"
 FUNCTION_GAME_EVENT_DESTROYED = "Function TAGame.GameEvent_Soccar_TA.Destroyed"
+FUNCTION_EVENT_CHAT_MESSAGE = "Function TAGame.GFxData_Chat_TA.OnChatMessage"
 
 CLASS_CORE_OBJECT = "Class Core.Object"
 
-GREEN = '\033[92m' # Texte vert
-RED = '\033[91m' # Texte rouge
-BLUE = '\033[94m' # Texte bleu
-YELLOW = '\033[93m' # Texte jaune
-END = '\033[0m'    # Réinitialiser le style
+GREEN = "\033[92m"  # Texte vert
+RED = "\033[91m"  # Texte rouge
+BLUE = "\033[94m"  # Texte bleu
+YELLOW = "\033[93m"  # Texte jaune
+END = "\033[0m"  # Réinitialiser le style
 
 # Event list
 
-ON_FUNCTION_HOOKED="on_function_called"
+ON_FUNCTION_HOOKED = "on_function_called"
 
 DEFAULT_CONFIG = {
     "gnames_offset": None,
     "gobjects_offset": None,
 }
 
 
 class RLSDK:
 
-    def __init__(self, hook_player_tick=False, pid=None):
-        
+    def __init__(self, pid=None):
+
         self.pid = pid
 
         self.config = DEFAULT_CONFIG
-        
+
         try:
             self.pm = pymem.Pymem(self.pid if self.pid else PROCESS_NAME)
             self.frida = frida.attach(self.pid if self.pid else PROCESS_NAME)
         except:
-            raise Exception(Fore.RED + "Rocket League not found. Make sure Rocket League is running." + END)
-
+            raise Exception(
+                Fore.RED
+                + "Rocket League not found. Make sure Rocket League is running."
+                + END
+            )
 
         # open sdk_config.json file to read offsets
-        
+
         try:
             with open("sdk_config.json", "r") as file:
                 self.config = json.load(file)
 
                 if self.config["gnames_offset"]:
                     self.g_names_offset = self.config["gnames_offset"]
-          
+
                 if self.config["gobjects_offset"]:
                     self.g_object_offset = self.config["gobjects_offset"]
         except:
             # create sdk_config.json file if it doesn't exist
             with open("sdk_config.json", "w") as file:
                 json.dump(DEFAULT_CONFIG, file, indent=4)
-        
-    
 
-        if self.config["gnames_offset"] == None or self.config["gobjects_offset"] == None:
+        if (
+            self.config["gnames_offset"] == None
+            or self.config["gobjects_offset"] == None
+        ):
             try:
                 self.resolve_offsets()
             except:
-                raise Exception(Fore.RED + "Offsets not found. Make sure Rocket League is running. If Rocket League is running, game memory structure may have changed and can't be scanned. Please try to obtain them by your own and update sdk_config.json" + END)
-            
+                raise Exception(
+                    Fore.RED
+                    + "Offsets not found. Make sure Rocket League is running. If Rocket League is running, game memory structure may have changed and can't be scanned. Please try to obtain them by your own and update sdk_config.json"
+                    + END
+                )
+
             # save offsets to sdk_config.json
-            
+
             with open("sdk_config.json", "w") as file:
                 json.dump(self.config, file, indent=4)
-            
+
         else:
             print(Fore.GREEN + "Offsets found in sdk_config.json" + END)
 
         self.event = Event()
 
         self.index_indexed_gnames = {}
         self.gnames = {}
 
         self.static_classes = {}
         self.static_functions = {}
 
         self.scan_result = []
         self.scan_response_received_event = threading.Event()
 
-
         try:
             self.load_gnames()
             self.map_objects()
-            
-            if len(self.gnames) == 0 or len(self.static_classes) == 0 or len(self.static_functions) == 0:
+
+            if (
+                len(self.gnames) == 0
+                or len(self.static_classes) == 0
+                or len(self.static_functions) == 0
+            ):
                 raise Exception("GNames or mapping objects not found")
 
         except:
-            print(Fore.RED + "Error while loading GNames and mapping objects. Trying to resolve offsets" + END)
-           # If an error occurs, offset may be wrong, try to resolve them again
+            print(
+                Fore.RED
+                + "Error while loading GNames and mapping objects. Trying to resolve offsets"
+                + END
+            )
+            # If an error occurs, offset may be wrong, try to resolve them again
             try:
                 self.resolve_offsets()
                 self.load_gnames()
                 self.map_objects()
-                
+
                 with open("sdk_config.json", "w") as file:
                     json.dump(self.config, file, indent=4)
             except:
-                raise Exception(Fore.RED + "Error while loading GNames and mapping objects. Make sure Rocket League is running." + END)
-
-            
+                raise Exception(
+                    Fore.RED
+                    + "Error while loading GNames and mapping objects. Make sure Rocket League is running."
+                    + END
+                )
 
         self.process_event_address = self.get_process_event_address()
         self.current_game_event = None
 
         if self.process_event_address == None:
-            print(Fore.RED + "ProcessEvent address not found. Make sure Rocket League is running." + END)
+            print(
+                Fore.RED
+                + "ProcessEvent address not found. Make sure Rocket League is running."
+                + END
+            )
             return
 
         print("ProcessEvent Address: " + hex(self.process_event_address))
-        print(Fore.GREEN + "ProcessEvent address found: " + Fore.BLUE + hex(self.process_event_address) + END)
-       
+        print(
+            Fore.GREEN
+            + "ProcessEvent address found: "
+            + Fore.BLUE
+            + hex(self.process_event_address)
+            + END
+        )
+
         print(Fore.YELLOW + "Injecting Frida script..." + END)
 
         self.frida_script = self.frida.create_script(frida_script)
         self.frida_script.load()
-        self.frida_script.on('message', self.on_frida_message)
+        self.frida_script.on("message", self.on_frida_message)
 
         # send process event address to frida
-        self.frida_script.post({"type": "process_event_address", "address": self.process_event_address})
+        self.frida_script.post(
+            {"type": "process_event_address", "address": self.process_event_address}
+        )
+
+        self.event.subscribe(
+            EventTypes.ON_HOOKED_FUNCTION_CALLED, self.on_function_called
+        )
 
         self.hook_function(FUNCTION_BOOST_PICKED_UP)
         self.hook_function(FUNCTION_BOOST_RESPAWN)
         self.hook_function(FUNCTION_ROUND_ACTIVE_BEGIN)
         self.hook_function(FUNCTION_ROUND_ACTIVE_END)
         self.hook_function(FUNCTION_RESET_PICKUPS)
         self.hook_function(FUNCTION_GAMEEVENT_BEGIN_PLAY)
-        # self.hook_function(FUNCTION_GAME_EVENT_ACTIVE_TICK)
-        self.hook_function(FUNCTION_KEY_PRESS, args_map=[(2, "bytes", "key_params", 0x1c)])
+        self.hook_function(
+            FUNCTION_KEY_PRESS, args_map=[( "key_params", "bytes", 0x1C)]
+        )
         self.hook_function(FUNCTION_GAME_VIEWPORT_CLIENT_TICK)
         self.hook_function(FUNCTION_GAME_EVENT_DESTROYED)
-
-        # player tick is conditional because it's called every frame, we don't want hook it if developer doesn't need it
-
-        if hook_player_tick:
-            self.hook_function(FUNCTION_PLAYER_TICK, args_map=[(2, "float", "deltatime")])
-
-
-        self.event.subscribe(EventTypes.ON_HOOKED_FUNCTION, self.on_function_called)
+        self.hook_function(FUNCTION_EVENT_CHAT_MESSAGE, args_map=[
+            ("message", "fstring"),
+            ("channel", "enum"),
+            ("unique_net_id", "bytes", 0x0042)
+        ])
 
         self.field = Field(self)
-        
+
+        time.sleep(1)
         print(Fore.GREEN + "SDK initialized" + END)
-      
+
     # ==========================================================
     # ================     Offsets finding     =================
     # ==========================================================
 
-        
     def resolve_offsets(self):
 
         print(Fore.YELLOW + "Finding GNames offset..." + END)
         try:
             self.g_names_offset = self.resolve_gnames_offset()
             self.config["gnames_offset"] = self.g_names_offset
         except:
             raise Exception("GNames offset not found")
 
+        print(
+            Fore.GREEN
+            + "GNames offset found at "
+            + Fore.BLUE
+            + hex(self.g_names_offset)
+            + END
+        )
 
-        print(Fore.GREEN + "GNames offset found at " + Fore.BLUE + hex(self.g_names_offset) + END)
-        
         print(Fore.YELLOW + "Finding GObjects offset..." + END)
-        
+
         try:
             self.g_object_offset = self.resolve_gobjects_offset()
             self.config["gobjects_offset"] = self.g_object_offset
         except:
             raise Exception(Fore.RED + "GObjects offset not found" + END)
-        
-        print(Fore.GREEN + "GObjects offset found at " + Fore.BLUE + hex(self.g_object_offset) + END)
 
-        
-        
-        
+        print(
+            Fore.GREEN
+            + "GObjects offset found at "
+            + Fore.BLUE
+            + hex(self.g_object_offset)
+            + END
+        )
+
     def resolve_gobjects_offset(self):
         # Pattern recherché
-        pattern = rb'\xE8....\x8B\x5D\xAF'
-        
+        pattern = rb"\xE8....\x8B\x5D\xAF"
+
         # Trouver l'adresse de base du pattern
         base_address = self.pm.pattern_scan_all(pattern, return_multiple=False)
         if base_address is None:
             return None
 
         # Calcul des différents offsets pour atteindre l'adresse finale
         # Lire l'offset relatif à partir de l'adresse de base + 1 et ajouter à base_address
         relative_offset = self.pm.read_int(base_address + 1)
-        intermediate_address = base_address + 1 + relative_offset + 4  # +4 pour la taille de l'int lu
+        intermediate_address = (
+            base_address + 1 + relative_offset + 4
+        )  # +4 pour la taille de l'int lu
 
         # Lire l'offset relatif à partir du nouvel emplacement + 0x65 et ajouter à l'adresse intermédiaire
         final_relative_offset = self.pm.read_int(intermediate_address + 0x65 + 3)
-        final_address = intermediate_address + 0x65 + 3 + final_relative_offset + 4  # +4 pour la taille de l'int lu
-        
+        final_address = (
+            intermediate_address + 0x65 + 3 + final_relative_offset + 4
+        )  # +4 pour la taille de l'int lu
+
         if not final_address:
             raise Exception("GObjects offset not found")
 
         return final_address - self.pm.base_address
 
     def resolve_gnames_offset(self):
         # Pattern recherché
-        pattern = rb'\x75.\xE8....\x48\xC7\xC7'
-        
+        pattern = rb"\x75.\xE8....\x48\xC7\xC7"
+
         # Trouver l'adresse de base du pattern
         base_address = self.pm.pattern_scan_all(pattern, return_multiple=False)
         if base_address is None:
             return None
 
         # Calcul des différents offsets pour atteindre l'adresse finale
         # Lire l'offset relatif à partir de l'adresse de base + 3 et ajouter à base_address
         relative_offset = self.pm.read_int(base_address + 3)
-        intermediate_address = base_address + 3 + relative_offset + 4  # +4 pour la taille de l'int lu
+        intermediate_address = (
+            base_address + 3 + relative_offset + 4
+        )  # +4 pour la taille de l'int lu
 
         # Lire l'offset relatif à partir du nouvel emplacement + 0x2F et ajouter à l'adresse intermédiaire
         final_relative_offset = self.pm.read_int(intermediate_address + 0x2F + 3)
-        final_address = intermediate_address + 0x2F + 3 + final_relative_offset + 4  # +4 pour la taille de l'int lu
-        
+        final_address = (
+            intermediate_address + 0x2F + 3 + final_relative_offset + 4
+        )  # +4 pour la taille de l'int lu
+
         if not final_address:
             raise Exception("GNames offset not found")
 
         return final_address - self.pm.base_address
 
-
     def get_provider(self):
         # Pattern recherché
-        pattern = rb'\xBA\xFA\x02\x00\x00\x48\x89\x05'
-        
+        pattern = rb"\xBA\xFA\x02\x00\x00\x48\x89\x05"
+
         # Trouver l'adresse de base du pattern
         base_address = self.pm.pattern_scan_all(pattern, return_multiple=False)
         if base_address is None:
             return None
 
         # Calcul des différents offsets pour atteindre l'adresse finale
         # Lire l'offset relatif à partir de l'adresse de base + 8 et ajouter à base_address
         relative_offset = self.pm.read_int(base_address + 8)
-        final_address = base_address + 8 + relative_offset + 4  # +4 pour la taille de l'int lu
+        final_address = (
+            base_address + 8 + relative_offset + 4
+        )  # +4 pour la taille de l'int lu
 
         # Lire l'adresse du UObjectProvider à partir de l'adresse calculée
         provider_address = self.pm.read_ulonglong(final_address)
         if not provider_address:
             return None
 
         # La structure commence à provider_address + 0xD8
         tarray_base_address = provider_address + 0xD8
 
         # Création et retour de l'objet TArray
         tarray = TArray(tarray_base_address, UObject, sdk=self)
-        
+
         return tarray
-    
-    
-    
-        
+
     def load_gnames(self):
 
         print(Fore.YELLOW + "Loading GNames..." + END)
         gnames_entries_tarray = self.get_gnames_entries_tarray()
-        print(Fore.GREEN + "GNames count: " + Fore.BLUE + str(len(gnames_entries_tarray)) + END)
-        
-        
+        print(
+            Fore.GREEN
+            + "GNames count: "
+            + Fore.BLUE
+            + str(len(gnames_entries_tarray))
+            + END
+        )
+
         for gname_entry in tqdm(gnames_entries_tarray):
 
             if not gname_entry.address:
                 continue
 
             self.gnames[gname_entry.get_index()] = gname_entry.get_name()
-            
 
         print(Fore.GREEN + "GNames loaded" + END)
 
     def map_objects(self):
         print(Fore.YELLOW + "Mapping objects..." + END)
         gobjects_tarray = self.get_gobjects_tarray()
         for gobject in tqdm(gobjects_tarray.get_items()):
             try:
                 if not gobject.address:
                     continue
                 # if full_name content "Class " then it's a UClass
 
-                full_name = gobject.get_full_name() 
-                
+                full_name = gobject.get_full_name()
+
                 if "Class " in full_name:
                     self.static_classes[full_name] = UClass(gobject.address, sdk=self)
                 elif "Function " in full_name:
-                    self.static_functions[full_name] = UFunction(gobject.address, sdk=self)
+                    self.static_functions[full_name] = UFunction(
+                        gobject.address, sdk=self
+                    )
             except:
                 continue
-        
-        
-        print(Fore.GREEN + "UClasses: " + Fore.BLUE + str(len(self.static_classes)) + END)
-        print(Fore.GREEN + "UFunctions: " + Fore.BLUE + str(len(self.static_functions)) + END)
-    
+
+        print(
+            Fore.GREEN + "UClasses: " + Fore.BLUE + str(len(self.static_classes)) + END
+        )
+        print(
+            Fore.GREEN
+            + "UFunctions: "
+            + Fore.BLUE
+            + str(len(self.static_functions))
+            + END
+        )
+
     # ==========================================================
     # ================ INTERNAL EVENT HANDLING =================
     # ==========================================================
-        
 
     def on_function_called(self, event: EventFunctionHooked):
 
         function_name = event.function.get_full_name()
 
         if function_name == FUNCTION_BOOST_PICKED_UP:
-           
-            pickup = VehiclePickupBoost(int(event.args['caller'], 16), sdk=self)
-    
+
+            pickup = VehiclePickupBoost(int(event.args["caller"], 16), sdk=self)
+
             boostpad = self.field.find_boostpad_from_pickup(pickup)
-      
+
             if boostpad:
                 boostpad.is_active = False
                 boostpad.pickup = pickup
                 boostpad.picked_up_time = time.time()
-                
-                
+
                 # update boostpad position to make sure it's accurate (because the pickup is not always at the same position according the map)
-                
+
                 self.field.update_boostpad_from_pickup(boostpad, pickup)
-              
-                self.event.fire(EventTypes.ON_BOOSTPAD_CHANGED, EventBoostPadChanged(boostpad))
+
+                self.event.fire(
+                    EventTypes.ON_BOOSTPAD_CHANGED, EventBoostPadChanged(boostpad)
+                )
 
         elif function_name == FUNCTION_BOOST_RESPAWN:
-         
-            pickup = VehiclePickupBoost(int(event.args['caller'], 16), sdk=self)
+
+            pickup = VehiclePickupBoost(int(event.args["caller"], 16), sdk=self)
             boostpad = self.field.find_boostpad_from_pickup(pickup)
-            
 
             if boostpad:
                 boostpad.is_active = True
                 boostpad.pickup = pickup
                 boostpad.picked_up_time = None
-                
+
                 self.field.update_boostpad_from_pickup(boostpad, pickup)
 
-                self.event.fire(EventTypes.ON_BOOSTPAD_CHANGED, EventBoostPadChanged(boostpad))
-                
-        
+                self.event.fire(
+                    EventTypes.ON_BOOSTPAD_CHANGED, EventBoostPadChanged(boostpad)
+                )
+
         elif function_name == FUNCTION_PLAYER_TICK:
-            
-            self.event.fire(EventTypes.ON_PLAYER_TICK, EventPlayerTick(event.args['deltatime']))
 
-        elif function_name == FUNCTION_ROUND_ACTIVE_BEGIN:
-            self.event.fire(EventTypes.ON_ROUND_ACTIVE_STATE_CHANGED, EventRoundActiveStateChanged(True))
+            self.event.fire(
+                EventTypes.ON_PLAYER_TICK, EventPlayerTick(event.args["deltatime"])
+            )
 
+        elif function_name == FUNCTION_ROUND_ACTIVE_BEGIN:
+            self.event.fire(
+                EventTypes.ON_ROUND_ACTIVE_STATE_CHANGED,
+                EventRoundActiveStateChanged(True),
+            )
 
         elif function_name == FUNCTION_ROUND_ACTIVE_END:
-            self.event.fire(EventTypes.ON_ROUND_ACTIVE_STATE_CHANGED, EventRoundActiveStateChanged(False))
+            self.event.fire(
+                EventTypes.ON_ROUND_ACTIVE_STATE_CHANGED,
+                EventRoundActiveStateChanged(False),
+            )
 
         elif function_name == FUNCTION_RESET_PICKUPS:
             self.event.fire(EventTypes.ON_RESET_PICKUPS, EventResetPickups())
             self.field.reset_boostpads()
         elif function_name == FUNCTION_GAMEEVENT_BEGIN_PLAY:
             self.event.fire(EventTypes.ON_GAME_EVENT_STARTED, EventGameEventStarted())
         elif function_name == FUNCTION_KEY_PRESS:
-            params = event.args['key_params']
-          
+            params = event.args["key_params"]
+
             data_bytes = bytes.fromhex(params)
-            fname_entry_id = int.from_bytes(data_bytes[4:8], byteorder='little')
+            fname_entry_id = int.from_bytes(data_bytes[4:8], byteorder="little")
             key_name = self.gnames[fname_entry_id]
             ev = EventKeyPressed(data_bytes, key_name)
 
             self.event.fire(EventTypes.ON_KEY_PRESSED, ev)
-        # elif function_name == FUNCTION_GAME_EVENT_ACTIVE_TICK:
 
-        #     viewport = GameViewportClient(int(event.args['caller'], 16), sdk=self)
-        #     self.current_game_event = viewport.get_game_event()
-        #     print(self.current_game_event.is_round_active())
         elif function_name == FUNCTION_GAME_VIEWPORT_CLIENT_TICK:
-            viewport = GameViewportClient(int(event.args['caller'], 16), sdk=self)
+            viewport = GameViewportClient(int(event.args["caller"], 16), sdk=self)
             self.current_game_event = viewport.get_game_event()
 
         elif function_name == FUNCTION_GAME_EVENT_DESTROYED:
             self.current_game_event = None
-            self.event.fire(EventTypes.ON_GAME_EVENT_DESTROYED, EventGameEventDestroyed())
+            self.event.fire(
+                EventTypes.ON_GAME_EVENT_DESTROYED, EventGameEventDestroyed()
+            )
+
+        elif function_name == FUNCTION_EVENT_CHAT_MESSAGE:
+            print("Chat message received")
+            print(event.args)
+            
+            # player_controller = PlayerController(
+            #     int(event.args["player_controller"], 16), sdk=self
+            # )
+            # message = event.args["message"]
+            # preset = event.args["preset"]   
+
+            # self.event.fire(
+            #     EventTypes.ON_CHAT_MESSAGE,
+            #     EventChatMessage(player_controller, message, preset)
+            # )
+            
 
-   
     # ==========================================================
     # ===================== DEBUG METHODS ======================
     # ==========================================================
 
 
     def scan_functions(self, duration=10):
         print("Scanning functions...")
-        
         self.scan_response_received_event.clear()
         self.frida_script.post({"type": "scan_functions", "duration": duration})
         received = self.scan_response_received_event.wait(duration + 10)
         if received:
+            
             print("Scan result received.")
+
+            headers = ["Count", "Address", "ThreadId", "Function Name"]
+            table = []
+            for func in self.scan_result:
+                count = Fore.GREEN + str(func.get("count")) + Style.RESET_ALL
+                address = Fore.BLUE + func.get("address") + Style.RESET_ALL
+                thread_id = Fore.YELLOW + str(func.get("thread_id")) + Style.RESET_ALL
+                name = Fore.MAGENTA + func.get("name") + Style.RESET_ALL
+                table.append([count, address, thread_id, name])
+
+            print(tabulate(table, headers, tablefmt="fancy_grid"))
+            print("Unique functions scanned: " + str(len(self.scan_result)))
             return self.scan_result
         else:
             print("Scan timed out.")
             return None
 
     # ==========================================================
     # ================ EXTRACTION METHODS ======================
@@ -428,106 +543,176 @@
         print("Extracting classes...")
         filename = "classes.txt"
         with open(filename, "w") as file:
             for class_name, class_object in self.static_classes.items():
                 file.write(hex(class_object.address) + " : " + class_name + "\n")
         print("Classes extracted to " + filename)
 
-
     def extract_functions(self):
         # write all functions name to a file with their address
         print("Extracting functions...")
         filename = "functions.txt"
         with open(filename, "w") as file:
             for function_name, function_object in self.static_functions.items():
                 file.write(hex(function_object.address) + " : " + function_name + "\n")
         print("Functions extracted to " + filename)
 
     # ==========================================================
     # ================ FRIDA HOOKING METHODS ===================
     # ==========================================================
 
     def on_frida_message(self, message, data):
-  
-        if message['type'] == 'send':
-            payload = message['payload']
-            if payload.get('type') == 'hooked_function_fired':
-                function = UFunction(int(payload.get('address'), 16), sdk=self)
-                
-                self.event.fire(EventTypes.ON_HOOKED_FUNCTION, EventFunctionHooked(function, payload.get('args')))
-        
-            if payload.get('type') == 'scan_result':
-                for f in payload.get('functions'):
-                    function_address = int(f, 16)
-                    self.scan_result.append(UFunction(function_address, sdk=self))
-                    self.scan_response_received_event.set()
-            elif payload.get('type') == 'log':
-                print(Fore.MAGENTA + "Frida log: " + END + payload.get('message'))
-           
+
+        if message["type"] == "send":
+            payload = message["payload"]
+            if payload.get("type") == "hooked_function_fired":
+                function = UFunction(int(payload.get("address"), 16), sdk=self)
+
+                self.event.fire(
+                    EventTypes.ON_HOOKED_FUNCTION_CALLED,
+                    EventFunctionHooked(function, payload.get("args")),
+                )
+
+            if payload.get("type") == "scan_result":
+                for f in payload.get("functions"):
+                    ufunction = UFunction(int(f.get("address"), 16), sdk=self)
+                    self.scan_result.append({
+                        "address": f.get("address"),
+                        "object": ufunction,
+                        "name": ufunction.get_full_name(),
+                        "count": f.get("count"),
+                        "thread_id": f.get("thread_id")
+                    })
+                    
+                self.scan_response_received_event.set()
+            elif payload.get("type") == "log":
+                print(Fore.MAGENTA + "Frida log: " + END + payload.get("message"))
 
         else:
             print("Received message:", message)
 
-    
     def hook_function(self, function_name, args_map=[]):
 
         function_address = self.find_static_function(function_name).address
         if function_address:
-            self.frida_script.post({"type": "hook_function", "address": function_address, "name": function_name, "args_map": args_map})
+            self.frida_script.post(
+                {
+                    "type": "hook_function",
+                    "address": function_address,
+                    "name": function_name,
+                    "args_map": args_map,
+                }
+            )
         else:
             pass
 
     def get_process_event_address(self):
         core_object = self.find_static_class(CLASS_CORE_OBJECT)
         if core_object:
             print("Core Object Address: " + hex(core_object.address))
             vtable_address = self.pm.read_ulonglong(core_object.address)
             return self.pm.read_ulonglong(vtable_address + (0x8 * 67))
         return None
 
-
     # ==========================================================
     # ===================== Accessors ==========================
     # ==========================================================
-    
+
     def get_game_event(self):
         return self.current_game_event
-    
+
     def get_field(self):
         return self.field
-    
 
     def get_gobjects_tarray(self):
-        return TArray(self.pm.base_address + self.g_object_offset, UObject, sdk=self)  # Remplacer UObject par la classe appropriée
+        return TArray(
+            self.pm.base_address + self.g_object_offset, UObject, sdk=self
+        )  # Remplacer UObject par la classe appropriée
 
     def get_gnames_entries_tarray(self):
         return TArray(self.pm.base_address + self.g_names_offset, FNameEntry, sdk=self)
-    
 
     def get_pm(self):
         return self.pm
-    
-    
+
     # ==========================================================
     # =====================   Methods  =========================
     # ==========================================================
-    
 
     def get_name(self, index):
         return self.gnames.get(index)
-        
-        
+
     def find_static_function(self, function_name):
         return self.static_functions.get(function_name)
-    
+
     def find_static_class(self, class_name):
         return self.static_classes.get(class_name)
-    
-    
+
     # Use to read cheat engine pointer offsets if needed
     def get_offsets_final_address(self, offsets):
         if self.pm != None:
             base_address = self.pm.base_address
             for offset in offsets:
                 base_address = self.pm.read_ulonglong(base_address + offset)
             return base_address
-        
+
+    def create_callable_function(self, function_name, arg_types=None):
+        TYPE_SIZES = {
+            "float": 4,
+            "int": 4,
+            "uint": 4,
+            "uint32": 4,
+            "uint8": 1,
+            "pointer": 8,  # 64 bits
+            "bool": 1,  # Booléen pour les flags, utilisé souvent comme uint8_t,
+            "fstring": 16,  # FString est une structure de 16 octets
+        }
+        function = self.find_static_function(function_name)
+        if function:
+
+            def call_function(caller: UObject, **kwargs):
+                args = []
+                total_size = 0
+                if arg_types:
+                    # Préparer les arguments pour Frida
+                    for arg_name, arg_type in arg_types.items():
+
+                        if arg_type == "pointer":
+                            if isinstance(kwargs.get(arg_name), UObject):
+                                value = kwargs.get(arg_name).address
+                                size = TYPE_SIZES[arg_type]
+                            else:
+                                raise Exception("Argument must be a UObject instance")
+                        elif arg_type == "string":
+
+                            # check if the string is a string
+                            if isinstance(kwargs.get(arg_name), str):
+                                value = kwargs.get(arg_name)
+                                size = len(kwargs.get(arg_name)) + 1
+                            else:
+                                raise Exception("Argument must be a string")
+                        else:
+                            value = kwargs.get(arg_name)
+                            size = TYPE_SIZES[arg_type]
+                        total_size += size
+                        args.append(
+                            {
+                                "name": arg_name,
+                                "type": arg_type,
+                                "value": value,
+                                "size": size,
+                            }
+                        )
+
+                self.frida_script.post(
+                    {
+                        "type": "call_function",
+                        "function_address": function.address,
+                        "caller_address": caller.address,
+                        "args": args,
+                        "total_size": total_size,
+                    }
+                )
+
+            return call_function
+        else:
+            raise Exception("Function not found")
```

### Comparing `rlsdk_python-0.4.2/PKG-INFO` & `rlsdk_python-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: rlsdk_python
-Version: 0.4.2
+Version: 0.5.0
 Summary: 
 Author: MarlburroW
 Author-email: nik0o@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pymem (>=1.13.1,<2.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: frida (>=16.2.1,<17.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # RLSDK Python
 
 This is reverse engineered python SDK package aiming to read data from RocketLeague.exe.
```

