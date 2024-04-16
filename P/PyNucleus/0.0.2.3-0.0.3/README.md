# Comparing `tmp/PyNucleus-0.0.2.3.tar.gz` & `tmp/pynucleus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNucleus-0.0.2.3.tar", last modified: Thu Apr 11 19:51:41 2024, max compression
+gzip compressed data, was "pynucleus-0.0.3.tar", last modified: Tue Apr 16 15:02:50 2024, max compression
```

## Comparing `PyNucleus-0.0.2.3.tar` & `pynucleus-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 19:51:41.707491 PyNucleus-0.0.2.3/
--rw-rw-rw-   0        0        0     1088 2024-04-11 15:50:32.000000 PyNucleus-0.0.2.3/LICENSE
--rw-rw-rw-   0        0        0      299 2024-04-11 19:51:41.705933 PyNucleus-0.0.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 19:51:41.692771 PyNucleus-0.0.2.3/PyNucleus/
--rw-rw-rw-   0        0        0      181 2024-04-11 18:56:07.000000 PyNucleus-0.0.2.3/PyNucleus/__init__.py
--rw-rw-rw-   0        0        0      540 2024-04-11 19:51:23.000000 PyNucleus-0.0.2.3/PyNucleus/__main__.py
--rw-rw-rw-   0        0        0     6376 2024-04-11 19:47:25.000000 PyNucleus-0.0.2.3/PyNucleus/calculator.py
--rw-rw-rw-   0        0        0     4890 2024-04-11 19:47:33.000000 PyNucleus-0.0.2.3/PyNucleus/commands.py
--rw-rw-rw-   0        0        0     1091 2024-04-11 19:28:37.000000 PyNucleus-0.0.2.3/PyNucleus/errors.py
--rw-rw-rw-   0        0        0     1867 2024-04-11 19:47:32.000000 PyNucleus-0.0.2.3/PyNucleus/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-11 19:51:41.704458 PyNucleus-0.0.2.3/PyNucleus.egg-info/
--rw-rw-rw-   0        0        0      299 2024-04-11 19:51:41.000000 PyNucleus-0.0.2.3/PyNucleus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-04-11 19:51:41.000000 PyNucleus-0.0.2.3/PyNucleus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 19:51:41.000000 PyNucleus-0.0.2.3/PyNucleus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 19:51:41.000000 PyNucleus-0.0.2.3/PyNucleus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      137 2024-04-11 15:51:51.000000 PyNucleus-0.0.2.3/README.md
--rw-rw-rw-   0        0        0      716 2024-04-11 19:51:21.000000 PyNucleus-0.0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 19:51:41.707491 PyNucleus-0.0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 15:02:50.094969 pynucleus-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2024-04-11 15:50:32.000000 pynucleus-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      536 2024-04-16 15:02:50.093302 pynucleus-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 15:02:50.077340 pynucleus-0.0.3/PyNucleus/
+-rw-rw-rw-   0        0        0      264 2024-04-16 14:46:58.000000 pynucleus-0.0.3/PyNucleus/__init__.py
+-rw-rw-rw-   0        0        0      538 2024-04-16 14:27:09.000000 pynucleus-0.0.3/PyNucleus/__main__.py
+-rw-rw-rw-   0        0        0     6376 2024-04-11 19:47:25.000000 pynucleus-0.0.3/PyNucleus/calculator.py
+-rw-rw-rw-   0        0        0     5633 2024-04-16 14:59:04.000000 pynucleus-0.0.3/PyNucleus/commands.py
+-rw-rw-rw-   0        0        0     1594 2024-04-16 14:52:39.000000 pynucleus-0.0.3/PyNucleus/decorators.py
+-rw-rw-rw-   0        0        0     1372 2024-04-12 18:51:38.000000 pynucleus-0.0.3/PyNucleus/errors.py
+-rw-rw-rw-   0        0        0     2043 2024-04-16 14:47:49.000000 pynucleus-0.0.3/PyNucleus/functions.py
+-rw-rw-rw-   0        0        0     2108 2024-04-16 14:50:22.000000 pynucleus-0.0.3/PyNucleus/memory.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:02:50.092301 pynucleus-0.0.3/PyNucleus.egg-info/
+-rw-rw-rw-   0        0        0      536 2024-04-16 15:02:50.000000 pynucleus-0.0.3/PyNucleus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2024-04-16 15:02:50.000000 pynucleus-0.0.3/PyNucleus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 15:02:50.000000 pynucleus-0.0.3/PyNucleus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-16 15:02:50.000000 pynucleus-0.0.3/PyNucleus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      376 2024-04-16 14:59:46.000000 pynucleus-0.0.3/README.md
+-rw-rw-rw-   0        0        0      749 2024-04-16 15:01:55.000000 pynucleus-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 15:02:50.095479 pynucleus-0.0.3/setup.cfg
```

### Comparing `PyNucleus-0.0.2.3/LICENSE` & `pynucleus-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNucleus-0.0.2.3/PyNucleus/__main__.py` & `pynucleus-0.0.3/PyNucleus/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 
-__version__ = "0.0.2.3"
+__version__ = "0.0.3"
 __author__ = "Bartek Kansy"
 
 def main():
     parser = argparse.ArgumentParser(description="Essential Python Toolkit.")
     parser.add_argument("--version", action="store_true", help="show package version")
     parser.add_argument("--author", action="store_true", help="show package author")
     args = parser.parse_args()
```

### Comparing `PyNucleus-0.0.2.3/PyNucleus/calculator.py` & `pynucleus-0.0.3/PyNucleus/calculator.py`

 * *Files identical despite different names*

### Comparing `PyNucleus-0.0.2.3/PyNucleus/commands.py` & `pynucleus-0.0.3/PyNucleus/commands.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #######################################
 # IMPORTS
 #######################################
 
 import inspect
 
-from PyNucleus.errors import *
+from PyNucleus.errors import (
+    InvalidCommand, 
+    InvalidCommandName, 
+    InvalidCommandFunction
+    )
 from PyNucleus.functions import PrintError
 
 from typing import Callable
 
 #######################################
 # CLASSES
 #######################################
 
-def __check_command_func(func) -> bool:
+def check_command_func(func) -> bool:
     """
     ## Check if command function is valid.
     """
     signature = inspect.signature(func)
     params = signature.parameters
 
     first_param_name = next(iter(params))
@@ -33,102 +37,104 @@
 
 #######################################
 # CLASSES
 #######################################
 
 class CommandBase:
     """
-    ## Only command class that is compatible with CommandRegister
+    ## Only command class that is compatible with CommandRegister.
 
-    ### >> Example of making command:
+    ### >> Example of usage:
     ```
     from PyNucleus.commands import CommandBase
 
     def HelpCommand(args: list[str]) -> int:
         print("This is an example help command!")
         return 0
 
-    command = CommandBase("help", HelpCommand)
-    ```
-
-    ### >> Example of usage with CommandRegister:
-    ```
-    from PyNucleus.commands import CommandBase, CommandRegister
-
-    def HelpCommand(args: list[str]) -> int:
-        print("This is an example help command!")
-        return 0
-
-    commandRegister = CommandRegister()
-    command = CommandBase("help", HelpCommand)
-
-    commandRegister.AddCommand(command)
-    # OR
-    commandRegister.commands.append(command)
+    command = CommandBase("help", "Display all commands", HelpCommand)
     ```
     """
-    def __init__(self, name: str, func: Callable) -> None:
+    def __init__(self, name: str, details: str, func: Callable) -> None:
         self.name = name
+        self.details = details
         self.func = func
 
     def Run(self, args: list[str]) -> int:
         return self.func(args)
 
     def __repr__(self) -> str:
         return f"Command '{self.name}'"
 
 class CommandRegister:
     """
     ## The command register is used to make command management easier.
 
-    ### Features:
-    * Adding commands
-    * Deleting commands
-    * Handling commands or entire inputs
+    ### >> Example of usage:
+    ```
+    from PyNucleus.commands import CommandRegister
+    
+    commandRegister = CommandRegister()
+    ```
     """
     def __init__(self, printErrors: bool=True) -> None:
         self.commands: list[CommandBase] = []
         self.printErrors = printErrors
 
     def AddCommand(self, name: str, func: Callable[[list[str]], int]) -> int:
         """
-        ## Add a command to the register, just enter its name and the function which will be called.
+        ## Add a command to the register.
 
         ### Posible errors:
         * Invalid Command Name
         * Invalid Command Function
 
-        ### >> Example of function:
+        ### >> Example of usage:
         ```
+        from PyNucleus.commands import CommandBase, CommandRegister
+
+        commandRegister = CommandRegister()
+
         def HelpCommand(args: list[str]) -> int:
-            print("This is example of help command function.")
+            print("This is an example help command.")
             return 0
 
-        # 0 - success | -1 - failed
+        newCommand = CommandBase("help", "Display all commands", HelpCommand)
+
+        commandRegister.AddCommand(newCommand)
         ```
         """
         for command in self.commands:
             if command.name == name:
                 if self.printErrors: PrintError(InvalidCommandName(name, "This name is already taken"))
                 return -1
             
-        if not __check_command_func(func):
+        if not check_command_func(func):
             if self.printErrors: PrintError(InvalidCommandFunction(name, "Look on example of function in AddCommand description"))
             return -1
         
         newCommand = CommandBase(name, func)
         self.commands.append(newCommand)
         return 0
 
     def DeleteCommand(self, name: str) -> int:
         """
         ## Delete a command from register.
 
         ### Posible errors:
         * Invalid Command Name
+
+        ### >> Example of usage:
+        ```
+        from PyNucleus.commands import CommandBase, CommandRegister
+
+        ...
+
+        commandRegister.DeleteCommand("help")
+        ```
         """
         index = 0
         for command in self.commands:
             if command.name == name:
                 self.commands.pop(index)
                 return 0
             index += 1
@@ -138,14 +144,33 @@
     
     def HandleCommand(self, command: str, args: list[str]=[]) -> int:
         """
         ## Handle command from user.
 
         ### Posible errors:
         * Invalid Command
+
+        ### >> Example of usage:
+        ```
+        from PyNucleus.commands import CommandRegister, CommandBase
+
+        ...
+        
+        userInput = input(">: ")
+        words = userInput.split()
+
+        command, args = "", []
+
+        if len(words) > 0: 
+            command = words[0]
+        if len(words) > 1:
+            args = words[1:]
+
+        commandRegister.HandleCommand(newCommand)
+        ```
         """
         for cmd in self.commands:
             if cmd.name == command:
                 cmd.Run(args)
                 return 0
         
         if self.printErrors: PrintError(InvalidCommand(command, "That command does not exist"))
@@ -153,14 +178,25 @@
     
     def HandleInput(self, entry: str="") -> int:
         """
         ## Handle the entire input from user.
 
         ### Posible errors:
         * Invalid Command
+
+        ### >> Example of usage:
+        ```
+        from PyNucleus.commands import CommandRegister, CommandBase
+
+        ...
+        
+        userInput = input(">: ")
+
+        commandRegister.HandleInput(userInput)
+        ```
         """
         words = entry.split()
         cmd = ""
         args = []
         if len(words) > 0: cmd = words[0]
         if len(words) > 1: args = words[1:]
```

### Comparing `PyNucleus-0.0.2.3/PyNucleus/errors.py` & `pynucleus-0.0.3/PyNucleus/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,8 +20,16 @@
 
 class InvalidCommand(ErrorBase):
     def __init__(self, command: str, details) -> None:
         super().__init__("Invalid Command", f"'{command}' {f'({details})' if details else ''}")
 
 class CalculatorException(ErrorBase):
     def __init__(self, details: str) -> None:
-        super().__init__("Calculator Exception", details)
+        super().__init__("Calculator Exception", details)
+
+class MemoryException(ErrorBase):
+    def __init__(self, details: str) -> None:
+        super().__init__("Memory Exception", details)
+
+class MemoryInitFailed(ErrorBase):
+    def __init__(self, details: str) -> None:
+        super().__init__("Memory Init Failed", details)
```

### Comparing `PyNucleus-0.0.2.3/PyNucleus/functions.py` & `pynucleus-0.0.3/PyNucleus/functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,21 @@
 def PrintError(error) -> int:
     """
     ## Print error with red foreground.
     """
     print(f"{Fore.RED}{error}{Style.RESET_ALL}")
     return 0
 
+def PrintSuccess(success) -> int:
+    """
+    ## Print success message with green foreground.
+    """
+    print(f"{Fore.GREEN}{success}{Style.RESET_ALL}")
+    return 0
+
 def generate_id(length: int=16, numbers: bool=True, lowers: bool=True, uppers: bool=True) -> str:
     """
     ## Generate ID with numbers, uppercase and lowercase letters.
 
     ### Example of generated ID: 
     * 7wCxklbqgbXkO0K6
     """
```

### Comparing `PyNucleus-0.0.2.3/pyproject.toml` & `pynucleus-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2250 794e 7563 6c65 7573 220d 0a76  = "PyNucleus"..v
-00000020: 6572 7369 6f6e 203d 2022 302e 302e 322e  ersion = "0.0.2.
-00000030: 3322 0d0a 6465 7363 7269 7074 696f 6e20  3"..description 
-00000040: 3d20 2245 7373 656e 7469 616c 2050 7974  = "Essential Pyt
-00000050: 686f 6e20 546f 6f6c 6b69 742e 220d 0a72  hon Toolkit."..r
-00000060: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
-00000070: 6d64 220d 0a0d 0a5b 6d65 7461 6461 7461  md"....[metadata
-00000080: 5d0d 0a6c 6f6e 675f 6465 7363 7269 7074  ]..long_descript
-00000090: 696f 6e20 3d20 2246 6f75 6e64 6174 696f  ion = "Foundatio
-000000a0: 6e61 6c20 5079 7468 6f6e 2074 6f6f 6c6b  nal Python toolk
-000000b0: 6974 206f 6666 6572 696e 6720 6573 7365  it offering esse
-000000c0: 6e74 6961 6c20 7574 696c 6974 6965 7320  ntial utilities 
-000000d0: 616e 6420 7374 7275 6374 7572 6573 2066  and structures f
-000000e0: 6f72 2073 7472 6561 6d6c 696e 6564 2064  or streamlined d
-000000f0: 6576 656c 6f70 6d65 6e74 206f 6620 7665  evelopment of ve
-00000100: 7273 6174 696c 6520 6170 706c 6963 6174  rsatile applicat
-00000110: 696f 6e73 2e22 0d0a 6465 7065 6e64 656e  ions."..dependen
-00000120: 6369 6573 203d 205b 2272 616e 646f 6d22  cies = ["random"
-00000130: 2c20 2263 6f6c 6f72 616d 6122 5d0d 0a72  , "colorama"]..r
-00000140: 6571 7569 7265 732d 7079 7468 6f6e 203d  equires-python =
-00000150: 2022 3e3d 332e 3132 220d 0a61 7574 686f   ">=3.12"..autho
-00000160: 7273 203d 205b 0d0a 2020 7b6e 616d 6520  rs = [..  {name 
-00000170: 3d20 2242 6172 7465 6b4b 616e 7379 222c  = "BartekKansy",
-00000180: 2065 6d61 696c 203d 2022 6b61 6e73 792e   email = "kansy.
-00000190: 6261 7274 6f73 7a40 696e 7465 7269 612e  bartosz@interia.
-000001a0: 706c 227d 2c0d 0a5d 0d0a 636c 6173 7369  pl"},..]..classi
-000001b0: 6669 6572 7320 3d20 5b0d 0a20 2020 2022  fiers = [..    "
-000001c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001e0: 3a20 3322 2c0d 0a20 2020 2022 4c69 6365  : 3",..    "Lice
-000001f0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000200: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-00000210: 7365 220d 0a5d 0d0a 6c69 6365 6e73 6520  se"..]..license 
-00000220: 3d20 7b74 6578 7420 3d20 224c 4943 454e  = {text = "LICEN
-00000230: 5345 227d 0d0a 6b65 7977 6f72 6473 203d  SE"}..keywords =
-00000240: 205b 2270 7974 686f 6e22 2c20 2263 6c61   ["python", "cla
-00000250: 7373 6573 222c 2022 7574 696c 6974 6965  sses", "utilitie
-00000260: 7322 5d0d 0a0d 0a5b 6275 696c 642d 7379  s"]....[build-sy
-00000270: 7374 656d 5d0d 0a72 6571 7569 7265 7320  stem]..requires 
-00000280: 3d20 5b22 7365 7475 7074 6f6f 6c73 3e3d  = ["setuptools>=
-00000290: 3430 2e38 2e30 225d 0d0a 6275 696c 642d  40.8.0"]..build-
-000002a0: 6261 636b 656e 6420 3d20 2273 6574 7570  backend = "setup
-000002b0: 746f 6f6c 732e 6275 696c 645f 6d65 7461  tools.build_meta
-000002c0: 3a5f 5f6c 6567 6163 795f 5f22            :__legacy__"
+00000020: 6572 7369 6f6e 203d 2022 302e 302e 3322  ersion = "0.0.3"
+00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
+00000040: 2245 7373 656e 7469 616c 2050 7974 686f  "Essential Pytho
+00000050: 6e20 546f 6f6c 6b69 742e 220d 0a72 6561  n Toolkit."..rea
+00000060: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
+00000070: 220d 0a0d 0a5b 6d65 7461 6461 7461 5d0d  "....[metadata].
+00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+00000090: 6e20 3d20 2246 6f75 6e64 6174 696f 6e61  n = "Foundationa
+000000a0: 6c20 5079 7468 6f6e 2074 6f6f 6c6b 6974  l Python toolkit
+000000b0: 206f 6666 6572 696e 6720 6573 7365 6e74   offering essent
+000000c0: 6961 6c20 7574 696c 6974 6965 7320 616e  ial utilities an
+000000d0: 6420 7374 7275 6374 7572 6573 2066 6f72  d structures for
+000000e0: 2073 7472 6561 6d6c 696e 6564 2064 6576   streamlined dev
+000000f0: 656c 6f70 6d65 6e74 206f 6620 7665 7273  elopment of vers
+00000100: 6174 696c 6520 6170 706c 6963 6174 696f  atile applicatio
+00000110: 6e73 2e22 0d0a 6465 7065 6e64 656e 6369  ns."..dependenci
+00000120: 6573 203d 205b 2272 616e 646f 6d22 2c20  es = ["random", 
+00000130: 2263 6f6c 6f72 616d 6122 5d0d 0a72 6571  "colorama"]..req
+00000140: 7569 7265 7320 3d20 5b22 7261 6e64 6f6d  uires = ["random
+00000150: 222c 2022 636f 6c6f 7261 6d61 225d 0d0a  ", "colorama"]..
+00000160: 7265 7175 6972 6573 2d70 7974 686f 6e20  requires-python 
+00000170: 3d20 223e 3d33 2e31 3222 0d0a 6175 7468  = ">=3.12"..auth
+00000180: 6f72 7320 3d20 5b0d 0a20 207b 6e61 6d65  ors = [..  {name
+00000190: 203d 2022 4261 7274 656b 4b61 6e73 7922   = "BartekKansy"
+000001a0: 2c20 656d 6169 6c20 3d20 226b 616e 7379  , email = "kansy
+000001b0: 2e62 6172 746f 737a 4069 6e74 6572 6961  .bartosz@interia
+000001c0: 2e70 6c22 7d2c 0d0a 5d0d 0a63 6c61 7373  .pl"},..]..class
+000001d0: 6966 6965 7273 203d 205b 0d0a 2020 2020  ifiers = [..    
+000001e0: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
+000001f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000200: 3a3a 2033 222c 0d0a 2020 2020 224c 6963  :: 3",..    "Lic
+00000210: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000220: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+00000230: 6e73 6522 0d0a 5d0d 0a6c 6963 656e 7365  nse"..]..license
+00000240: 203d 207b 7465 7874 203d 2022 4c49 4345   = {text = "LICE
+00000250: 4e53 4522 7d0d 0a6b 6579 776f 7264 7320  NSE"}..keywords 
+00000260: 3d20 5b22 7079 7468 6f6e 222c 2022 636c  = ["python", "cl
+00000270: 6173 7365 7322 2c20 2275 7469 6c69 7469  asses", "utiliti
+00000280: 6573 225d 0d0a 0d0a 5b62 7569 6c64 2d73  es"]....[build-s
+00000290: 7973 7465 6d5d 0d0a 7265 7175 6972 6573  ystem]..requires
+000002a0: 203d 205b 2273 6574 7570 746f 6f6c 733e   = ["setuptools>
+000002b0: 3d34 302e 382e 3022 5d0d 0a62 7569 6c64  =40.8.0"]..build
+000002c0: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
+000002d0: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
+000002e0: 613a 5f5f 6c65 6761 6379 5f5f 22         a:__legacy__"
```

