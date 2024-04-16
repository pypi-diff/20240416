# Comparing `tmp/drumpler-2.0.1.tar.gz` & `tmp/drumpler-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler-2.0.1.tar", last modified: Tue Apr 16 18:09:06 2024, max compression
+gzip compressed data, was "drumpler-2.1.0.tar", last modified: Tue Apr 16 20:02:33 2024, max compression
```

## Comparing `drumpler-2.0.1.tar` & `drumpler-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 18:09:06.831872 drumpler-2.0.1/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 18:09:06.830002 drumpler-2.0.1/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-16 18:09:06.000000 drumpler-2.0.1/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      595 2024-04-16 18:09:06.000000 drumpler-2.0.1/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 18:09:06.000000 drumpler-2.0.1/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-16 18:09:06.000000 drumpler-2.0.1/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 18:09:06.000000 drumpler-2.0.1/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.0.1/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-16 18:09:06.830990 drumpler-2.0.1/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.0.1/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 18:09:06.824442 drumpler-2.0.1/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 drumpler-2.0.1/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      786 2024-04-16 18:08:34.000000 drumpler-2.0.1/drumpler/config_drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)      308 2024-04-16 18:08:37.000000 drumpler-2.0.1/drumpler/config_mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)     8214 2024-04-16 18:08:30.000000 drumpler-2.0.1/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)     3147 2024-04-16 18:06:40.000000 drumpler-2.0.1/drumpler/http_request.py
--rw-r--r--   0 Karel      (503) staff       (20)     3456 2024-04-16 18:08:04.000000 drumpler-2.0.1/drumpler/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)       69 2024-04-16 18:06:37.000000 drumpler-2.0.1/drumpler/sql_base.py
--rw-r--r--   0 Karel      (503) staff       (20)      493 2024-04-16 18:06:36.000000 drumpler-2.0.1/drumpler/sql_event.py
--rw-r--r--   0 Karel      (503) staff       (20)      706 2024-04-16 18:06:36.000000 drumpler-2.0.1/drumpler/sql_job.py
--rw-r--r--   0 Karel      (503) staff       (20)      635 2024-04-16 18:06:35.000000 drumpler-2.0.1/drumpler/sql_request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 18:09:06.832025 drumpler-2.0.1/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-16 18:06:30.000000 drumpler-2.0.1/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 18:09:06.828887 drumpler-2.0.1/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.0.1/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:02:33.927339 drumpler-2.1.0/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:02:33.925536 drumpler-2.1.0/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 20:02:33.000000 drumpler-2.1.0/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      514 2024-04-16 20:02:33.000000 drumpler-2.1.0/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 20:02:33.000000 drumpler-2.1.0/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       64 2024-04-16 20:02:33.000000 drumpler-2.1.0/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 20:02:33.000000 drumpler-2.1.0/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.1.0/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 20:02:33.926560 drumpler-2.1.0/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.1.0/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:02:33.919631 drumpler-2.1.0/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-16 18:54:33.000000 drumpler-2.1.0/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.1.0/drumpler/config.py
+-rw-r--r--   0 Karel      (503) staff       (20)     8574 2024-04-16 20:01:16.000000 drumpler-2.1.0/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)       69 2024-04-16 18:54:36.000000 drumpler-2.1.0/drumpler/sql_base.py
+-rw-r--r--   0 Karel      (503) staff       (20)      497 2024-04-16 18:54:38.000000 drumpler-2.1.0/drumpler/sql_event.py
+-rw-r--r--   0 Karel      (503) staff       (20)      710 2024-04-16 18:54:37.000000 drumpler-2.1.0/drumpler/sql_job.py
+-rw-r--r--   0 Karel      (503) staff       (20)      635 2024-04-16 18:54:37.000000 drumpler-2.1.0/drumpler/sql_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 20:02:33.927534 drumpler-2.1.0/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      783 2024-04-16 20:02:15.000000 drumpler-2.1.0/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:02:33.924345 drumpler-2.1.0/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.1.0/test/test_drumpler.py
```

### Comparing `drumpler-2.0.1/Drumpler.egg-info/PKG-INFO` & `drumpler-2.1.0/Drumpler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.0.1
+Version: 2.1.0
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask
 Requires-Dist: python-dotenv
 Requires-Dist: SQLAlchemy
 Requires-Dist: Flask_SQLAlchemy
-Requires-Dist: requests
-Requires-Dist: schedule
 Requires-Dist: psycopg2-binary
 
 
 # `Drumpler`
 
 `Drumpler` is a general-purpose application designed to facilitate efficient workflow automation through RESTful API interactions and job processing. Built on Flask and SQLAlchemy, this application serves as a robust backend for capturing, storing, and processing HTTP requests in a scalable manner. The application is split into two main components: `drumpler.py` for handling RESTful API requests and `mammoth.py` for querying the API and processing jobs asynchronously.
```

### Comparing `drumpler-2.0.1/Drumpler.egg-info/SOURCES.txt` & `drumpler-2.1.0/Drumpler.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,16 @@
 setup.py
 Drumpler.egg-info/PKG-INFO
 Drumpler.egg-info/SOURCES.txt
 Drumpler.egg-info/dependency_links.txt
 Drumpler.egg-info/requires.txt
 Drumpler.egg-info/top_level.txt
 drumpler/__init__.py
-drumpler/config_drumpler.py
-drumpler/config_mammoth.py
+drumpler/config.py
 drumpler/drumpler.py
-drumpler/http_request.py
-drumpler/mammoth.py
 drumpler/sql_base.py
 drumpler/sql_event.py
 drumpler/sql_job.py
 drumpler/sql_request.py
 drumpler.egg-info/PKG-INFO
 drumpler.egg-info/SOURCES.txt
 drumpler.egg-info/dependency_links.txt
```

### Comparing `drumpler-2.0.1/LICENSE` & `drumpler-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler-2.0.1/PKG-INFO` & `drumpler-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.0.1
+Version: 2.1.0
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask
 Requires-Dist: python-dotenv
 Requires-Dist: SQLAlchemy
 Requires-Dist: Flask_SQLAlchemy
-Requires-Dist: requests
-Requires-Dist: schedule
 Requires-Dist: psycopg2-binary
 
 
 # `Drumpler`
 
 `Drumpler` is a general-purpose application designed to facilitate efficient workflow automation through RESTful API interactions and job processing. Built on Flask and SQLAlchemy, this application serves as a robust backend for capturing, storing, and processing HTTP requests in a scalable manner. The application is split into two main components: `drumpler.py` for handling RESTful API requests and `mammoth.py` for querying the API and processing jobs asynchronously.
```

### Comparing `drumpler-2.0.1/README.md` & `drumpler-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `drumpler-2.0.1/drumpler/config_drumpler.py` & `drumpler-2.1.0/drumpler/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Drumpler/config.py
 import os
 from dotenv import load_dotenv
 
 load_dotenv('/home/sammy/drumpler/.env')  # Use an appropriate path
 
-class ConfigDrumpler:
+class Config:
     AUTHORIZATION_KEY = os.getenv('AUTHORIZATION_KEY')
     DRUMPLER_HOST = os.getenv('DRUMPLER_HOST', "http://127.0.0.1")
     DRUMPLER_PORT = int(os.getenv('DRUMPLER_PORT', "5000"))
     DRUMPLER_DEBUG = bool(os.getenv('DRUMPLER_DEBUG', "True"))
     DATABASE_URI = os.getenv('DATABASE_URI')  # Ensure this is set in your .env for Drumpler
 
     @staticmethod
     def drumpler_url():
-        if ConfigDrumpler.DRUMPLER_HOST.startswith("https") or ConfigDrumpler.DRUMPLER_PORT == 443:
-            return f"{ConfigDrumpler.DRUMPLER_HOST}"
+        if Config.DRUMPLER_HOST.startswith("https") or Config.DRUMPLER_PORT == 443:
+            return f"{Config.DRUMPLER_HOST}"
         else:
-            return f"{ConfigDrumpler.DRUMPLER_HOST}:{ConfigDrumpler.DRUMPLER_PORT}"
+            return f"{Config.DRUMPLER_HOST}:{Config.DRUMPLER_PORT}"
```

### Comparing `drumpler-2.0.1/drumpler/drumpler.py` & `drumpler-2.1.0/drumpler/drumpler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,50 @@
+# drumpler.py
 import os
+import json
 import sys
 from flask import Flask, request, jsonify
-from .config_drumpler import ConfigDrumpler
-import json
 from flask_sqlalchemy import SQLAlchemy
-from .sql_base import Base
+from .config import Config
+from .sql_base import Base  # Import the Base declarative class directly
 from .sql_request import SqlRequest
 from .sql_job import SqlJob
 from .sql_event import SqlEvent
 
 app = Flask(__name__)
 db = SQLAlchemy()
-Base.metadata.bind = db.engine
 
 class Drumpler:
     def __init__(self):
+        self.app = app  # Use the global app instance
         self.__init_env()
-        self.app = Flask(__name__)
-        self.AUTHORIZATION_KEY = ConfigDrumpler.AUTHORIZATION_KEY
+        self.__init_config()
+        self.__init_db()
+        self.__setup_routes()
 
-        # Fetching environment variables or using defaults
-        self.host = os.environ.get("DRUMPLER_HOST", ConfigDrumpler.DRUMPLER_HOST)
-        self.port = os.environ.get("DRUMPLER_PORT", ConfigDrumpler.DRUMPLER_PORT)
-        self.debug = os.environ.get("DRUMPLER_DEBUG", ConfigDrumpler.DRUMPLER_DEBUG)
-        
-        self.app.config['SQLALCHEMY_DATABASE_URI'] = ConfigDrumpler.DATABASE_URI
+    def __init_config(self):
+        self.app.config['SQLALCHEMY_DATABASE_URI'] = Config.DATABASE_URI
         self.app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
+        self.AUTHORIZATION_KEY = Config.AUTHORIZATION_KEY
+        self.host = Config.DRUMPLER_HOST
+        self.port = Config.DRUMPLER_PORT
+        self.debug = Config.DRUMPLER_DEBUG
 
-        # Initialize SQLAlchemy with the Flask app here instead of global scope
-        db.init_app(self.app)
-
+    def __init_db(self):
+        db.init_app(self.app)  # Initialize SQLAlchemy with app
         with self.app.app_context():
-            Base.metadata.create_all(db.engine)  # Ensure this is Base.metadata.create_all
-            
-        self.__setup_routes()
+            Base.metadata.create_all(db.engine)  # Create tables from the same Base used in model definitions
 
     def __setup_routes(self):
         self.app.add_url_rule('/', view_func=self.hello_world, methods=['GET'])
         self.app.add_url_rule('/request', view_func=self.__process_request, methods=['POST'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__get_request, methods=['GET'])
         self.app.add_url_rule('/request/next-unhandled', view_func=self.__get_next_unhandled_request, methods=['GET'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__update_request, methods=['PUT'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__delete_request, methods=['DELETE'])
-        self.app.add_url_rule('/jobs', view_func=self.__create_job, methods=['POST'])
         self.app.add_url_rule('/jobs/<int:job_id>', view_func=self.__update_job, methods=['PUT'])
         self.app.add_url_rule('/events', view_func=self.__create_event, methods=['POST'])
 
     def __init_env(self):
         if not os.path.exists(".env"):
             sys.exit("ERROR! You must create a .env file that contains a single line 'AUTHORIZATION_KEY=YourAuthorizationKeyHere'")
 
@@ -69,17 +67,29 @@
             user_agent=request.user_agent.string,
             method=request.method,
             request_url=request.url,
             request_raw=json.dumps(data),
             custom_value=custom_value
         )
         db.session.add(new_request)
-        db.session.commit()
-        return jsonify({"message": "Request processed successfully", "id": new_request.id}), 200
-    
+        db.session.flush()  # Flush here to assign an ID to new_request without committing the transaction
+
+        if custom_value:
+            # do more stuff
+            new_job = SqlJob(
+                request_id=new_request.id,  # Now new_request.id should be available
+                status='Pending'
+            )
+            db.session.add(new_job)
+            db.session.commit()
+            return jsonify({"message": "Request processed successfully", "id": new_request.id, "job_id": new_job.id}), 200
+        else:
+            db.session.commit()
+            return jsonify({"message": "Request processed successfully", "id": new_request.id}), 200
+
     def __get_next_unhandled_request(self):
         with db.session.begin():
             query = db.session.query(SqlRequest)\
                 .filter(SqlRequest.is_handled == 0, 
                         SqlRequest.is_being_processed == False)
             custom_value = request.args.get('custom_value', None)
             if custom_value is not None:
@@ -175,11 +185,12 @@
         new_event = SqlEvent(job_id=data['job_id'], message=data['message'])
         db.session.add(new_event)
         db.session.commit()
         return jsonify({'event_id': new_event.id}), 201
 
     def run(self):
         app.run(host=self.host, port=self.port, debug=self.debug)
+        #self.app.run()
 
 if __name__ == '__main__':
     drumpler = Drumpler()
     drumpler.run()
```

### Comparing `drumpler-2.0.1/drumpler/sql_job.py` & `drumpler-2.1.0/drumpler/sql_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
     __tablename__ = 'jobs'
     id = Column(Integer, primary_key=True)
     request_id = Column(Integer, nullable=False)
     created_date = Column(DateTime(timezone=True), default=lambda: datetime.now(timezone.utc))
     modified_date = Column(DateTime(timezone=True), default=lambda: datetime.now(timezone.utc), onupdate=lambda: datetime.now(timezone.utc))
     finished_date = Column(DateTime(timezone=True))
     status = Column(String)
-    events = relationship("Event", backref="job")
+    events = relationship("SqlEvent", backref="job")
```

### Comparing `drumpler-2.0.1/drumpler/sql_request.py` & `drumpler-2.1.0/drumpler/sql_request.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.0.1/setup.py` & `drumpler-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='2.0.1',
+    version='2.1.0',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
@@ -17,12 +17,10 @@
     ],
     python_requires='>=3.6',
     install_requires=[
         'Flask',
         'python-dotenv',
         'SQLAlchemy',
         'Flask_SQLAlchemy',
-        'requests',
-        'schedule',
         'psycopg2-binary',
     ],
 )
```

### Comparing `drumpler-2.0.1/test/test_drumpler.py` & `drumpler-2.1.0/test/test_drumpler.py`

 * *Files identical despite different names*

