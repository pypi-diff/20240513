# Comparing `tmp/IvmInstruments-0.2.0.tar.gz` & `tmp/ivminstruments-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IvmInstruments-0.2.0.tar", last modified: Mon May 13 13:39:59 2024, max compression
+gzip compressed data, was "ivminstruments-0.2.2.tar", last modified: Mon May 13 14:07:58 2024, max compression
```

## Comparing `IvmInstruments-0.2.0.tar` & `ivminstruments-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 13:39:59.783496 IvmInstruments-0.2.0/
-drwxrwxrwx   0        0        0        0 2024-05-13 13:39:59.759801 IvmInstruments-0.2.0/Instruments/
--rw-rw-rw-   0        0        0     4894 2024-05-07 08:11:02.000000 IvmInstruments-0.2.0/Instruments/DigitalScope.py
--rw-rw-rw-   0        0        0    23545 2024-05-07 08:11:02.000000 IvmInstruments-0.2.0/Instruments/KeySight_N670x.py
--rw-rw-rw-   0        0        0     2777 2024-05-07 08:11:02.000000 IvmInstruments-0.2.0/Instruments/KeySight_RP7954.py
--rw-rw-rw-   0        0        0    12743 2024-05-07 08:11:02.000000 IvmInstruments-0.2.0/Instruments/Keysight_34461.py
--rw-rw-rw-   0        0        0     3139 2024-05-07 08:11:02.000000 IvmInstruments-0.2.0/Instruments/Keysight_E362x.py
--rw-rw-rw-   0        0        0      214 2024-05-13 10:49:43.000000 IvmInstruments-0.2.0/Instruments/__init__.py
--rw-rw-rw-   0        0        0     5261 2024-05-09 13:15:43.000000 IvmInstruments-0.2.0/Instruments/multimeter.py
-drwxrwxrwx   0        0        0        0 2024-05-13 13:39:59.779016 IvmInstruments-0.2.0/IvmInstruments.egg-info/
--rw-rw-rw-   0        0        0      140 2024-05-13 13:39:59.000000 IvmInstruments-0.2.0/IvmInstruments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2024-05-13 13:39:59.000000 IvmInstruments-0.2.0/IvmInstruments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 13:39:59.000000 IvmInstruments-0.2.0/IvmInstruments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-13 13:39:59.000000 IvmInstruments-0.2.0/IvmInstruments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1103 2024-05-09 13:09:14.000000 IvmInstruments-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      140 2024-05-13 13:39:59.781487 IvmInstruments-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-13 13:39:59.784866 IvmInstruments-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      275 2024-05-13 13:39:55.000000 IvmInstruments-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:07:58.573287 ivminstruments-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:07:58.573287 ivminstruments-0.2.2/Instruments/
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-13 14:07:44.000000 ivminstruments-0.2.2/Instruments/DigitalScope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23077 2024-05-13 14:07:44.000000 ivminstruments-0.2.2/Instruments/KeySight_N670x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-13 14:07:44.000000 ivminstruments-0.2.2/Instruments/KeySight_RP7954.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-05-13 14:07:44.000000 ivminstruments-0.2.2/Instruments/Keysight_34461.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-13 14:07:44.000000 ivminstruments-0.2.2/Instruments/Keysight_E362x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 14:07:44.000000 ivminstruments-0.2.2/Instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-13 14:07:44.000000 ivminstruments-0.2.2/Instruments/multimeter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:07:58.573287 ivminstruments-0.2.2/IvmInstruments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-13 14:07:58.000000 ivminstruments-0.2.2/IvmInstruments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-13 14:07:58.000000 ivminstruments-0.2.2/IvmInstruments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:07:58.000000 ivminstruments-0.2.2/IvmInstruments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 14:07:58.000000 ivminstruments-0.2.2/IvmInstruments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-13 14:07:44.000000 ivminstruments-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-13 14:07:58.573287 ivminstruments-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 14:07:44.000000 ivminstruments-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:07:58.573287 ivminstruments-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-13 14:07:44.000000 ivminstruments-0.2.2/setup.py
```

### Comparing `IvmInstruments-0.2.0/Instruments/DigitalScope.py` & `ivminstruments-0.2.2/Instruments/DigitalScope.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-import time
-
-import pyvisa as visa
-from pyvisa.attributes import *
-from pyvisa.constants import *
-
-class dpo_2014B:
-
-    def __init__(self, usb_id):
-        rm = visa.ResourceManager()
-        # rm.list_resources()
-        self.scope = rm.open_resource(usb_id)
-        self.scope.read_termination = '\n'
-        self.scope.write_termination = '\n'
-
-        # self.reset()
-
-    def get_IDN(self):
-        return (self.scope.query('*IDN?'))
-
-    def reset(self):
-        self.scope.write('*RST')     
-
-    def get_error(self):
-        return self.scope.query('SYST:ERR?')  
-    
-    def meas_Freq(self,Meas='MEAS1'):
-        self.scope.write(f'MEASUrement:{Meas}:TYPE FREQUENCY')
-        return float(self.scope.query('MEASUrement:MEAS1:VALUE?'))
-    
-    def set_trigger__mode(self,mode='AUTO'):
-        # TRIGger:MAIn:MODe { AUTO | NORMal }
-        self.scope.write(f'TRIGger:MAIn:MODe {mode}')
-
-    def init_scopePosEdge__Trigger(self,channel='CH1'):
-        self.scope.write(':TRIG:A:TYP EDG')
-        self.scope.write(f':TRIG:A:EDGE:SOU {channel}')
-        self.scope.write(':TRIG:A:EDGE:SLO RIS')
-        self.scope.write('ACQUIRE:STOPAFTER SEQUENCE')
-        # self.scope.write('ACTONEV:EVENTTYP TRIG')
-        # self.scope.write(':ACTONEV:NUMACQ 1')
-        # self.scope.write(':ACTONEV:REPEATC 1')
-        
-    def init_scopeNegEdge__Trigger(self,channel='CH1'):
-        self.scope.write(':TRIG:A:TYP EDG')
-        self.scope.write(f':TRIG:A:EDGE:SOU {channel}')
-        self.scope.write(':TRIG:A:EDGE:SLO FALL')
-        self.scope.write('ACQUIRE:STOPAFTER SEQUENCE')
-        # self.scope.write('ACTONEV:EVENTTYP TRIG')
-        # self.scope.write(':ACTONEV:NUMACQ 1')
-        # self.scope.write(':ACTONEV:REPEATC 1')
-
-    def single_Trigger__ON(self):
-        self.scope.write('ACQuire:STATE ON')
-    def single_Trigger__RUN(self):
-        self.scope.write('ACQuire:STATE RUN')
-    def set_Channel__VScale(self,channel=1,scale=0.05):
-        self.scope.write(f'CH{str(channel)}:SCAle {str(scale)}')
-    def get_Channel__VScale(self,channel=1):
-        return float(self.scope.query(f'CH{str(channel)}:SCAle?'))
-    def set_HScale(self,scale='400E-9'):
-        self.scope.write(f'HORizontal:MAIn:SCAle {scale}')
-    def get_HScale(self):
-        return float(self.scope.query(f'HORizontal:MAIn:SCAle'))
-    
-    def set_autoSet(self):
-        self.scope.write('AUTOSet EXECute')
-
-    @property
-    def acquireState(self):
-        if float(self.scope.query('ACQuire:STATE?')) == 1.0:
-            State = True 
-        else :
-            State = False 
-
-        return State
-    
-    def get_trigger__level(self):
-        return float(self.scope.query('TRIGger:MAIn:LEVel?')) 
-    
-    def set_trigger__level(self,level):
-        self.scope.write(f'TRIGger:MAIn:LEVel {str(level)}')
-
-    def scopeTrigger_Acquire(self,channel='CH1'):
-        self.scope.write('ACQUIRE:STATE OFF')
-        self.scope.write(f'SELECT:{channel} ON')
-        self.scope.write('ACQUIRE:MODE SAMPLE')
-        self.scope.write('ACQUIRE:STOPAFTER SEQUENCE')
-        # /* Acquire waveform data */
-        self.scope.write('ACQUIRE:STATE ON')
-        # /* Set up the measurement parameters */
-        self.scope.write('MEASUREMENT:IMMED:TYPE FREQUENCY')
-        self.scope.write(f'MEASUREMENT:IMMED:SOURCE {channel}')
-        # /* Wait until the acquisition is complete before taking
-        # the measurement */
-        # While BUSY?
-    @property
-    def scopeAcquire_BUSY(self):
-        return int(float(self.scope.query('BUSY?')))
-
-    def Meas_Amp(self,channel='CH1',Meas='MEAS1'):
-        # self.scope.write('MEASUREMENT:IMMED:TYPE AMPLITUDE')
-        # self.scope.write(f'MEASUREMENT:IMMED:SOURCE {channel}')
-        self.scope.write(f'MEASUrement:{Meas}:TYPE AMPLITUDE')
-        return float(self.scope.query(f'MEASUrement:{Meas}:VALUE?'))
-    
-    def Meas_Mean(self,channel='CH1',Meas='MEAS1'):
-        # self.scope.write('MEASUREMENT:IMMED:TYPE AMPLITUDE')
-        # self.scope.write(f'MEASUREMENT:IMMED:SOURCE {channel}')
-        self.scope.write(f'MEASUrement:{Meas}:TYPE MEAN')
-        return float(self.scope.query(f'MEASUrement:{Meas}:VALUE?'))
-    
-if __name__ == '__main__':
-    scope = dpo_2014B('USB0::0x0699::0x0456::C014546::INSTR')
-    # print(scope.meas_Freq())
-    # print(scope.get_error())
-    # scope.set_trigger__mode(mode='AUTO')
-    # scope.scope.write('ACQUIRE:STATE OFF')
-    scope.set_trigger__mode(mode='NORM')
-    # time.sleep(1)
-    scope.init_scopePosEdge__Trigger(channel='CH3')
-    # time.sleep(1)
-    scope.single_Trigger__ON()
-    time.sleep(1)
-    # print('State',scope.acquireState)
-    while scope.acquireState == True :
-       print('rotate')
-    # time.sleep(1)
-    scope.scope.write('ACQUIRE:STATE OFF')
-    # scope.single_Trigger__RUN()
-
+import time
+
+import pyvisa as visa
+from pyvisa.attributes import *
+from pyvisa.constants import *
+
+class dpo_2014B:
+
+    def __init__(self, usb_id):
+        rm = visa.ResourceManager()
+        # rm.list_resources()
+        self.scope = rm.open_resource(usb_id)
+        self.scope.read_termination = '\n'
+        self.scope.write_termination = '\n'
+
+        # self.reset()
+
+    def get_IDN(self):
+        return (self.scope.query('*IDN?'))
+
+    def reset(self):
+        self.scope.write('*RST')     
+
+    def get_error(self):
+        return self.scope.query('SYST:ERR?')  
+    
+    def meas_Freq(self,Meas='MEAS1'):
+        self.scope.write(f'MEASUrement:{Meas}:TYPE FREQUENCY')
+        return float(self.scope.query('MEASUrement:MEAS1:VALUE?'))
+    
+    def set_trigger__mode(self,mode='AUTO'):
+        # TRIGger:MAIn:MODe { AUTO | NORMal }
+        self.scope.write(f'TRIGger:MAIn:MODe {mode}')
+
+    def init_scopePosEdge__Trigger(self,channel='CH1'):
+        self.scope.write(':TRIG:A:TYP EDG')
+        self.scope.write(f':TRIG:A:EDGE:SOU {channel}')
+        self.scope.write(':TRIG:A:EDGE:SLO RIS')
+        self.scope.write('ACQUIRE:STOPAFTER SEQUENCE')
+        # self.scope.write('ACTONEV:EVENTTYP TRIG')
+        # self.scope.write(':ACTONEV:NUMACQ 1')
+        # self.scope.write(':ACTONEV:REPEATC 1')
+        
+    def init_scopeNegEdge__Trigger(self,channel='CH1'):
+        self.scope.write(':TRIG:A:TYP EDG')
+        self.scope.write(f':TRIG:A:EDGE:SOU {channel}')
+        self.scope.write(':TRIG:A:EDGE:SLO FALL')
+        self.scope.write('ACQUIRE:STOPAFTER SEQUENCE')
+        # self.scope.write('ACTONEV:EVENTTYP TRIG')
+        # self.scope.write(':ACTONEV:NUMACQ 1')
+        # self.scope.write(':ACTONEV:REPEATC 1')
+
+    def single_Trigger__ON(self):
+        self.scope.write('ACQuire:STATE ON')
+    def single_Trigger__RUN(self):
+        self.scope.write('ACQuire:STATE RUN')
+    def set_Channel__VScale(self,channel=1,scale=0.05):
+        self.scope.write(f'CH{str(channel)}:SCAle {str(scale)}')
+    def get_Channel__VScale(self,channel=1):
+        return float(self.scope.query(f'CH{str(channel)}:SCAle?'))
+    def set_HScale(self,scale='400E-9'):
+        self.scope.write(f'HORizontal:MAIn:SCAle {scale}')
+    def get_HScale(self):
+        return float(self.scope.query(f'HORizontal:MAIn:SCAle'))
+    
+    def set_autoSet(self):
+        self.scope.write('AUTOSet EXECute')
+
+    @property
+    def acquireState(self):
+        if float(self.scope.query('ACQuire:STATE?')) == 1.0:
+            State = True 
+        else :
+            State = False 
+
+        return State
+    
+    def get_trigger__level(self):
+        return float(self.scope.query('TRIGger:MAIn:LEVel?')) 
+    
+    def set_trigger__level(self,level):
+        self.scope.write(f'TRIGger:MAIn:LEVel {str(level)}')
+
+    def scopeTrigger_Acquire(self,channel='CH1'):
+        self.scope.write('ACQUIRE:STATE OFF')
+        self.scope.write(f'SELECT:{channel} ON')
+        self.scope.write('ACQUIRE:MODE SAMPLE')
+        self.scope.write('ACQUIRE:STOPAFTER SEQUENCE')
+        # /* Acquire waveform data */
+        self.scope.write('ACQUIRE:STATE ON')
+        # /* Set up the measurement parameters */
+        self.scope.write('MEASUREMENT:IMMED:TYPE FREQUENCY')
+        self.scope.write(f'MEASUREMENT:IMMED:SOURCE {channel}')
+        # /* Wait until the acquisition is complete before taking
+        # the measurement */
+        # While BUSY?
+    @property
+    def scopeAcquire_BUSY(self):
+        return int(float(self.scope.query('BUSY?')))
+
+    def Meas_Amp(self,channel='CH1',Meas='MEAS1'):
+        # self.scope.write('MEASUREMENT:IMMED:TYPE AMPLITUDE')
+        # self.scope.write(f'MEASUREMENT:IMMED:SOURCE {channel}')
+        self.scope.write(f'MEASUrement:{Meas}:TYPE AMPLITUDE')
+        return float(self.scope.query(f'MEASUrement:{Meas}:VALUE?'))
+    
+    def Meas_Mean(self,channel='CH1',Meas='MEAS1'):
+        # self.scope.write('MEASUREMENT:IMMED:TYPE AMPLITUDE')
+        # self.scope.write(f'MEASUREMENT:IMMED:SOURCE {channel}')
+        self.scope.write(f'MEASUrement:{Meas}:TYPE MEAN')
+        return float(self.scope.query(f'MEASUrement:{Meas}:VALUE?'))
+    
+if __name__ == '__main__':
+    scope = dpo_2014B('USB0::0x0699::0x0456::C014546::INSTR')
+    # print(scope.meas_Freq())
+    # print(scope.get_error())
+    # scope.set_trigger__mode(mode='AUTO')
+    # scope.scope.write('ACQUIRE:STATE OFF')
+    scope.set_trigger__mode(mode='NORM')
+    # time.sleep(1)
+    scope.init_scopePosEdge__Trigger(channel='CH3')
+    # time.sleep(1)
+    scope.single_Trigger__ON()
+    time.sleep(1)
+    # print('State',scope.acquireState)
+    while scope.acquireState == True :
+       print('rotate')
+    # time.sleep(1)
+    scope.scope.write('ACQUIRE:STATE OFF')
+    # scope.single_Trigger__RUN()
+
```

### Comparing `IvmInstruments-0.2.0/Instruments/KeySight_N670x.py` & `ivminstruments-0.2.2/Instruments/KeySight_N670x.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,469 +1,469 @@
-import time 
-import pyvisa as visa
-from pyvisa.attributes import *
-from pyvisa.constants import *
-
-# ('USB0::0x2A8D::0x0F02::MY56002702::INSTR', 'USB0::0x0699::0x0401::C020132::INSTR', 'TCPIP0::172.16.10.29::inst0::INSTR', 'GPIB0::6::INSTR')
-class N670x:
-
-    def __init__(self,port='USB0::0x2A8D::0x0F02::MY56002702::INSTR') -> None:
-        rm = visa.ResourceManager()
-        rm.list_resources()
-        self.my_instr = rm.open_resource(port)
-        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_BAUD, 9600)
-        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_DATA_BITS, 8)
-        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_STOP_BITS, VI_ASRL_STOP_TWO)
-        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_PARITY, visa.constants.VI_ASRL_PAR_NONE)
-        self.my_instr.read_termination = '\n'
-        self.my_instr.write_termination = '\n'
-
-        self.channel = {
-                            1:"OUT1",
-                            2:"OUT2",
-                            3:"OUT3",
-                            4:"OUT4",
-                        }
-
-        self.erroMSG = {
-            -100 :"Command error [generic command error]",
-            -101 :"Invalid character",
-            -102 :"Syntax error [unrecognized command or data type]",
-            -103 :"Invalid separator [illegal character encountered in place of separator]",
-            -104 :"Data type error [e.g., “numeric or string expected, got block date”]",
-            -105 :"GET not allowed [ <GET> inside a program message]",
-            -108 :"Parameter not allowed [too many parameters]",
-            -109 :"Missing parameter [too few parameters]",
-            -112 :"Program mnemonic too long [maximum 12 characters]",
-            -113 :"Undefined header [syntactical correct but not defined for this device]",
-            -121 :"Invalid character in number [e.g. alpha in decimal data, etc.]",
-            -123 :"Exponent too large [ numeric overflow; exponent magnitude >32000]",
-            -124 :"Too many digits [number too long; more than 255 digits received]",
-            -128 :"Numeric data not allowed [numeric data not accepted where positioned]",
-            -131 :"Invalid suffix [unrecognized suffix, or suffix not appropriate]",
-            -138 :"Suffix not allowed [numeric element does not allow suffixes]"
-        }
-        
-    # ! SYST:REM system remote connection 
-    # * *IDN?' Instrument id Query 
-    # ? provide the minimum sleep time(1 Sec) to configure for the remote connection time.sleep(1)
-    def get_IDN(self):
-        self.my_instr.write('SYST:REM') 
-        time.sleep(1)
-        return (self.my_instr.query('*IDN?'))
-        
-    
-    # * Rest the instrument 
-    def reset(self):
-        self.my_instr.write('*RST')  
-
-    # * switch off the Channle 
-    def outp_OFF(self,channel:int):
-        self.my_instr.write(f'OUTP OFF,(@{str(channel)})')  
-
-    # * Switch on the channel 
-    def outp_ON(self,channel:int):
-        self.my_instr.write(f'OUTP ON,(@{str(channel)})')  
-
-    # * Error Que Clear
-    def clear_errors(self):
-        self.my_instr.write('*CLS')  
-
-    # * Installed Options in the Channl
-    def modelNumber(self,channel:int):
-        return self.my_instr.query(f'SYST:CHAN:MOD? (@{str(channel)})')
-    
-    # * Serial number of the channel
-    def serialNumber(self,channel:int):
-        return self.my_instr.query(f'SYST:CHAN:SER? (@{str(channel)})')
-    
-    # * installed Options in the channel
-    def installedOptions(self,channel:int):
-        return self.my_instr.query(f'SYST:CHAN:OPT? (@{str(channel)})')
-
-    # Returns the error number and error string
-    def errorLog(self):
-        return (self.my_instr.query('SYST:ERR?'))
-
-    # * Multi channel voltage set method 
-    # ! first argument is the channel number shuold be in int  channel Number 1-4
-    # ! voltage must be in the float ex: 1.4 
-    # ? default it will provide the fist chanlle Voltage 
-    # def setVoltage(self, channel:int, voltage:float):
-    #     if channel in self.channel.keys() :
-    #         ch = self.channel.get(channel)
-    #     else:
-    #         ch = self.channel.get(1)
-    #     command = 'INST:SEL ' +  ch
-    #     self.my_instr.write(command)   
-    #     command = 'VOLT ' + str(voltage) 
-    #     self.my_instr.write(command)  
-
-    # * Multi channel voltage set method 
-    # ! first argument is the channel number shuold be in int  channel Number 1-4
-    # ! current must be in the float ex: 1.4 
-    # ? default it will provide the fist chanlle current 
-    # def setCurrent(self, channel:int, current:float):
-    #     if channel in self.channel.keys() :
-    #         ch = self.channel.get(channel)
-    #     else:
-    #         ch = self.channel.get(1)
-    #     command = 'INST:SEL ' +  ch
-    #     self.my_instr.write(command)   
-    #     command = 'CURR ' + str(current) 
-    #     self.my_instr.write(command)  
-
-    def setCurrent(self, channel:int, current:float):
-        self.my_instr.write(f'CURR {current},(@{channel})')
-
-    def setVoltage(self, channel:int, voltage:float):
-        self.my_instr.write(f'VOLT {voltage},(@{channel})')
-    # ? get the output status 
-    def getOutStatus(self):  
-        # time.sleep(0.2)
-        return self.my_instr.query('OUTP:STAT?')  
-    
-    # * set the Voltage Range of the channel 
-    # * Channel Number must be int it is between 1-4 
-    # * Voltage range must be float
-    def setRange_Voltage(self,channel:int,voltageRange:float):
-        self.my_instr.write(f'VOLT:RANG {str(voltageRange)},(@{str(channel)})')
-
-    # * set the Current Range of the channel 
-    # * Channel Number must be int it is between 1-4 
-    # * Current range must be float
-    def setRange_Current(self,channel:int,voltageRange:float):
-        self.my_instr.write(f'CURR:RANG {str(voltageRange)},(@{str(channel)})')
-
-
-    # * set the channel to the current mode =
-    # * Channel Number must be int it is between 1-4 
-    def setCurrentMode(self,channel:int):
-        self.my_instr.write(f'OUTP:PMOD CURR,(@{str(channel)})')
-        
-    # * set the channel to the Voltage mode =
-    # * Channel Number must be int it is between 1-4 
-    def setVoltageMode(self,channel:int):
-        self.my_instr.write(f'OUTP:PMOD VOLT,(@{str(channel)})')
-
-    # * To reverse the relay polarity on units with Option 760
-    # * Channel Number must be int it is between 1-4 
-    def setReverseRelay_Polarity(self,channel:int):
-        self.my_instr.write(f'OUTP:REL:POL REV,(@{str(channel)})')
-
-    # * To return the relay polarity to normal
-    # * Channel Number must be int it is between 1-4 
-    def setNormalRelay_Polarity(self,channel:int):
-        self.my_instr.write(f'OUTP:REL:POL NORM,(@{str(channel)})')
-
-    # To set the positive current limit of output ex:1 to 1 A:
-    def setCurrent_Positive_Limit(self,channel:int,current:float):
-        self.my_instr.write(f'CURR:LIM {str(current)},(@{str(channel)})')
-
-    # To set the negative current limit, you must first turn limit coupling
-    # (tracking) off. Then set the negative current limit
-    def setCurrent_Negative_Limit(self,channel:int,current:float):
-        self.my_instr.write(f'CURR:LIM:COUP OFF,(@{str(channel)})')
-        self.my_instr.write(f'CURR:LIM:NEG {str(current)},(@{str(channel)})')
-
-    # To set the voltage priority mode:
-    def setVoltage_Priority(self,channel:int):
-        self.my_instr.write(f'FUNC VOLT,(@{str(channel)})')
-
-    # To set the Current priority mode:
-    def setCurrent_Priority(self,channel:int):
-        self.my_instr.write(f'FUNC CURR,(@{str(channel)})')
-
-    # TTo program turn-on delay 
-    def setTurn_ON_Delay(self,channel:int,delay:float):
-        self.my_instr.write(f'OUTP:DEL:RISE  {str(delay)},(@{str(channel)})')
-
-    # TTo program turn-on delay 
-    def setTurn_OFF_Delay(self,channel:int,delay:float):
-        self.my_instr.write(f'OUTP:DEL:FALL  {str(delay)},(@{str(channel)})')
-
-
-    # # ! Coupling of the channel is pending 
-    # !!!
-    # !!!
-
-
-
-    # To program the OVP level for outputs
-    def setOVP_Protection(self,channel:int,OVP:float):
-        self.my_instr.write(f'VOLT:PROT  {str(OVP)},(@{str(channel)})')
-
-    # To enable OCP for outputs 
-    def setOCP_Protection(self,channel:int,OCP:float):
-        self.my_instr.write(f'CURR:PROT:STAT  {str(OCP)},(@{str(channel)})')
-
-    # To specify a 10 millisecond delay for the OCP
-    def setOCP_Delay(self,channel:int,delay:float):
-        self.my_instr.write(f'CURR:PROT:DEL  {str(delay)},(@{str(channel)})')
-    
-    # To enable output protection coupling
-    def setOutput_Protection_Coupling_ON(self):
-        self.my_instr.write('OUTP:PROT:COUP ON')
-
-
-    def setOutput_Current_Protection_ON(self,channel:int):
-        self.my_instr.write(f'CURR:PROT:STAT ON,(@{str(channel)})')
-
-
-    def setOutput_Current_Protection_OFF(self,channel:int):
-        self.my_instr.write(f'CURR:PROT:STAT OFF,(@{str(channel)})')
-
-
-    def setOutput_Voltage_Protection_ON(self,channel:int):
-        self.my_instr.write(f'VOLT:PROT:STAT ON,(@{str(channel)})')
-
-    def setOutput_Voltage_Protection_OFF(self,channel:int):
-        self.my_instr.write(f'VOLT:PROT:STAT OFF,(@{str(channel)})')
-
-    # To clear an output protection fault
-    def clearOutput_Protection_Clear(self,channel:int):
-        self.my_instr.write(f'OUTP:PROT:CLE (@{str(channel)})')
-
-    def protection_Status_Current(self):
-        return self.my_instr.query('CURRent:PROTection:STATe?')
-
-    def protection_Status_Voltage(self):
-        return self.my_instr.query('VOLTage:PROTection:STATe?')
-
-
-    
-    def arbFunction_Priority__Voltage(self,channel:int):
-        self.my_instr.write(f'ARB:FUNC:TYPE VOLT,(@{str(channel)})')
-
-    def arbFunction_Sequence__Set(self,channel:int):
-        self.my_instr.write(f'ARB:FUNC:SHAP SEQ,(@{str(channel)})')
-
-    def arbFunction_Sequence__Reset(self,channel:int):
-        self.my_instr.write(f'ARB:SEQ:RES(@{str(channel)})')
-    
-    def arbSet_Sequence_Waveform(self,channel:int):
-        self.arbFunction_Priority__Voltage(channel)
-        self.arbFunction_Sequence__Set(channel)
-
-    def arb_Pulse__Voltage(self,channel:int,initial_Voltage:float,end_Voltage:float,initial_Time:float,top_Time:float,end_Time:float):
-        self.my_instr.write(f'ARB:VOLT:PULS:STAR  {str(initial_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:PULS:TOP  {str(end_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:PULS:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:PULS:TOP:TIM  {str(top_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:PULS:END:TIM   {str(end_Time)},(@{str(channel)})')
-    def arb_Pulse__Current(self,channel:int,initial_Current:float,end_Current:float,initial_Time:float,top_Time:float,end_Time:float):
-        self.my_instr.write(f'ARB:CURR:PULS:STAR  {str(initial_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:PULS:TOP  {str(end_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:PULS:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:PULS:TOP:TIM  {str(top_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:PULS:END:TIM   {str(end_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:TERM:LAST OFF,(@{str(channel)})')
-        self.my_instr.write(f'TRIG:ARB:SOUR BUS')
-        self.my_instr.write(f'INIT:TRAN(@{str(channel)})')
-    
-    # The parameter setting remains at the last Arb value after the Arb completes.
-    def arbLast_Value_ON(self,channel:int):
-        self.my_instr.write(f'ARB:TERM:LAST ON,(@{str(channel)})')
-
-    # The parameter setting returns to the DC value that was in effect prior to the Arb
-    def arbLast_Value_OFF(self,channel:int):
-        self.my_instr.write(f'ARB:TERM:LAST OFF,(@{str(channel)})')
-    
-    def arb_Trigger(self):
-        self.my_instr.write('*TRG')
-
-    def arb_Step__Current(self,channel:int,initial_Current:float,end_Current:float,initial_Time:float):
-        self.my_instr.write(f'ARB:CURR:STEP:STAR  {str(initial_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:STEP:END  {str(end_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:STEP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-
-    def arb_Step__Voltage(self,channel:int,initial_Voltage:float,end_Voltage:float,initial_Time:float):
-        self.my_instr.write(f'ARB:VOLT:STEP:STAR  {str(initial_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:STEP:END  {str(end_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:STEP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-    
-    def arb_Ramp__Voltage(self,channel:int,initial_Voltage:float,end_Voltage:float,initial_Time:float,raise_Time:float,end_Time:float):
-        self.my_instr.write(f'ARB:VOLT:RAMP:STAR  {str(initial_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:RAMP:END  {str(end_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:RAMP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:RAMP:END:TIM  {str(end_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:RAMP:RTIM  {str(raise_Time)},(@{str(channel)})')
-    
-    def arb_Ramp__Current(self,channel:int,initial_Current:float,end_Current:float,initial_Time:float,raise_Time:float,end_Time:float):
-        self.my_instr.write(f'ARB:CURR:RAMP:STAR  {str(initial_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:RAMP:END  {str(end_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:RAMP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:RAMP:END:TIM  {str(end_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:RAMP:RTIM  {str(raise_Time)},(@{str(channel)})')
-    
-    def arb_Staircase__Voltage(self,channel:int,steps:int,initial_Voltage:float,end_Voltage:float,initial_Time:float,raise_Time:float,end_Time:float):
-        self.my_instr.write(f'ARB:VOLT:STA:STAR  {str(initial_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:STA:END  {str(end_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:STA:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:STA:END:TIM  {str(end_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:STA:TIM  {str(raise_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:STA:NST  {str(steps)},(@{str(channel)})')
-    
-    def arb_Staircase__Current(self,channel:int,steps:int,initial_Current:float,end_Current:float,initial_Time:float,raise_Time:float,end_Time:float):
-        self.my_instr.write(f'ARB:CURR:STA:STAR  {str(initial_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:STA:END  {str(end_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:STA:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:STA:END:TIM  {str(end_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:STA:TIM  {str(raise_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:STA:NST  {str(steps)},(@{str(channel)})')
-    
-    def arb_Trapezoid__Voltage(self,channel:int,initial_Voltage:float,end_Voltage:float,initial_Time:float,raise_Time:float,top_Time:float,fall_Time:float,end_Time:float):
-        self.my_instr.write(f'ARB:volt:TRAP:STAR  {str(initial_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:volt:TRAP:END  {str(end_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:volt:TRAP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:volt:TRAP:END:TIM  {str(end_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:volt:TRAP:TOP:TIM  {str(top_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:volt:TRAP:RTIM  {str(raise_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:volt:TRAP:FTIM  {str(fall_Time)},(@{str(channel)})')
-    
-    def arb_Trapezoid__Current(self,channel:int,initial_Current:float,end_Current:float,initial_Time:float,raise_Time:float,top_Time:float,fall_Time:float,end_Time:float,count=1,LastOFF=0):
-        self.my_instr.write(f'CURR:MODE ARB,(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:TRAP:STAR  {str(initial_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:TRAP:TOP  {str(end_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:TRAP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:TRAP:END:TIM  {str(end_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:TRAP:TOP:TIM  {str(top_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:TRAP:RTIM  {str(raise_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:TRAP:FTIM  {str(fall_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:COUN  {str(count)},(@{str(channel)})')
-        self.arbLast_Value_OFF(channel=1)
-        if LastOFF !=0 :
-            self.arbLast_Value_ON(channel=1)
-    
-    def arb_Exponential__Current(self,channel:int,initial_Current:float,end_Current:float,initial_Time:float,tcon_Time:float,end_Time:float):
-        self.my_instr.write(f'ARB:CURR:EXP:STAR  {str(initial_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:EXP:END  {str(end_Current)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:EXP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:EXP:TIM  {str(end_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:CURR:EXP:TCON  {str(tcon_Time)},(@{str(channel)})')
-   
-    def arb_Exponential__Voltage(self,channel:int,initial_Voltage:float,end_Voltage:float,initial_Time:float,tcon_Time:float,end_Time:float):
-        self.my_instr.write(f'ARB:VOLT:EXP:STAR  {str(initial_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:EXP:END  {str(end_Voltage)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:EXP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:EXP:TIM  {str(end_Time)},(@{str(channel)})')
-        self.my_instr.write(f'ARB:VOLT:EXP:TCON  {str(tcon_Time)},(@{str(channel)})')
-     
-    def arb_Immediate_Trigger(self):
-        self.my_instr.write('TRIG:ARB:SOUR IMM')
-    
-    def arb_Mode__Voltage(self,channel:int):
-        self.my_instr.write(f'VOLT:MODE ARB(@{str(channel)})')
-    
-    def arb_Mode__Current(self,channel:int):
-        self.my_instr.write(f'CURR:MODE ARB(@{str(channel)})')
-    
-
-        
-    def getVoltage(self, channel:int):
-        if channel in self.channel.keys() :
-            ch = self.channel.get(channel)
-        else:
-            ch = self.channel.get(1)
-        command = 'INST:SEL ' +  ch
-        self.my_instr.write(command)
-        # ! sleep time to measure the voltage is optional but minimum sleep time needs to provided even atleast in the main program    
-        # time.sleep(0.2)
-        return float(self.my_instr.query(f'MEAS:VOLT? (@{str(channel)})'))
-    
-    def getCurrent(self, channel:int):
-        if channel in self.channel.keys() :
-            ch = self.channel.get(channel)
-        else:
-            ch = self.channel.get(1)
-        command = 'INST:SEL ' +  ch
-        self.my_instr.write(command)
-        # ! sleep time to measure the voltage is optional but minimum sleep time needs to provided even atleast in the main program    
-        # time.sleep(0.2)
-        return float(self.my_instr.query(f'MEAS:CURR? (@{str(channel)})'))
-    
-    def setCurrRange(self, channel:int):
-        if channel in self.channel.keys() :
-            ch = self.channel.get(channel)
-        else:
-            ch = self.channel.get(1)
-        command = 'INST:SEL ' +  ch
-        self.my_instr.write(command)
-        # ! sleep time to measure the voltage is optional but minimum sleep time needs to provided even atleast in the main program    
-        # time.sleep(0.2)
-        string = (f'SENS:CURR:RANG 10e-3,(@{str(channel)})')
-        self.my_instr.write(string)
-        print (string)
-        print(ch)
-        return
-        
-    def get_PeviousTriggered_Voltage(self, channel:int):
-        if channel in self.channel.keys() :
-            ch = self.channel.get(channel)
-        else:
-            ch = self.channel.get(1)
-        command = 'INST:SEL ' +  ch
-        self.my_instr.write(command)
-        # ! sleep time to measure the voltage is optional but minimum sleep time needs to provided even atleast in the main program    
-        # time.sleep(0.2)
-        return float(self.my_instr.query('FETC:VOLT?'))
-    
-    def get_PeviousTriggered_Current(self, channel:int):
-        if channel in self.channel.keys() :
-            ch = self.channel.get(channel)
-        else:
-            ch = self.channel.get(1)
-        command = 'INST:SEL ' +  ch
-        self.my_instr.write(command)
-        # ! sleep time to measure the voltage is optional but minimum sleep time needs to provided even atleast in the main program    
-        # time.sleep(0.2)
-        return float(self.my_instr.query('FETC:CURR?'))
-        
-    # o enable seamless voltage or current autoranging
-    def setMeter_Range_Auto__Current(self,channel:int):
-        self.my_instr.write(f'SENS:CURR:RANG:AUTO ON,(@{str(channel)})')
-
-    def setMeter_Range_Auto__Voltage(self,channel:int):
-        self.my_instr.write(f'SENS:VOLT:RANG:AUTO ON,(@{str(channel)})')
-
-        
-
-
-#         Specifies the emulation mode on N678xA <type> = PS4Q, PS2Q,
-# PS1Q, BATTery, CHARger, CCLoad, CVLoad, VMETer, AMETer
-    def emulMode_Battery(self,channel:int):
-        self.my_instr.write(f'EMUL BATTery,(@{str(channel)})')
-
-    def emulMode_2Q(self,channel:int):
-        self.my_instr.write(f'EMUL PS2Q,(@{str(channel)})')
-
-    def emulMode_1Q(self,channel:int):
-        self.my_instr.write(f'EMUL PS2Q,(@{str(channel)})')
-
-    def emulMode_4Q(self,channel:int):
-        self.my_instr.write(f'EMUL PS4Q,(@{str(channel)})')
-
-    def emulMode_CC_Load(self,channel:int):
-        self.my_instr.write(f'EMUL CCLoad,(@{str(channel)})')
-
-    def emulMode_CV_Load(self,channel:int):
-        self.my_instr.write(f'EMUL CVLoad,(@{str(channel)})')
-
-if __name__ == '__main__':
-    supply = N670x('USB0::0x0957::0x0F07::MY50002157::INSTR')
-    # print(supply.get_IDN())
-    # supply.emulMode_1Q(channel=1)
-    # supply.setCurrent_Priority(channel=3)
-    # # supply.my_instr.write('OUTP ON,(@1)') 
-    # print(supply.errorLog())
-    # supply.setCurrent(channel=3,current=-1)
-    # supply.outp_ON(channel=3)
-    # time.sleep(2)
-    # supply.outp_OFF(channel=3)
-    supply.my_instr.write('CURR:MODE ARB,(@1)')
-    supply.arb_Trapezoid__Current(channel=1,initial_Current=0,end_Current=-5.2,initial_Time=0,raise_Time=0.001,top_Time=0,fall_Time=0.001,end_Time=0)
-    # supply.my_instr.write('TRIG:ARB:SOUR BUS,(@1)')
-    # time.sleep(0.1)
-    # supply.my_instr.write('INIT:TRAN(@1)')
-    # supply.my_instr.write('TRIG:TRAN(@1)')
-    # supply.my_instr.write('*TRG')
+import time 
+import pyvisa as visa
+from pyvisa.attributes import *
+from pyvisa.constants import *
+
+# ('USB0::0x2A8D::0x0F02::MY56002702::INSTR', 'USB0::0x0699::0x0401::C020132::INSTR', 'TCPIP0::172.16.10.29::inst0::INSTR', 'GPIB0::6::INSTR')
+class N670x:
+
+    def __init__(self,port='USB0::0x2A8D::0x0F02::MY56002702::INSTR') -> None:
+        rm = visa.ResourceManager()
+        rm.list_resources()
+        self.my_instr = rm.open_resource(port)
+        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_BAUD, 9600)
+        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_DATA_BITS, 8)
+        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_STOP_BITS, VI_ASRL_STOP_TWO)
+        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_PARITY, visa.constants.VI_ASRL_PAR_NONE)
+        self.my_instr.read_termination = '\n'
+        self.my_instr.write_termination = '\n'
+
+        self.channel = {
+                            1:"OUT1",
+                            2:"OUT2",
+                            3:"OUT3",
+                            4:"OUT4",
+                        }
+
+        self.erroMSG = {
+            -100 :"Command error [generic command error]",
+            -101 :"Invalid character",
+            -102 :"Syntax error [unrecognized command or data type]",
+            -103 :"Invalid separator [illegal character encountered in place of separator]",
+            -104 :"Data type error [e.g., “numeric or string expected, got block date”]",
+            -105 :"GET not allowed [ <GET> inside a program message]",
+            -108 :"Parameter not allowed [too many parameters]",
+            -109 :"Missing parameter [too few parameters]",
+            -112 :"Program mnemonic too long [maximum 12 characters]",
+            -113 :"Undefined header [syntactical correct but not defined for this device]",
+            -121 :"Invalid character in number [e.g. alpha in decimal data, etc.]",
+            -123 :"Exponent too large [ numeric overflow; exponent magnitude >32000]",
+            -124 :"Too many digits [number too long; more than 255 digits received]",
+            -128 :"Numeric data not allowed [numeric data not accepted where positioned]",
+            -131 :"Invalid suffix [unrecognized suffix, or suffix not appropriate]",
+            -138 :"Suffix not allowed [numeric element does not allow suffixes]"
+        }
+        
+    # ! SYST:REM system remote connection 
+    # * *IDN?' Instrument id Query 
+    # ? provide the minimum sleep time(1 Sec) to configure for the remote connection time.sleep(1)
+    def get_IDN(self):
+        self.my_instr.write('SYST:REM') 
+        time.sleep(1)
+        return (self.my_instr.query('*IDN?'))
+        
+    
+    # * Rest the instrument 
+    def reset(self):
+        self.my_instr.write('*RST')  
+
+    # * switch off the Channle 
+    def outp_OFF(self,channel:int):
+        self.my_instr.write(f'OUTP OFF,(@{str(channel)})')  
+
+    # * Switch on the channel 
+    def outp_ON(self,channel:int):
+        self.my_instr.write(f'OUTP ON,(@{str(channel)})')  
+
+    # * Error Que Clear
+    def clear_errors(self):
+        self.my_instr.write('*CLS')  
+
+    # * Installed Options in the Channl
+    def modelNumber(self,channel:int):
+        return self.my_instr.query(f'SYST:CHAN:MOD? (@{str(channel)})')
+    
+    # * Serial number of the channel
+    def serialNumber(self,channel:int):
+        return self.my_instr.query(f'SYST:CHAN:SER? (@{str(channel)})')
+    
+    # * installed Options in the channel
+    def installedOptions(self,channel:int):
+        return self.my_instr.query(f'SYST:CHAN:OPT? (@{str(channel)})')
+
+    # Returns the error number and error string
+    def errorLog(self):
+        return (self.my_instr.query('SYST:ERR?'))
+
+    # * Multi channel voltage set method 
+    # ! first argument is the channel number shuold be in int  channel Number 1-4
+    # ! voltage must be in the float ex: 1.4 
+    # ? default it will provide the fist chanlle Voltage 
+    # def setVoltage(self, channel:int, voltage:float):
+    #     if channel in self.channel.keys() :
+    #         ch = self.channel.get(channel)
+    #     else:
+    #         ch = self.channel.get(1)
+    #     command = 'INST:SEL ' +  ch
+    #     self.my_instr.write(command)   
+    #     command = 'VOLT ' + str(voltage) 
+    #     self.my_instr.write(command)  
+
+    # * Multi channel voltage set method 
+    # ! first argument is the channel number shuold be in int  channel Number 1-4
+    # ! current must be in the float ex: 1.4 
+    # ? default it will provide the fist chanlle current 
+    # def setCurrent(self, channel:int, current:float):
+    #     if channel in self.channel.keys() :
+    #         ch = self.channel.get(channel)
+    #     else:
+    #         ch = self.channel.get(1)
+    #     command = 'INST:SEL ' +  ch
+    #     self.my_instr.write(command)   
+    #     command = 'CURR ' + str(current) 
+    #     self.my_instr.write(command)  
+
+    def setCurrent(self, channel:int, current:float):
+        self.my_instr.write(f'CURR {current},(@{channel})')
+
+    def setVoltage(self, channel:int, voltage:float):
+        self.my_instr.write(f'VOLT {voltage},(@{channel})')
+    # ? get the output status 
+    def getOutStatus(self):  
+        # time.sleep(0.2)
+        return self.my_instr.query('OUTP:STAT?')  
+    
+    # * set the Voltage Range of the channel 
+    # * Channel Number must be int it is between 1-4 
+    # * Voltage range must be float
+    def setRange_Voltage(self,channel:int,voltageRange:float):
+        self.my_instr.write(f'VOLT:RANG {str(voltageRange)},(@{str(channel)})')
+
+    # * set the Current Range of the channel 
+    # * Channel Number must be int it is between 1-4 
+    # * Current range must be float
+    def setRange_Current(self,channel:int,voltageRange:float):
+        self.my_instr.write(f'CURR:RANG {str(voltageRange)},(@{str(channel)})')
+
+
+    # * set the channel to the current mode =
+    # * Channel Number must be int it is between 1-4 
+    def setCurrentMode(self,channel:int):
+        self.my_instr.write(f'OUTP:PMOD CURR,(@{str(channel)})')
+        
+    # * set the channel to the Voltage mode =
+    # * Channel Number must be int it is between 1-4 
+    def setVoltageMode(self,channel:int):
+        self.my_instr.write(f'OUTP:PMOD VOLT,(@{str(channel)})')
+
+    # * To reverse the relay polarity on units with Option 760
+    # * Channel Number must be int it is between 1-4 
+    def setReverseRelay_Polarity(self,channel:int):
+        self.my_instr.write(f'OUTP:REL:POL REV,(@{str(channel)})')
+
+    # * To return the relay polarity to normal
+    # * Channel Number must be int it is between 1-4 
+    def setNormalRelay_Polarity(self,channel:int):
+        self.my_instr.write(f'OUTP:REL:POL NORM,(@{str(channel)})')
+
+    # To set the positive current limit of output ex:1 to 1 A:
+    def setCurrent_Positive_Limit(self,channel:int,current:float):
+        self.my_instr.write(f'CURR:LIM {str(current)},(@{str(channel)})')
+
+    # To set the negative current limit, you must first turn limit coupling
+    # (tracking) off. Then set the negative current limit
+    def setCurrent_Negative_Limit(self,channel:int,current:float):
+        self.my_instr.write(f'CURR:LIM:COUP OFF,(@{str(channel)})')
+        self.my_instr.write(f'CURR:LIM:NEG {str(current)},(@{str(channel)})')
+
+    # To set the voltage priority mode:
+    def setVoltage_Priority(self,channel:int):
+        self.my_instr.write(f'FUNC VOLT,(@{str(channel)})')
+
+    # To set the Current priority mode:
+    def setCurrent_Priority(self,channel:int):
+        self.my_instr.write(f'FUNC CURR,(@{str(channel)})')
+
+    # TTo program turn-on delay 
+    def setTurn_ON_Delay(self,channel:int,delay:float):
+        self.my_instr.write(f'OUTP:DEL:RISE  {str(delay)},(@{str(channel)})')
+
+    # TTo program turn-on delay 
+    def setTurn_OFF_Delay(self,channel:int,delay:float):
+        self.my_instr.write(f'OUTP:DEL:FALL  {str(delay)},(@{str(channel)})')
+
+
+    # # ! Coupling of the channel is pending 
+    # !!!
+    # !!!
+
+
+
+    # To program the OVP level for outputs
+    def setOVP_Protection(self,channel:int,OVP:float):
+        self.my_instr.write(f'VOLT:PROT  {str(OVP)},(@{str(channel)})')
+
+    # To enable OCP for outputs 
+    def setOCP_Protection(self,channel:int,OCP:float):
+        self.my_instr.write(f'CURR:PROT:STAT  {str(OCP)},(@{str(channel)})')
+
+    # To specify a 10 millisecond delay for the OCP
+    def setOCP_Delay(self,channel:int,delay:float):
+        self.my_instr.write(f'CURR:PROT:DEL  {str(delay)},(@{str(channel)})')
+    
+    # To enable output protection coupling
+    def setOutput_Protection_Coupling_ON(self):
+        self.my_instr.write('OUTP:PROT:COUP ON')
+
+
+    def setOutput_Current_Protection_ON(self,channel:int):
+        self.my_instr.write(f'CURR:PROT:STAT ON,(@{str(channel)})')
+
+
+    def setOutput_Current_Protection_OFF(self,channel:int):
+        self.my_instr.write(f'CURR:PROT:STAT OFF,(@{str(channel)})')
+
+
+    def setOutput_Voltage_Protection_ON(self,channel:int):
+        self.my_instr.write(f'VOLT:PROT:STAT ON,(@{str(channel)})')
+
+    def setOutput_Voltage_Protection_OFF(self,channel:int):
+        self.my_instr.write(f'VOLT:PROT:STAT OFF,(@{str(channel)})')
+
+    # To clear an output protection fault
+    def clearOutput_Protection_Clear(self,channel:int):
+        self.my_instr.write(f'OUTP:PROT:CLE (@{str(channel)})')
+
+    def protection_Status_Current(self):
+        return self.my_instr.query('CURRent:PROTection:STATe?')
+
+    def protection_Status_Voltage(self):
+        return self.my_instr.query('VOLTage:PROTection:STATe?')
+
+
+    
+    def arbFunction_Priority__Voltage(self,channel:int):
+        self.my_instr.write(f'ARB:FUNC:TYPE VOLT,(@{str(channel)})')
+
+    def arbFunction_Sequence__Set(self,channel:int):
+        self.my_instr.write(f'ARB:FUNC:SHAP SEQ,(@{str(channel)})')
+
+    def arbFunction_Sequence__Reset(self,channel:int):
+        self.my_instr.write(f'ARB:SEQ:RES(@{str(channel)})')
+    
+    def arbSet_Sequence_Waveform(self,channel:int):
+        self.arbFunction_Priority__Voltage(channel)
+        self.arbFunction_Sequence__Set(channel)
+
+    def arb_Pulse__Voltage(self,channel:int,initial_Voltage:float,end_Voltage:float,initial_Time:float,top_Time:float,end_Time:float):
+        self.my_instr.write(f'ARB:VOLT:PULS:STAR  {str(initial_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:PULS:TOP  {str(end_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:PULS:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:PULS:TOP:TIM  {str(top_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:PULS:END:TIM   {str(end_Time)},(@{str(channel)})')
+    def arb_Pulse__Current(self,channel:int,initial_Current:float,end_Current:float,initial_Time:float,top_Time:float,end_Time:float):
+        self.my_instr.write(f'ARB:CURR:PULS:STAR  {str(initial_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:PULS:TOP  {str(end_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:PULS:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:PULS:TOP:TIM  {str(top_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:PULS:END:TIM   {str(end_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:TERM:LAST OFF,(@{str(channel)})')
+        self.my_instr.write(f'TRIG:ARB:SOUR BUS')
+        self.my_instr.write(f'INIT:TRAN(@{str(channel)})')
+    
+    # The parameter setting remains at the last Arb value after the Arb completes.
+    def arbLast_Value_ON(self,channel:int):
+        self.my_instr.write(f'ARB:TERM:LAST ON,(@{str(channel)})')
+
+    # The parameter setting returns to the DC value that was in effect prior to the Arb
+    def arbLast_Value_OFF(self,channel:int):
+        self.my_instr.write(f'ARB:TERM:LAST OFF,(@{str(channel)})')
+    
+    def arb_Trigger(self):
+        self.my_instr.write('*TRG')
+
+    def arb_Step__Current(self,channel:int,initial_Current:float,end_Current:float,initial_Time:float):
+        self.my_instr.write(f'ARB:CURR:STEP:STAR  {str(initial_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:STEP:END  {str(end_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:STEP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+
+    def arb_Step__Voltage(self,channel:int,initial_Voltage:float,end_Voltage:float,initial_Time:float):
+        self.my_instr.write(f'ARB:VOLT:STEP:STAR  {str(initial_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:STEP:END  {str(end_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:STEP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+    
+    def arb_Ramp__Voltage(self,channel:int,initial_Voltage:float,end_Voltage:float,initial_Time:float,raise_Time:float,end_Time:float):
+        self.my_instr.write(f'ARB:VOLT:RAMP:STAR  {str(initial_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:RAMP:END  {str(end_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:RAMP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:RAMP:END:TIM  {str(end_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:RAMP:RTIM  {str(raise_Time)},(@{str(channel)})')
+    
+    def arb_Ramp__Current(self,channel:int,initial_Current:float,end_Current:float,initial_Time:float,raise_Time:float,end_Time:float):
+        self.my_instr.write(f'ARB:CURR:RAMP:STAR  {str(initial_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:RAMP:END  {str(end_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:RAMP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:RAMP:END:TIM  {str(end_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:RAMP:RTIM  {str(raise_Time)},(@{str(channel)})')
+    
+    def arb_Staircase__Voltage(self,channel:int,steps:int,initial_Voltage:float,end_Voltage:float,initial_Time:float,raise_Time:float,end_Time:float):
+        self.my_instr.write(f'ARB:VOLT:STA:STAR  {str(initial_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:STA:END  {str(end_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:STA:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:STA:END:TIM  {str(end_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:STA:TIM  {str(raise_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:STA:NST  {str(steps)},(@{str(channel)})')
+    
+    def arb_Staircase__Current(self,channel:int,steps:int,initial_Current:float,end_Current:float,initial_Time:float,raise_Time:float,end_Time:float):
+        self.my_instr.write(f'ARB:CURR:STA:STAR  {str(initial_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:STA:END  {str(end_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:STA:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:STA:END:TIM  {str(end_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:STA:TIM  {str(raise_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:STA:NST  {str(steps)},(@{str(channel)})')
+    
+    def arb_Trapezoid__Voltage(self,channel:int,initial_Voltage:float,end_Voltage:float,initial_Time:float,raise_Time:float,top_Time:float,fall_Time:float,end_Time:float):
+        self.my_instr.write(f'ARB:volt:TRAP:STAR  {str(initial_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:volt:TRAP:END  {str(end_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:volt:TRAP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:volt:TRAP:END:TIM  {str(end_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:volt:TRAP:TOP:TIM  {str(top_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:volt:TRAP:RTIM  {str(raise_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:volt:TRAP:FTIM  {str(fall_Time)},(@{str(channel)})')
+    
+    def arb_Trapezoid__Current(self,channel:int,initial_Current:float,end_Current:float,initial_Time:float,raise_Time:float,top_Time:float,fall_Time:float,end_Time:float,count=1,LastOFF=0):
+        self.my_instr.write(f'CURR:MODE ARB,(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:TRAP:STAR  {str(initial_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:TRAP:TOP  {str(end_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:TRAP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:TRAP:END:TIM  {str(end_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:TRAP:TOP:TIM  {str(top_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:TRAP:RTIM  {str(raise_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:TRAP:FTIM  {str(fall_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:COUN  {str(count)},(@{str(channel)})')
+        self.arbLast_Value_OFF(channel=1)
+        if LastOFF !=0 :
+            self.arbLast_Value_ON(channel=1)
+    
+    def arb_Exponential__Current(self,channel:int,initial_Current:float,end_Current:float,initial_Time:float,tcon_Time:float,end_Time:float):
+        self.my_instr.write(f'ARB:CURR:EXP:STAR  {str(initial_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:EXP:END  {str(end_Current)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:EXP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:EXP:TIM  {str(end_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:CURR:EXP:TCON  {str(tcon_Time)},(@{str(channel)})')
+   
+    def arb_Exponential__Voltage(self,channel:int,initial_Voltage:float,end_Voltage:float,initial_Time:float,tcon_Time:float,end_Time:float):
+        self.my_instr.write(f'ARB:VOLT:EXP:STAR  {str(initial_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:EXP:END  {str(end_Voltage)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:EXP:STAR:TIM  {str(initial_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:EXP:TIM  {str(end_Time)},(@{str(channel)})')
+        self.my_instr.write(f'ARB:VOLT:EXP:TCON  {str(tcon_Time)},(@{str(channel)})')
+     
+    def arb_Immediate_Trigger(self):
+        self.my_instr.write('TRIG:ARB:SOUR IMM')
+    
+    def arb_Mode__Voltage(self,channel:int):
+        self.my_instr.write(f'VOLT:MODE ARB(@{str(channel)})')
+    
+    def arb_Mode__Current(self,channel:int):
+        self.my_instr.write(f'CURR:MODE ARB(@{str(channel)})')
+    
+
+        
+    def getVoltage(self, channel:int):
+        if channel in self.channel.keys() :
+            ch = self.channel.get(channel)
+        else:
+            ch = self.channel.get(1)
+        command = 'INST:SEL ' +  ch
+        self.my_instr.write(command)
+        # ! sleep time to measure the voltage is optional but minimum sleep time needs to provided even atleast in the main program    
+        # time.sleep(0.2)
+        return float(self.my_instr.query(f'MEAS:VOLT? (@{str(channel)})'))
+    
+    def getCurrent(self, channel:int):
+        if channel in self.channel.keys() :
+            ch = self.channel.get(channel)
+        else:
+            ch = self.channel.get(1)
+        command = 'INST:SEL ' +  ch
+        self.my_instr.write(command)
+        # ! sleep time to measure the voltage is optional but minimum sleep time needs to provided even atleast in the main program    
+        # time.sleep(0.2)
+        return float(self.my_instr.query(f'MEAS:CURR? (@{str(channel)})'))
+    
+    def setCurrRange(self, channel:int):
+        if channel in self.channel.keys() :
+            ch = self.channel.get(channel)
+        else:
+            ch = self.channel.get(1)
+        command = 'INST:SEL ' +  ch
+        self.my_instr.write(command)
+        # ! sleep time to measure the voltage is optional but minimum sleep time needs to provided even atleast in the main program    
+        # time.sleep(0.2)
+        string = (f'SENS:CURR:RANG 10e-3,(@{str(channel)})')
+        self.my_instr.write(string)
+        print (string)
+        print(ch)
+        return
+        
+    def get_PeviousTriggered_Voltage(self, channel:int):
+        if channel in self.channel.keys() :
+            ch = self.channel.get(channel)
+        else:
+            ch = self.channel.get(1)
+        command = 'INST:SEL ' +  ch
+        self.my_instr.write(command)
+        # ! sleep time to measure the voltage is optional but minimum sleep time needs to provided even atleast in the main program    
+        # time.sleep(0.2)
+        return float(self.my_instr.query('FETC:VOLT?'))
+    
+    def get_PeviousTriggered_Current(self, channel:int):
+        if channel in self.channel.keys() :
+            ch = self.channel.get(channel)
+        else:
+            ch = self.channel.get(1)
+        command = 'INST:SEL ' +  ch
+        self.my_instr.write(command)
+        # ! sleep time to measure the voltage is optional but minimum sleep time needs to provided even atleast in the main program    
+        # time.sleep(0.2)
+        return float(self.my_instr.query('FETC:CURR?'))
+        
+    # o enable seamless voltage or current autoranging
+    def setMeter_Range_Auto__Current(self,channel:int):
+        self.my_instr.write(f'SENS:CURR:RANG:AUTO ON,(@{str(channel)})')
+
+    def setMeter_Range_Auto__Voltage(self,channel:int):
+        self.my_instr.write(f'SENS:VOLT:RANG:AUTO ON,(@{str(channel)})')
+
+        
+
+
+#         Specifies the emulation mode on N678xA <type> = PS4Q, PS2Q,
+# PS1Q, BATTery, CHARger, CCLoad, CVLoad, VMETer, AMETer
+    def emulMode_Battery(self,channel:int):
+        self.my_instr.write(f'EMUL BATTery,(@{str(channel)})')
+
+    def emulMode_2Q(self,channel:int):
+        self.my_instr.write(f'EMUL PS2Q,(@{str(channel)})')
+
+    def emulMode_1Q(self,channel:int):
+        self.my_instr.write(f'EMUL PS2Q,(@{str(channel)})')
+
+    def emulMode_4Q(self,channel:int):
+        self.my_instr.write(f'EMUL PS4Q,(@{str(channel)})')
+
+    def emulMode_CC_Load(self,channel:int):
+        self.my_instr.write(f'EMUL CCLoad,(@{str(channel)})')
+
+    def emulMode_CV_Load(self,channel:int):
+        self.my_instr.write(f'EMUL CVLoad,(@{str(channel)})')
+
+if __name__ == '__main__':
+    supply = N670x('USB0::0x0957::0x0F07::MY50002157::INSTR')
+    # print(supply.get_IDN())
+    # supply.emulMode_1Q(channel=1)
+    # supply.setCurrent_Priority(channel=3)
+    # # supply.my_instr.write('OUTP ON,(@1)') 
+    # print(supply.errorLog())
+    # supply.setCurrent(channel=3,current=-1)
+    # supply.outp_ON(channel=3)
+    # time.sleep(2)
+    # supply.outp_OFF(channel=3)
+    supply.my_instr.write('CURR:MODE ARB,(@1)')
+    supply.arb_Trapezoid__Current(channel=1,initial_Current=0,end_Current=-5.2,initial_Time=0,raise_Time=0.001,top_Time=0,fall_Time=0.001,end_Time=0)
+    # supply.my_instr.write('TRIG:ARB:SOUR BUS,(@1)')
+    # time.sleep(0.1)
+    # supply.my_instr.write('INIT:TRAN(@1)')
+    # supply.my_instr.write('TRIG:TRAN(@1)')
+    # supply.my_instr.write('*TRG')
     # supply.arb_Trigger()
```

### Comparing `IvmInstruments-0.2.0/Instruments/KeySight_RP7954.py` & `ivminstruments-0.2.2/Instruments/KeySight_RP7954.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import time 
-import pyvisa as visa
-from pyvisa.attributes import *
-from pyvisa.constants import *
-
-# ('USB0::0x2A8D::0x0F02::MY56002702::INSTR', 'USB0::0x0699::0x0401::C020132::INSTR', 'TCPIP0::172.16.10.29::inst0::INSTR', 'GPIB0::6::INSTR')
-class RP790x:
-
-    def __init__(self,port='USB0::0x2A8D::0x2802::MY59003109::INSTR') -> None:
-        rm = visa.ResourceManager()
-        rm.list_resources()
-        self.my_instr = rm.open_resource(port)
-        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_BAUD, 9600)
-        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_DATA_BITS, 8)
-        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_STOP_BITS, VI_ASRL_STOP_TWO)
-        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_PARITY, visa.constants.VI_ASRL_PAR_NONE)
-        self.my_instr.read_termination = '\n'
-        self.my_instr.write_termination = '\n'
-
-        # * switch off the Channle 
-    def outp_OFF(self):
-        self.my_instr.write(f'OUTP OFF')  
-
-    # * Switch on the channel 
-    def outp_ON(self):
-        self.my_instr.write(f'OUTP ON')
-
-    def setCurrent_Priority(self):
-        self.my_instr.write(f'FUNC CURR')  
-
-    def setVoltage_Priority(self):
-        self.my_instr.write(f'FUNC VOLT')  
-    # * Switch on the channel 
-    def setCurrent_Limit(self,current):
-        if current >= 0:
-            self.my_instr.write(f'CURR:LIM {str(current)}')
-        else:
-            self.my_instr.write(f'CURR:LIM:NEG {str(current)}')
-
-    def setVoltage(self,voltage):
-        self.my_instr.write(f'VOLT {str(voltage)}')
-    
-    def setCurrent(self,current):
-        self.my_instr.write(f'CURR {str(current)}')
-        
-    def setVoltage_Limit(self,voltage):
-        self.my_instr.write(f'VOLT:LIM {str(voltage)}')
-      
-    def setVoltage_Limit__LOW(self,voltage):
-        self.my_instr.write(f'VOLT:LIM:LOW {str(voltage)}')
-    
-    def rest(self):
-        self.my_instr.write(f'*RST')
-
-    def getVotlage(self):
-        return float(self.my_instr.query(f'MEASure:VOLTage?'))
-    
-    def getCurrent(self):
-        return float(self.my_instr.query(f'MEASure:CURR?'))
-    def getPower(self):
-        return float(self.my_instr.query(f'MEASure:POW?'))
-    
-    def getError(self):
-        self.my_instr.query(f'SYST:ERR?')
-
-
-if __name__ == '__main__':
-    supply = RP790x()
-    # supply.outp_OFF()
-    # time.sleep(0.1)
-    # supply.rest()
-    # supply.setCurrent_Priority()
-    # supply.setCurrent_Limit(current=-1)
-    # supply.setVoltage_Limit(voltage=4.3)
-    # supply.setVoltage(voltage=4)
-    # supply.setCurrent(current=-1)
-    # print(supply.getError())
-    # supply.outp_ON()
-    print(supply.getCurrent())
+import time 
+import pyvisa as visa
+from pyvisa.attributes import *
+from pyvisa.constants import *
+
+# ('USB0::0x2A8D::0x0F02::MY56002702::INSTR', 'USB0::0x0699::0x0401::C020132::INSTR', 'TCPIP0::172.16.10.29::inst0::INSTR', 'GPIB0::6::INSTR')
+class RP790x:
+
+    def __init__(self,port='USB0::0x2A8D::0x2802::MY59003109::INSTR') -> None:
+        rm = visa.ResourceManager()
+        rm.list_resources()
+        self.my_instr = rm.open_resource(port)
+        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_BAUD, 9600)
+        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_DATA_BITS, 8)
+        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_STOP_BITS, VI_ASRL_STOP_TWO)
+        # self.my_instr.set_visa_attribute(visa.constants.VI_ATTR_ASRL_PARITY, visa.constants.VI_ASRL_PAR_NONE)
+        self.my_instr.read_termination = '\n'
+        self.my_instr.write_termination = '\n'
+
+        # * switch off the Channle 
+    def outp_OFF(self):
+        self.my_instr.write(f'OUTP OFF')  
+
+    # * Switch on the channel 
+    def outp_ON(self):
+        self.my_instr.write(f'OUTP ON')
+
+    def setCurrent_Priority(self):
+        self.my_instr.write(f'FUNC CURR')  
+
+    def setVoltage_Priority(self):
+        self.my_instr.write(f'FUNC VOLT')  
+    # * Switch on the channel 
+    def setCurrent_Limit(self,current):
+        if current >= 0:
+            self.my_instr.write(f'CURR:LIM {str(current)}')
+        else:
+            self.my_instr.write(f'CURR:LIM:NEG {str(current)}')
+
+    def setVoltage(self,voltage):
+        self.my_instr.write(f'VOLT {str(voltage)}')
+    
+    def setCurrent(self,current):
+        self.my_instr.write(f'CURR {str(current)}')
+        
+    def setVoltage_Limit(self,voltage):
+        self.my_instr.write(f'VOLT:LIM {str(voltage)}')
+      
+    def setVoltage_Limit__LOW(self,voltage):
+        self.my_instr.write(f'VOLT:LIM:LOW {str(voltage)}')
+    
+    def rest(self):
+        self.my_instr.write(f'*RST')
+
+    def getVotlage(self):
+        return float(self.my_instr.query(f'MEASure:VOLTage?'))
+    
+    def getCurrent(self):
+        return float(self.my_instr.query(f'MEASure:CURR?'))
+    def getPower(self):
+        return float(self.my_instr.query(f'MEASure:POW?'))
+    
+    def getError(self):
+        self.my_instr.query(f'SYST:ERR?')
+
+
+if __name__ == '__main__':
+    supply = RP790x()
+    # supply.outp_OFF()
+    # time.sleep(0.1)
+    # supply.rest()
+    # supply.setCurrent_Priority()
+    # supply.setCurrent_Limit(current=-1)
+    # supply.setVoltage_Limit(voltage=4.3)
+    # supply.setVoltage(voltage=4)
+    # supply.setCurrent(current=-1)
+    # print(supply.getError())
+    # supply.outp_ON()
+    print(supply.getCurrent())
```

### Comparing `IvmInstruments-0.2.0/Instruments/Keysight_34461.py` & `ivminstruments-0.2.2/Instruments/Keysight_34461.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,299 +1,299 @@
-import time 
-import pyvisa as visa
-# from pyvisa.attributes import *
-# from pyvisa.constants import *
-
-
-class A34461:
-
-    def __init__(self,port:str) -> None:
-        rm = visa.ResourceManager()
-        rm.list_resources()
-        self.meter = rm.open_resource(port)
-        # self.meter.set_visa_attribute(visa.constants.VI_ATTR_ASRL_BAUD, 9600)
-        # self.meter.set_visa_attribute(visa.constants.VI_ATTR_ASRL_DATA_BITS, 8)
-        # self.meter.set_visa_attribute(visa.constants.VI_ATTR_ASRL_STOP_BITS, VI_ASRL_STOP_TWO)
-        # self.meter.set_visa_attribute(visa.constants.VI_ATTR_ASRL_PARITY, visa.constants.VI_ASRL_PAR_NONE)
-        # self.meter.read_termination = '\n'
-        # self.meter.write_termination = '\n'
-
-    
-    def get_IDN(self):
-        return (self.meter.query('*IDN?'))
-    
-    def reset(self):
-        self.meter.write('*RST')     
-
-    def get_error(self):
-        return self.meter.query('SYST:ERR?')  
-    
-    def reset(self):
-        self.meter.write('*RST')     
-
-    def get_error(self):
-        return self.meter.query('SYST:ERR?')  
-
-
-    def read_value(self, cnt):
-        self.meter.write(':SAMP:COUN ' + str(cnt) +';:TRIG:SOUR IMM')      
-        data_str= self.meter.query(':READ?')
-        data_split = data_str.split(sep =',')
-        value = list(map(float, data_split))
-        return(sum(value) / len(value))
-
-    def meas_V(self, range = -1, count = 4):
-        self.meter.write(':FUNC "VOLT:DC"') 
-        #Range: Autorange (-1), 100 mV, 1 V, 10 V, 100 V, or 750 V
-        range_list = [-1, 0.1, 1, 10, 100, 750]
-        if range in range_list:
-            range_auto = ':VOLT:DC:RANG:AUTO '
-            range_val = ';:VOLT:DC:RANG '
-            res_com = ';:VOLT:DC:RES '
-
-            if range == -1:
-                range_auto_cmd = 'ON'
-                range_val = ''
-                range_val_str = ''
-                res_com = ''
-                res_val_str = ''
-            else:
-                range_auto_cmd = 'OFF'
-                range_val_str = str(range)
-                if range == 0.1 or range == 1:
-                    res = 1e-6
-                elif range == 10:
-                    res = 1e-5
-                elif range == 100:
-                    res = 1e-4    
-                else:   
-                    res = 1e-3
-                res_val_str = str(res)
-
-            com = range_auto + range_auto_cmd +  range_val + range_val_str + res_com + res_val_str
-            self.meter.write(com) 
-            self.meter.write('VOLT:IMP:AUTO ON')
-            array = []
-            while count>0:
-                if count > 4:
-                    cnt = 4
-                else:
-                    cnt = count 
-                array.append(self.read_value(cnt))
-                count -= 4 
-            return(sum(array)/len(array))   
-        else:
-            return('ERR: Wrong range')   
-
-    
-
-    def meas_I(self, range = -1, count = 4):
-        self.meter.write(':FUNC "CURR:DC"') 
-        #Range: : Autorange (-1), 100 µA, 1 mA, 10 mA, 100 mA, 1 A, 3 A, or 10 A
-        range_list = [-1, 100e-6, 1e-3, 0.01, 0.1, 1, 3]
-        if range in range_list:
-            range_auto = ':CURR:DC:RANG:AUTO '
-            range_val = ';:CURR:DC:RANG '
-            res_com = ';:CURR:DC:RES '
-
-            if range == -1:
-                range_auto_cmd = 'ON'
-                range_val = ''
-                range_val_str = ''
-                res_com = ''
-                res_val_str = ''
-            else:
-                range_auto_cmd = 'OFF'
-                range_val_str = str(range)
-                if range in list([100e-6, 1e-3]):
-                    res = 1e-9
-                elif range == 10e-3:
-                    res = 1e-8
-                elif range == 100e-3:
-                    res = 1e-7   
-                elif range == 1:
-                    res = 1e-6
-                else:   
-                    res = 1e-5
-                res_val_str = str(res)
-
-            com = range_auto + range_auto_cmd +  range_val + range_val_str + res_com + res_val_str
-            self.meter.write(com) 
-            #self.meter.write('VOLT:IMP:AUTO ON')
-            array = []
-            while count>0:
-                if count > 4:
-                    cnt = 4
-                else:
-                    cnt = count 
-                array.append(self.read_value(cnt))
-                count -= 4 
-            return(sum(array)/len(array))   
-        else:
-            return('ERR: Wrong range')  
-
-    # ? VOLTage:DC:RANGe {<range>|MIN|MAX|DEF}
-    def set_Meter_DC__Voltage___Range(self,range:int):
-        self.meter.write(f'VOLT:DC:RANG {str(range)}')  
-
-    # ? VOLTage:DC:RANGe {<range>|MIN|MAX|DEF}
-    def get_Meter_DC__Voltage___Range(self,range:int):
-        return self.meter.write(f'VOLT:DC:RANG {str(range)}')   
-    
-
-    #* SET the trigger edge 
-    #? OUTPut:TRIGger:SLOPe {POSitive|NEGative}
-    #? OUTPut:TRIGger:SLOPe?
-
-    def set_meter_TriggerSlope__Positve(self):
-        self.meter.write('OUTP:TRIG:SLOP POS') 
-
-    def set_meter_TriggerSlope__Negative(self):
-        self.meter.write('OUTP:TRIG:SLOP NEG')
-
-    def get_meter_TriggerSlope(self):
-        return self.meter.query('OUTP:TRIG:SLOP?')
-     
-    #? The following method is uses INITiate, The INITiate command places the instrument in the "wait-for-trigger" state, 
-    #? triggers a measurement when the rearpanel Ext Trig input is pulsed (low by default), and 
-    #? sends the measurement to reading memory. 
-    #? The FETCh? query  must use to transfers the measurement from reading memory to the instrument's output buffer
-    def set_meter_External__Positivetrigger___Voltage(self):
-        self.meter.write('CONF:VOLT:DC')
-        self.meter.write('TRIG:SOUR EXT')
-        self.meter.write('INIT')
-
-    def fetch_meter__Reading(self):
-        return float(self.meter.query('FETCh?'))    
-
-
-    #* Meter Configureations 
-
-    def get_meter__Configuration(self):
-        return self.meter.query('CONF?')
-        
-    #?  <range>: {100 µA|1 mA|10 mA|100 mA|1 A|3 A|10 A}. Default: AUTO (autorange). 
-    def configure_meter__Mode__DcCurrent(self,Range:int,resolution:float):
-        self.meter.write(f'CONF:CURR:DC {str(Range)},{str(resolution)}')
-
-    #?  <range>: {100 µA|1 mA|10 mA|100 mA|1 A|3 A|10 A}. Default: AUTO (autorange). 
-    def configure_meter__Mode__AcCurrent(self,Range:int,resolution:float):
-        self.meter.write(f'CONF:CURR:AC {str(Range)},{str(resolution)}')
-
-    #? The FETCh?, READ?, and MEASure:DIODe? queries return the measured voltage, regardless of its value.
-    def configure_meter__Mode__Diode(self):
-        self.meter.write('CONF:DIOD')
-
-    #?  <range>: 100 Ω, 1 kΩ, 10 kΩ, 100 kΩ, 1 MΩ, 10 MΩ, 100 MΩ, 1GΩ, AUTO,or DEFault 
-    def configure_meter__Mode__Resistance(self,Range:int,resolution:float):
-        self.meter.write(f'CONF:RES {str(Range)},{str(resolution)}')
-
-    #?  <range>: {100 mV|1 V|10 V|100 V|1000 V}. Default: AUTO (autorange). 
-    def configure_meter__Mode__DcVoltage(self,Range:int,resolution:float):
-        self.meter.write(f'CONF:CURR:DC {str(Range)},{str(resolution)}')
-
-    #?  <range>: {100 mV|1 V|10 V|100 V|1000 V}. Default: AUTO (autorange). 
-    def configure_meter__Mode__AcVoltage(self,Range:int,resolution:float):
-        self.meter.write(f'CONF:CURR:AC {str(Range)},{str(resolution)}')
-
-    #* Measure functions 
-    # ? With the MEASure? queries, you can select the function, range and resolution in one command. All other
-    # ? parameters are set to their default values (below).
-
-    # ? Measurement Parameter                       Default Setting
-    # ?     AC Input Filter (bandwidth)                     20 Hz (medium filter)
-    # ?     Autozero                                        OFF if resolution setting results in NPLC < 1
-    # ?                                                     ON if resolution setting results in NPLC ≥ 1
-    # ? 
-    # ?     Range                                           AUTO (including voltage range for frequency and period measurements)
-    # ?     Samples per Trigger                             1 sample
-    # ?     Trigger Count                                   1 trigger
-    # ?     Trigger Delay                                   Automatic delay
-    # ?     Trigger Source                                  Immediate
-    # ?     Trigger Slope                                   NEGative
-    # ?     Math Functions                                  Disabled. Other parameters are unchanged.
-    # ?     Per-function Null State                         Disabled
-
-    # <range>: {1 nF|10 nF|100 nF|1 µF|10 µF|100 µF}. Default:AUTO.
-    # <resolution>: optional and ignored; fixed at 4½ digits.
-    def meas_meter__Capacitance(self):
-        return float(self.meter.query('MEAS:CAP?'))
-    
-    # <range>: {100 µA|1 mA|10 mA|100 mA|1 A|3 A|10 A}. Default: AUTO(autorange).
-    # <resolution> (AC): optional and ignored; fixed at 6½ digits.
-    def meas_meter__AcCurrent(self):
-        return float(self.meter.query('MEAS:CURR:AC?'))
-    
-    # <range>: {100 µA|1 mA|10 mA|100 mA|1 A|3 A|10 A}. Default: AUTO(autorange).
-    # <resolution> (DC): optional and ignored; fixed at 6½ digits.
-    def meas_meter__DcCurrent(self):
-        return float(self.meter.query('MEAS:CURR:DC?'))
-    
-
-    # Resolution 0.001 PLC 0.002 PLC 0.006 PLC 0.02 PLC 0.06 PLC  0.2 PLC  1 PLC  10 PLC 100 PLC
-    def meas_meter__Diod(self):
-        return float(self.meter.query('MEAS:DIOD?'))
-    
-    # <range>: 100 mV, 1 V, 10 V, 100 V, 1000 V, AUTO (default) or DEFault
-    # <resolution> (DC): optional and ignored; fixed at 6½ digits.  
-    # # Resolution 0.001 PLC 0.002 PLC 0.006 PLC 0.02 PLC 0.06 PLC  0.2 PLC  1 PLC  10 PLC 100 PLC
-    def meas_meter__DcVoltage(self):
-        return float(self.meter.query('MEAS:VOLT:DC?'))
-    
-    # <range>: 100 mV, 1 V, 10 V, 100 V, 1000 V, AUTO (default) or DEFault
-    # <resolution> (DC): optional and ignored; fixed at 6½ digits.  
-    # # Resolution 0.001 PLC 0.002 PLC 0.006 PLC 0.02 PLC 0.06 PLC  0.2 PLC  1 PLC  10 PLC 100 PLC
-    def meas_meter__AcCurrent(self):
-        return float(self.meter.query('MEAS:VOLT:AC?'))
-    
-
-    #? @@@@@@@@@@@@@@@@@@@@@@@@@@@@@        Trigger Function @@@@@@@@@@@@@@@@@@@
-
-    # 0 to ~3600 seconds (~1 µs steps). Default: 1 s.
-    def set_meter__Trigger___Delay(self,delay:float):
-        self.meter.write(f'SAMP:COUN 1')
-        self.meter.write(f'TRIGger:DELay:AUTO OFF')
-        self.meter.write(f'TRIG:DEL {str(delay)}')
-        self.meter.write('CONF:VOLT:DC 1,0.0001') 
-        self.meter.write('TRIG:SOUR INT')                   
-        self.meter.write('TRIG:LEV 0.75')
-        self.meter.write('TRIG:SLOP POS')
-        self.meter.write('INIT')
-
-    # 0 to ~3600 seconds (~1 µs steps). Default: 1 s.
-    def get_meter__Trigger___Delay(self):
-        return float(self.meter.query(f'TRIG:DEL?'))
-    
-    # <level> (see bullet points below). Default: 0. 
-    def get_meter__Trigger___Level(self):
-        return float(self.meter.query(f'TRIG:LEV?'))
-    
-    # <level> (see bullet points below). Default: 0. 
-    def set_meter__Trigger___Level(self,levle:float):
-        self.meter.write(f'TRIG:LEV {str(levle)}')
-
-
-    # {ON|1|OFF|0}. Default: OFF. 0 (OFF) or 1 (ON)
-    # ?  OFF: the input impedance for DC voltage measurements is fixed at 10 MΩ for all ranges to minimize noise pickup.
-    def set_meter__OutputVoltage___ImdpedenceAuto____On(self):
-        self.meter.write(f'VOLT:IMP:AUTO ON')
-    def set_meter__OutputCurrent___ImdpedenceAuto____On(self):
-        self.meter.write(f'CURR:IMP:AUTO ON')
-
-    # ?  ON: the input impedance for DC voltage measurements varies by range. It is set to "HI-Z" (>10 GΩ) for
-    #?        the 100 mV, 1 V, and 10 V ranges to reduce the effects of measurement loading errors on these lower
-    #?        ranges. The 100 V and 1000 V ranges remain at a 10 MΩ input impedance.
-    # {ON|1|OFF|0}. Default: OFF. 0 (OFF) or 1 (ON)
-    def set_meter__OutputVoltage___ImdpedenceAuto____Off(self):
-        self.meter.write(f'VOLT:IMP:AUTO ON')
-
-    def get_meter__OutputVoltage___ImdpedenceAuto____Status(self):
-        return float(self.meter.write(f'VOLT:IMP:AUTO?'))
-
-    def set_Voltage__NPLC(self,NPLC):
-        self.meter.write(f'VOLT:DC:NPLC {str(NPLC)}')
-
-if __name__ == '__main__':
-    meter = A34461('USB0::0x2A8D::0x1401::MY57216238::INSTR')
-    # print(meter.meas_V())
-    # print(meter.meas_I())
+import time 
+import pyvisa as visa
+# from pyvisa.attributes import *
+# from pyvisa.constants import *
+
+
+class A34461:
+
+    def __init__(self,port:str) -> None:
+        rm = visa.ResourceManager()
+        rm.list_resources()
+        self.meter = rm.open_resource(port)
+        # self.meter.set_visa_attribute(visa.constants.VI_ATTR_ASRL_BAUD, 9600)
+        # self.meter.set_visa_attribute(visa.constants.VI_ATTR_ASRL_DATA_BITS, 8)
+        # self.meter.set_visa_attribute(visa.constants.VI_ATTR_ASRL_STOP_BITS, VI_ASRL_STOP_TWO)
+        # self.meter.set_visa_attribute(visa.constants.VI_ATTR_ASRL_PARITY, visa.constants.VI_ASRL_PAR_NONE)
+        # self.meter.read_termination = '\n'
+        # self.meter.write_termination = '\n'
+
+    
+    def get_IDN(self):
+        return (self.meter.query('*IDN?'))
+    
+    def reset(self):
+        self.meter.write('*RST')     
+
+    def get_error(self):
+        return self.meter.query('SYST:ERR?')  
+    
+    def reset(self):
+        self.meter.write('*RST')     
+
+    def get_error(self):
+        return self.meter.query('SYST:ERR?')  
+
+
+    def read_value(self, cnt):
+        self.meter.write(':SAMP:COUN ' + str(cnt) +';:TRIG:SOUR IMM')      
+        data_str= self.meter.query(':READ?')
+        data_split = data_str.split(sep =',')
+        value = list(map(float, data_split))
+        return(sum(value) / len(value))
+
+    def meas_V(self, range = -1, count = 4):
+        self.meter.write(':FUNC "VOLT:DC"') 
+        #Range: Autorange (-1), 100 mV, 1 V, 10 V, 100 V, or 750 V
+        range_list = [-1, 0.1, 1, 10, 100, 750]
+        if range in range_list:
+            range_auto = ':VOLT:DC:RANG:AUTO '
+            range_val = ';:VOLT:DC:RANG '
+            res_com = ';:VOLT:DC:RES '
+
+            if range == -1:
+                range_auto_cmd = 'ON'
+                range_val = ''
+                range_val_str = ''
+                res_com = ''
+                res_val_str = ''
+            else:
+                range_auto_cmd = 'OFF'
+                range_val_str = str(range)
+                if range == 0.1 or range == 1:
+                    res = 1e-6
+                elif range == 10:
+                    res = 1e-5
+                elif range == 100:
+                    res = 1e-4    
+                else:   
+                    res = 1e-3
+                res_val_str = str(res)
+
+            com = range_auto + range_auto_cmd +  range_val + range_val_str + res_com + res_val_str
+            self.meter.write(com) 
+            self.meter.write('VOLT:IMP:AUTO ON')
+            array = []
+            while count>0:
+                if count > 4:
+                    cnt = 4
+                else:
+                    cnt = count 
+                array.append(self.read_value(cnt))
+                count -= 4 
+            return(sum(array)/len(array))   
+        else:
+            return('ERR: Wrong range')   
+
+    
+
+    def meas_I(self, range = -1, count = 4):
+        self.meter.write(':FUNC "CURR:DC"') 
+        #Range: : Autorange (-1), 100 µA, 1 mA, 10 mA, 100 mA, 1 A, 3 A, or 10 A
+        range_list = [-1, 100e-6, 1e-3, 0.01, 0.1, 1, 3]
+        if range in range_list:
+            range_auto = ':CURR:DC:RANG:AUTO '
+            range_val = ';:CURR:DC:RANG '
+            res_com = ';:CURR:DC:RES '
+
+            if range == -1:
+                range_auto_cmd = 'ON'
+                range_val = ''
+                range_val_str = ''
+                res_com = ''
+                res_val_str = ''
+            else:
+                range_auto_cmd = 'OFF'
+                range_val_str = str(range)
+                if range in list([100e-6, 1e-3]):
+                    res = 1e-9
+                elif range == 10e-3:
+                    res = 1e-8
+                elif range == 100e-3:
+                    res = 1e-7   
+                elif range == 1:
+                    res = 1e-6
+                else:   
+                    res = 1e-5
+                res_val_str = str(res)
+
+            com = range_auto + range_auto_cmd +  range_val + range_val_str + res_com + res_val_str
+            self.meter.write(com) 
+            #self.meter.write('VOLT:IMP:AUTO ON')
+            array = []
+            while count>0:
+                if count > 4:
+                    cnt = 4
+                else:
+                    cnt = count 
+                array.append(self.read_value(cnt))
+                count -= 4 
+            return(sum(array)/len(array))   
+        else:
+            return('ERR: Wrong range')  
+
+    # ? VOLTage:DC:RANGe {<range>|MIN|MAX|DEF}
+    def set_Meter_DC__Voltage___Range(self,range:int):
+        self.meter.write(f'VOLT:DC:RANG {str(range)}')  
+
+    # ? VOLTage:DC:RANGe {<range>|MIN|MAX|DEF}
+    def get_Meter_DC__Voltage___Range(self,range:int):
+        return self.meter.write(f'VOLT:DC:RANG {str(range)}')   
+    
+
+    #* SET the trigger edge 
+    #? OUTPut:TRIGger:SLOPe {POSitive|NEGative}
+    #? OUTPut:TRIGger:SLOPe?
+
+    def set_meter_TriggerSlope__Positve(self):
+        self.meter.write('OUTP:TRIG:SLOP POS') 
+
+    def set_meter_TriggerSlope__Negative(self):
+        self.meter.write('OUTP:TRIG:SLOP NEG')
+
+    def get_meter_TriggerSlope(self):
+        return self.meter.query('OUTP:TRIG:SLOP?')
+     
+    #? The following method is uses INITiate, The INITiate command places the instrument in the "wait-for-trigger" state, 
+    #? triggers a measurement when the rearpanel Ext Trig input is pulsed (low by default), and 
+    #? sends the measurement to reading memory. 
+    #? The FETCh? query  must use to transfers the measurement from reading memory to the instrument's output buffer
+    def set_meter_External__Positivetrigger___Voltage(self):
+        self.meter.write('CONF:VOLT:DC')
+        self.meter.write('TRIG:SOUR EXT')
+        self.meter.write('INIT')
+
+    def fetch_meter__Reading(self):
+        return float(self.meter.query('FETCh?'))    
+
+
+    #* Meter Configureations 
+
+    def get_meter__Configuration(self):
+        return self.meter.query('CONF?')
+        
+    #?  <range>: {100 µA|1 mA|10 mA|100 mA|1 A|3 A|10 A}. Default: AUTO (autorange). 
+    def configure_meter__Mode__DcCurrent(self,Range:int,resolution:float):
+        self.meter.write(f'CONF:CURR:DC {str(Range)},{str(resolution)}')
+
+    #?  <range>: {100 µA|1 mA|10 mA|100 mA|1 A|3 A|10 A}. Default: AUTO (autorange). 
+    def configure_meter__Mode__AcCurrent(self,Range:int,resolution:float):
+        self.meter.write(f'CONF:CURR:AC {str(Range)},{str(resolution)}')
+
+    #? The FETCh?, READ?, and MEASure:DIODe? queries return the measured voltage, regardless of its value.
+    def configure_meter__Mode__Diode(self):
+        self.meter.write('CONF:DIOD')
+
+    #?  <range>: 100 Ω, 1 kΩ, 10 kΩ, 100 kΩ, 1 MΩ, 10 MΩ, 100 MΩ, 1GΩ, AUTO,or DEFault 
+    def configure_meter__Mode__Resistance(self,Range:int,resolution:float):
+        self.meter.write(f'CONF:RES {str(Range)},{str(resolution)}')
+
+    #?  <range>: {100 mV|1 V|10 V|100 V|1000 V}. Default: AUTO (autorange). 
+    def configure_meter__Mode__DcVoltage(self,Range:int,resolution:float):
+        self.meter.write(f'CONF:CURR:DC {str(Range)},{str(resolution)}')
+
+    #?  <range>: {100 mV|1 V|10 V|100 V|1000 V}. Default: AUTO (autorange). 
+    def configure_meter__Mode__AcVoltage(self,Range:int,resolution:float):
+        self.meter.write(f'CONF:CURR:AC {str(Range)},{str(resolution)}')
+
+    #* Measure functions 
+    # ? With the MEASure? queries, you can select the function, range and resolution in one command. All other
+    # ? parameters are set to their default values (below).
+
+    # ? Measurement Parameter                       Default Setting
+    # ?     AC Input Filter (bandwidth)                     20 Hz (medium filter)
+    # ?     Autozero                                        OFF if resolution setting results in NPLC < 1
+    # ?                                                     ON if resolution setting results in NPLC ≥ 1
+    # ? 
+    # ?     Range                                           AUTO (including voltage range for frequency and period measurements)
+    # ?     Samples per Trigger                             1 sample
+    # ?     Trigger Count                                   1 trigger
+    # ?     Trigger Delay                                   Automatic delay
+    # ?     Trigger Source                                  Immediate
+    # ?     Trigger Slope                                   NEGative
+    # ?     Math Functions                                  Disabled. Other parameters are unchanged.
+    # ?     Per-function Null State                         Disabled
+
+    # <range>: {1 nF|10 nF|100 nF|1 µF|10 µF|100 µF}. Default:AUTO.
+    # <resolution>: optional and ignored; fixed at 4½ digits.
+    def meas_meter__Capacitance(self):
+        return float(self.meter.query('MEAS:CAP?'))
+    
+    # <range>: {100 µA|1 mA|10 mA|100 mA|1 A|3 A|10 A}. Default: AUTO(autorange).
+    # <resolution> (AC): optional and ignored; fixed at 6½ digits.
+    def meas_meter__AcCurrent(self):
+        return float(self.meter.query('MEAS:CURR:AC?'))
+    
+    # <range>: {100 µA|1 mA|10 mA|100 mA|1 A|3 A|10 A}. Default: AUTO(autorange).
+    # <resolution> (DC): optional and ignored; fixed at 6½ digits.
+    def meas_meter__DcCurrent(self):
+        return float(self.meter.query('MEAS:CURR:DC?'))
+    
+
+    # Resolution 0.001 PLC 0.002 PLC 0.006 PLC 0.02 PLC 0.06 PLC  0.2 PLC  1 PLC  10 PLC 100 PLC
+    def meas_meter__Diod(self):
+        return float(self.meter.query('MEAS:DIOD?'))
+    
+    # <range>: 100 mV, 1 V, 10 V, 100 V, 1000 V, AUTO (default) or DEFault
+    # <resolution> (DC): optional and ignored; fixed at 6½ digits.  
+    # # Resolution 0.001 PLC 0.002 PLC 0.006 PLC 0.02 PLC 0.06 PLC  0.2 PLC  1 PLC  10 PLC 100 PLC
+    def meas_meter__DcVoltage(self):
+        return float(self.meter.query('MEAS:VOLT:DC?'))
+    
+    # <range>: 100 mV, 1 V, 10 V, 100 V, 1000 V, AUTO (default) or DEFault
+    # <resolution> (DC): optional and ignored; fixed at 6½ digits.  
+    # # Resolution 0.001 PLC 0.002 PLC 0.006 PLC 0.02 PLC 0.06 PLC  0.2 PLC  1 PLC  10 PLC 100 PLC
+    def meas_meter__AcCurrent(self):
+        return float(self.meter.query('MEAS:VOLT:AC?'))
+    
+
+    #? @@@@@@@@@@@@@@@@@@@@@@@@@@@@@        Trigger Function @@@@@@@@@@@@@@@@@@@
+
+    # 0 to ~3600 seconds (~1 µs steps). Default: 1 s.
+    def set_meter__Trigger___Delay(self,delay:float):
+        self.meter.write(f'SAMP:COUN 1')
+        self.meter.write(f'TRIGger:DELay:AUTO OFF')
+        self.meter.write(f'TRIG:DEL {str(delay)}')
+        self.meter.write('CONF:VOLT:DC 1,0.0001') 
+        self.meter.write('TRIG:SOUR INT')                   
+        self.meter.write('TRIG:LEV 0.75')
+        self.meter.write('TRIG:SLOP POS')
+        self.meter.write('INIT')
+
+    # 0 to ~3600 seconds (~1 µs steps). Default: 1 s.
+    def get_meter__Trigger___Delay(self):
+        return float(self.meter.query(f'TRIG:DEL?'))
+    
+    # <level> (see bullet points below). Default: 0. 
+    def get_meter__Trigger___Level(self):
+        return float(self.meter.query(f'TRIG:LEV?'))
+    
+    # <level> (see bullet points below). Default: 0. 
+    def set_meter__Trigger___Level(self,levle:float):
+        self.meter.write(f'TRIG:LEV {str(levle)}')
+
+
+    # {ON|1|OFF|0}. Default: OFF. 0 (OFF) or 1 (ON)
+    # ?  OFF: the input impedance for DC voltage measurements is fixed at 10 MΩ for all ranges to minimize noise pickup.
+    def set_meter__OutputVoltage___ImdpedenceAuto____On(self):
+        self.meter.write(f'VOLT:IMP:AUTO ON')
+    def set_meter__OutputCurrent___ImdpedenceAuto____On(self):
+        self.meter.write(f'CURR:IMP:AUTO ON')
+
+    # ?  ON: the input impedance for DC voltage measurements varies by range. It is set to "HI-Z" (>10 GΩ) for
+    #?        the 100 mV, 1 V, and 10 V ranges to reduce the effects of measurement loading errors on these lower
+    #?        ranges. The 100 V and 1000 V ranges remain at a 10 MΩ input impedance.
+    # {ON|1|OFF|0}. Default: OFF. 0 (OFF) or 1 (ON)
+    def set_meter__OutputVoltage___ImdpedenceAuto____Off(self):
+        self.meter.write(f'VOLT:IMP:AUTO ON')
+
+    def get_meter__OutputVoltage___ImdpedenceAuto____Status(self):
+        return float(self.meter.write(f'VOLT:IMP:AUTO?'))
+
+    def set_Voltage__NPLC(self,NPLC):
+        self.meter.write(f'VOLT:DC:NPLC {str(NPLC)}')
+
+if __name__ == '__main__':
+    meter = A34461('USB0::0x2A8D::0x1401::MY57216238::INSTR')
+    # print(meter.meas_V())
+    # print(meter.meas_I())
     print(meter.fetch_meter__Reading() )
```

### Comparing `IvmInstruments-0.2.0/Instruments/Keysight_E362x.py` & `ivminstruments-0.2.2/Instruments/Keysight_E362x.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import time 
-import pyvisa as visa
-from pyvisa.attributes import *
-from pyvisa.constants import *
-
-
-class E362X:
-
-    def __init__(self,port='GPIB0::7::INSTR') -> None:
-        rm = visa.ResourceManager()
-        rm.list_resources()
-        self.supply = rm.open_resource(port)
-        # self.supply.set_visa_attribute(visa.constants.VI_ATTR_ASRL_BAUD, 9600)
-        # self.supply.set_visa_attribute(visa.constants.VI_ATTR_ASRL_DATA_BITS, 8)
-        # self.supply.set_visa_attribute(visa.constants.VI_ATTR_ASRL_STOP_BITS, VI_ASRL_STOP_TWO)
-        # self.supply.set_visa_attribute(visa.constants.VI_ATTR_ASRL_PARITY, visa.constants.VI_ASRL_PAR_NONE)
-        self.supply.read_termination = '\n'
-        self.supply.write_termination = '\n'
-
-
-    def get__IDN(self):
-        return self.supply.query('*IDN?')
-    
-    def set_supply__On(self,channel:int):
-        self.supply.write(f'OUTP ON,(@{str(channel)})')
-
-    def set_supply__Off(self,channel:int):
-        self.supply.write(f'OUTP OFF,(@{str(channel)})')
-
-    def set_supply__On__Status(self):
-        return self.supply.query(f'OUTP?')
-    
-
-    #? @@@@@@@@@@@@@@@@@ Measurements @@@@@@@@@@@@@@@@@@@
-
-    def meas_supply__Voltage(self,channel:int):
-        return float(self.supply.query(f'MEAS:VOLT? (@{str(channel)})'))
-    
-    def meas_supply__Current(self,channel:int):
-        return float(self.supply.query(f'MEAS:CURR? (@{str(channel)})'))
-    
-    
-    #? @@@@@@@@@@@@@@@@@ Protections @@@@@@@@@@@@@@@@@@@
-
-    # To set the over-voltage protection for output 1 to the maximum limit:
-    def set_supply__Voltage___protection___Max(self,channel:int):
-        self.supply.write(f'VOLT:PROT MAX(@{str(channel)})')
-    
-    # To enable the over-current protection for output 1
-    def set_supply__Current___protection__On(self,channel:int):
-        self.supply.write(f'CURR:PROT:STAT ON (@{str(channel)})')
-
-    # To clear protection for output
-    def set_supply__OutpProtection___Clear(self,channel:int):
-        self.supply.write(f'OUTP:PROT:CLE (@{str(channel)})')
-
-    # To set the remote sense relay to 4-wire sense at output
-    def set_supply__4Wire___Sense(self,channel:int):
-        self.supply.write(f'VOLT:SENS EXT (@{str(channel)})')
-
-
-    #? @@@@@@@@@@@@@@@@@@@@ Delay @@@@@@@@@@@@@@@@@@@@@@@
-    # To program turn-on and turn-off delays for outputs
-    def set_supply__Raise___Delay(self,channel:int,delay:float):
-        self.supply.write(f'UTP:DEL:RISE {str(delay)},(@{str(channel)})')
-
-    # To program turn-on and turn-off delays for outputs
-    def set_supply__Fall___Delay(self,channel:int,delay:float):
-        self.supply.write(f'UTP:DEL:FALL {str(delay)},(@{str(channel)})')
-
-    # To only include outputs 1 and 2 in a sequence:
-    def set_supply__Channels___Couple(self):
-        self.supply.write(f'OUTP:COUP:CHAN CH1,CH2')
-
-    # To enable Auto-Series mode:
-    def set_supply__Channels___Series(self):
-        self.supply.write(f'OUT:PAIR SER')
-
-    # To enable Auto-Series mode:
-    def set_supply__Channels___Parallel(self):
+import time 
+import pyvisa as visa
+from pyvisa.attributes import *
+from pyvisa.constants import *
+
+
+class E362X:
+
+    def __init__(self,port='GPIB0::7::INSTR') -> None:
+        rm = visa.ResourceManager()
+        rm.list_resources()
+        self.supply = rm.open_resource(port)
+        # self.supply.set_visa_attribute(visa.constants.VI_ATTR_ASRL_BAUD, 9600)
+        # self.supply.set_visa_attribute(visa.constants.VI_ATTR_ASRL_DATA_BITS, 8)
+        # self.supply.set_visa_attribute(visa.constants.VI_ATTR_ASRL_STOP_BITS, VI_ASRL_STOP_TWO)
+        # self.supply.set_visa_attribute(visa.constants.VI_ATTR_ASRL_PARITY, visa.constants.VI_ASRL_PAR_NONE)
+        self.supply.read_termination = '\n'
+        self.supply.write_termination = '\n'
+
+
+    def get__IDN(self):
+        return self.supply.query('*IDN?')
+    
+    def set_supply__On(self,channel:int):
+        self.supply.write(f'OUTP ON,(@{str(channel)})')
+
+    def set_supply__Off(self,channel:int):
+        self.supply.write(f'OUTP OFF,(@{str(channel)})')
+
+    def set_supply__On__Status(self):
+        return self.supply.query(f'OUTP?')
+    
+
+    #? @@@@@@@@@@@@@@@@@ Measurements @@@@@@@@@@@@@@@@@@@
+
+    def meas_supply__Voltage(self,channel:int):
+        return float(self.supply.query(f'MEAS:VOLT? (@{str(channel)})'))
+    
+    def meas_supply__Current(self,channel:int):
+        return float(self.supply.query(f'MEAS:CURR? (@{str(channel)})'))
+    
+    
+    #? @@@@@@@@@@@@@@@@@ Protections @@@@@@@@@@@@@@@@@@@
+
+    # To set the over-voltage protection for output 1 to the maximum limit:
+    def set_supply__Voltage___protection___Max(self,channel:int):
+        self.supply.write(f'VOLT:PROT MAX(@{str(channel)})')
+    
+    # To enable the over-current protection for output 1
+    def set_supply__Current___protection__On(self,channel:int):
+        self.supply.write(f'CURR:PROT:STAT ON (@{str(channel)})')
+
+    # To clear protection for output
+    def set_supply__OutpProtection___Clear(self,channel:int):
+        self.supply.write(f'OUTP:PROT:CLE (@{str(channel)})')
+
+    # To set the remote sense relay to 4-wire sense at output
+    def set_supply__4Wire___Sense(self,channel:int):
+        self.supply.write(f'VOLT:SENS EXT (@{str(channel)})')
+
+
+    #? @@@@@@@@@@@@@@@@@@@@ Delay @@@@@@@@@@@@@@@@@@@@@@@
+    # To program turn-on and turn-off delays for outputs
+    def set_supply__Raise___Delay(self,channel:int,delay:float):
+        self.supply.write(f'UTP:DEL:RISE {str(delay)},(@{str(channel)})')
+
+    # To program turn-on and turn-off delays for outputs
+    def set_supply__Fall___Delay(self,channel:int,delay:float):
+        self.supply.write(f'UTP:DEL:FALL {str(delay)},(@{str(channel)})')
+
+    # To only include outputs 1 and 2 in a sequence:
+    def set_supply__Channels___Couple(self):
+        self.supply.write(f'OUTP:COUP:CHAN CH1,CH2')
+
+    # To enable Auto-Series mode:
+    def set_supply__Channels___Series(self):
+        self.supply.write(f'OUT:PAIR SER')
+
+    # To enable Auto-Series mode:
+    def set_supply__Channels___Parallel(self):
         self.supply.write(f'OUT:PAIR PAR')
```

### Comparing `IvmInstruments-0.2.0/LICENSE` & `ivminstruments-0.2.2/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Harish Kumar Shivaramappa
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Harish Kumar Shivaramappa
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

