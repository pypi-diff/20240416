# Comparing `tmp/python-sscma-0.2.1.tar.gz` & `tmp/python-sscma-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sscma-0.2.1.tar", last modified: Fri Jan  5 10:44:05 2024, max compression
+gzip compressed data, was "python-sscma-0.5.0.tar", last modified: Tue Apr 16 07:00:47 2024, max compression
```

## Comparing `python-sscma-0.2.1.tar` & `python-sscma-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-01-05 10:44:05.250620 python-sscma-0.2.1/
--rw-rw-rw-   0        0        0     2816 2024-01-05 10:44:05.249622 python-sscma-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2316 2024-01-05 06:15:33.000000 python-sscma-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-05 10:44:05.234207 python-sscma-0.2.1/python_sscma.egg-info/
--rw-rw-rw-   0        0        0     2816 2024-01-05 10:44:05.000000 python-sscma-0.2.1/python_sscma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2024-01-05 10:44:05.000000 python-sscma-0.2.1/python_sscma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-05 10:44:05.000000 python-sscma-0.2.1/python_sscma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-01-05 10:44:05.000000 python-sscma-0.2.1/python_sscma.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-05 10:44:05.250620 python-sscma-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-01-05 06:37:15.000000 python-sscma-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-05 10:44:05.234207 python-sscma-0.2.1/sscma/
--rw-rw-rw-   0        0        0       42 2024-01-05 10:43:00.000000 python-sscma-0.2.1/sscma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-05 10:44:05.235217 python-sscma-0.2.1/sscma/fonts/
--rw-rw-rw-   0        0        0  1580784 2024-01-05 06:01:46.000000 python-sscma-0.2.1/sscma/fonts/Arial.ttf
-drwxrwxrwx   0        0        0        0 2024-01-05 10:44:05.244221 python-sscma-0.2.1/sscma/micro/
--rw-rw-rw-   0        0        0      341 2024-01-05 06:01:46.000000 python-sscma-0.2.1/sscma/micro/__init__.py
--rw-rw-rw-   0        0        0    13707 2024-01-05 10:15:02.000000 python-sscma-0.2.1/sscma/micro/client.py
--rw-rw-rw-   0        0        0     4730 2024-01-05 06:15:11.000000 python-sscma-0.2.1/sscma/micro/const.py
--rw-rw-rw-   0        0        0    24553 2024-01-05 10:41:04.000000 python-sscma-0.2.1/sscma/micro/device.py
--rw-rw-rw-   0        0        0     1231 2024-01-05 06:01:46.000000 python-sscma-0.2.1/sscma/micro/exceptions.py
--rw-rw-rw-   0        0        0    10869 2024-01-05 06:01:46.000000 python-sscma-0.2.1/sscma/micro/info.py
-drwxrwxrwx   0        0        0        0 2024-01-05 10:44:05.248609 python-sscma-0.2.1/tests/
--rw-rw-rw-   0        0        0      122 2024-01-05 06:01:46.000000 python-sscma-0.2.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2239 2024-01-05 06:15:33.000000 python-sscma-0.2.1/tests/test_mqtt.py
--rw-rw-rw-   0        0        0     2040 2024-01-05 10:22:46.000000 python-sscma-0.2.1/tests/test_mqttclient.py
--rw-rw-rw-   0        0        0     2135 2024-01-05 06:15:33.000000 python-sscma-0.2.1/tests/test_serial.py
--rw-rw-rw-   0        0        0     1540 2024-01-05 06:20:11.000000 python-sscma-0.2.1/tests/test_serialclient.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.044881 python-sscma-0.5.0/
+-rw-rw-rw-   0        0        0     2914 2024-04-16 07:00:47.044881 python-sscma-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2396 2024-04-16 06:53:08.000000 python-sscma-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.014584 python-sscma-0.5.0/python_sscma.egg-info/
+-rw-rw-rw-   0        0        0     2914 2024-04-16 07:00:46.000000 python-sscma-0.5.0/python_sscma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2024-04-16 07:00:46.000000 python-sscma-0.5.0/python_sscma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 07:00:46.000000 python-sscma-0.5.0/python_sscma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-16 07:00:46.000000 python-sscma-0.5.0/python_sscma.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 07:00:46.000000 python-sscma-0.5.0/python_sscma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 07:00:47.044881 python-sscma-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1148 2024-04-16 06:56:43.000000 python-sscma-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.015585 python-sscma-0.5.0/sscma/
+-rw-rw-rw-   0        0        0       42 2024-04-16 06:59:44.000000 python-sscma-0.5.0/sscma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.019587 python-sscma-0.5.0/sscma/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-16 06:11:20.000000 python-sscma-0.5.0/sscma/cli/__init__.py
+-rw-rw-rw-   0        0        0      253 2024-04-16 06:30:55.000000 python-sscma-0.5.0/sscma/cli/cli.py
+-rw-rw-rw-   0        0        0     4773 2024-04-16 06:49:24.000000 python-sscma-0.5.0/sscma/cli/client.py
+-rw-rw-rw-   0        0        0     2367 2024-04-16 06:12:54.000000 python-sscma-0.5.0/sscma/cli/flahser.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.023586 python-sscma-0.5.0/sscma/flashers/
+-rw-rw-rw-   0        0        0       73 2024-04-16 06:11:41.000000 python-sscma-0.5.0/sscma/flashers/__init__.py
+-rw-rw-rw-   0        0        0      768 2024-04-16 06:01:44.000000 python-sscma-0.5.0/sscma/flashers/base.py
+-rw-rw-rw-   0        0        0     5161 2024-04-16 06:09:27.000000 python-sscma-0.5.0/sscma/flashers/core.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.025586 python-sscma-0.5.0/sscma/fonts/
+-rw-rw-rw-   0        0        0  1580784 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/fonts/Arial.ttf
+drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.033878 python-sscma-0.5.0/sscma/micro/
+-rw-rw-rw-   0        0        0      341 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/micro/__init__.py
+-rw-rw-rw-   0        0        0    13707 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/micro/client.py
+-rw-rw-rw-   0        0        0     4730 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/micro/const.py
+-rw-rw-rw-   0        0        0    24553 2024-04-16 06:21:15.000000 python-sscma-0.5.0/sscma/micro/device.py
+-rw-rw-rw-   0        0        0     1231 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/micro/exceptions.py
+-rw-rw-rw-   0        0        0    10869 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/micro/info.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.036879 python-sscma-0.5.0/sscma/utils/
+-rw-rw-rw-   0        0        0        0 2024-01-11 03:24:44.000000 python-sscma-0.5.0/sscma/utils/__init__.py
+-rw-rw-rw-   0        0        0      844 2024-01-11 03:24:44.000000 python-sscma-0.5.0/sscma/utils/image.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.043877 python-sscma-0.5.0/tests/
+-rw-rw-rw-   0        0        0      122 2024-04-16 05:34:06.000000 python-sscma-0.5.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2239 2024-04-16 05:34:06.000000 python-sscma-0.5.0/tests/test_mqtt.py
+-rw-rw-rw-   0        0        0     2039 2024-04-16 05:34:06.000000 python-sscma-0.5.0/tests/test_mqttclient.py
+-rw-rw-rw-   0        0        0     2135 2024-04-16 05:34:06.000000 python-sscma-0.5.0/tests/test_serial.py
+-rw-rw-rw-   0        0        0     1540 2024-04-16 05:34:06.000000 python-sscma-0.5.0/tests/test_serialclient.py
```

### Comparing `python-sscma-0.2.1/README.md` & `python-sscma-0.5.0/tests/test_mqttclient.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,90 @@
-# Python SSCMA-Micro
-
-## Description
-
-This is a client for the
-[sscma_micro](https://github.com/Seeed-Studio/sscma_micro), which is a
-microcontroller at server for the [SSCMA](https://github.com/Seeed-Studio/SSCMA)
-models.
-
-More information about the sscma_micro can be found at
-[here](https://github.com/Seeed-Studio/sscma_micro/blob/dev/docs/protocol/at_protocol.md)
-
-## Usage
-
-### Install
+import paho.mqtt.client as mqtt
+import time
 
-```bash
-pip install python-sscma
-```
-```python
-from sscma.micro.client import Client, SerialClient
+from sscma.micro.client import MQTTClient
 from sscma.micro.device import Device
 from sscma.micro.const import *
-import serial
-import threading
 import time
 import logging
-import signal
 import cv2
 import base64
 import numpy as np
+import signal
 
 logging.basicConfig(level=logging.DEBUG)
 
 _LOGGER = logging.getLogger(__name__)
 
 
+# 定义代理服务器和主题
+broker_address = "192.168.6.149"
+rx_topic = "sscma/v0/grove_vision_ai_we2_bdf65343/tx"
+tx_topic = "sscma/v0/grove_vision_ai_we2_bdf65343/rx"
+
+
+def on_connect(client, userdata, flags, rc):
+    print("Connected with result code "+str(rc))
+    client.subscribe(rx_topic)
+
+
+def on_message(client, tclient, msg):
+    tclient.on_recieve(msg.payload)
+
+
 def monitor_handler(device, msg):
+
     if "image" in msg:
         jpeg_bytes = base64.b64decode(msg["image"])
 
         # Convert the bytes into a numpy array
         nparr = np.frombuffer(jpeg_bytes, np.uint8)
 
         # Decode the image array using OpenCV
         img = cv2.imdecode(nparr, cv2.IMREAD_COLOR)
 
         # Display the image
         cv2.imshow('Base64 Image', img)
         cv2.waitKey(1)
         msg.pop("image")
+
     print(msg)
 
 
 def on_device_connect(device):
     print("device connected")
     device.Invoke(-1, False, True)
-    device.tscore = 70
-    device.tiou = 70
+    device.tscore = 50
+    device.tiou = 35
+
 
+device = Device(MQTTClient(host=broker_address, port=1883, tx_topic=tx_topic,
+                           rx_topic=rx_topic, username="sscma", password="sscma"))
 
-client = SerialClient("COM83")
 
 def signal_handler(signal, frame):
-    print("Ctrl+C pressed!")
-    client.loop_stop()
-   
-def main():
+    device.loop_stop()
+    exit(0)
 
-    signal.signal(signal.SIGINT, signal_handler)
- 
-    device = Device(client)
+
+def main():
 
     device.on_monitor = monitor_handler
     device.on_connect = on_device_connect
-     
     device.loop_start()
 
-    print(device.info)
+    signal.signal(signal.SIGINT, signal_handler)
 
     i = 60
-
     while True:
-        print(device.wifi)
-        print(device.mqtt)
-        print(device.info)
-        print(device.model)
-        device.tscore = i
-        device.tiou = i
-        i = i + 1
-        if i > 100:
-            i = 30
+        print("model:{}".format(device.model))
+        # device.tscore = i
+        # device.tiou = i
+        # i = i + 1
+        # if i > 100:
+        #     i = 30
 
         time.sleep(2)
 
 
 if __name__ == "__main__":
     main()
-
-```
-
-## Contributing
-
-If you have any idea or suggestion, please open an issue first.
-
-If you want to contribute code, please fork this repository and submit a pull
-request.
-
-## License
-
-MIT License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-sscma-0.2.1/setup.py` & `python-sscma-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import setuptools
 from setuptools import find_packages
 import re
 
 with open("./sscma/__init__.py", 'r') as f:
     content = f.read()
-    # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='python-sscma',
     version=version,
     author='Seeed Studio',
     author_email='lht856@foxmail.com',
-    description='<INSERT_DESCRIPTION>',
+    description='Python library for sscma',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Seeed-Studio/python-sscma',
     packages=find_packages(),
     package_data={'sscma': ['fonts/*.ttf']},
     install_requires=[],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-    ]
+    ],
+    license='MIT',
+    entry_points={
+        'console_scripts': [
+            'sscma.cli = sscma.cli.cli:main',
+        ]
+    }
 )
```

### Comparing `python-sscma-0.2.1/sscma/fonts/Arial.ttf` & `python-sscma-0.5.0/sscma/fonts/Arial.ttf`

 * *Files identical despite different names*

### Comparing `python-sscma-0.2.1/sscma/micro/client.py` & `python-sscma-0.5.0/sscma/micro/client.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.2.1/sscma/micro/const.py` & `python-sscma-0.5.0/sscma/micro/const.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.2.1/sscma/micro/device.py` & `python-sscma-0.5.0/sscma/micro/device.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.2.1/sscma/micro/exceptions.py` & `python-sscma-0.5.0/sscma/micro/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.2.1/sscma/micro/info.py` & `python-sscma-0.5.0/sscma/micro/info.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.2.1/tests/test_mqtt.py` & `python-sscma-0.5.0/tests/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.2.1/tests/test_mqttclient.py` & `python-sscma-0.5.0/tests/test_serial.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,92 @@
-import paho.mqtt.client as mqtt
-import time
-
-from sscma.micro.client import MQTTClient
+from sscma.micro.client import Client
 from sscma.micro.device import Device
 from sscma.micro.const import *
+import serial
+import threading
 import time
 import logging
+import signal
 import cv2
 import base64
 import numpy as np
-import signal
 
-logging.basicConfig(level=logging.INFO)
+logging.basicConfig(level=logging.DEBUG)
 
 _LOGGER = logging.getLogger(__name__)
 
+recieve_thread_running = True
 
-# 定义代理服务器和主题
-broker_address = "192.168.199.230"
-rx_topic = "sscma/v0/grove_vision_ai_we2_bdf65343/tx"
-tx_topic = "sscma/v0/grove_vision_ai_we2_bdf65343/rx"
 
-
-def on_connect(client, userdata, flags, rc):
-    print("Connected with result code "+str(rc))
-    client.subscribe(rx_topic)
-
-
-def on_message(client, tclient, msg):
-    tclient.on_recieve(msg.payload)
+def recieve_thread(serial_port, client):
+    while recieve_thread_running:
+        if serial_port.in_waiting:
+            msg = serial_port.read(serial_port.in_waiting)
+            if msg != b'':
+                client.on_recieve(msg)
 
 
 def monitor_handler(device, msg):
-
     if "image" in msg:
         jpeg_bytes = base64.b64decode(msg["image"])
 
         # Convert the bytes into a numpy array
         nparr = np.frombuffer(jpeg_bytes, np.uint8)
 
         # Decode the image array using OpenCV
         img = cv2.imdecode(nparr, cv2.IMREAD_COLOR)
 
         # Display the image
         cv2.imshow('Base64 Image', img)
         cv2.waitKey(1)
         msg.pop("image")
-
     print(msg)
 
 
 def on_device_connect(device):
     print("device connected")
     device.Invoke(-1, False, True)
-    device.tscore = 50
-    device.tiou = 35
-
-
-device = Device(MQTTClient(host=broker_address, port=1883, tx_topic=tx_topic,
-                           rx_topic=rx_topic, username="user", password="user"))
+    device.tscore = 70
+    device.tiou = 70
 
 
 def signal_handler(signal, frame):
-    device.loop_stop()
+    print("Ctrl+C pressed!")
+    global recieve_thread_running
+    recieve_thread_running = False
     exit(0)
 
 
 def main():
+    signal.signal(signal.SIGINT, signal_handler)
+    serial_port = serial.Serial("COM83", 921600, timeout=0.1)
+    client = Client(lambda msg: serial_port.write(msg))
+    threading.Thread(target=recieve_thread, args=(
+        serial_port, client)).start()
+
+    device = Device(client)
 
     device.on_monitor = monitor_handler
     device.on_connect = on_device_connect
+
     device.loop_start()
 
-    signal.signal(signal.SIGINT, signal_handler)
+    print(device.info)
 
     i = 60
+
     while True:
-        # print("model:{}".format(device.model))
-        # device.tscore = i
-        # device.tiou = i
-        # i = i + 1
-        # if i > 100:
-        #     i = 30
+        print(device.wifi)
+        print(device.mqtt)
+        print(device.info)
+        print(device.model)
+        device.tscore = i
+        device.tiou = i
+        i = i + 1
+        if i > 100:
+            i = 30
 
         time.sleep(2)
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python-sscma-0.2.1/tests/test_serial.py` & `python-sscma-0.5.0/tests/test_serialclient.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sscma.micro.client import Client
+from sscma.micro.client import Client, SerialClient
 from sscma.micro.device import Device
 from sscma.micro.const import *
 import serial
 import threading
 import time
 import logging
 import signal
@@ -10,24 +10,14 @@
 import base64
 import numpy as np
 
 logging.basicConfig(level=logging.DEBUG)
 
 _LOGGER = logging.getLogger(__name__)
 
-recieve_thread_running = True
-
-
-def recieve_thread(serial_port, client):
-    while recieve_thread_running:
-        if serial_port.in_waiting:
-            msg = serial_port.read(serial_port.in_waiting)
-            if msg != b'':
-                client.on_recieve(msg)
-
 
 def monitor_handler(device, msg):
     if "image" in msg:
         jpeg_bytes = base64.b64decode(msg["image"])
 
         # Convert the bytes into a numpy array
         nparr = np.frombuffer(jpeg_bytes, np.uint8)
@@ -41,52 +31,44 @@
         msg.pop("image")
     print(msg)
 
 
 def on_device_connect(device):
     print("device connected")
     device.Invoke(-1, False, True)
-    device.tscore = 70
-    device.tiou = 70
+    device.tscore = 50
+    device.tiou = 35
 
 
+client = SerialClient("/dev/ttyACM0")
+
 def signal_handler(signal, frame):
     print("Ctrl+C pressed!")
-    global recieve_thread_running
-    recieve_thread_running = False
-    exit(0)
-
-
+    client.loop_stop()
+   
 def main():
-    signal.signal(signal.SIGINT, signal_handler)
-    serial_port = serial.Serial("COM83", 921600, timeout=0.1)
-    client = Client(lambda msg: serial_port.write(msg))
-    threading.Thread(target=recieve_thread, args=(
-        serial_port, client)).start()
 
+    signal.signal(signal.SIGINT, signal_handler)
+ 
     device = Device(client)
 
     device.on_monitor = monitor_handler
     device.on_connect = on_device_connect
-
+     
     device.loop_start()
 
     print(device.info)
 
     i = 60
 
     while True:
         print(device.wifi)
         print(device.mqtt)
         print(device.info)
         print(device.model)
-        device.tscore = i
-        device.tiou = i
-        i = i + 1
-        if i > 100:
-            i = 30
+
 
         time.sleep(2)
 
 
 if __name__ == "__main__":
     main()
```

