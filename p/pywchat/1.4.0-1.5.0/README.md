# Comparing `tmp/pywchat-1.4.0.tar.gz` & `tmp/pywchat-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywchat-1.4.0.tar", last modified: Fri Jan 26 12:55:45 2024, max compression
+gzip compressed data, was "pywchat-1.5.0.tar", last modified: Tue Apr 16 13:00:26 2024, max compression
```

## Comparing `pywchat-1.4.0.tar` & `pywchat-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-01-26 12:55:45.149477 pywchat-1.4.0/
--rw-rw-rw-   0        0        0    35823 2021-09-15 12:58:14.000000 pywchat-1.4.0/LICENSE
--rw-rw-rw-   0        0        0    10917 2024-01-26 12:55:45.146164 pywchat-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    10460 2024-01-26 12:17:03.000000 pywchat-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-26 12:55:45.117700 pywchat-1.4.0/pywchat/
--rw-rw-rw-   0        0        0       24 2021-09-15 12:58:14.000000 pywchat-1.4.0/pywchat/__init__.py
--rw-rw-rw-   0        0        0      325 2021-09-15 12:58:14.000000 pywchat-1.4.0/pywchat/chatapi.py
--rw-rw-rw-   0        0        0     5478 2021-09-15 12:58:14.000000 pywchat-1.4.0/pywchat/send.py
--rw-rw-rw-   0        0        0    12921 2024-01-26 12:52:43.000000 pywchat-1.4.0/pywchat/workhandler.py
-drwxrwxrwx   0        0        0        0 2024-01-26 12:55:45.146164 pywchat-1.4.0/pywchat.egg-info/
--rw-rw-rw-   0        0        0    10917 2024-01-26 12:55:45.000000 pywchat-1.4.0/pywchat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-01-26 12:55:45.000000 pywchat-1.4.0/pywchat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-26 12:55:45.000000 pywchat-1.4.0/pywchat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-01-26 12:55:45.000000 pywchat-1.4.0/pywchat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-26 12:55:45.000000 pywchat-1.4.0/pywchat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-26 12:55:45.149477 pywchat-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      761 2024-01-26 12:22:05.000000 pywchat-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:26.028585 pywchat-1.5.0/
+-rw-rw-rw-   0        0        0    35823 2021-09-15 12:58:14.000000 pywchat-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0    11378 2024-04-16 13:00:26.027584 pywchat-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10890 2024-04-16 12:55:42.000000 pywchat-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:26.004584 pywchat-1.5.0/pywchat/
+-rw-rw-rw-   0        0        0       24 2021-09-15 12:58:14.000000 pywchat-1.5.0/pywchat/__init__.py
+-rw-rw-rw-   0        0        0      389 2024-04-16 12:39:23.000000 pywchat-1.5.0/pywchat/chatapi.py
+-rw-rw-rw-   0        0        0     5903 2024-04-16 12:50:45.000000 pywchat-1.5.0/pywchat/send.py
+-rw-rw-rw-   0        0        0    13284 2024-04-16 12:47:34.000000 pywchat-1.5.0/pywchat/workhandler.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:26.026581 pywchat-1.5.0/pywchat.egg-info/
+-rw-rw-rw-   0        0        0    11378 2024-04-16 13:00:25.000000 pywchat-1.5.0/pywchat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-04-16 13:00:25.000000 pywchat-1.5.0/pywchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 13:00:25.000000 pywchat-1.5.0/pywchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-16 13:00:25.000000 pywchat-1.5.0/pywchat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 13:00:25.000000 pywchat-1.5.0/pywchat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 13:00:26.029592 pywchat-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      759 2024-04-16 12:58:56.000000 pywchat-1.5.0/setup.py
```

### Comparing `pywchat-1.4.0/LICENSE` & `pywchat-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywchat-1.4.0/PKG-INFO` & `pywchat-1.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,27 @@
-Metadata-Version: 2.1
-Name: pywchat
-Version: 1.4.0
-Summary: Custom WeChat push information database
-Home-page: https://github.com/HangJau/pychatbot
-Author: Hangjau
-Author-email: hangjau818@gmail.com
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pywchat
 ### 项目介绍
 
 项目是根据企业微信可与微信进行互通的前提，通过操作企业微信的开放API达到将消息通知到微信.只封装了**微信能够接收的信息类型**以及上传临时素材等一些辅助接口. 
-要使用该项目请先自己注册一个企业微信(无需认证) 注册文档
+要使用该项目请先自己注册一个企业微信(无需认证) [注册文档](https://mp.weixin.qq.com/s/EIw_kdNFzrJjDarEzN6-gA
+)
 
 ### 项目相关文档
 
 ​		**项目地址** ：https://github.com/HangJau/pywchat.git
 
 ​		**企业微信API**：[ 企业微信API (qq.com)](https://work.weixin.qq.com/api/doc/90000/90135/90236)
 
 ### 项目实现	
 
 1. 已实现配置信息进行初始化.
 
 2. 已实现对token的离线保存，以及token失效的自动获取.
 
-3. 已实现对[text](#send_text)、[image](#send_image)、[voice](#send_voice)、[video](#send_video)、[file](#send_file)、[textcard](#send_textcard)、[graphic](#send_graphic)、[upload_image](#upload_image)、[get_user_id](#get_user_id)消息的发送封装.
+3. 已实现对[text](#send_text)、[image](#send_image)、[voice](#send_voice)、[video](#send_video)、[file](#send_file)、[textcard](#send_textcard)、[graphic](#send_graphic)、[upload_image](#upload_image)、[get_user_id](#get_user_id)、[get_user_id_by_email](#get_user_id_by_email)消息的发送封装.
 
 4. 已实现对错误返回的处理.
 
   
 
 ### 项目下载		
 
@@ -56,14 +43,22 @@
     app = Sender(corpid,corpsecret,agentid)
     
     第二种：传入配置文件路径.读取配置并在当前路径生成一个.token文件(理论上文件也可无后缀且能读取成text即可，格式可参考配置介绍)
     app = Sender(path=r"G:\chat\conf.ini")
     
     第三种：不传任何参. 动态输入所需的corpid,corpsecret,agentid,并在当前路径生成一个.chatkey,.token两个文件
     app = Sender()
+    
+#### tips:
+
+    corpid: str
+    
+    corpsecret: str
+    
+    agentid: int
 
 
 ​    
 
 ### 配置介绍
 
     目前会有两个文件“ .chatkey” “ .token”
@@ -90,15 +85,15 @@
 
 #### <span id="send_text">send_text</span>
 
       发送纯文本消息，支持换行、以及A标签，大小最长不超过2048字节
       
       参数：
            message: 需要发送的消息
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认touser=@all
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认touser=@all
            
       例：
            app.send_text("又有一个富婆看了你的帅照啦..", touser="ZhuRen|user1")
            app.send_text("又有一个富婆看了你的帅照啦..", todept="1|2")
            app.send_text("又有一个富婆看了你的帅照啦..", totags="A")
       		
       tips:
@@ -111,15 +106,15 @@
 
 #### <span id="send_image">send_image</span>
 
       发送纯图片消息，仅支持jpg,png格式，大小5B~2M
       接收的多个用户用 | 拼接
       参数：
            iamge_path: 发送图片的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_image(r"G:\caht\image.jpg", touser="ZhuRen|user1")
            app.send_image(r"G:\caht\image.jpg", todept="1|2")
            app.send_image(r"G:\caht\image.jpg", totags="A")
            
       tips:
@@ -131,15 +126,15 @@
 
 #### <span id="send_voice">send_voice</span>
 
       发送语音消息，仅支持amr格式，大小5B~2M
       
       参数：
            voice_path: 发送语音文件的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_voice(r"G:\caht\语音.amr", touser="ZhuRen|user1")
            app.send_voice(r"G:\caht\语音.amr", todept="1|2")
            app.send_voice(r"G:\caht\语音.amr", totags="A")
            
       tips:
@@ -150,15 +145,15 @@
 
 #### <span id="send_video">send_video</span>
 
       发送视频消息，仅支持MP4格式的视频消息，大小5B~10M
       
       参数：
            video_path: 发送视频文件的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_video(r"G:\caht\视频.mp4", touser="ZhuRen|user1")
            app.send_video(r"G:\caht\视频.MP4", todept="1|2")
            app.send_video(r"G:\caht\视频.mp4", totags="A")
            
       tips:
@@ -171,15 +166,15 @@
 
 #### <span id="send_file">send_file</span>
 
       发送文件消息, 大小5B~10M
       
       参数：
            file_path: 发送文件的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_file(r"G:\caht\富婆联系表.xlsx", touser="ZhuRen|user1")
            app.send_file(r"G:\caht\富婆联系表.xlsx", todept="1|2")
            app.send_file(r"G:\caht\富婆联系表.xlsx", totags="A")
            
       tips:
@@ -195,15 +190,15 @@
       发送文字卡片消息，点击卡片后跳转到设定的链接
       
       参数：
            card_title: 标题，不超过128个字节，超过会自动截断
            desc: 描述，不超过512个字节，超过会自动截断
            link: 点击后跳转的链接。最长2048字节，请确保包含了协议头(http/https)
            btn: 按钮文字。 默认为“详情”， 不超过4个文字，超过自动截断.
-           kwargs: 可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs: 可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
        
       例：
            app.send_textcard("富婆任务通知", "2021年10月24日\n您关注的富婆发布了最新的任务.","https://www.RichWoman.com/task/1",touser="ZhuRen")
            
            app.send_textcard("富婆任务通知", "2021年10月24日\n您关注的富婆发布了最新的任务.","https://www.RichWoman.com/task/1",todept="1|2")
            
            app.send_textcard("富婆任务通知", "2021年10月24日\n您关注的富婆发布了最新的任务.","https://www.RichWoman.com/task/1",totags="A")
@@ -222,15 +217,15 @@
   发送图文卡片消息，点击卡片后跳转到设定的链接
   
   参数：
        cardtitle: 标题，不超过128个字节，超过会自动截断
        desc: 描述，不超过512个字节，超过会自动截断
        link: 点击后跳转的链接。最长2048字节，请确保包含了协议头(http/https)
        image_link: 卡片中显示图片的url.如何获取参考(upload_iamge)
-       kwargs: 可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+       kwargs: 可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
        
   例：
        app.send_graphic("富婆动态通知", "您关注的富婆发布了最新的照片.", "https://www.RichWoman.com/dynamic/1/", "https://www.RichWoman.com/dynamic/1/photos/fp.jpg", touser="ZhuRen|user1")
        app.send_graphic("富婆动态通知", "您关注的富婆发布了最新的照片.", "https://www.RichWoman.com/dynamic/1/", "https://www.RichWoman.com/dynamic/1/photos/fp.jpg", todeot="1|2")
        app.send_graphic("富婆动态通知", "您关注的富婆发布了最新的照片.", "https://www.RichWoman.com/dynamic/1/", "https://www.RichWoman.com/dynamic/1/photos/fp.jpg", totags="A")
    
    tips:
@@ -271,14 +266,23 @@
            fetch_child: 是否递归子部门下的员工信息，默认为0，不递归
       
       例：
            get_userid(1)
            
       tips:
       		该方法会输出并返回用户.
-      		默认为touser=@all, 发送全体用户，注意指定接收对象
-      		接收的多个用户用 | 拼接
-
 
+#### <span id="get_user_id_by_email">get_user_id_by_email</span> 
+     通过email获取员工信息
+    
+    参数：
+           email: 邮箱账号
+           email_type: 邮箱类型 1：企业 2：个人，默认为1
+      
+      例：
+           get_user_id_by_email("test@cloub.com")
+           
+      tips:
+      		该方法会返回用户信息.
```

### Comparing `pywchat-1.4.0/README.md` & `pywchat-1.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,42 @@
+Metadata-Version: 2.1
+Name: pywchat
+Version: 1.5.0
+Summary: Custom WeChat push information database
+Home-page: https://github.com/HangJau/pywchat
+Author: Hangjau
+Author-email: hangjau818@gmail.com
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.22.0
+
 # pywchat
 ### 项目介绍
 
 项目是根据企业微信可与微信进行互通的前提，通过操作企业微信的开放API达到将消息通知到微信.只封装了**微信能够接收的信息类型**以及上传临时素材等一些辅助接口. 
-要使用该项目请先自己注册一个企业微信(无需认证) 注册文档
+要使用该项目请先自己注册一个企业微信(无需认证) [注册文档](https://mp.weixin.qq.com/s/EIw_kdNFzrJjDarEzN6-gA
+)
 
 ### 项目相关文档
 
 ​		**项目地址** ：https://github.com/HangJau/pywchat.git
 
 ​		**企业微信API**：[ 企业微信API (qq.com)](https://work.weixin.qq.com/api/doc/90000/90135/90236)
 
 ### 项目实现	
 
 1. 已实现配置信息进行初始化.
 
 2. 已实现对token的离线保存，以及token失效的自动获取.
 
-3. 已实现对[text](#send_text)、[image](#send_image)、[voice](#send_voice)、[video](#send_video)、[file](#send_file)、[textcard](#send_textcard)、[graphic](#send_graphic)、[upload_image](#upload_image)、[get_user_id](#get_user_id)消息的发送封装.
+3. 已实现对[text](#send_text)、[image](#send_image)、[voice](#send_voice)、[video](#send_video)、[file](#send_file)、[textcard](#send_textcard)、[graphic](#send_graphic)、[upload_image](#upload_image)、[get_user_id](#get_user_id)、[get_user_id_by_email](#get_user_id_by_email)消息的发送封装.
 
 4. 已实现对错误返回的处理.
 
   
 
 ### 项目下载		
 
@@ -42,14 +58,22 @@
     app = Sender(corpid,corpsecret,agentid)
     
     第二种：传入配置文件路径.读取配置并在当前路径生成一个.token文件(理论上文件也可无后缀且能读取成text即可，格式可参考配置介绍)
     app = Sender(path=r"G:\chat\conf.ini")
     
     第三种：不传任何参. 动态输入所需的corpid,corpsecret,agentid,并在当前路径生成一个.chatkey,.token两个文件
     app = Sender()
+    
+#### tips:
+
+    corpid: str
+    
+    corpsecret: str
+    
+    agentid: int
 
 
 ​    
 
 ### 配置介绍
 
     目前会有两个文件“ .chatkey” “ .token”
@@ -76,15 +100,15 @@
 
 #### <span id="send_text">send_text</span>
 
       发送纯文本消息，支持换行、以及A标签，大小最长不超过2048字节
       
       参数：
            message: 需要发送的消息
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认touser=@all
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认touser=@all
            
       例：
            app.send_text("又有一个富婆看了你的帅照啦..", touser="ZhuRen|user1")
            app.send_text("又有一个富婆看了你的帅照啦..", todept="1|2")
            app.send_text("又有一个富婆看了你的帅照啦..", totags="A")
       		
       tips:
@@ -97,15 +121,15 @@
 
 #### <span id="send_image">send_image</span>
 
       发送纯图片消息，仅支持jpg,png格式，大小5B~2M
       接收的多个用户用 | 拼接
       参数：
            iamge_path: 发送图片的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_image(r"G:\caht\image.jpg", touser="ZhuRen|user1")
            app.send_image(r"G:\caht\image.jpg", todept="1|2")
            app.send_image(r"G:\caht\image.jpg", totags="A")
            
       tips:
@@ -117,15 +141,15 @@
 
 #### <span id="send_voice">send_voice</span>
 
       发送语音消息，仅支持amr格式，大小5B~2M
       
       参数：
            voice_path: 发送语音文件的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_voice(r"G:\caht\语音.amr", touser="ZhuRen|user1")
            app.send_voice(r"G:\caht\语音.amr", todept="1|2")
            app.send_voice(r"G:\caht\语音.amr", totags="A")
            
       tips:
@@ -136,15 +160,15 @@
 
 #### <span id="send_video">send_video</span>
 
       发送视频消息，仅支持MP4格式的视频消息，大小5B~10M
       
       参数：
            video_path: 发送视频文件的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_video(r"G:\caht\视频.mp4", touser="ZhuRen|user1")
            app.send_video(r"G:\caht\视频.MP4", todept="1|2")
            app.send_video(r"G:\caht\视频.mp4", totags="A")
            
       tips:
@@ -157,15 +181,15 @@
 
 #### <span id="send_file">send_file</span>
 
       发送文件消息, 大小5B~10M
       
       参数：
            file_path: 发送文件的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_file(r"G:\caht\富婆联系表.xlsx", touser="ZhuRen|user1")
            app.send_file(r"G:\caht\富婆联系表.xlsx", todept="1|2")
            app.send_file(r"G:\caht\富婆联系表.xlsx", totags="A")
            
       tips:
@@ -181,15 +205,15 @@
       发送文字卡片消息，点击卡片后跳转到设定的链接
       
       参数：
            card_title: 标题，不超过128个字节，超过会自动截断
            desc: 描述，不超过512个字节，超过会自动截断
            link: 点击后跳转的链接。最长2048字节，请确保包含了协议头(http/https)
            btn: 按钮文字。 默认为“详情”， 不超过4个文字，超过自动截断.
-           kwargs: 可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs: 可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
        
       例：
            app.send_textcard("富婆任务通知", "2021年10月24日\n您关注的富婆发布了最新的任务.","https://www.RichWoman.com/task/1",touser="ZhuRen")
            
            app.send_textcard("富婆任务通知", "2021年10月24日\n您关注的富婆发布了最新的任务.","https://www.RichWoman.com/task/1",todept="1|2")
            
            app.send_textcard("富婆任务通知", "2021年10月24日\n您关注的富婆发布了最新的任务.","https://www.RichWoman.com/task/1",totags="A")
@@ -208,15 +232,15 @@
   发送图文卡片消息，点击卡片后跳转到设定的链接
   
   参数：
        cardtitle: 标题，不超过128个字节，超过会自动截断
        desc: 描述，不超过512个字节，超过会自动截断
        link: 点击后跳转的链接。最长2048字节，请确保包含了协议头(http/https)
        image_link: 卡片中显示图片的url.如何获取参考(upload_iamge)
-       kwargs: 可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+       kwargs: 可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
        
   例：
        app.send_graphic("富婆动态通知", "您关注的富婆发布了最新的照片.", "https://www.RichWoman.com/dynamic/1/", "https://www.RichWoman.com/dynamic/1/photos/fp.jpg", touser="ZhuRen|user1")
        app.send_graphic("富婆动态通知", "您关注的富婆发布了最新的照片.", "https://www.RichWoman.com/dynamic/1/", "https://www.RichWoman.com/dynamic/1/photos/fp.jpg", todeot="1|2")
        app.send_graphic("富婆动态通知", "您关注的富婆发布了最新的照片.", "https://www.RichWoman.com/dynamic/1/", "https://www.RichWoman.com/dynamic/1/photos/fp.jpg", totags="A")
    
    tips:
@@ -257,14 +281,23 @@
            fetch_child: 是否递归子部门下的员工信息，默认为0，不递归
       
       例：
            get_userid(1)
            
       tips:
       		该方法会输出并返回用户.
-      		默认为touser=@all, 发送全体用户，注意指定接收对象
-      		接收的多个用户用 | 拼接
-
 
+#### <span id="get_user_id_by_email">get_user_id_by_email</span> 
+     通过email获取员工信息
+    
+    参数：
+           email: 邮箱账号
+           email_type: 邮箱类型 1：企业 2：个人，默认为1
+      
+      例：
+           get_user_id_by_email("test@cloub.com")
+           
+      tips:
+      		该方法会返回用户信息.
```

### Comparing `pywchat-1.4.0/pywchat/send.py` & `pywchat-1.5.0/pywchat/send.py`

 * *Files 8% similar despite different names*

```diff
@@ -131,8 +131,18 @@
         :param fetch_child:  是否递归查询子部门员工
         :return: 会显示所有的员工信息，主要用于查询对应用户的userid进行发送
         """
 
         params = {"department_id": department_id, "fetch_child": fetch_child}
         self._Handler.get_users_id(params)
 
+    def get_user_id_by_email(self, email, email_type=1):
+        """
+        通过email查询员工
+        :param email: 邮箱
+        :param email_type:  邮箱类型 1 企业 2 个人
+        :return: 会显示所有的员工信息，主要用于查询对应用户的userid进行发送
+        """
+
+        params = {"email": email, "email_type": email_type}
+        self._Handler.get_user_id_by_email(params)
```

### Comparing `pywchat-1.4.0/pywchat/workhandler.py` & `pywchat-1.5.0/pywchat/workhandler.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,18 @@
     @abstractmethod
     def upload_image(self, *args, **kwargs):
         pass
 
     @abstractmethod
     def get_users_id(self, *args, **kwargs):
         pass
-
+        
+    @abstractmethod
+    def get_user_id_by_email(self, *args, **kwargs):
+        pass
 
 tokenp = Path.cwd().joinpath(".token")
 logging.basicConfig(level=logging.INFO, format=("%(asctime)s  [%(levelname)s]  %(message)s"))
 
 
 class HandlerTool:
     """
@@ -338,7 +341,15 @@
         data["access_token"] = self.token
         rsp_users = self._get(chat_api.get('GET_USERS'), params=data)
         users_info = rsp_users.get("userlist")
         for i in users_info:
             logging.info(i)
 
         return users_info
+
+    def get_user_id_by_email(self, data):
+        data["access_token"] = self.token
+        rsp_users = self._get(chat_api.get('GET_USERID_EMAIL'), params=data)
+        user_id = rsp_users.get("userid")
+        logging.info(user_id)
+
+        return user_id
```

### Comparing `pywchat-1.4.0/pywchat.egg-info/PKG-INFO` & `pywchat-1.5.0/pywchat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: pywchat
-Version: 1.4.0
+Version: 1.5.0
 Summary: Custom WeChat push information database
-Home-page: https://github.com/HangJau/pychatbot
+Home-page: https://github.com/HangJau/pywchat
 Author: Hangjau
 Author-email: hangjau818@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.22.0
 
 # pywchat
 ### 项目介绍
 
 项目是根据企业微信可与微信进行互通的前提，通过操作企业微信的开放API达到将消息通知到微信.只封装了**微信能够接收的信息类型**以及上传临时素材等一些辅助接口. 
-要使用该项目请先自己注册一个企业微信(无需认证) 注册文档
+要使用该项目请先自己注册一个企业微信(无需认证) [注册文档](https://mp.weixin.qq.com/s/EIw_kdNFzrJjDarEzN6-gA
+)
 
 ### 项目相关文档
 
 ​		**项目地址** ：https://github.com/HangJau/pywchat.git
 
 ​		**企业微信API**：[ 企业微信API (qq.com)](https://work.weixin.qq.com/api/doc/90000/90135/90236)
 
 ### 项目实现	
 
 1. 已实现配置信息进行初始化.
 
 2. 已实现对token的离线保存，以及token失效的自动获取.
 
-3. 已实现对[text](#send_text)、[image](#send_image)、[voice](#send_voice)、[video](#send_video)、[file](#send_file)、[textcard](#send_textcard)、[graphic](#send_graphic)、[upload_image](#upload_image)、[get_user_id](#get_user_id)消息的发送封装.
+3. 已实现对[text](#send_text)、[image](#send_image)、[voice](#send_voice)、[video](#send_video)、[file](#send_file)、[textcard](#send_textcard)、[graphic](#send_graphic)、[upload_image](#upload_image)、[get_user_id](#get_user_id)、[get_user_id_by_email](#get_user_id_by_email)消息的发送封装.
 
 4. 已实现对错误返回的处理.
 
   
 
 ### 项目下载		
 
@@ -56,14 +58,22 @@
     app = Sender(corpid,corpsecret,agentid)
     
     第二种：传入配置文件路径.读取配置并在当前路径生成一个.token文件(理论上文件也可无后缀且能读取成text即可，格式可参考配置介绍)
     app = Sender(path=r"G:\chat\conf.ini")
     
     第三种：不传任何参. 动态输入所需的corpid,corpsecret,agentid,并在当前路径生成一个.chatkey,.token两个文件
     app = Sender()
+    
+#### tips:
+
+    corpid: str
+    
+    corpsecret: str
+    
+    agentid: int
 
 
 ​    
 
 ### 配置介绍
 
     目前会有两个文件“ .chatkey” “ .token”
@@ -90,15 +100,15 @@
 
 #### <span id="send_text">send_text</span>
 
       发送纯文本消息，支持换行、以及A标签，大小最长不超过2048字节
       
       参数：
            message: 需要发送的消息
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认touser=@all
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认touser=@all
            
       例：
            app.send_text("又有一个富婆看了你的帅照啦..", touser="ZhuRen|user1")
            app.send_text("又有一个富婆看了你的帅照啦..", todept="1|2")
            app.send_text("又有一个富婆看了你的帅照啦..", totags="A")
       		
       tips:
@@ -111,15 +121,15 @@
 
 #### <span id="send_image">send_image</span>
 
       发送纯图片消息，仅支持jpg,png格式，大小5B~2M
       接收的多个用户用 | 拼接
       参数：
            iamge_path: 发送图片的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_image(r"G:\caht\image.jpg", touser="ZhuRen|user1")
            app.send_image(r"G:\caht\image.jpg", todept="1|2")
            app.send_image(r"G:\caht\image.jpg", totags="A")
            
       tips:
@@ -131,15 +141,15 @@
 
 #### <span id="send_voice">send_voice</span>
 
       发送语音消息，仅支持amr格式，大小5B~2M
       
       参数：
            voice_path: 发送语音文件的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_voice(r"G:\caht\语音.amr", touser="ZhuRen|user1")
            app.send_voice(r"G:\caht\语音.amr", todept="1|2")
            app.send_voice(r"G:\caht\语音.amr", totags="A")
            
       tips:
@@ -150,15 +160,15 @@
 
 #### <span id="send_video">send_video</span>
 
       发送视频消息，仅支持MP4格式的视频消息，大小5B~10M
       
       参数：
            video_path: 发送视频文件的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_video(r"G:\caht\视频.mp4", touser="ZhuRen|user1")
            app.send_video(r"G:\caht\视频.MP4", todept="1|2")
            app.send_video(r"G:\caht\视频.mp4", totags="A")
            
       tips:
@@ -171,15 +181,15 @@
 
 #### <span id="send_file">send_file</span>
 
       发送文件消息, 大小5B~10M
       
       参数：
            file_path: 发送文件的本地路径
-           kwargs:  可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs:  可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
     
       例：
            app.send_file(r"G:\caht\富婆联系表.xlsx", touser="ZhuRen|user1")
            app.send_file(r"G:\caht\富婆联系表.xlsx", todept="1|2")
            app.send_file(r"G:\caht\富婆联系表.xlsx", totags="A")
            
       tips:
@@ -195,15 +205,15 @@
       发送文字卡片消息，点击卡片后跳转到设定的链接
       
       参数：
            card_title: 标题，不超过128个字节，超过会自动截断
            desc: 描述，不超过512个字节，超过会自动截断
            link: 点击后跳转的链接。最长2048字节，请确保包含了协议头(http/https)
            btn: 按钮文字。 默认为“详情”， 不超过4个文字，超过自动截断.
-           kwargs: 可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+           kwargs: 可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
        
       例：
            app.send_textcard("富婆任务通知", "2021年10月24日\n您关注的富婆发布了最新的任务.","https://www.RichWoman.com/task/1",touser="ZhuRen")
            
            app.send_textcard("富婆任务通知", "2021年10月24日\n您关注的富婆发布了最新的任务.","https://www.RichWoman.com/task/1",todept="1|2")
            
            app.send_textcard("富婆任务通知", "2021年10月24日\n您关注的富婆发布了最新的任务.","https://www.RichWoman.com/task/1",totags="A")
@@ -222,15 +232,15 @@
   发送图文卡片消息，点击卡片后跳转到设定的链接
   
   参数：
        cardtitle: 标题，不超过128个字节，超过会自动截断
        desc: 描述，不超过512个字节，超过会自动截断
        link: 点击后跳转的链接。最长2048字节，请确保包含了协议头(http/https)
        image_link: 卡片中显示图片的url.如何获取参考(upload_iamge)
-       kwargs: 可选择发送对象，tousers(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
+       kwargs: 可选择发送对象，touser(用户), todept(部门), totags(标签用户)可同时填入,默认为发送全部人
        
   例：
        app.send_graphic("富婆动态通知", "您关注的富婆发布了最新的照片.", "https://www.RichWoman.com/dynamic/1/", "https://www.RichWoman.com/dynamic/1/photos/fp.jpg", touser="ZhuRen|user1")
        app.send_graphic("富婆动态通知", "您关注的富婆发布了最新的照片.", "https://www.RichWoman.com/dynamic/1/", "https://www.RichWoman.com/dynamic/1/photos/fp.jpg", todeot="1|2")
        app.send_graphic("富婆动态通知", "您关注的富婆发布了最新的照片.", "https://www.RichWoman.com/dynamic/1/", "https://www.RichWoman.com/dynamic/1/photos/fp.jpg", totags="A")
    
    tips:
@@ -271,14 +281,23 @@
            fetch_child: 是否递归子部门下的员工信息，默认为0，不递归
       
       例：
            get_userid(1)
            
       tips:
       		该方法会输出并返回用户.
-      		默认为touser=@all, 发送全体用户，注意指定接收对象
-      		接收的多个用户用 | 拼接
-
 
+#### <span id="get_user_id_by_email">get_user_id_by_email</span> 
+     通过email获取员工信息
+    
+    参数：
+           email: 邮箱账号
+           email_type: 邮箱类型 1：企业 2：个人，默认为1
+      
+      例：
+           get_user_id_by_email("test@cloub.com")
+           
+      tips:
+      		该方法会返回用户信息.
```

### Comparing `pywchat-1.4.0/setup.py` & `pywchat-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r",encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pywchat",
-    version="1.4.0",
+    version="1.5.0",
     author="Hangjau",
     author_email="hangjau818@gmail.com",
     description="Custom WeChat push information database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     platforms='any',
-    url="https://github.com/HangJau/pychatbot",
+    url="https://github.com/HangJau/pywchat",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests>=2.22.0"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
```

