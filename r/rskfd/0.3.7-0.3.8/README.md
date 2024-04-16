# Comparing `tmp/rskfd-0.3.7.tar.gz` & `tmp/rskfd-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rskfd-0.3.7.tar", last modified: Fri Jan 19 12:01:59 2024, max compression
+gzip compressed data, was "rskfd-0.3.8.tar", last modified: Tue Apr 16 13:27:37 2024, max compression
```

## Comparing `rskfd-0.3.7.tar` & `rskfd-0.3.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-01-19 12:01:59.339490 rskfd-0.3.7/
--rw-rw-rw-   0        0        0     2248 2024-01-19 12:01:59.339490 rskfd-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     1386 2020-07-13 06:29:17.000000 rskfd-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2024-01-19 12:01:59.308244 rskfd-0.3.7/examples/
--rw-rw-rw-   0        0        0     3705 2023-02-16 10:45:21.000000 rskfd-0.3.7/examples/Wv2BinStream.py
--rw-rw-rw-   0        0        0      984 2023-11-21 08:38:13.000000 rskfd-0.3.7/examples/fileopening.py
--rw-rw-rw-   0        0        0     6637 2020-10-13 07:00:50.000000 rskfd-0.3.7/examples/instrumentexamples.py
--rw-rw-rw-   0        0        0     1082 2020-07-08 13:59:40.000000 rskfd-0.3.7/license.txt
-drwxrwxrwx   0        0        0        0 2024-01-19 12:01:59.308244 rskfd-0.3.7/rskfd/
--rw-rw-rw-   0        0        0     1299 2023-03-15 14:55:14.000000 rskfd-0.3.7/rskfd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-19 12:01:59.308244 rskfd-0.3.7/rskfd/helper/
--rw-rw-rw-   0        0        0     4431 2023-08-14 11:42:04.000000 rskfd-0.3.7/rskfd/helper/helper.py
-drwxrwxrwx   0        0        0        0 2024-01-19 12:01:59.323867 rskfd-0.3.7/rskfd/iq_data_handling/
--rw-rw-rw-   0        0        0    20946 2022-10-26 18:06:47.000000 rskfd-0.3.7/rskfd/iq_data_handling/iqdata.py
-drwxrwxrwx   0        0        0        0 2024-01-19 12:01:59.323867 rskfd-0.3.7/rskfd/remote_control/
--rw-rw-rw-   0        0        0    14822 2024-01-19 11:57:25.000000 rskfd-0.3.7/rskfd/remote_control/instrument.py
--rw-rw-rw-   0        0        0     1352 2022-06-15 06:04:19.000000 rskfd-0.3.7/rskfd/remote_control/instrumentRS.py
--rw-rw-rw-   0        0        0      675 2019-12-09 13:08:45.000000 rskfd-0.3.7/rskfd/remote_control/instrumentRSExceptions.py
--rw-rw-rw-   0        0        0     8506 2020-10-20 07:35:56.000000 rskfd-0.3.7/rskfd/remote_control/instrumentRS_FSW.py
--rw-rw-rw-   0        0        0     1905 2019-12-09 13:10:19.000000 rskfd-0.3.7/rskfd/remote_control/instrumentRS_VSE.py
-drwxrwxrwx   0        0        0        0 2024-01-19 12:01:59.323867 rskfd-0.3.7/rskfd/signal_generation/
--rw-rw-rw-   0        0        0     2290 2020-12-11 07:28:48.000000 rskfd-0.3.7/rskfd/signal_generation/signal_generation.py
-drwxrwxrwx   0        0        0        0 2024-01-19 12:01:59.323867 rskfd-0.3.7/rskfd/snp_handling/
--rw-rw-rw-   0        0        0     9605 2021-03-16 15:49:04.000000 rskfd-0.3.7/rskfd/snp_handling/snpfiles.py
-drwxrwxrwx   0        0        0        0 2024-01-19 12:01:59.323867 rskfd-0.3.7/rskfd.egg-info/
--rw-rw-rw-   0        0        0     2248 2024-01-19 12:01:59.000000 rskfd-0.3.7/rskfd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2024-01-19 12:01:59.000000 rskfd-0.3.7/rskfd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-19 12:01:59.000000 rskfd-0.3.7/rskfd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-01-19 12:01:59.000000 rskfd-0.3.7/rskfd.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-01-19 12:01:59.000000 rskfd-0.3.7/rskfd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-01-19 12:01:59.341494 rskfd-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1439 2024-01-19 12:01:50.000000 rskfd-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.792232 rskfd-0.3.8/
+-rw-rw-rw-   0        0        0     2248 2024-04-16 13:27:37.792232 rskfd-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1386 2020-07-13 06:29:17.000000 rskfd-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.760985 rskfd-0.3.8/examples/
+-rw-rw-rw-   0        0        0     3705 2023-02-16 10:45:21.000000 rskfd-0.3.8/examples/Wv2BinStream.py
+-rw-rw-rw-   0        0        0      984 2023-11-21 08:38:13.000000 rskfd-0.3.8/examples/fileopening.py
+-rw-rw-rw-   0        0        0     6637 2020-10-13 07:00:50.000000 rskfd-0.3.8/examples/instrumentexamples.py
+-rw-rw-rw-   0        0        0     1082 2020-07-08 13:59:40.000000 rskfd-0.3.8/license.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.760985 rskfd-0.3.8/rskfd/
+-rw-rw-rw-   0        0        0     1299 2023-03-15 14:55:14.000000 rskfd-0.3.8/rskfd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.776609 rskfd-0.3.8/rskfd/helper/
+-rw-rw-rw-   0        0        0     4389 2024-04-15 19:01:01.000000 rskfd-0.3.8/rskfd/helper/helper.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.776609 rskfd-0.3.8/rskfd/iq_data_handling/
+-rw-rw-rw-   0        0        0    21129 2024-04-16 13:07:29.000000 rskfd-0.3.8/rskfd/iq_data_handling/iqdata.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.792232 rskfd-0.3.8/rskfd/remote_control/
+-rw-rw-rw-   0        0        0    14935 2024-04-16 04:51:55.000000 rskfd-0.3.8/rskfd/remote_control/instrument.py
+-rw-rw-rw-   0        0        0     1352 2022-06-15 06:04:19.000000 rskfd-0.3.8/rskfd/remote_control/instrumentRS.py
+-rw-rw-rw-   0        0        0      675 2019-12-09 13:08:45.000000 rskfd-0.3.8/rskfd/remote_control/instrumentRSExceptions.py
+-rw-rw-rw-   0        0        0     8562 2024-04-15 13:54:25.000000 rskfd-0.3.8/rskfd/remote_control/instrumentRS_FSW.py
+-rw-rw-rw-   0        0        0     1905 2019-12-09 13:10:19.000000 rskfd-0.3.8/rskfd/remote_control/instrumentRS_VSE.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.792232 rskfd-0.3.8/rskfd/signal_generation/
+-rw-rw-rw-   0        0        0     2290 2020-12-11 07:28:48.000000 rskfd-0.3.8/rskfd/signal_generation/signal_generation.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.792232 rskfd-0.3.8/rskfd/snp_handling/
+-rw-rw-rw-   0        0        0     9605 2021-03-16 15:49:04.000000 rskfd-0.3.8/rskfd/snp_handling/snpfiles.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.792232 rskfd-0.3.8/rskfd.egg-info/
+-rw-rw-rw-   0        0        0     2248 2024-04-16 13:27:37.000000 rskfd-0.3.8/rskfd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-04-16 13:27:37.000000 rskfd-0.3.8/rskfd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 13:27:37.000000 rskfd-0.3.8/rskfd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 13:27:37.000000 rskfd-0.3.8/rskfd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2024-04-16 13:27:37.000000 rskfd-0.3.8/rskfd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-16 13:27:37.792232 rskfd-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1439 2024-04-16 13:27:01.000000 rskfd-0.3.8/setup.py
```

### Comparing `rskfd-0.3.7/PKG-INFO` & `rskfd-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rskfd
-Version: 0.3.7
+Version: 0.3.8
 Summary: Python Package for Instrument Control and Data Handling
 Home-page: https://gitlab.com/ramian/rskfd
 Download-URL: https://gitlab.com/ramian/rskfd/
 Author: Florian Ramian
 Author-email: gitlab@ramian.eu
 License: MIT
 Keywords: INSTRUMENT CONTROL,I/Q DATA,WV,IQ.TAR
```

### Comparing `rskfd-0.3.7/README.md` & `rskfd-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/examples/Wv2BinStream.py` & `rskfd-0.3.8/examples/Wv2BinStream.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/examples/fileopening.py` & `rskfd-0.3.8/examples/fileopening.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/examples/instrumentexamples.py` & `rskfd-0.3.8/examples/instrumentexamples.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/license.txt` & `rskfd-0.3.8/license.txt`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/rskfd/__init__.py` & `rskfd-0.3.8/rskfd/__init__.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/rskfd/helper/helper.py` & `rskfd-0.3.8/rskfd/helper/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,41 +15,41 @@
 
 def ShowLogFFT( data, fs = 1, MaxFftLength = 10000, bPlotRelative = True):
     """Helper function showing the magnitude of the FFT on a logarithmic scale.
     Signal length is limited to MaxFftLength to speed up FFT calculation.
     Input data is interpreted as Volts and converted to dBm."""
 
     # currently disabled
-    pass
+    # pass
 
-    # import matplotlib.pyplot as plt
-    # import numpy
-    # limiterlen = min(MaxFftLength,len(data))
-
-    # plt.ion()
-    # plt.show()
-
-    # if bPlotRelative:
-    #     mag = 20*numpy.log10(numpy.abs(numpy.fft.fftshift(numpy.fft.fft(data[:limiterlen]))))
-    #     # normalize to mean
-    #     meanmag = 10*numpy.log10( numpy.mean( numpy.power( 10, mag/10)))
-    #     mag = mag - meanmag
-    # else:
-    #     mag = 10*numpy.log10(numpy.power( numpy.abs( numpy.fft.fftshift( numpy.fft.fft( data[:limiterlen]))), 2)/50/limiterlen)+30
+    import matplotlib.pyplot as plt
+    import numpy
+    limiterlen = min(MaxFftLength,len(data))
+
+    plt.ion()
+    plt.show()
+
+    if bPlotRelative:
+        mag = 20*numpy.log10(numpy.abs(numpy.fft.fftshift(numpy.fft.fft(data[:limiterlen]))))
+        # normalize to mean
+        meanmag = 10*numpy.log10( numpy.mean( numpy.power( 10, mag/10)))
+        mag = mag - meanmag
+    else:
+        mag = 10*numpy.log10(numpy.power( numpy.abs( numpy.fft.fftshift( numpy.fft.fft( data[:limiterlen]))), 2)/50/limiterlen)+30
     
-    # freq = numpy.multiply( range( -limiterlen//2,(limiterlen+1)//2), fs/limiterlen)
-    # plt.plot(freq,mag)
-    # plt.grid( True)
-    # plt.xlabel( 'freq / Hz')
-    # if bPlotRelative:
-    #     plt.ylabel( 'relative power / dB')
-    # else:
-    #     plt.ylabel( 'power / dBm')
-    # plt.draw()
-    # plt.pause(.001)
+    freq = numpy.multiply( range( -limiterlen//2,(limiterlen+1)//2), fs/limiterlen)
+    plt.plot(freq,mag)
+    plt.grid( True)
+    plt.xlabel( 'freq / Hz')
+    if bPlotRelative:
+        plt.ylabel( 'relative power / dB')
+    else:
+        plt.ylabel( 'power / dBm')
+    plt.draw()
+    plt.pause(.001)
 
 
 
 def ConvertUnit( data, inUnit=unit.volt, outUnit=unit.dBm, impedance = 50):
     """
     ConverUnit converts a vector or scalar from an input unit to an output unit using the given impedance.
     data:       input vector or scalar; values can be complex for volts
```

### Comparing `rskfd-0.3.7/rskfd/iq_data_handling/iqdata.py` & `rskfd-0.3.8/rskfd/iq_data_handling/iqdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,80 +228,84 @@
     except:
         logging.error("File (" + FileName +") write error!" )
         
     return NumberOfSamples
 
 
 
-def ReadWv( FileName, ReadData = True):
+def ReadWv( FileName, ReadData=True, ConvertData=True):
     """Reads a WV file. Returns a list with complex numbers (I/Q) and the sampling rate
     iqiqiqList,fs = ReadWv("MyFile.wv")
-    ReadData:   if set to False, we'll only return the parameters from the header"""
-    
+    ReadData:       if set to False, we'll only return the parameters from the header
+    ConvertData:    convert to complex floating point, otherwise keep original format"""
+
     import re
     import struct
     import logging
     from numpy import NaN
 
     try:
         file = open(FileName, "rb")
-        if( ReadData):
+        if(ReadData):
             data = file.read()
         else:
             data = file.read( 30000)     # for the header, 30 kB should be sufficient
         file.close()
     except:
         logging.error( "File open error ("+ FileName+")!")
+        return
 
     binaryStart = 0
     tags = ""
     Counter = 0
     ConverterSize = 20
     while (binaryStart == 0) & (Counter < len(data)):
-        tags += data[Counter:Counter+ConverterSize].decode("ASCII","ignore")
+        tags += data[Counter:Counter+ConverterSize].decode("ASCII", "ignore")
         Counter += ConverterSize
         #{WAVEFORM-20001: #
-        res = re.search("WAVEFORM.{0,20}:.{0,3}#",tags)
-        if res != None:
+        res = re.search("WAVEFORM.{0,20}:.{0,3}#", tags)
+        if res is not None:
             binaryStart = res.span()[1]
 
     if (Counter > len(data)) & (binaryStart == 0):
-        logging.warning( "Required tags not found, potentially incompatible file format!")
+        logging.warning("Required tags not found, potentially incompatible file format!")
 
-    res = re.search("SAMPLES[ ]*:[ ]*(?P<NumberOfSamples>[0-9]*)[ ]*}",tags)
+    res = re.search("SAMPLES[ ]*:[ ]*(?P<NumberOfSamples>[0-9]*)[ ]*}", tags)
     if res:
-        NumberOfSamples = int( res.group("NumberOfSamples"))
+        NumberOfSamples = int(res.group("NumberOfSamples"))
     else:
         NumberOfSamples = NaN
     # res = re.search("CLOCK[ ]*:[ ]*(?P<SamplingRate>[0-9]*.[0-9]*[eE]?[+\-]?[0-9]*)",tags)
-    res = re.search("CLOCK[ ]*:[ ]*(?P<SamplingRate>[0-9]*.[0-9]*[eE]?[+\-]?[0-9]*)[ ]*}",tags)
+    res = re.search("CLOCK[ ]*:[ ]*(?P<SamplingRate>[0-9]*.[0-9]*[eE]?[+\-]?[0-9]*)[ ]*}", tags)
     if res:
-        SamplingRate = float( res.group("SamplingRate"))
+        SamplingRate = float(res.group("SamplingRate"))
     else:
         SamplingRate = NaN
-    res = re.search("LEVEL OFFS[ ]*:[ ]*(?P<RMSLevelOffset>[0-9]*.?[0-9]*),",tags)
+    res = re.search("LEVEL OFFS[ ]*:[ ]*(?P<RMSLevelOffset>[0-9]*.?[0-9]*),", tags)
     if res:
-        RmsLevelOffset = float( res.group("RMSLevelOffset"))
+        RmsLevelOffset = float(res.group("RMSLevelOffset"))
     else:
         RmsLevelOffset = NaN
-    res = re.search("Signal generated for SMx RMS level[ ]*:[ ]*(?P<RfRmsLevel>-?[0-9]*.?[0-9]*)[ ]*",tags)
+    res = re.search("Signal generated for SMx RMS level[ ]*:[ ]*(?P<RfRmsLevel>-?[0-9]*.?[0-9]*)[ ]*", tags)
     if res:
-        RfRmsLevel = float( res.group("RfRmsLevel"))
+        RfRmsLevel = float(res.group("RfRmsLevel"))
     else:
         RfRmsLevel = NaN
 
-    if ReadData:
+    if ReadData and ConvertData:
         data = list(struct.unpack("h"*NumberOfSamples*2, data[binaryStart:binaryStart+NumberOfSamples*4]))
-        data = list(map( lambda x: x/32767.0, data ))
-        data = Iqiq2Complex( data)
-    
+        data = list(map( lambda x: x/32767.0, data))
+        data = Iqiq2Complex(data)
+    else:
+        data = data[binaryStart:]
+
     if ReadData:
-        return data,SamplingRate
+        return data, SamplingRate
     else:
-        return SamplingRate,NumberOfSamples,RmsLevelOffset,RfRmsLevel
+        return SamplingRate, NumberOfSamples, RmsLevelOffset, RfRmsLevel
 
 
 
 def __WriteXml( fs, NumberOfSamples, filenameiqw, filenamexml, fCenterFrequency = 0):
     """Function to write the xml part of the iq.tar
     __WriteXml( samplingrate, numberofsamples, filenameiqw, filenamexml)"""
```

### Comparing `rskfd-0.3.7/rskfd/remote_control/instrument.py` & `rskfd-0.3.8/rskfd/remote_control/instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,19 @@
 
         if self.__msocket is None:
             raise Exception('Connection is closed, use connect first!')
 
         if NumberOfBytes == -1:
             NumberOfBytes = self._InBufferSize
 
-        data = self.__msocket.recv(NumberOfBytes)
+        try:
+            data = self.__msocket.recv(NumberOfBytes)
+        except:
+            logging.warn("Timeout while reading data!")
+            return None
 
         if decode:
             try:
                 data = data.decode("ASCII")
                 if data.endswith("\n"):
                     data = data[:-1]
             except:
@@ -301,18 +305,18 @@
                 data = str(len(data)) + " binary bytes"
 
             if self.__LogReadings:
                 self.___LogToFile( data)
         else:
             if self.__LogReadings:
                 self.___LogToFile( "{} bytes of binary data read".format(len(data))) 
+        
         return data
-    
-    
-    
+
+
     def Query( self, Command):
         """Write command and read result from connected instrument"""
         
         self.Write( Command)
         data = self.Read()
         
         return data
```

### Comparing `rskfd-0.3.7/rskfd/remote_control/instrumentRS.py` & `rskfd-0.3.8/rskfd/remote_control/instrumentRS.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/rskfd/remote_control/instrumentRSExceptions.py` & `rskfd-0.3.8/rskfd/remote_control/instrumentRSExceptions.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/rskfd/remote_control/instrumentRS_FSW.py` & `rskfd-0.3.8/rskfd/remote_control/instrumentRS_FSW.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,21 +100,23 @@
             localfile:  file name on local machine; file extension automatically sets file type
 
         Supported file types:
             png, jpg, wmf, bmp
         """
         import os
 
-        remotefile = "C:\\temp\\temp"
+        remotefile = r"C:\temp\temp"
         # store current display update mode
         dispupdate = self.Query("SYST:DISP:UPD?")
         # display update on
         self.Write("SYST:DISP:UPD ON")
         # softkeys off
         self.Write("DISP:SKEY:STAT OFF")
+        # logo off
+        self.Write("DISP:LOGO OFF")
         # screencolor, no color change
         self.Write("HCOP:CMAP:DEF4")
         # No timestamp
         self.Write("HCOP:TDST:STAT OFF")
         # destination mass memory MMEM
         self.Write("HCOP:DEST 'MMEM'")
         # format
```

### Comparing `rskfd-0.3.7/rskfd/remote_control/instrumentRS_VSE.py` & `rskfd-0.3.8/rskfd/remote_control/instrumentRS_VSE.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/rskfd/signal_generation/signal_generation.py` & `rskfd-0.3.8/rskfd/signal_generation/signal_generation.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/rskfd/snp_handling/snpfiles.py` & `rskfd-0.3.8/rskfd/snp_handling/snpfiles.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/rskfd.egg-info/PKG-INFO` & `rskfd-0.3.8/rskfd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rskfd
-Version: 0.3.7
+Version: 0.3.8
 Summary: Python Package for Instrument Control and Data Handling
 Home-page: https://gitlab.com/ramian/rskfd
 Download-URL: https://gitlab.com/ramian/rskfd/
 Author: Florian Ramian
 Author-email: gitlab@ramian.eu
 License: MIT
 Keywords: INSTRUMENT CONTROL,I/Q DATA,WV,IQ.TAR
```

### Comparing `rskfd-0.3.7/rskfd.egg-info/SOURCES.txt` & `rskfd-0.3.8/rskfd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.7/setup.py` & `rskfd-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   long_description = filein.read()
 
 setuptools.setup(
   name = 'rskfd',
   #packages = ['rskfd','rskfd.remote_control','rskfd.iq_data_handling','rskfd.signal_generation','rskfd.helper'],
   #packages = setuptools.find_packages(),
   packages = setuptools.find_namespace_packages(),
-  version = '0.3.7',
+  version = '0.3.8',
   license='MIT',
   description = 'Python Package for Instrument Control and Data Handling',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   author = 'Florian Ramian', 
   author_email = 'gitlab@ramian.eu',
   url = 'https://gitlab.com/ramian/rskfd',   # gitlab
```

