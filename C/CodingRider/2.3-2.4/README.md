# Comparing `tmp/CodingRider-2.3.tar.gz` & `tmp/codingrider-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodingRider-2.3.tar", last modified: Tue Apr  9 06:23:53 2024, max compression
+gzip compressed data, was "codingrider-2.4.tar", last modified: Mon May 13 07:26:43 2024, max compression
```

## Comparing `CodingRider-2.3.tar` & `codingrider-2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 06:23:53.799744 CodingRider-2.3/
-drwxrwxrwx   0        0        0        0 2024-04-09 06:23:53.790837 CodingRider-2.3/CodingRider/
--rw-rw-rw-   0        0        0      109 2024-04-05 06:35:16.000000 CodingRider-2.3/CodingRider/__init__.py
--rw-rw-rw-   0        0        0      484 2023-12-25 23:04:18.000000 CodingRider-2.3/CodingRider/__main__.py
--rw-rw-rw-   0        0        0     4609 2023-03-28 08:35:12.000000 CodingRider-2.3/CodingRider/crc.py
--rw-rw-rw-   0        0        0    44020 2024-04-05 00:11:47.000000 CodingRider-2.3/CodingRider/drone.py
--rw-rw-rw-   0        0        0    73925 2024-04-09 06:19:26.000000 CodingRider-2.3/CodingRider/protocol.py
--rw-rw-rw-   0        0        0     7088 2023-11-15 01:18:50.000000 CodingRider-2.3/CodingRider/receiver.py
--rw-rw-rw-   0        0        0     1904 2023-12-25 23:03:04.000000 CodingRider-2.3/CodingRider/storage.py
--rw-rw-rw-   0        0        0    10249 2023-03-28 08:35:12.000000 CodingRider-2.3/CodingRider/system.py
-drwxrwxrwx   0        0        0        0 2024-04-09 06:23:53.798144 CodingRider-2.3/CodingRider.egg-info/
--rw-rw-rw-   0        0        0      626 2024-04-09 06:23:53.000000 CodingRider-2.3/CodingRider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-04-09 06:23:53.000000 CodingRider-2.3/CodingRider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 06:23:53.000000 CodingRider-2.3/CodingRider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-09 06:23:53.000000 CodingRider-2.3/CodingRider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 06:23:53.000000 CodingRider-2.3/CodingRider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-03-28 08:35:12.000000 CodingRider-2.3/LICENSE
--rw-rw-rw-   0        0        0       36 2023-03-28 08:35:12.000000 CodingRider-2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      626 2024-04-09 06:23:53.798736 CodingRider-2.3/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-11-15 03:15:25.000000 CodingRider-2.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 06:23:53.799744 CodingRider-2.3/setup.cfg
--rw-rw-rw-   0        0        0      772 2024-04-09 06:16:55.000000 CodingRider-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:26:43.962782 codingrider-2.4/
+drwxrwxrwx   0        0        0        0 2024-05-13 07:26:43.949356 codingrider-2.4/CodingRider/
+-rw-rw-rw-   0        0        0      109 2024-05-13 04:58:42.000000 codingrider-2.4/CodingRider/__init__.py
+-rw-rw-rw-   0        0        0      484 2024-05-13 04:58:42.000000 codingrider-2.4/CodingRider/__main__.py
+-rw-rw-rw-   0        0        0     4609 2024-05-13 04:58:42.000000 codingrider-2.4/CodingRider/crc.py
+-rw-rw-rw-   0        0        0    44020 2024-05-13 04:58:42.000000 codingrider-2.4/CodingRider/drone.py
+-rw-rw-rw-   0        0        0    64836 2024-05-13 06:07:28.000000 codingrider-2.4/CodingRider/protocol.py
+-rw-rw-rw-   0        0        0     7088 2024-05-13 05:16:52.000000 codingrider-2.4/CodingRider/receiver.py
+-rw-rw-rw-   0        0        0     1904 2024-05-13 04:58:42.000000 codingrider-2.4/CodingRider/storage.py
+-rw-rw-rw-   0        0        0    10249 2024-05-13 04:58:42.000000 codingrider-2.4/CodingRider/system.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:26:43.961633 codingrider-2.4/CodingRider.egg-info/
+-rw-rw-rw-   0        0        0      718 2024-05-13 07:26:43.000000 codingrider-2.4/CodingRider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-13 07:26:43.000000 codingrider-2.4/CodingRider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 07:26:43.000000 codingrider-2.4/CodingRider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-13 07:26:43.000000 codingrider-2.4/CodingRider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-13 07:26:43.000000 codingrider-2.4/CodingRider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-13 04:58:42.000000 codingrider-2.4/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-13 04:58:42.000000 codingrider-2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      718 2024-05-13 07:26:43.962782 codingrider-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-13 04:58:42.000000 codingrider-2.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 07:26:43.962782 codingrider-2.4/setup.cfg
+-rw-rw-rw-   0        0        0      772 2024-05-13 07:10:29.000000 codingrider-2.4/setup.py
```

### Comparing `CodingRider-2.3/CodingRider/crc.py` & `codingrider-2.4/CodingRider/crc.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.3/CodingRider/drone.py` & `codingrider-2.4/CodingRider/drone.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.3/CodingRider/protocol.py` & `codingrider-2.4/CodingRider/protocol.py`

 * *Files 14% similar despite different names*

```diff
@@ -1525,414 +1525,14 @@
         data.colors     = Colors(data.colors)
 
         return data
 
 
 # Light End
 
-
-
-# Display Start
-
-
-class DisplayPixel(Enum):
-    
-    Black               = 0x00
-    White               = 0x01
-    Inverse             = 0x02
-    Outline             = 0x03
-
-
-
-class DisplayFont(Enum):
-    
-    LiberationMono5x8   = 0x00
-    LiberationMono10x16 = 0x01
-
-
-
-class DisplayAlign(Enum):
-    
-    Left                = 0x00
-    Center              = 0x01
-    Right               = 0x02
-
-
-
-class DisplayLine(Enum):
-    
-    Solid               = 0x00
-    Dotted              = 0x01
-    Dashed              = 0x02
-
-
-
-class DisplayClearAll(ISerializable):
-
-    def __init__(self):
-        self.pixel       = DisplayPixel.White
-
-
-    @classmethod
-    def getSize(cls):
-        return 1
-
-
-    def toArray(self):
-        return pack('<B', self.pixel.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayClearAll()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.pixel, = unpack('<B', dataArray)
-        data.pixel  = DisplayPixel(data.pixel)
-        
-        return data
-
-
-
-class DisplayClear(ISerializable):
-
-    def __init__(self):
-        self.x           = 0
-        self.y           = 0
-        self.width       = 0
-        self.height      = 0
-        self.pixel       = DisplayPixel.White
-
-
-    @classmethod
-    def getSize(cls):
-        return 9
-
-
-    def toArray(self):
-        return pack('<hhhhB', self.x, self.y, self.width, self.height, self.pixel.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayClear()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x, data.y, data.width, data.height, data.pixel = unpack('<hhhhB', dataArray)
-
-        data.pixel = DisplayPixel(data.pixel)
-        
-        return data
-
-
-
-class DisplayInvert(ISerializable):
-
-    def __init__(self):
-        self.x           = 0
-        self.y           = 0
-        self.width       = 0
-        self.height      = 0
-
-
-    @classmethod
-    def getSize(cls):
-        return 8
-
-
-    def toArray(self):
-        return pack('<hhhh', self.x, self.y, self.width, self.height)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayInvert()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x, data.y, data.width, data.height = unpack('<hhhh', dataArray)
-        
-        return data
-
-
-
-class DisplayDrawPoint(ISerializable):
-
-    def __init__(self):
-        self.x           = 0
-        self.y           = 0
-        self.pixel       = DisplayPixel.White
-
-
-    @classmethod
-    def getSize(cls):
-        return 5
-
-
-    def toArray(self):
-        return pack('<hhB', self.x, self.y, self.pixel.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawPoint()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x, data.y, data.pixel = unpack('<hhB', dataArray)
-
-        data.pixel = DisplayPixel(data.pixel)
-        
-        return data
-
-
-
-class DisplayDrawLine(ISerializable):
-
-    def __init__(self):
-        self.x1          = 0
-        self.y1          = 0
-        self.x2          = 0
-        self.y2          = 0
-        self.pixel       = DisplayPixel.White
-        self.line        = DisplayLine.Solid
-
-
-    @classmethod
-    def getSize(cls):
-        return 10
-
-
-    def toArray(self):
-        return pack('<hhhhBB', self.x1, self.y1, self.x2, self.y2, self.pixel.value, self.line.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawLine()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x1, data.y1, data.x2, data.y2, data.pixel, data.line = unpack('<hhhhBB', dataArray)
-
-        data.pixel  = DisplayPixel(data.pixel)
-        data.line   = DisplayLine(data.line)
-        
-        return data
-
-
-
-class DisplayDrawRect(ISerializable):
-
-    def __init__(self):
-        self.x          = 0
-        self.y          = 0
-        self.width      = 0
-        self.height     = 0
-        self.pixel      = DisplayPixel.White
-        self.flagFill   = True
-        self.line       = DisplayLine.Solid
-
-
-    @classmethod
-    def getSize(cls):
-        return 11
-
-
-    def toArray(self):
-        return pack('<hhhhB?B', self.x, self.y, self.width, self.height, self.pixel.value, self.flagFill, self.line.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawRect()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x, data.y, data.width, data.height, data.pixel, data.flagFill, data.line = unpack('<hhhhB?B', dataArray)
-
-        data.pixel  = DisplayPixel(data.pixel)
-        data.line   = DisplayLine(data.line)
-        
-        return data
-
-
-
-class DisplayDrawCircle(ISerializable):
-
-    def __init__(self):
-        self.x          = 0
-        self.y          = 0
-        self.radius     = 0
-        self.pixel      = DisplayPixel.White
-        self.flagFill   = True
-
-
-    @classmethod
-    def getSize(cls):
-        return 8
-
-
-    def toArray(self):
-        return pack('<hhhB?', self.x, self.y, self.radius, self.pixel.value, self.flagFill)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawCircle()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x, data.y, data.radius, data.pixel, data.flagFill = unpack('<hhhB?', dataArray)
-
-        data.pixel = DisplayPixel(data.pixel)
-        
-        return data
-
-
-
-class DisplayDrawString(ISerializable):
-
-    def __init__(self):
-        self.x          = 0
-        self.y          = 0
-        self.font       = DisplayFont.LiberationMono5x8
-        self.pixel      = DisplayPixel.White
-        self.message    = ""
-
-
-    @classmethod
-    def getSize(cls):
-        return 6
-
-
-    def getSizeTotal(self):
-        return self.getSize() + len(self.message)
-
-
-    def toArray(self):
-        dataArray = bytearray()
-        dataArray.extend(pack('<hhBB', self.x, self.y, self.font.value, self.pixel.value))
-        dataArray.extend(self.message.encode('ascii', 'ignore'))
-        return dataArray
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawString()
-        
-        if len(dataArray) <= cls.getSize():
-            return None
-
-        data.x, data.y, data.font, data.pixel = unpack('<hhBB', dataArray[0:cls.getSize()])
-
-        data.font       = DisplayFont(data.font)
-        data.pixel      = DisplayPixel(data.pixel)
-        data.message    = dataArray[cls.getSize():len(dataArray)].decode()
-        
-        return data
-
-
-
-class DisplayDrawStringAlign(ISerializable):
-
-    def __init__(self):
-        
-        self.x_start    = 0
-        self.x_end      = 0
-        self.y          = 0
-        self.align      = DisplayAlign.Center
-        self.font       = DisplayFont.LiberationMono5x8
-        self.pixel      = DisplayPixel.White
-        self.message    = ""
-
-
-    @classmethod
-    def getSize(cls):
-        return 9
-
-
-
-    def getSizeTotal(self):
-        return self.getSize() + len(self.message)
-
-
-
-    def toArray(self):
-        dataArray = bytearray()
-        dataArray.extend(pack('<hhhBBB', self.x_start, self.x_end, self.y, self.align.value, self.font.value, self.pixel.value))
-        dataArray.extend(self.message.encode('ascii', 'ignore'))
-        return dataArray
-    
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawStringAlign()
-        
-        if len(dataArray) <= cls.getSize():
-            return None
-
-        data.x_start, data.x_end, data.y, data.align, data.font, data.pixel, data.message = unpack('<hhhBBBs', dataArray[0:cls.getSize()])
-        data.align = DisplayAlign(data.align)
-        data.font = DisplayFont(data.font)
-        data.pixel = DisplayPixel(data.pixel)
-        data.message = dataArray[cls.getSize():len(dataArray)].decode()
-        
-        return data
-
-
-
-class DisplayImage(ISerializable):
-
-    def __init__(self):
-        self.x          = 0
-        self.y          = 0
-        self.width      = 0
-        self.height     = 0
-        self.image      = bytearray()
-
-
-    @classmethod
-    def getSize(cls):
-        return 8
-
-
-    def toArray(self):
-        dataArray = bytearray()
-        dataArray.extend(pack('<hhhh', self.x, self.y, self.width, self.height))
-        dataArray.extend(self.image)
-        return dataArray
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayImage()
-        
-        if len(dataArray) <= cls.getSize():
-            return None
-
-        data.x, data.y, data.width, data.height = unpack('<hhhh', dataArray)
-        data.image = dataArray[cls.getSize():(len(dataArray) - cls.getSize())]
-        
-        return data
-
-
-# Display End
-
-
-
 # Buzzer Start
 
 
 class BuzzerMode(Enum):
 
     Stop                = 0     # 정지(Mode에서의 Stop은 통신에서 받았을 때 Buzzer를 끄는 용도로 사용, set으로만 호출)
```

### Comparing `CodingRider-2.3/CodingRider/receiver.py` & `codingrider-2.4/CodingRider/receiver.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.3/CodingRider/storage.py` & `codingrider-2.4/CodingRider/storage.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.3/CodingRider/system.py` & `codingrider-2.4/CodingRider/system.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.3/setup.py` & `codingrider-2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # http://swdeveloper.tistory.com/34
 # https://code.tutsplus.com/ko/tutorials/how-to-share-your-python-packages--cms-26114
 # https://code.tutsplus.com/ko/tutorials/how-to-write-your-own-python-packages--cms-26076
 from setuptools import setup, find_packages
 
 setup(
     name = "CodingRider",
-    version = "2.3",
+    version = "2.4",
     description = "Library for CodingRider",
     author = "ALUX",
     author_email = "devdrone@aluxonline.com",
     url = "https://imssam.me/shop/view.php?index_no=4031",
     packages = find_packages(exclude=['tests']),
     install_requires = [
         'pyserial>=3.4',
```

