# Comparing `tmp/wxauto-3.9.8.15.1.tar.gz` & `tmp/wxauto-3.9.8.15.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wxauto-3.9.8.15.1.tar", last modified: Thu Apr 11 07:55:22 2024, max compression
+gzip compressed data, was "dist\wxauto-3.9.8.15.2.tar", last modified: Tue Apr 16 07:35:38 2024, max compression
```

## Comparing `wxauto-3.9.8.15.1.tar` & `wxauto-3.9.8.15.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 07:55:22.000000 wxauto-3.9.8.15.1/
--rw-rw-rw-   0        0        0     1083 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.1/LICENSE
--rw-rw-rw-   0        0        0     3771 2024-04-11 07:55:22.000000 wxauto-3.9.8.15.1/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 07:55:22.000000 wxauto-3.9.8.15.1/setup.cfg
--rw-rw-rw-   0        0        0      736 2024-04-11 07:55:09.000000 wxauto-3.9.8.15.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 07:55:22.000000 wxauto-3.9.8.15.1/wxauto/
--rw-rw-rw-   0        0        0       52 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.1/wxauto/__init__.py
--rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.1/wxauto/color.py
--rw-rw-rw-   0        0        0    23156 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.1/wxauto/elements.py
--rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.1/wxauto/errors.py
--rw-rw-rw-   0        0        0     5449 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.1/wxauto/languages.py
--rw-rw-rw-   0        0        0     8735 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.1/wxauto/utils.py
--rw-rw-rw-   0        0        0    23943 2024-04-11 02:50:33.000000 wxauto-3.9.8.15.1/wxauto/wxauto.py
-drwxrwxrwx   0        0        0        0 2024-04-11 07:55:22.000000 wxauto-3.9.8.15.1/wxauto.egg-info/
--rw-rw-rw-   0        0        0     3771 2024-04-11 07:55:22.000000 wxauto-3.9.8.15.1/wxauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-04-11 07:55:22.000000 wxauto-3.9.8.15.1/wxauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 07:55:22.000000 wxauto-3.9.8.15.1/wxauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-11 07:55:22.000000 wxauto-3.9.8.15.1/wxauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-11 07:55:22.000000 wxauto-3.9.8.15.1/wxauto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/
+-rw-rw-rw-   0        0        0     3648 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3283 2024-04-16 07:34:36.000000 wxauto-3.9.8.15.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/setup.cfg
+-rw-rw-rw-   0        0        0      736 2024-04-16 02:16:13.000000 wxauto-3.9.8.15.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto/
+-rw-rw-rw-   0        0        0       52 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/__init__.py
+-rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/color.py
+-rw-rw-rw-   0        0        0    23156 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/elements.py
+-rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/errors.py
+-rw-rw-rw-   0        0        0     5449 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/languages.py
+-rw-rw-rw-   0        0        0     8735 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/utils.py
+-rw-rw-rw-   0        0        0    23945 2024-04-16 02:16:44.000000 wxauto-3.9.8.15.2/wxauto/wxauto.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/
+-rw-rw-rw-   0        0        0     3648 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/top_level.txt
```

### Comparing `wxauto-3.9.8.15.1/PKG-INFO` & `wxauto-3.9.8.15.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.1
+Version: 3.9.8.15.2
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # wxauto  (适用PC微信3.9.8.15版本）
 
 ### 2023-11-20重写wxauto，欢迎指出bug，欢迎pull requests
 
 Windows版本微信客户端自动化，可实现简单的发送、接收微信消息、保存聊天图片
 
@@ -31,20 +30,18 @@
 |  微信  | [![Wechat](https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-3.9.8.X-07c160?logo=wechat&logoColor=white)](https://pan.baidu.com/s/1FvSw0Fk54GGvmQq8xSrNjA?pwd=vsmj) **(3.9.9疑似容易掉线)** |
 | Python | [![Python](https://img.shields.io/badge/Python-3.X-blue?logo=python&logoColor=white)](https://www.python.org/) **(不支持3.7.6和3.8.1)**|
 
 
 
 [![Star History Chart](https://api.star-history.com/svg?repos=cluic/wxauto&type=Date)](https://star-history.com/#cluic/wxauto)
 
-## 获取wxauto（请勿直接pip install）
+## 获取wxauto
 cmd窗口：
 ```shell
-git clone https://github.com/cluic/wxauto.git
-cd wxauto
-pip install -r requirements.txt
+pip install wxauto
 ```
 python窗口：
 ```python
 >>> import wxauto
 >>> wxauto.VERSION
 '3.9.8.15'
 >>> wx = wxauto.WeChat()
```

### Comparing `wxauto-3.9.8.15.1/README.md` & `wxauto-3.9.8.15.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,20 +18,18 @@
 |  微信  | [![Wechat](https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-3.9.8.X-07c160?logo=wechat&logoColor=white)](https://pan.baidu.com/s/1FvSw0Fk54GGvmQq8xSrNjA?pwd=vsmj) **(3.9.9疑似容易掉线)** |
 | Python | [![Python](https://img.shields.io/badge/Python-3.X-blue?logo=python&logoColor=white)](https://www.python.org/) **(不支持3.7.6和3.8.1)**|
 
 
 
 [![Star History Chart](https://api.star-history.com/svg?repos=cluic/wxauto&type=Date)](https://star-history.com/#cluic/wxauto)
 
-## 获取wxauto（请勿直接pip install）
+## 获取wxauto
 cmd窗口：
 ```shell
-git clone https://github.com/cluic/wxauto.git
-cd wxauto
-pip install -r requirements.txt
+pip install wxauto
 ```
 python窗口：
 ```python
 >>> import wxauto
 >>> wxauto.VERSION
 '3.9.8.15'
 >>> wx = wxauto.WeChat()
```

### Comparing `wxauto-3.9.8.15.1/setup.py` & `wxauto-3.9.8.15.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wxauto',
-    version='3.9.8.15.1',
+    version='3.9.8.15.2',
     author='Cluic',
     author_email='tikic@qq.com',
     description='A simple wechat automation tool',
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

### Comparing `wxauto-3.9.8.15.1/wxauto/color.py` & `wxauto-3.9.8.15.2/wxauto/color.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.1/wxauto/elements.py` & `wxauto-3.9.8.15.2/wxauto/elements.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.1/wxauto/languages.py` & `wxauto-3.9.8.15.2/wxauto/languages.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.1/wxauto/utils.py` & `wxauto-3.9.8.15.2/wxauto/utils.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.1/wxauto/wxauto.py` & `wxauto-3.9.8.15.2/wxauto/wxauto.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,15 @@
         self.listen[who].savepic = savepic
 
     def GetListenMessage(self):
         """获取监听对象的新消息"""
         msgs = {}
         for who in self.listen:
             chat = self.listen[who]
-            chat._show()
+            # chat._show()
             msg = chat.GetNewMessage(savepic=chat.savepic)
             # if [i for i in msg if i[0] != 'Self']:
             if msg:
                 msgs[chat] = msg
         return msgs
 
     def SwitchToContact(self):
```

### Comparing `wxauto-3.9.8.15.1/wxauto.egg-info/PKG-INFO` & `wxauto-3.9.8.15.2/wxauto.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.1
+Version: 3.9.8.15.2
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # wxauto  (适用PC微信3.9.8.15版本）
 
 ### 2023-11-20重写wxauto，欢迎指出bug，欢迎pull requests
 
 Windows版本微信客户端自动化，可实现简单的发送、接收微信消息、保存聊天图片
 
@@ -31,20 +30,18 @@
 |  微信  | [![Wechat](https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-3.9.8.X-07c160?logo=wechat&logoColor=white)](https://pan.baidu.com/s/1FvSw0Fk54GGvmQq8xSrNjA?pwd=vsmj) **(3.9.9疑似容易掉线)** |
 | Python | [![Python](https://img.shields.io/badge/Python-3.X-blue?logo=python&logoColor=white)](https://www.python.org/) **(不支持3.7.6和3.8.1)**|
 
 
 
 [![Star History Chart](https://api.star-history.com/svg?repos=cluic/wxauto&type=Date)](https://star-history.com/#cluic/wxauto)
 
-## 获取wxauto（请勿直接pip install）
+## 获取wxauto
 cmd窗口：
 ```shell
-git clone https://github.com/cluic/wxauto.git
-cd wxauto
-pip install -r requirements.txt
+pip install wxauto
 ```
 python窗口：
 ```python
 >>> import wxauto
 >>> wxauto.VERSION
 '3.9.8.15'
 >>> wx = wxauto.WeChat()
```

