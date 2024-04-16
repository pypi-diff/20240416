# Comparing `tmp/discord_drive-0.0.4.tar.gz` & `tmp/discord_drive-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_drive-0.0.4.tar", last modified: Mon Apr 15 13:27:25 2024, max compression
+gzip compressed data, was "discord_drive-0.0.5.tar", last modified: Tue Apr 16 17:05:33 2024, max compression
```

## Comparing `discord_drive-0.0.4.tar` & `discord_drive-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-15 13:27:25.949736 discord_drive-0.0.4/
--rw-r--r--   0 ryankarch   (501) staff       (20)     1081 2024-01-26 22:14:00.000000 discord_drive-0.0.4/LICENSE.md
--rw-r--r--   0 ryankarch   (501) staff       (20)      511 2024-04-15 13:27:25.948864 discord_drive-0.0.4/PKG-INFO
--rw-r--r--   0 ryankarch   (501) staff       (20)     3473 2024-04-12 19:58:00.000000 discord_drive-0.0.4/README.md
-drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-15 13:27:25.945136 discord_drive-0.0.4/discord_drive/
--rw-r--r--   0 ryankarch   (501) staff       (20)       43 2024-04-15 13:26:55.000000 discord_drive-0.0.4/discord_drive/__init__.py
--rw-r--r--   0 ryankarch   (501) staff       (20)    13545 2024-04-15 13:23:17.000000 discord_drive-0.0.4/discord_drive/_drive.py
--rw-r--r--   0 ryankarch   (501) staff       (20)      241 2024-02-23 21:48:33.000000 discord_drive-0.0.4/discord_drive/_utils.py
--rw-r--r--   0 ryankarch   (501) staff       (20)    27158 2024-04-15 12:36:22.000000 discord_drive-0.0.4/discord_drive/discord_drive.py
-drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-15 13:27:25.948278 discord_drive-0.0.4/discord_drive.egg-info/
--rw-r--r--   0 ryankarch   (501) staff       (20)      511 2024-04-15 13:27:25.000000 discord_drive-0.0.4/discord_drive.egg-info/PKG-INFO
--rw-r--r--   0 ryankarch   (501) staff       (20)      318 2024-04-15 13:27:25.000000 discord_drive-0.0.4/discord_drive.egg-info/SOURCES.txt
--rw-r--r--   0 ryankarch   (501) staff       (20)        1 2024-04-15 13:27:25.000000 discord_drive-0.0.4/discord_drive.egg-info/dependency_links.txt
--rw-r--r--   0 ryankarch   (501) staff       (20)      120 2024-04-15 13:27:25.000000 discord_drive-0.0.4/discord_drive.egg-info/requires.txt
--rw-r--r--   0 ryankarch   (501) staff       (20)       14 2024-04-15 13:27:25.000000 discord_drive-0.0.4/discord_drive.egg-info/top_level.txt
--rw-r--r--   0 ryankarch   (501) staff       (20)       38 2024-04-15 13:27:25.949974 discord_drive-0.0.4/setup.cfg
--rw-r--r--   0 ryankarch   (501) staff       (20)      710 2024-04-15 13:27:10.000000 discord_drive-0.0.4/setup.py
+drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-16 17:05:33.471509 discord_drive-0.0.5/
+-rw-r--r--   0 ryankarch   (501) staff       (20)     1081 2024-01-26 22:14:00.000000 discord_drive-0.0.5/LICENSE.md
+-rw-r--r--   0 ryankarch   (501) staff       (20)     2629 2024-04-16 17:05:33.471016 discord_drive-0.0.5/PKG-INFO
+-rw-r--r--   0 ryankarch   (501) staff       (20)     3169 2024-04-16 16:58:41.000000 discord_drive-0.0.5/README.md
+drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-16 17:05:33.468130 discord_drive-0.0.5/discord_drive/
+-rw-r--r--   0 ryankarch   (501) staff       (20)       44 2024-04-16 16:58:41.000000 discord_drive-0.0.5/discord_drive/__init__.py
+-rw-r--r--   0 ryankarch   (501) staff       (20)    24580 2024-04-16 16:58:41.000000 discord_drive-0.0.5/discord_drive/_discord_drive.py
+-rw-r--r--   0 ryankarch   (501) staff       (20)    13783 2024-04-16 16:58:41.000000 discord_drive-0.0.5/discord_drive/_drive.py
+-rw-r--r--   0 ryankarch   (501) staff       (20)      241 2024-04-16 16:58:41.000000 discord_drive-0.0.5/discord_drive/_utils.py
+drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-16 17:05:33.470545 discord_drive-0.0.5/discord_drive.egg-info/
+-rw-r--r--   0 ryankarch   (501) staff       (20)     2629 2024-04-16 17:05:33.000000 discord_drive-0.0.5/discord_drive.egg-info/PKG-INFO
+-rw-r--r--   0 ryankarch   (501) staff       (20)      319 2024-04-16 17:05:33.000000 discord_drive-0.0.5/discord_drive.egg-info/SOURCES.txt
+-rw-r--r--   0 ryankarch   (501) staff       (20)        1 2024-04-16 17:05:33.000000 discord_drive-0.0.5/discord_drive.egg-info/dependency_links.txt
+-rw-r--r--   0 ryankarch   (501) staff       (20)      120 2024-04-16 17:05:33.000000 discord_drive-0.0.5/discord_drive.egg-info/requires.txt
+-rw-r--r--   0 ryankarch   (501) staff       (20)       14 2024-04-16 17:05:33.000000 discord_drive-0.0.5/discord_drive.egg-info/top_level.txt
+-rw-r--r--   0 ryankarch   (501) staff       (20)       38 2024-04-16 17:05:33.471610 discord_drive-0.0.5/setup.cfg
+-rw-r--r--   0 ryankarch   (501) staff       (20)     2789 2024-04-16 17:03:36.000000 discord_drive-0.0.5/setup.py
```

### Comparing `discord_drive-0.0.4/LICENSE.md` & `discord_drive-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `discord_drive-0.0.4/README.md` & `discord_drive-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,40 +10,35 @@
 Interface with the Google Drive API using any user’s OAuth token
 Generate an initial file structure or link to an existing one
 Want to be able to upload files/folders to Google Drive
 Want to be able to retrieve files/folders from Google Drive
 Support some “root” directory
 
 ## Usage:
-1. Clone the repository (this will change soon to installing through pip)
-2. Get the id of your server, create a file named `.env` in the directory that your bot runs out of, and put the following code in it:
+1. Install the library:
    ```
-   set
-   DD_GUILD_ID=<server id>
+   pip install discord-drive
    ```
-3. Follow the official [Google quick-start instructions](https://developers.google.com/drive/api/quickstart/python) to generate your credentials file.
-4. Save the credentials file as `credentials.json` in the same directory as the .env file.
-5. Open Google Drive, go to the directory that you want to root the bot to, and get the link.
+2. Follow the official [Google Drive Developer quick-start instructions](https://developers.google.com/drive/api/quickstart/python) to generate your credentials file.
+3. Save the credentials file as `credentials.json` in the running directory of your Discord bot.
+4. Open Google Drive, go to the directory that you want to root the bot to, and get the link.
    - It should be of format: `https://drive.google.com/drive/folders/folder_id`
-6. Create a Discord bot using Pycord, and add the DiscordDrive command suite to it with the following code:
+5. Create a Discord bot using Pycord, and add the DiscordDrive command suite to it with the following code:
    ```python
-   from dotenv import load_dotenv
-   load_dotenv()
    from discord_drive import DriveAPICommands
    bot.add_cog(DriveAPICommands(bot, "<link from step 5>"))
    ```
-   - It is very important that `load_dotenv()` is called before importing the module.
-7. Run the bot, and use `/authenticate` to ensure that DiscordDrive is authorized to access your Google Account.
+6. Run the bot, and use `/authenticate` to ensure that DiscordDrive is authorized to access your Google Account.
 
 ## Commands:
 `/authenticate`: Regenerates the token needed to enable the API. If re-authentication is needed, the bot will DM the caller a link and wait for the authentication code given to the caller by Google\
 `/cd <directory>`: Navigates the caller down into a child directory of their current directory. Autocomplete is provided for hints.\
 `/download <file> <timeout (optional)> <public (optional)>`: Gives the user the file (or a link) to download the file specified. Files have autocomplete. Timeout defaults to 60 seconds, where the file will then no longer be allowed to be downloaded. Public defaults to False, where no other users can see the file.\
 `/ls`: Shows the caller the contents of their current directory.\
 `/pwd`: Shows the caller the file path of their current directory.\
 `/share <file> <user> <timeout (optional)>`: Sends a specified server member a dm with a file from the caller's current directory. Files and users have autocomplete. Timeout defaults to 60 seconds, where the file will then no longer be allowed to be downloaded.\
 `/upload <attachment>`: Uploads a file or zip file to the caller's current directory. Zip files must contain just the files, and no folders, as they will not be read.
 
 ## Team:
 Ryan Karch (karchr) - Official Project Lead
 
-Dominic Beyer (beyerd) - Co-Project Lead
+Dominic Beyer (beyerd) - Co-Project Lead
```

### Comparing `discord_drive-0.0.4/discord_drive/_drive.py` & `discord_drive-0.0.5/discord_drive/_drive.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,15 +96,18 @@
         self.ROOT_ID = root.rsplit("/",1)[1]
         
         creds = None
         # The file token.json stores the user's access and refresh tokens, and is
         # created automatically when the authorization flow completes for the first
         # time.
         if os.path.exists("token.json"):
-            creds = Credentials.from_authorized_user_file("token.json", self.SCOPES)
+            try:
+                creds = Credentials.from_authorized_user_file("token.json", self.SCOPES)
+            except:
+                creds = None
         # If there are no (valid) credentials available, attempt to do it for them.
         if not creds or not creds.valid:
             if creds and creds.expired and creds.refresh_token:
                 try:
                     creds.refresh(Request())
                     with open("token.json", "w") as token:
                         token.write(creds.to_json())
@@ -112,21 +115,26 @@
                 except:
                     pass
         # if creds are good, build the service
         else:
             self.create_service(creds)
 
     def generate_flow(self):
-        flow = InstalledAppFlow.from_client_secrets_file(
-                "credentials.json", self.SCOPES,
-                redirect_uri='urn:ietf:wg:oauth:2.0:oob'
-            )
-        
-        auth_url, _ = flow.authorization_url(prompt='consent', )
-        return flow, auth_url
+        if not os.path.exists("credentials.json"):
+            return None, None
+        try:
+            flow = InstalledAppFlow.from_client_secrets_file(
+                    "credentials.json", self.SCOPES,
+                    redirect_uri='urn:ietf:wg:oauth:2.0:oob'
+                )
+            
+            auth_url, _ = flow.authorization_url(prompt='consent', )
+            return flow, auth_url
+        except:
+            return None, None
 
     @_input_validator
     def create_service(self, creds: Credentials):
         try:
             self.service = build("drive", "v3", credentials=creds)
 
             folder = self.service.files().get(fileId=self.ROOT_ID).execute()
```

### Comparing `discord_drive-0.0.4/discord_drive/discord_drive.py` & `discord_drive-0.0.5/discord_drive/_discord_drive.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,15 @@
 from datetime import datetime
 from discord.ext.commands import has_permissions, MissingPermissions
 from discord.ext.pages import Paginator, Page
 from mimetypes import guess_extension
 from pprint import pprint
 from typing import List
 
-from .drive import DriveAPI
-
-class Command:
-    def __init__(self, str_, params: dict):
-        self._str = str_
-        self._params = params
-        self._timestamp = datetime.now()
+from ._drive import DriveAPI
 
 class DriveAPICommands(discord.ext.commands.Cog):
     
     _drive_state = defaultdict(lambda: defaultdict(id=None, folders=[], files=[]))
     _wd_cache = None
     
 
@@ -47,43 +41,20 @@
             DriveAPICommands._drive_state[self.root_path]["id"] = self.API.ROOT_ID
             DriveAPICommands._drive_state[self.root_path]["folders"] = [folder["name"] for folder in items if folder['mimeType'].startswith(self.API.FOLDER_TYPE)]
             DriveAPICommands._drive_state[self.root_path]["files"] = [file["name"] for file in items if not file['mimeType'].startswith(self.API.FOLDER_TYPE)]
         
         # self.root_alias = '~'
         self.capacity = 15
         
-        self._command_history = defaultdict(lambda: deque())
         DriveAPICommands._wd_cache = defaultdict(lambda: [pathlib.Path(self.root), pathlib.Path(self.root)])
         
     async def _API_ready(self, ctx: discord.ApplicationContext):
         if not (result := bool(self.API.service)):
             await ctx.send_response("Please use `/authenticate` to validate your Google Account's credentials before using any commands!")
         return result
-
-    def _save_to_history(self, id_, command: Command):
-        if len(self._command_history[id_]) == self.capacity:
-            self._command_history[id_].popleft()
-            
-        self._command_history[id_].append(command)
-        # print(self._history[id_].pop()._str)
-        # print(command._str, command._params)
-    
-    def _get_last_command(self, id_) -> Command:
-        return self._command_history[id_].pop()
-    
-    def _get_last_commands(self, id_, n: int) -> List[Command]:
-        
-        if n > len(self._command_history[id_]):
-            raise IndexError
-        
-        commands = []
-        for _ in range(n):
-            commands.append(self._get_last_command(id_))
-        
-        return commands
     
     async def _get_user_color(self, ctx: discord.ApplicationContext) -> discord.Colour:
         avatar_byte_array = await ctx.author.display_avatar.with_format("png").read()
         arr = np.asarray(bytearray(avatar_byte_array), dtype=np.uint8)
         img = cv2.imdecode(arr, -1)
         
         red = int(np.average(img[:, :, 0]))
@@ -105,16 +76,14 @@
     @discord.ext.commands.slash_command(name="upload", description="Upload a file to your Google Drive")
     async def upload(self, ctx: discord.ApplicationContext, file: discord.SlashCommandOptionType.attachment):
 
         if not await self._API_ready(ctx):
             return
         
         await ctx.defer()
-        
-        locals_ = locals()
 
         folder_id = DriveAPICommands._drive_state[DriveAPICommands._wd_cache[ctx.author.id][0]]["id"]
         result = await self.API.upload_from_discord(file=file, parent=folder_id)
         if result:
             files = self.API.search(parent=folder_id, folders=False, page_size=100, recursive=True)
             DriveAPICommands._drive_state[DriveAPICommands._wd_cache[ctx.author.id][0]]["files"] = [file["name"] for file in files]
 
@@ -129,23 +98,14 @@
             embed.add_field(name="", value=result, inline=True)
 
             embed.set_footer(text=DriveAPICommands._wd_cache[ctx.author.id][0])
 
             await ctx.send_followup(embed=embed)
         else:
             return
-        
-        
-        self._save_to_history(
-            id_=ctx.author.id,
-            command=Command(
-                str_=sys._getframe(0).f_code.co_name,
-                params=locals_
-            )
-        )
     
     @discord.ext.commands.slash_command(name="pwd", description="Print your current working directory")
     async def pwd(self, ctx: discord.ApplicationContext):
 
         if not await self._API_ready(ctx):
             return
 
@@ -179,16 +139,14 @@
         return ["~", "..", *DriveAPICommands._drive_state[DriveAPICommands._wd_cache[ctx.interaction.user.id][0]]["folders"]]
 
     @discord.ext.commands.slash_command(name="cd", description="Change your current working directory")
     async def cd(self, ctx: discord.ApplicationContext, path: discord.Option(str, "Pick a folder", autocomplete=discord.utils.basic_autocomplete(_get_folders))): # type: ignore
         
         if not await self._API_ready(ctx):
             return
-    
-        locals_ = locals()
         
         folder_id = DriveAPICommands._drive_state[DriveAPICommands._wd_cache[ctx.author.id][0]]["id"]
         
         last_path = DriveAPICommands._wd_cache[ctx.author.id][0]
         DriveAPICommands._wd_cache[ctx.author.id][1] = last_path
         
         user_color = await self._get_user_color(ctx)
@@ -233,22 +191,14 @@
             if not folder:
                 embed.add_field(name="", value=f"{path} is not reachable from your current directory.", inline=True)
                 await ctx.send_response(embed=embed)
                 return
 
             path, folder_id = folder[0]["name"], folder[0]["id"]
             DriveAPICommands._wd_cache[ctx.author.id][0] /= path
-
-        self._save_to_history(
-            id_=ctx.author.id,
-            command=Command(
-                str_=sys._getframe(0).f_code.co_name,
-                params=locals_
-            )
-        )
         
         items = self.API.search(parent=folder_id, page_size=100, recursive=True)
         DriveAPICommands._drive_state[DriveAPICommands._wd_cache[ctx.author.id][0]]["id"] = folder_id
         DriveAPICommands._drive_state[DriveAPICommands._wd_cache[ctx.author.id][0]]["folders"] = [folder["name"] for folder in items if folder['mimeType'].startswith(self.API.FOLDER_TYPE)]
         DriveAPICommands._drive_state[DriveAPICommands._wd_cache[ctx.author.id][0]]["files"] = [file["name"] for file in items if not file['mimeType'].startswith(self.API.FOLDER_TYPE)]
         
         embed.add_field(name="", value=f"Directory changed to `{DriveAPICommands._wd_cache[ctx.author.id][0]}`", inline=True)
@@ -256,17 +206,14 @@
         
     @discord.ext.commands.slash_command(name="ls", description="List all files in your current working directory")
     async def ls(self, ctx: discord.ApplicationContext):
 
         if not await self._API_ready(ctx):
             return
         
-        locals_ = locals()
-        # items_per_page = int(items_per_page)
-        
         def convert_size(size_bytes):
             if size_bytes == 0:
                 return "0 B"
             size_name = ("B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB")
             i = int(math.floor(math.log(size_bytes, 1024)))
             p = math.pow(1024, i)
             s = round(size_bytes / p, 2)
@@ -312,22 +259,14 @@
                         ]# Pycord provides a class with default colors you can choose from
                 )
                 for i in range(0, len(item_icon_list), items_per_page)
             ]
         )
 
         await paginated_list.respond(ctx.interaction, ephemeral=True)
-        
-        self._save_to_history(
-            id_=ctx.author.id,
-            command=Command(
-                str_=sys._getframe(0).f_code.co_name,
-                params=locals_
-            )
-        )
     
     async def _get_files(ctx: discord.AutocompleteContext):
         return DriveAPICommands._drive_state[DriveAPICommands._wd_cache[ctx.interaction.user.id][0]]["files"]
 
     @discord.ext.commands.slash_command(name="download", description="Download a file from your current working directory")
     async def download(
         self, 
@@ -433,16 +372,14 @@
     
     @discord.ext.commands.slash_command(name="mkdir", description="Make a new folder in your current working directory")
     @has_permissions(administrator=True)
     async def mkdir(self, ctx: discord.ApplicationContext, folder_name: discord.SlashCommandOptionType.string):
 
         if not await self._API_ready(ctx):
             return
-        
-        locals_ = locals()
 
         parent_id = DriveAPICommands._drive_state[DriveAPICommands._wd_cache[ctx.author.id][0]]["id"]
         success = self.API.make_folder(file_name=folder_name, parent=parent_id)
         
         user_color = await self._get_user_color(ctx)
         embed = discord.Embed(
             title=f"Make Directory",
@@ -458,23 +395,14 @@
             folders = self.API.search(parent=parent_id, files=False, page_size=100, recursive=True)
             DriveAPICommands._drive_state[DriveAPICommands._wd_cache[ctx.author.id][0]]["id"] = parent_id
             DriveAPICommands._drive_state[DriveAPICommands._wd_cache[ctx.author.id][0]]["folders"] = [folder["name"] for folder in folders]
             
         else:
             embed.add_field(name="", value="Could not create folder.", inline=True)
             await ctx.send_response(embed=embed)
-            
-        self._save_to_history(
-            id_=ctx.author.id,
-            command=Command(
-                str_=sys._getframe(0).f_code.co_name,
-                params=locals_
-            )
-        )
-    
     
     @discord.ext.commands.slash_command(name="authenticate", description="Authenticate your google account")
     @has_permissions(administrator=True)
     async def authenticate(self, ctx: discord.ApplicationContext):
         await ctx.defer()
 
         embed = discord.Embed(
@@ -489,14 +417,20 @@
             embed.set_author(name=ctx.author.name, icon_url=ctx.author.display_avatar.url)
 
             await ctx.respond(embed=embed)
             return
 
         # Generate a url for the user to visit
         flow, auth_url = self.API.generate_flow()
+        if (flow, auth_url) == (None, None):
+            embed.title = "credentials.json was not found or could not be processed, please ensure that you have generated the file correctly with Google Cloud and that it is in the working directory."
+            embed.add_field(name="", value="[Google Drive Developer quick-start instructions](https://developers.google.com/drive/api/quickstart/python)")
+            response = await ctx.respond(embed=embed)
+            return
+            
 
         # Tell the user to check their dms
         response = await ctx.respond(embed=embed)
         
         # DM the user to visit the url
         await ctx.author.send(f'Please go to [this URL]({auth_url}) and respond with the authorization code.')
 
@@ -525,44 +459,14 @@
         
         if self.API.service is not None:
             items = self.API.search(parent=self.API.ROOT_ID, page_size=100, recursive=True)
             DriveAPICommands._drive_state[self.root_path]["id"] = self.API.ROOT_ID
             DriveAPICommands._drive_state[self.root_path]["folders"] = [folder["name"] for folder in items if folder['mimeType'].startswith(self.API.FOLDER_TYPE)]
             DriveAPICommands._drive_state[self.root_path]["files"] = [file["name"] for file in items if not file['mimeType'].startswith(self.API.FOLDER_TYPE)]
     
-    @discord.ext.commands.slash_command(name="getn", description="DEBUG: Get last n commands")
-    @has_permissions(administrator=True)
-    async def getn(self, ctx: discord.ApplicationContext, n: discord.SlashCommandOptionType.integer):
-
-        if not await self._API_ready(ctx):
-            return
-        
-        locals_ = locals()
-        
-        try:
-            commands = self._get_last_commands(ctx.author.id, int(n))
-        except IndexError:
-            await ctx.send_response("Error retrieving commands")
-            return
-            
-        
-        for command in commands:
-            pprint(f"{command._timestamp} - Command: {command._str}\nParams: {command._params}")
-        
-        self._save_to_history(
-            id_=ctx.author.id,
-            command=Command(
-                str_=sys._getframe(0).f_code.co_name,
-                params=locals_
-            )
-        )
-        
-        # print(locals_)
-        await ctx.send_response("Commands printed")
-    
     @discord.ext.commands.slash_command(name="discord_drive_commands", description="Show all useable commands")
     async def help(self, ctx: discord.ApplicationContext):
         user_color = await self._get_user_color(ctx)
         embed = discord.Embed(
             title=f"Commands List",
             color=user_color,
         )
```

