# Comparing `tmp/python-bmob-1.6.0.tar.gz` & `tmp/python-bmob-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\python-bmob-1.6.0.tar", last modified: Sun Apr 14 10:10:44 2024, max compression
+gzip compressed data, was "python-bmob-1.7.0.tar", last modified: Tue Apr 16 07:13:25 2024, max compression
```

## Comparing `python-bmob-1.6.0.tar` & `python-bmob-1.7.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 10:10:44.531114 python-bmob-1.6.0/
--rw-rw-rw-   0        0        0      280 2024-04-14 10:10:44.531114 python-bmob-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-09 14:01:42.000000 python-bmob-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 10:10:44.518174 python-bmob-1.6.0/bmobpy/
--rw-rw-rw-   0        0        0       25 2024-04-09 14:54:42.000000 python-bmob-1.6.0/bmobpy/__init__.py
--rw-rw-rw-   0        0        0    36073 2024-04-14 10:09:23.000000 python-bmob-1.6.0/bmobpy/bmob.py
--rw-rw-rw-   0        0        0     4364 2024-04-14 09:53:19.000000 python-bmob-1.6.0/bmobpy/test.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:10:44.530114 python-bmob-1.6.0/python_bmob.egg-info/
--rw-rw-rw-   0        0        0      280 2024-04-14 10:10:44.000000 python-bmob-1.6.0/python_bmob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-04-14 10:10:44.000000 python-bmob-1.6.0/python_bmob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 10:10:44.000000 python-bmob-1.6.0/python_bmob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-14 10:10:44.000000 python-bmob-1.6.0/python_bmob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 10:10:44.531114 python-bmob-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      393 2024-04-14 10:10:30.000000 python-bmob-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:13:25.359569 python-bmob-1.7.0/
+-rw-rw-rw-   0        0        0     1084 2024-04-08 06:19:14.000000 python-bmob-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0      262 2024-04-16 07:13:25.358566 python-bmob-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-08 06:23:02.000000 python-bmob-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 07:13:25.337696 python-bmob-1.7.0/bmobpy/
+-rw-rw-rw-   0        0        0       25 2024-04-10 04:57:50.000000 python-bmob-1.7.0/bmobpy/__init__.py
+-rw-rw-rw-   0        0        0    38143 2024-04-16 07:09:58.000000 python-bmob-1.7.0/bmobpy/bmob.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:13:25.355567 python-bmob-1.7.0/python_bmob.egg-info/
+-rw-rw-rw-   0        0        0      262 2024-04-16 07:13:24.000000 python-bmob-1.7.0/python_bmob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-16 07:13:25.000000 python-bmob-1.7.0/python_bmob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 07:13:24.000000 python-bmob-1.7.0/python_bmob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-16 07:13:24.000000 python-bmob-1.7.0/python_bmob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 07:13:24.000000 python-bmob-1.7.0/python_bmob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 07:13:25.359569 python-bmob-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      382 2024-04-16 07:13:11.000000 python-bmob-1.7.0/setup.py
```

### Comparing `python-bmob-1.6.0/bmobpy/bmob.py` & `python-bmob-1.7.0/bmobpy/bmob.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-#coding=utf-8
-
 import json
 import time
 import os
 import mimetypes
-import base64
 import datetime
+from websockets.sync.client import connect
 
 try:
 	from urllib import quote, urlpase
 	import urllib2 as import_urllib
 except ImportError:
 	from urllib.parse import quote,urlparse
 	import urllib.request as import_urllib
@@ -324,37 +322,51 @@
 			near["$maxDistanceInKilometers"] = maxKM
 		if maxRadians != None:
 			near["$maxDistanceInRadians"] = maxRadians
 		return self.putWhereFilter(key, near)
 
 	def addWhereWithinGeoBox(self, key,southwest, northeast):
 		return self.putWhereFilter(key, {"$box": [southwest.__dict__, northeast.__dict__]}, "$within")
+	
 	# 列表
 	def addWhereContainedIn(self, key, value, isIn = True):
 		if isIn:
 			isIn = "$in"
 		else:
 			isIn = "$nin"
 		return self.putWhereFilter(key, value, isIn)
+	
 	def addWhereNotContainedIn(self, key, value):
 		return self.addWhereContainedIn(key, value, False)
+	
 	def addWhereContainsAll(self, key, value):
 		return self.putWhereFilter(key, value, "$all")
-	# 模糊查询
+	
 	def addWhereStrContains(self, key, value):
+		"""模糊查询（正则查询）
+
+		Args:
+			key (str): 列名
+			value (str): 是否存在的字符串
+
+		Returns:
+			self: 自身
+		"""		
 		return self.putWhereFilter(key, value, "$regex")
+	
 	# 子查询
 	def addWhereMatchesSelect(self, key, innerQuery, innerKey, innerTable = None, isMatch = True):
 		if isMatch:
 			isMatch = "$select"
 		else:
 			isMatch = "$dontSelect"
 		if isinstance(innerQuery, BmobQuery):
 			innerQuery = {"className": innerTable, "where": innerQuery.filter}
 		return self.putWhereFilter(key, {"key": innerKey, "query": innerQuery}, isMatch)
+	
 	def addWhereInQuery(self, key, value, className = None, isIn = True):
 		if isIn:
 			isIn = "$inQuery"
 		else:
 			isIn = "$notInQuery"
 		if isinstance(value, BmobQuery):
 			innerQuery = {"className": className, "where": value.filter}
@@ -443,27 +455,106 @@
 	else:
 		errMsg = "Unknown Error"
 		return BmobResult({'error':errMsg,'code':-1})
 
 class Bmob:
     
 	error = {}
+	chatList = {}
+	reply = ''
     
 	def __init__(self, application_id, rest_api_key):
 		"""初始化Bmob
 
 		Args:
 			application_id (string): 进入Bmob控制台，具体应用 -> 设置 -> 应用密钥 -> Application ID
 			rest_api_key (string): 进入Bmob控制台，具体应用 -> 设置 -> 应用密钥 -> REST API Key
 		"""		
 		self.domain = 'https://api.codenow.cn'
 		self.headers = {"X-Bmob-Application-Id": application_id, "X-Bmob-REST-API-Key": rest_api_key, "Content-Type": "application/json"}
 		self.appid = application_id
 		self.restkey = rest_api_key
-  
+
+	def connectAI(self):
+		"""初始化AI服务
+		"""		
+		url = 'wss://api.codenow.cn/1/ai'
+		self.ws = connect(url,additional_headers=self.headers)
+	
+	def closeAI(self):
+		"""关闭AI服务
+		"""		
+		try:
+			self.ws.close()
+		except Exception as e:
+			pass
+
+	def chat(self,chatmsg='你好',session='default'):
+		"""开始对话
+
+		Args:
+			chatmsg (str, optional): 发送的对话内容. Defaults to '你好'.
+			session (str, optional): 会话名称. Defaults to 'default'.
+
+		Returns:
+			str: AI服务器返回的文字
+		"""		
+		# 发送消息到AI服务器
+		if session not in self.chatList:
+			self.chatList[session] = []
+				
+		sessionchatlist = self.chatList[session]
+
+		if len(sessionchatlist) >=1:
+			last = sessionchatlist[-1]
+			if last['role'] =='assistant':
+				sessionchatlist.append({
+					'role':'user',
+					'content':chatmsg
+				})
+		else:
+			sessionchatlist.append({
+				'role':'user',
+				'content':chatmsg
+			})
+
+		if len(sessionchatlist) > 5:
+			realsend = sessionchatlist[-6:]
+		else:
+			realsend = sessionchatlist
+		
+		sendmsg = {
+			'messages':realsend,
+			'session':'python'
+		}
+
+		self.ws.send(json.dumps(sendmsg))
+		self.reply = ''
+
+		while True:
+			try:
+				message = self.ws.recv_messages.get()
+				data = json.loads(message)
+
+				if 'choices' in message:
+					finish = data['choices'][0]['finish_reason']
+					if finish!='':
+						sessionchatlist.append({
+							'role':'assistant',
+							'content':self.reply
+						})
+						return self.reply
+					self.reply += data['choices'][0]['delta']['content']		
+				else:
+					print('ai的数据格式错误')
+					return self.reply
+			except Exception as e:
+				print(e)
+				return self.reply
+
 	def getError(self):
 		"""获取错误信息
 
 		Returns:
 			dict: 错误码和错误信息
 		"""     
 		return self.error
@@ -507,15 +598,16 @@
 		from bmob import *
 		b = Bmob('application_id','rest_api_key')
 		rs = b.signUp('13800138002','123456', userInfo={
 			'sex':True,
 			'age':100
 		})
 		
-		其中，13800138002是注册的账号，123456是登录的密码，userInfo是其他的用户信息，可为空
+		其中，13800138002是注册的账号，123456是登录的密码，userInfo是其他的用户信息，可为空.
+
 		Args:
 			username (string): 账号
 			password (string): 密码
 			userInfo (dict, optional): 用户表的其他字段信息. Defaults to None.
 
 		Returns:
 			object: 注册成功之后的用户记录信息
@@ -526,17 +618,17 @@
 				'username':username,
 				'password':password
 			}
 		else:
 			userInfo['username'] = username
 			userInfo['password'] = password
 
-		return self._signUp(userInfo)
+		return self.__signUp(userInfo)
 
-	def _signUp(self, userInfo):
+	def __signUp(self, userInfo):
 		"""用户注册
 
 		Args:
 			userInfo (dict): 用户的注册数据信息，封装为dict类型
 
 		Returns:
 			object: 注册成功之后的用户记录信息
@@ -863,15 +955,15 @@
 		Args:
 			className (string): 数据表名称
 			where (string or BmboQuery, optional): 查询条件. Defaults to None.
 
 		Returns:
 			int: 记录数。如果发生异常，返回None.
 		"""     
-		return self._basefindObjects(className,where=where,limit=0,count=1)
+		return self.__basefindObjects(className,where=where,limit=0,count=1)
 
 	def sum(self,className, sumName ,where = None):
 		"""查询where条件下，sumName的和
   
 		示例代码：
   
 		from bmob import *
@@ -885,15 +977,15 @@
 			className (string): 数据表名称
 			sumName (string or list): 求和的列，多列求和用list
 			where (string or BmboQuery, optional): 查询条件. Defaults to None.
 
 		Returns:
 			dict or int: 和的结果
 		"""     
-		return self._basefindObjects(className,where=where, sum=sumName)
+		return self.__basefindObjects(className,where=where, sum=sumName)
 
 	def max(self,className, maxName ,where = None):
 		"""查询where条件下，maxName列的最大值
   
 		示例代码：
 		from bmob import *
 		b = Bmob('application_id','rest_api_key')
@@ -906,15 +998,15 @@
 			className (string): 数据表名称
 			maxName (string or list): 求最大值的列，多列求最大值用list
 			where (string or BmboQuery, optional): 查询条件. Defaults to None.
 
 		Returns:
 			dict or int: 最大值
 		"""     
-		return self._basefindObjects(className,where=where, max=maxName)
+		return self.__basefindObjects(className,where=where, max=maxName)
 
 	def min(self,className, minName ,where = None):
 		"""查询where条件下，minName列的最小值
   
 		示例代码：
   
 		from bmob import *
@@ -928,15 +1020,15 @@
 			className (string): 数据表名称
 			minName (string or list): 求最小值的列，多列求最小值用list
 			where (string or BmboQuery, optional): 查询条件. Defaults to None.
 
 		Returns:
 			dict or int: 最小值
 		"""     
-		return self._basefindObjects(className,where=where, min=minName)
+		return self.__basefindObjects(className,where=where, min=minName)
 
 	def mean(self,className, meanName ,where = None):
 		"""查询where条件下，meanName列的平均值
   
 		from bmob import *
 		b = Bmob('application_id','rest_api_key')
 		rs = b.mean('ai_log', ['count','isShow'], where=None)
@@ -948,20 +1040,20 @@
 			className (string): 数据表名称
 			meanName (string or list): 求平均值的列，多列求平均值用list
 			where (string or BmboQuery, optional): 查询条件. Defaults to None.
 
 		Returns:
 			dict or int: 平均值
 		"""     
-		return self._basefindObjects(className,where=where, average=meanName)
+		return self.__basefindObjects(className,where=where, average=meanName)
 
 	def findObjects(self, className, where = None, limit = None, skip = None, order = None, include = None, keys = None,groupby = None, groupcount = None, having = None):
-		return self._basefindObjects(className,where=where,limit=limit,skip=skip,order=order,include=include,keys=keys,groupby=groupby,groupcount=groupcount,having=having)
+		return self.__basefindObjects(className,where=where,limit=limit,skip=skip,order=order,include=include,keys=keys,groupby=groupby,groupcount=groupcount,having=having)
 	
-	def _basefindObjects(self, className, where = None, limit = None, skip = None, order = None, include = None, keys = None, count = None, groupby = None, groupcount = None, min = None, max = None, sum = None, average = None, having = None):
+	def __basefindObjects(self, className, where = None, limit = None, skip = None, order = None, include = None, keys = None, count = None, groupby = None, groupcount = None, min = None, max = None, sum = None, average = None, having = None):
 		"""多条数据的条件查询
 
 		示例代码：
 		from bmob import *
 		b = Bmob('application_id','rest_api_key')
 		rs = b.findObjects('ai_log',limit=10,order='-createdAt')
 		for r in rs:
@@ -1084,22 +1176,22 @@
 
 		示例代码：
 		from bmob import *
 		b = Bmob('application_id','rest_api_key')
 		r = b.getObject("ai_log", "5949973169")
 		print(r.messages)
 
-		其中，ai_log是表名，5949973169是这条记录的objectId，messages是记录的字段名
+		其中，ai_log是表名，5949973169是这条记录的objectId，messages是记录的字段名.
 
 		Args:
-			className (string): 数据表名称
-			objectId (string): 这条记录的objectId
+			className (string): 数据表名称.
+			objectId (string): 这条记录的objectId.
 
 		Returns:
-			object: 数据的查询结果，
+			object: 数据的查询结果.
 		"""	
 		
 		bmobResult =  BmobRequest(url = self.domain + '/1/classes/' + className + '/' + objectId, method = 'GET', headers = self.headers)
 	
 		self.error = bmobResult.getError()
 		if self.error['error'] is None:
 			data = BmobDict(bmobResult.jsonData)
@@ -1142,11 +1234,19 @@
 				print(f'发生异常:{e}')
 				return False
 		else:
 			print('找不到对应的文件')
 			return None
 
 	def delFile(self,url):
+		"""删除文件
+
+		Args:
+			url (str): 要删除的文件的url
+
+		Returns:
+			bool: 是否删除成功.
+		"""		
 		path = urlparse(url).path
-		bmobResult =  BmobRequest(url = self.domain + f'/2/files/upyun/{path}', method = 'DELETE', headers = self.headers)
+		bmobResult =  BmobRequest(url = self.domain + f'/2/files/upyun{path}', method = 'DELETE', headers = self.headers)
 		self.error = bmobResult.getError()
 		return dealBmobResult(bmobResult,'删除文件')
```

