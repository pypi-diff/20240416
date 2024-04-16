# Comparing `tmp/Drumpler-1.2.2.tar.gz` & `tmp/drumpler-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Drumpler-1.2.2.tar", last modified: Wed Apr 10 18:13:22 2024, max compression
+gzip compressed data, was "drumpler-2.0.1.tar", last modified: Tue Apr 16 18:09:06 2024, max compression
```

## Comparing `Drumpler-1.2.2.tar` & `drumpler-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-10 18:13:22.413919 Drumpler-1.2.2/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-10 18:13:22.412222 Drumpler-1.2.2/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-10 18:13:22.000000 Drumpler-1.2.2/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-10 18:13:22.000000 Drumpler-1.2.2/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-10 18:13:22.000000 Drumpler-1.2.2/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-10 18:13:22.000000 Drumpler-1.2.2/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-10 18:13:22.000000 Drumpler-1.2.2/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.2.2/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-10 18:13:22.413082 Drumpler-1.2.2/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 Drumpler-1.2.2/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-10 18:13:22.406667 Drumpler-1.2.2/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.2.2/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      804 2024-04-10 16:47:26.000000 Drumpler-1.2.2/drumpler/constants.py
--rw-r--r--   0 Karel      (503) staff       (20)     7632 2024-04-10 18:12:02.000000 Drumpler-1.2.2/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)     7906 2024-04-10 18:10:48.000000 Drumpler-1.2.2/drumpler/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)     3143 2024-04-09 21:57:52.000000 Drumpler-1.2.2/drumpler/request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-10 18:13:22.414076 Drumpler-1.2.2/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-10 18:13:07.000000 Drumpler-1.2.2/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-10 18:13:22.411029 Drumpler-1.2.2/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.2.2/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 18:09:06.831872 drumpler-2.0.1/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 18:09:06.830002 drumpler-2.0.1/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-16 18:09:06.000000 drumpler-2.0.1/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      595 2024-04-16 18:09:06.000000 drumpler-2.0.1/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 18:09:06.000000 drumpler-2.0.1/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-16 18:09:06.000000 drumpler-2.0.1/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 18:09:06.000000 drumpler-2.0.1/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.0.1/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-16 18:09:06.830990 drumpler-2.0.1/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.0.1/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 18:09:06.824442 drumpler-2.0.1/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 drumpler-2.0.1/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      786 2024-04-16 18:08:34.000000 drumpler-2.0.1/drumpler/config_drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)      308 2024-04-16 18:08:37.000000 drumpler-2.0.1/drumpler/config_mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)     8214 2024-04-16 18:08:30.000000 drumpler-2.0.1/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3147 2024-04-16 18:06:40.000000 drumpler-2.0.1/drumpler/http_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3456 2024-04-16 18:08:04.000000 drumpler-2.0.1/drumpler/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)       69 2024-04-16 18:06:37.000000 drumpler-2.0.1/drumpler/sql_base.py
+-rw-r--r--   0 Karel      (503) staff       (20)      493 2024-04-16 18:06:36.000000 drumpler-2.0.1/drumpler/sql_event.py
+-rw-r--r--   0 Karel      (503) staff       (20)      706 2024-04-16 18:06:36.000000 drumpler-2.0.1/drumpler/sql_job.py
+-rw-r--r--   0 Karel      (503) staff       (20)      635 2024-04-16 18:06:35.000000 drumpler-2.0.1/drumpler/sql_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 18:09:06.832025 drumpler-2.0.1/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-16 18:06:30.000000 drumpler-2.0.1/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 18:09:06.828887 drumpler-2.0.1/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.0.1/test/test_drumpler.py
```

### Comparing `Drumpler-1.2.2/Drumpler.egg-info/PKG-INFO` & `drumpler-2.0.1/Drumpler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.2.2
+Version: 2.0.1
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.2.2/LICENSE` & `drumpler-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Drumpler-1.2.2/PKG-INFO` & `drumpler-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.2.2
+Version: 2.0.1
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.2.2/README.md` & `drumpler-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Drumpler-1.2.2/drumpler/drumpler.py` & `drumpler-2.0.1/drumpler/drumpler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,54 @@
 import os
 import sys
 from flask import Flask, request, jsonify
-from .constants import DRUMPLER_HOST, DRUMPLER_PORT, DRUMPLER_DEBUG, DATABASE_URI, AUTHORIZATION_KEY
+from .config_drumpler import ConfigDrumpler
 import json
 from flask_sqlalchemy import SQLAlchemy
-from .request import Request as BaseRequest
+from .sql_base import Base
+from .sql_request import SqlRequest
+from .sql_job import SqlJob
+from .sql_event import SqlEvent
 
 app = Flask(__name__)
-app.config['SQLALCHEMY_DATABASE_URI'] = DATABASE_URI
-app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
-db = SQLAlchemy(app)
-
-class Request(db.Model, BaseRequest):
-    id = db.Column(db.Integer, primary_key=True)
-    timestamp = db.Column(db.DateTime, default=db.func.current_timestamp())
-    source_ip = db.Column(db.String(128))
-    user_agent = db.Column(db.String(256))
-    method = db.Column(db.String(8))
-    request_url = db.Column(db.String(256))
-    request_raw = db.Column(db.Text)
-    custom_value = db.Column(db.String(256))
-    is_handled = db.Column(db.Integer, default=0)
-    is_being_processed = db.Column(db.Boolean, default=False)
+db = SQLAlchemy()
+Base.metadata.bind = db.engine
 
 class Drumpler:
     def __init__(self):
         self.__init_env()
         self.app = Flask(__name__)
-        self.DATABASE = 'requests.db'
-        self.AUTHORIZATION_KEY = AUTHORIZATION_KEY
+        self.AUTHORIZATION_KEY = ConfigDrumpler.AUTHORIZATION_KEY
 
         # Fetching environment variables or using defaults
-        self.host = os.environ.get("DRUMPLER_HOST", DRUMPLER_HOST)
-        self.port = os.environ.get("DRUMPLER_PORT", DRUMPLER_PORT)
-        self.debug = os.environ.get("DRUMPLER_DEBUG",DRUMPLER_DEBUG)
+        self.host = os.environ.get("DRUMPLER_HOST", ConfigDrumpler.DRUMPLER_HOST)
+        self.port = os.environ.get("DRUMPLER_PORT", ConfigDrumpler.DRUMPLER_PORT)
+        self.debug = os.environ.get("DRUMPLER_DEBUG", ConfigDrumpler.DRUMPLER_DEBUG)
         
-        self.app.config['SQLALCHEMY_DATABASE_URI'] = DATABASE_URI
+        self.app.config['SQLALCHEMY_DATABASE_URI'] = ConfigDrumpler.DATABASE_URI
         self.app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 
         # Initialize SQLAlchemy with the Flask app here instead of global scope
         db.init_app(self.app)
 
         with self.app.app_context():
-            db.create_all()  # Move database initialization here
-        
+            Base.metadata.create_all(db.engine)  # Ensure this is Base.metadata.create_all
+            
         self.__setup_routes()
 
     def __setup_routes(self):
         self.app.add_url_rule('/', view_func=self.hello_world, methods=['GET'])
         self.app.add_url_rule('/request', view_func=self.__process_request, methods=['POST'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__get_request, methods=['GET'])
         self.app.add_url_rule('/request/next-unhandled', view_func=self.__get_next_unhandled_request, methods=['GET'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__update_request, methods=['PUT'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__delete_request, methods=['DELETE'])
+        self.app.add_url_rule('/jobs', view_func=self.__create_job, methods=['POST'])
+        self.app.add_url_rule('/jobs/<int:job_id>', view_func=self.__update_job, methods=['PUT'])
+        self.app.add_url_rule('/events', view_func=self.__create_event, methods=['POST'])
 
     def __init_env(self):
         if not os.path.exists(".env"):
             sys.exit("ERROR! You must create a .env file that contains a single line 'AUTHORIZATION_KEY=YourAuthorizationKeyHere'")
 
     def __authorize_request(self):
         authorization = request.headers.get('Authorization')
@@ -68,71 +60,58 @@
     def __process_request(self):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
 
         data = request.get_json() or {}  # Fallback to an empty dict if no JSON is provided
         custom_value = request.args.get('custom_value', None)
 
-        new_request = Request(
+        new_request = SqlRequest(
             source_ip=request.remote_addr,
             user_agent=request.user_agent.string,
             method=request.method,
             request_url=request.url,
             request_raw=json.dumps(data),
             custom_value=custom_value
         )
         db.session.add(new_request)
         db.session.commit()
         return jsonify({"message": "Request processed successfully", "id": new_request.id}), 200
     
     def __get_next_unhandled_request(self):
         with db.session.begin():
-            # Start with a base query
-            query = db.session.query(Request)\
-                .filter(Request.is_handled == 0, 
-                        Request.is_being_processed == False)
-
-            # Conditionally add the custom_value filter if it is provided
+            query = db.session.query(SqlRequest)\
+                .filter(SqlRequest.is_handled == 0, 
+                        SqlRequest.is_being_processed == False)
             custom_value = request.args.get('custom_value', None)
             if custom_value is not None:
-                query = query.filter(Request.custom_value == custom_value)
-
-            # Execute the query with ordering and locking
-            unhandled_request = query.order_by(Request.id)\
+                query = query.filter(SqlRequest.custom_value == custom_value)
+            unhandled_request = query.order_by(SqlRequest.id)\
                 .with_for_update(skip_locked=True).first()
-
             if unhandled_request:
-                # Prepare data before committing the transaction
+                unhandled_request.is_being_processed = True
                 request_data = {
                     "id": unhandled_request.id,
                     "timestamp": unhandled_request.timestamp.isoformat(),
                     "source_ip": unhandled_request.source_ip,
                     "user_agent": unhandled_request.user_agent,
                     "method": unhandled_request.method,
                     "request_url": unhandled_request.request_url,
                     "request_raw": unhandled_request.request_raw,
-                    "custom_value": unhandled_request.custom_value,  # Include the custom field in the response
+                    "custom_value": unhandled_request.custom_value,
                     "is_handled": unhandled_request.is_handled
                 }
-
-                # Mark the request as being processed
-                unhandled_request.is_being_processed = True
-                # Commit is done by the context manager upon exit
-
-        # Return outside the context manager to avoid accessing the session
         if unhandled_request:
             return jsonify(request_data), 200
         else:
             return jsonify({"message": "No unhandled requests found."}), 404
 
     def __get_request(self, request_id):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
-
-        request_entry = Request.query.get(request_id)
+        request_entry = SqlRequest.query.get(request_id)
         if request_entry:
             return jsonify({
                 "id": request_entry.id,
                 "timestamp": request_entry.timestamp.isoformat(),
                 "source_ip": request_entry.source_ip,
                 "user_agent": request_entry.user_agent,
                 "method": request_entry.method,
@@ -143,36 +122,64 @@
             }), 200
         else:
             return jsonify({"message": "Request not found"}), 404
 
     def __update_request(self, request_id):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
-
-        data = request.get_json()
-        request_entry = Request.query.get(request_id)
+        request_entry = SqlRequest.query.get(request_id)
         if request_entry:
-            if 'is_handled' in data:
-                request_entry.is_handled = data['is_handled']
+            data = request.get_json()
+            request_entry.is_handled = data.get('is_handled', request_entry.is_handled)
             db.session.commit()
             return jsonify({"message": "Request updated successfully"}), 200
         else:
             return jsonify({"message": "Request not found"}), 404
 
     def __delete_request(self, request_id):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
-
-        request_entry = Request.query.get(request_id)
+        request_entry = SqlRequest.query.get(request_id)
         if request_entry:
             db.session.delete(request_entry)
             db.session.commit()
             return jsonify({"message": "Request deleted successfully"}), 200
         else:
             return jsonify({"message": "Request not found"}), 404
 
+    def __create_job(self):
+        if not self.__authorize_request():
+            return jsonify({"message": "Unauthorized access"}), 401
+        data = request.get_json()
+        new_job = SqlJob(request_id=data['request_id'], status='Pending')
+        db.session.add(new_job)
+        db.session.commit()
+        return jsonify({'job_id': new_job.id}), 201
+
+    def __update_job(self, job_id):
+        if not self.__authorize_request():
+            return jsonify({"message": "Unauthorized access"}), 401
+        data = request.get_json()
+        job = SqlJob.query.get(job_id)
+        if job:
+            job.status = data.get('status', job.status)
+            job.finished_date = data.get('finished_date', job.finished_date)
+            db.session.commit()
+            return jsonify({"message": "Job updated successfully"}), 200
+        else:
+            return jsonify({"message": "Job not found"}), 404
+
+    def __create_event(self):
+        if not self.__authorize_request():
+            return jsonify({"message": "Unauthorized access"}), 401
+        data = request.get_json()
+        new_event = SqlEvent(job_id=data['job_id'], message=data['message'])
+        db.session.add(new_event)
+        db.session.commit()
+        return jsonify({'event_id': new_event.id}), 201
+
     def run(self):
         app.run(host=self.host, port=self.port, debug=self.debug)
 
 if __name__ == '__main__':
     drumpler = Drumpler()
-    drumpler.run()
+    drumpler.run()
```

### Comparing `Drumpler-1.2.2/drumpler/request.py` & `drumpler-2.0.1/drumpler/http_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import json
 from .constants import DRUMPLER_URL, AUTHORIZATION_KEY
 
-class Request:
+class HttpRequest:
     def __init__(self, id, timestamp, source_ip, user_agent, method, request_url, request_raw, custom_value, is_handled):
         self._id = id
         self._timestamp = timestamp
         self._source_ip = source_ip
         self._user_agent = user_agent
         self._method = method
         self._request_url = request_url
```

### Comparing `Drumpler-1.2.2/setup.py` & `drumpler-2.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='1.2.2',
+    version='2.0.1',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `Drumpler-1.2.2/test/test_drumpler.py` & `drumpler-2.0.1/test/test_drumpler.py`

 * *Files identical despite different names*

