# Comparing `tmp/socktalk-0.1.9.tar.gz` & `tmp/socktalk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socktalk-0.1.9.tar", last modified: Thu Apr 11 15:39:34 2024, max compression
+gzip compressed data, was "socktalk-0.2.0.tar", last modified: Tue Apr 16 19:50:52 2024, max compression
```

## Comparing `socktalk-0.1.9.tar` & `socktalk-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 15:39:34.198003 socktalk-0.1.9/
--rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.9/LICENSE
--rw-r--r--   0 mike      (1000) mike      (1000)     4724 2024-04-11 15:39:34.198003 socktalk-0.1.9/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     3725 2024-04-11 15:38:01.000000 socktalk-0.1.9/README.md
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 15:39:34.198003 socktalk-0.1.9/server_client/
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.9/server_client/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5390 2024-04-11 11:39:20.000000 socktalk-0.1.9/server_client/ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.9/server_client/client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      477 2024-04-11 15:19:14.000000 socktalk-0.1.9/server_client/main.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.9/server_client/server.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3456 2024-04-11 11:27:09.000000 socktalk-0.1.9/server_client/start_server_with_ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-11 15:39:34.198003 socktalk-0.1.9/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     1320 2024-04-11 15:21:08.000000 socktalk-0.1.9/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 15:39:34.198003 socktalk-0.1.9/socktalk.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)     4724 2024-04-11 15:39:34.000000 socktalk-0.1.9/socktalk.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      388 2024-04-11 15:39:34.000000 socktalk-0.1.9/socktalk.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-11 15:39:34.000000 socktalk-0.1.9/socktalk.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       53 2024-04-11 15:39:34.000000 socktalk-0.1.9/socktalk.egg-info/entry_points.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      301 2024-04-11 15:39:34.000000 socktalk-0.1.9/socktalk.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-11 15:39:34.000000 socktalk-0.1.9/socktalk.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 19:50:52.986607 socktalk-0.2.0/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.2.0/LICENSE
+-rw-r--r--   0 mike      (1000) mike      (1000)     5014 2024-04-16 19:50:52.986607 socktalk-0.2.0/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4015 2024-04-16 19:48:25.000000 socktalk-0.2.0/README.md
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 19:50:52.986607 socktalk-0.2.0/server_client/
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.2.0/server_client/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5489 2024-04-16 17:07:47.000000 socktalk-0.2.0/server_client/ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.2.0/server_client/client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      614 2024-04-16 16:42:54.000000 socktalk-0.2.0/server_client/main.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2832 2024-04-16 19:45:03.000000 socktalk-0.2.0/server_client/new_main.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4739 2024-04-16 17:05:12.000000 socktalk-0.2.0/server_client/server.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3456 2024-04-11 11:27:09.000000 socktalk-0.2.0/server_client/start_server_with_ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2779 2024-04-16 18:48:07.000000 socktalk-0.2.0/server_client/terminal_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-16 19:50:52.986607 socktalk-0.2.0/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1320 2024-04-11 17:50:39.000000 socktalk-0.2.0/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-16 19:50:52.986607 socktalk-0.2.0/socktalk.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     5014 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      447 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       53 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/entry_points.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      301 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-16 19:50:52.000000 socktalk-0.2.0/socktalk.egg-info/top_level.txt
```

### Comparing `socktalk-0.1.9/LICENSE` & `socktalk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.9/PKG-INFO` & `socktalk-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.1.9
+Version: 0.2.0
 Summary: Socket-based AI chat server and multi-user chat client
 Project-URL: Source, https://github.com/mdkmk/socktalk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -39,43 +39,55 @@
 
 ## Install "socktalk" using pip
 If installing socktalk using pip, create and enter a virtual environment then enter into your terminal:  
 "pip install socktalk"  
 
 You can use the following terminal commands:
 1) "socktalk --ai": Runs the chat server with a connected AI client. Uses gpt-3.5-turbo model by default.
-    You should create an environment file named ".env" in the working directory from which you execute the python
-    commands for the package, in order to adjust the AI modes and chat server settings.
+    You should create an environment file named ".env" in the working directory from which you execute the terminal
+    commands to call the package, in order to adjust the AI modes and chat server settings.
 
-    Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
-    The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted. Mode2 content can be adjusted. See below for more details.
-
-    ### AI Client Modes:
-   1. Respond every N lines: the bot reads the conversation and responds to the conversation once every N lines
-   2. ⁠Respond every N seconds: the bot says something completely new and unrelated every N seconds
-
-       ### ".env" file example
-
-       OPENAI_API_KEY=<OPENAI_API_KEY_HERE>  
-       SERVER_IP_ADDRESS=127.0.0.1  
-       SERVER_PORT=1234  
-       SEND_FULL_CHAT_HISTORY=True  
-       AI_MODE1_ACTIVE=True  
-       AI_MODE1_INTERVAL=1  
-       AI_MODE1_MODEL=gpt-3.5-turbo  
-       AI_MODE2_ACTIVE=True  
-       AI_MODE2_INTERVAL=60  
-       AI_MODE2_MODEL=gpt-3.5-turbo  
-       AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
+    Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key
+    to function you will need to load at least 5$ of credit on your OpenAI account. The AI client has two modes which
+    can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted.
+    Mode2 content can be adjusted. You can adjust a setting to send the full chat history to the chatgpt API, so that
+    the chatbot will have memory. See below for more details.
+    
+
+   ### AI Client Modes:
+i. Respond every N lines: the bot reads the conversation and responds to the conversation once every N lines  
+ii. Respond every N seconds: the bot says something completely new and unrelated every N seconds
+
+-------------------------------------------
+### ".env" file example
+
+    OPENAI_API_KEY=<OPENAI_API_KEY_HERE>  
+    SERVER_IP_ADDRESS=127.0.0.1  
+    SERVER_PORT=1234  
+    SEND_FULL_CHAT_HISTORY=True  
+    AI_MODE1_ACTIVE=True  
+    AI_MODE1_INTERVAL=1  
+    AI_MODE1_MODEL=gpt-3.5-turbo  
+    AI_MODE2_ACTIVE=True  
+    AI_MODE2_INTERVAL=60  
+    AI_MODE2_MODEL=gpt-3.5-turbo  
+    AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
 
+-------------------------------------------
 
 2) "socktalk --server": Runs a chat server without a connected AI client. No .env file necessary.
 
 
-3) "socktalk --client": Runs the multi-user chat client.
+3) "socktalk --client": Runs the advanced multi-user chat client.  
+
+
+4) "socktalk --terminal": Runs the simplistic and limited terminal-based multi-user chat client.
+
+
+
 
 
 ## Python Networking Task: Building a Chat Server and Client
 
 Server
 
 The server should be able to handle multiple clients concurrently. It should be able to receive a message from a client and broadcast it to all other connected clients. The server should use non-blocking sockets and select.select() to handle multiple connections.
```

### Comparing `socktalk-0.1.9/README.md` & `socktalk-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,43 +9,55 @@
 
 ## Install "socktalk" using pip
 If installing socktalk using pip, create and enter a virtual environment then enter into your terminal:  
 "pip install socktalk"  
 
 You can use the following terminal commands:
 1) "socktalk --ai": Runs the chat server with a connected AI client. Uses gpt-3.5-turbo model by default.
-    You should create an environment file named ".env" in the working directory from which you execute the python
-    commands for the package, in order to adjust the AI modes and chat server settings.
+    You should create an environment file named ".env" in the working directory from which you execute the terminal
+    commands to call the package, in order to adjust the AI modes and chat server settings.
 
-    Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
-    The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted. Mode2 content can be adjusted. See below for more details.
-
-    ### AI Client Modes:
-   1. Respond every N lines: the bot reads the conversation and responds to the conversation once every N lines
-   2. ⁠Respond every N seconds: the bot says something completely new and unrelated every N seconds
-
-       ### ".env" file example
-
-       OPENAI_API_KEY=<OPENAI_API_KEY_HERE>  
-       SERVER_IP_ADDRESS=127.0.0.1  
-       SERVER_PORT=1234  
-       SEND_FULL_CHAT_HISTORY=True  
-       AI_MODE1_ACTIVE=True  
-       AI_MODE1_INTERVAL=1  
-       AI_MODE1_MODEL=gpt-3.5-turbo  
-       AI_MODE2_ACTIVE=True  
-       AI_MODE2_INTERVAL=60  
-       AI_MODE2_MODEL=gpt-3.5-turbo  
-       AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
+    Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key
+    to function you will need to load at least 5$ of credit on your OpenAI account. The AI client has two modes which
+    can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted.
+    Mode2 content can be adjusted. You can adjust a setting to send the full chat history to the chatgpt API, so that
+    the chatbot will have memory. See below for more details.
+    
+
+   ### AI Client Modes:
+i. Respond every N lines: the bot reads the conversation and responds to the conversation once every N lines  
+ii. Respond every N seconds: the bot says something completely new and unrelated every N seconds
+
+-------------------------------------------
+### ".env" file example
+
+    OPENAI_API_KEY=<OPENAI_API_KEY_HERE>  
+    SERVER_IP_ADDRESS=127.0.0.1  
+    SERVER_PORT=1234  
+    SEND_FULL_CHAT_HISTORY=True  
+    AI_MODE1_ACTIVE=True  
+    AI_MODE1_INTERVAL=1  
+    AI_MODE1_MODEL=gpt-3.5-turbo  
+    AI_MODE2_ACTIVE=True  
+    AI_MODE2_INTERVAL=60  
+    AI_MODE2_MODEL=gpt-3.5-turbo  
+    AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
 
+-------------------------------------------
 
 2) "socktalk --server": Runs a chat server without a connected AI client. No .env file necessary.
 
 
-3) "socktalk --client": Runs the multi-user chat client.
+3) "socktalk --client": Runs the advanced multi-user chat client.  
+
+
+4) "socktalk --terminal": Runs the simplistic and limited terminal-based multi-user chat client.
+
+
+
 
 
 ## Python Networking Task: Building a Chat Server and Client
 
 Server
 
 The server should be able to handle multiple clients concurrently. It should be able to receive a message from a client and broadcast it to all other connected clients. The server should use non-blocking sockets and select.select() to handle multiple connections.
```

### Comparing `socktalk-0.1.9/server_client/ai_client.py` & `socktalk-0.2.0/server_client/ai_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,17 @@
                     break
 
             except Exception as e:
                 print(f"Error receiving message: {e}")
                 break
 
     def handle_message(self, message):
+        if "has joined the chat" in message or "has left the chat" in message:
+            return
+
         username, _, content = message.partition(' > ')
         if username.strip() != self.username:
             self.conversation_history.append({"role": "user", "content": content})
             if self.mode1_enabled:
                 self.line_count += 1
                 if self.line_count >= self.mode1_interval:
                     self.respond_to_message()
```

### Comparing `socktalk-0.1.9/server_client/client.py` & `socktalk-0.2.0/server_client/client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.9/server_client/server.py` & `socktalk-0.2.0/server_client/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,18 +38,23 @@
                         client_socket, client_address = self.server_socket.accept()
                         user = self.receive_message(client_socket)
                         if user is False:
                             continue
                         self.sockets_list.append(client_socket)
                         self.clients[client_socket] = user
                         print(f"Accepted new connection from {client_address[0]}:{client_address[1]} username:{user['data'].decode('utf-8')}")
+                        welcome_message = f"{user['data'].decode('utf-8')} has joined the chat!"
+                        self.broadcast_message(welcome_message, source_socket=client_socket)
                     else:
                         message = self.receive_message(notified_socket)
                         if message is False:
-                            print(f"Closed connection from {self.clients[notified_socket]['data'].decode('utf-8')}")
+                            username = self.clients[notified_socket]['data'].decode('utf-8')
+                            print(f"Closed connection from {username}")
+                            self.broadcast_message(f"{username}"
+                                                   f" has left the chat", notified_socket)
                             self.sockets_list.remove(notified_socket)
                             del self.clients[notified_socket]
                             continue
                         user = self.clients[notified_socket]
                         print(f"Received message from {user['data'].decode('utf-8')}: {message['data'].decode('utf-8')}")
                         for client_socket in self.clients:
                             if client_socket != notified_socket:
@@ -66,14 +71,21 @@
                     print(f"Server accept error: {e}")
                 else:
                     print("Server socket closed")
                     break
             except Exception as e:
                 print(f"Unexpected error: {e}")
 
+    def broadcast_message(self, message, source_socket=None):
+        message_encoded = message.encode("utf-8")
+        message_header = f"{len(message_encoded):<{self.HEADER_LENGTH}}".encode("utf-8")
+        for client_socket in self.clients:
+            if client_socket != source_socket:
+                client_socket.send(message_header + message_encoded)
+
     def shutdown(self):
         self.running = False
         self.server_socket.close()
 
 
 def main():
     server_ip = input("Enter server IP (for default 127.0.0.1, press enter): ") or "127.0.0.1"
```

### Comparing `socktalk-0.1.9/server_client/start_server_with_ai_client.py` & `socktalk-0.2.0/server_client/start_server_with_ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.9/setup.py` & `socktalk-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='socktalk',
-    version='0.1.9',
+    version='0.2.0',
     packages=find_packages(),
     project_urls={
         'Source': 'https://github.com/mdkmk/socktalk'
     },
     install_requires=[
         'annotated-types==0.6.0',
         'anyio==4.3.0',
```

### Comparing `socktalk-0.1.9/socktalk.egg-info/PKG-INFO` & `socktalk-0.2.0/socktalk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.1.9
+Version: 0.2.0
 Summary: Socket-based AI chat server and multi-user chat client
 Project-URL: Source, https://github.com/mdkmk/socktalk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -39,43 +39,55 @@
 
 ## Install "socktalk" using pip
 If installing socktalk using pip, create and enter a virtual environment then enter into your terminal:  
 "pip install socktalk"  
 
 You can use the following terminal commands:
 1) "socktalk --ai": Runs the chat server with a connected AI client. Uses gpt-3.5-turbo model by default.
-    You should create an environment file named ".env" in the working directory from which you execute the python
-    commands for the package, in order to adjust the AI modes and chat server settings.
+    You should create an environment file named ".env" in the working directory from which you execute the terminal
+    commands to call the package, in order to adjust the AI modes and chat server settings.
 
-    Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
-    The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted. Mode2 content can be adjusted. See below for more details.
-
-    ### AI Client Modes:
-   1. Respond every N lines: the bot reads the conversation and responds to the conversation once every N lines
-   2. ⁠Respond every N seconds: the bot says something completely new and unrelated every N seconds
-
-       ### ".env" file example
-
-       OPENAI_API_KEY=<OPENAI_API_KEY_HERE>  
-       SERVER_IP_ADDRESS=127.0.0.1  
-       SERVER_PORT=1234  
-       SEND_FULL_CHAT_HISTORY=True  
-       AI_MODE1_ACTIVE=True  
-       AI_MODE1_INTERVAL=1  
-       AI_MODE1_MODEL=gpt-3.5-turbo  
-       AI_MODE2_ACTIVE=True  
-       AI_MODE2_INTERVAL=60  
-       AI_MODE2_MODEL=gpt-3.5-turbo  
-       AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
+    Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key
+    to function you will need to load at least 5$ of credit on your OpenAI account. The AI client has two modes which
+    can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted.
+    Mode2 content can be adjusted. You can adjust a setting to send the full chat history to the chatgpt API, so that
+    the chatbot will have memory. See below for more details.
+    
+
+   ### AI Client Modes:
+i. Respond every N lines: the bot reads the conversation and responds to the conversation once every N lines  
+ii. Respond every N seconds: the bot says something completely new and unrelated every N seconds
+
+-------------------------------------------
+### ".env" file example
+
+    OPENAI_API_KEY=<OPENAI_API_KEY_HERE>  
+    SERVER_IP_ADDRESS=127.0.0.1  
+    SERVER_PORT=1234  
+    SEND_FULL_CHAT_HISTORY=True  
+    AI_MODE1_ACTIVE=True  
+    AI_MODE1_INTERVAL=1  
+    AI_MODE1_MODEL=gpt-3.5-turbo  
+    AI_MODE2_ACTIVE=True  
+    AI_MODE2_INTERVAL=60  
+    AI_MODE2_MODEL=gpt-3.5-turbo  
+    AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
 
+-------------------------------------------
 
 2) "socktalk --server": Runs a chat server without a connected AI client. No .env file necessary.
 
 
-3) "socktalk --client": Runs the multi-user chat client.
+3) "socktalk --client": Runs the advanced multi-user chat client.  
+
+
+4) "socktalk --terminal": Runs the simplistic and limited terminal-based multi-user chat client.
+
+
+
 
 
 ## Python Networking Task: Building a Chat Server and Client
 
 Server
 
 The server should be able to handle multiple clients concurrently. It should be able to receive a message from a client and broadcast it to all other connected clients. The server should use non-blocking sockets and select.select() to handle multiple connections.
```

