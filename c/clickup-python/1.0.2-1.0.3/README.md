# Comparing `tmp/clickup_python-1.0.2.tar.gz` & `tmp/clickup_python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickup_python-1.0.2.tar", max compression
+gzip compressed data, was "clickup_python-1.0.3.tar", max compression
```

## Comparing `clickup_python-1.0.2.tar` & `clickup_python-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-03-28 14:02:04.026035 clickup_python-1.0.2/LICENSE
--rw-r--r--   0        0        0      823 2023-03-28 14:02:04.026247 clickup_python-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-03-28 14:02:04.026337 clickup_python-1.0.2/clickup/__init__.py
--rw-r--r--   0        0        0    21849 2023-03-28 14:02:04.026469 clickup_python-1.0.2/clickup/client.py
--rw-r--r--   0        0        0     1072 2023-03-28 14:02:04.026563 clickup_python-1.0.2/clickup/exceptions.py
--rw-r--r--   0        0        0      493 2023-03-28 14:02:04.026648 clickup_python-1.0.2/clickup/response.py
--rw-r--r--   0        0        0      394 2023-03-28 14:03:08.726230 clickup_python-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 clickup_python-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-16 15:23:39.842721 clickup_python-1.0.3/clickup/__init__.py
+-rw-r--r--   0        0        0    25105 2024-04-16 15:23:39.842721 clickup_python-1.0.3/clickup/client.py
+-rw-r--r--   0        0        0     1165 2024-04-16 15:23:39.842721 clickup_python-1.0.3/clickup/exceptions.py
+-rw-r--r--   0        0        0      511 2024-04-16 15:23:39.843727 clickup_python-1.0.3/clickup/response.py
+-rw-r--r--   0        0        0     1086 2024-04-16 15:23:39.841718 clickup_python-1.0.3/LICENSE
+-rw-r--r--   0        0        0      403 2024-04-16 15:23:39.843727 clickup_python-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      845 2024-04-16 15:23:39.841718 clickup_python-1.0.3/README.md
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 clickup_python-1.0.3/PKG-INFO
```

### Comparing `clickup_python-1.0.2/LICENSE` & `clickup_python-1.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 GearPlug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 GearPlug
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `clickup_python-1.0.2/README.md` & `clickup_python-1.0.3/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# clickup-python
-ClickUp API wrapper written in python
-
-## Installing
-```
-pip install git+https://github.com/GearPlug/clickup-python.git
-```
-
-## Requirements
-- requests
-
-## Contributing
-We are always grateful for any kind of contribution including but not limited to bug reports, code enhancements, bug fixes, and even functionality suggestions.
-
-#### You can report any bug you find or suggest new functionality with a new [issue](https://github.com/GearPlug/clickup-python/issues).
-
-#### If you want to add yourself some functionality to the wrapper:
-1. Fork it ( https://github.com/GearPlug/clickup-python )
-2. Create your feature branch (git checkout -b my-new-feature)
-3. Commit your changes (git commit -am 'Adds my new feature')   
-4. Push to the branch (git push origin my-new-feature)
-5. Create a new Pull Request
+# clickup-python
+ClickUp API wrapper written in python
+
+## Installing
+```
+pip install git+https://github.com/GearPlug/clickup-python.git
+```
+
+## Requirements
+- requests
+
+## Contributing
+We are always grateful for any kind of contribution including but not limited to bug reports, code enhancements, bug fixes, and even functionality suggestions.
+
+#### You can report any bug you find or suggest new functionality with a new [issue](https://github.com/GearPlug/clickup-python/issues).
+
+#### If you want to add yourself some functionality to the wrapper:
+1. Fork it ( https://github.com/GearPlug/clickup-python )
+2. Create your feature branch (git checkout -b my-new-feature)
+3. Commit your changes (git commit -am 'Adds my new feature')   
+4. Push to the branch (git push origin my-new-feature)
+5. Create a new Pull Request
```

### Comparing `clickup_python-1.0.2/clickup/client.py` & `clickup_python-1.0.3/clickup/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,678 +1,756 @@
-import json
-from clickup import exceptions
-from clickup.response import Response
-from urllib.parse import urlencode
-
-import requests
-
-
-class Client(object):
-    BASE_URL = "https://api.clickup.com/api/"
-    AUTH_URL = "https://app.clickup.com/api"
-    VERSION = "v2"
-
-    WORKSPACE = BASE_URL + VERSION + "/team"
-    SPACE = BASE_URL + VERSION + "/team/{team_id}/space"
-    FOLDER = BASE_URL + VERSION + "/space/{space_id}/folder"
-    LIST = BASE_URL + VERSION + "/folder/{folder_id}/list"
-    TASKS = BASE_URL + VERSION + "/list/{list_id}/task"
-    TASK = BASE_URL + VERSION + "/task/{task_id}"
-    WEBHOOK = BASE_URL + VERSION + "/team/{team_id}/webhook"
-    DEL_WEBHOOK = BASE_URL + VERSION + "/webhook/{webhook_id}"
-    REQUEST_TOKEN = BASE_URL + VERSION + "/oauth/token"
-
-    EVENTS = [
-        "taskCreated",
-        "taskUpdated",
-        "taskDeleted",
-        "taskPriorityUpdated",
-        "taskStatusUpdated",
-        "taskAssigneeUpdated",
-        "taskDueDateUpdated",
-        "taskTagUpdated",
-        "taskMoved",
-        "taskCommentPosted",
-        "taskCommentUpdated",
-        "taskTimeEstimateUpdated",
-        "taskTimeTrackedUpdated",
-        "listCreated",
-        "listUpdated",
-        "listDeleted",
-        "folderCreated",
-        "folderUpdated",
-        "folderDeleted",
-        "spaceCreated",
-        "spaceUpdated",
-        "spaceDeleted",
-        "goalCreated",
-        "goalUpdated",
-        "goalDeleted",
-        "keyResultCreated",
-        "keyResultUpdated",
-        "keyResultDeleted",
-    ]
-
-    def __init__(self, client_id: str, client_secret: str) -> None:
-        self.token = None
-        self.client_id = client_id
-        self.client_secret = client_secret
-
-    def authorization_url(self, redirect_uri: str) -> str:
-        params = {"client_id": self.client_id, "client_secret": self.client_secret, "redirect_uri": redirect_uri}
-        url = self.AUTH_URL + "?" + urlencode(params)
-        return url
-
-    def exchange_code(self, code: str) -> Response:
-        """_summary_
-        example:
-        {
-            "access_token": "42901062_76970dae7a8efa65bf8b9ddea7106aefb5a81008"
-        }
-        Args:
-            code (str): _description_
-
-        Returns:
-            Response: _description_
-        """
-        data = json.dumps({"client_id": self.client_id, "client_secret": self.client_secret, "code": code})
-        response = self._post(self.REQUEST_TOKEN, data=data)
-        # response = self._parse(requests.request(method, url, headers=_headers, **kwargs))
-        return response
-
-    def set_token(self, token: dict) -> None:
-        """Sets the User token for its use in this library.
-        Args:
-            token (dict): User token data.
-        """
-        self.token = token
-
-    def get_workspace(self) -> dict:
-        """Return Team ID
-        {
-            "teams":[
-                {
-                    "id":"31016756",
-                    "name":"Gearplug Test",
-                    "color":"#ff4081",
-                    "avatar":"None",
-                    "members":[
-                        {
-                        "user":{
-                            "id":42901062,
-                            "username":"Johann Sebastián",
-                            "email":"jcardenas@gearplug.io",
-                            "color":"#81b1ff",
-                            "profilePicture":"None",
-                            "initials":"JS",
-                            "role":1,
-                            "custom_role":"None",
-                            "last_active":"1646340664585",
-                            "date_joined":"1646059972931",
-                            "date_invited":"1646059972931"
-                        }
-                        }
-                    ]
-                }
-            ]
-            }
-        Returns:
-            dict: _description_
-        """
-        response = self._get(self.WORKSPACE)
-        return response
-
-    def get_spaces(self, team_id: str) -> dict:
-        """Return the spaces list
-        {
-        "spaces":[
-            {
-                "id":"49179567",
-                "name":"Gearplug Test Space 2",
-                "private":false,
-                "statuses":[
-                    {
-                    "id":"p49179567_MCAIkheF",
-                    "status":"to do",
-                    "type":"open",
-                    "orderindex":0,
-                    "color":"#d3d3d3"
-                    },
-                    {
-                    "id":"p49179567_Z1xfhaQK",
-                    "status":"progress",
-                    "type":"custom",
-                    "orderindex":1,
-                    "color":"#3397dd"
-                    },
-                    {
-                    "id":"p49179567_saAGakZL",
-                    "status":"complete",
-                    "type":"closed",
-                    "orderindex":2,
-                    "color":"#6bc950"
-                    }
-                ],
-                "multiple_assignees":true,
-                "features":{
-                    "due_dates":{
-                    "enabled":true,
-                    "start_date":true,
-                    "remap_due_dates":false,
-                    "remap_closed_due_date":false
-                    },
-                    "sprints":{
-                    "enabled":false
-                    },
-                    "time_tracking":{
-                    "enabled":true,
-                    "harvest":false,
-                    "rollup":false
-                    },
-                    "points":{
-                    "enabled":false
-                    },
-                    "custom_items":{
-                    "enabled":false
-                    },
-                    "priorities":{
-                    "enabled":true,
-                    "priorities":[
-                        {
-                            "id":"1",
-                            "priority":"urgent",
-                            "color":"#f50000",
-                            "orderindex":"1"
-                        },
-                        {
-                            "id":"2",
-                            "priority":"high",
-                            "color":"#ffcc00",
-                            "orderindex":"2"
-                        },
-                        {
-                            "id":"3",
-                            "priority":"normal",
-                            "color":"#6fddff",
-                            "orderindex":"3"
-                        },
-                        {
-                            "id":"4",
-                            "priority":"low",
-                            "color":"#d8d8d8",
-                            "orderindex":"4"
-                        }
-                    ]
-                    },
-                    "tags":{
-                    "enabled":true
-                    },
-                    "check_unresolved":{
-                    "enabled":true,
-                    "subtasks":"None",
-                    "checklists":"None",
-                    "comments":"None"
-                    },
-                    "zoom":{
-                    "enabled":false
-                    },
-                    "milestones":{
-                    "enabled":false
-                    },
-                    "custom_fields":{
-                    "enabled":true
-                    },
-                    "dependency_warning":{
-                    "enabled":true
-                    },
-                    "multiple_assignees":{
-                    "enabled":true
-                    }
-                },
-                "archived":false
-            }
-        ]
-        }
-        Args:
-            team_id (_type_): _description_
-
-        Returns:
-            dict: spaces
-        """
-
-        response = self._get(self.SPACE.format(team_id=team_id))
-        return response
-
-    def get_folder(self, space_id: str) -> dict:
-        """Return the folders list
-        {
-        "folders":[
-            {
-                "id":"103039546",
-                "name":"folder 1",
-                "orderindex":1,
-                "override_statuses":false,
-                "hidden":false,
-                "space":{
-                    "id":"49179567",
-                    "name":"Gearplug Test Space 2"
-                },
-                "task_count":"1",
-                "archived":false,
-                "statuses":[
-
-                ],
-                "lists":[
-                    {
-                    "id":"175125718",
-                    "name":"List",
-                    "orderindex":0,
-                    "status":"None",
-                    "priority":"None",
-                    "assignee":"None",
-                    "task_count":1,
-                    "due_date":"None",
-                    "start_date":"None",
-                    "space":{
-                        "id":"49179567",
-                        "name":"Gearplug Test Space 2",
-                        "access":true
-                    },
-                    "archived":false,
-                    "override_statuses":"None",
-                    "statuses":[
-                        {
-                            "id":"p49179567_MCAIkheF",
-                            "status":"to do",
-                            "orderindex":0,
-                            "color":"#d3d3d3",
-                            "type":"open"
-                        },
-                        {
-                            "id":"p49179567_Z1xfhaQK",
-                            "status":"progress",
-                            "orderindex":1,
-                            "color":"#3397dd",
-                            "type":"custom"
-                        },
-                        {
-                            "id":"p49179567_saAGakZL",
-                            "status":"complete",
-                            "orderindex":2,
-                            "color":"#6bc950",
-                            "type":"closed"
-                        }
-                    ],
-                    "permission_level":"create"
-                    }
-                ],
-                "permission_level":"create"
-                }
-            ]
-        }
-        Args:
-            space_id (_type_): _description_
-
-        Returns:
-            dict: folders
-        """
-
-        response = self._get(self.FOLDER.format(space_id=space_id))
-        return response
-
-    def get_list(self, folder_id: str) -> dict:
-        """Return lists of list
-        {
-        "lists":[
-            {
-                "id":"175125718",
-                "name":"List",
-                "orderindex":0,
-                "status":"None",
-                "priority":"None",
-                "assignee":"None",
-                "task_count":1,
-                "due_date":"None",
-                "start_date":"None",
-                "folder":{
-                    "id":"103039546",
-                    "name":"folder 1",
-                    "hidden":false,
-                    "access":true
-                },
-                "space":{
-                    "id":"49179567",
-                    "name":"Gearplug Test Space 2",
-                    "access":true
-                },
-                "archived":false,
-                "override_statuses":"None",
-                "permission_level":"create"
-            }
-        ]
-        }
-        Args:
-            folder_id (_type_): _description_
-
-        Returns:
-            list: dict of lists
-        """
-
-        response = self._get(self.LIST.format(folder_id=folder_id))
-        return response
-
-    def get_task(self, task_id: str) -> dict:
-        """Return single task
-
-        Args:
-            task_id (_type_): _description_
-
-        Returns:
-            dict: task
-        """
-
-        response = self._get(self.TASK.format(task_id=task_id))
-        return response
-
-    def get_tasks(self, list_id: str) -> dict:
-        """Return the list of the current task inside of a list
-        {
-        "tasks":[
-            {
-                "id":"25d7z4v",
-                "custom_id":"None",
-                "name":"task 1",
-                "text_content":"None",
-                "description":"None",
-                "status":{
-                    "status":"to do",
-                    "color":"#d3d3d3",
-                    "type":"open",
-                    "orderindex":0
-                },
-                "orderindex":"7221303.00017640000000000000000000000000",
-                "date_created":"1646261029519",
-                "date_updated":"1646261044142",
-                "date_closed":"None",
-                "archived":false,
-                "creator":{
-                    "id":42901062,
-                    "username":"Johann Sebastián",
-                    "color":"#81b1ff",
-                    "email":"jcardenas@gearplug.io",
-                    "profilePicture":"None"
-                },
-                "assignees":[
-                    {
-                    "id":42901062,
-                    "username":"Johann Sebastián",
-                    "color":"#81b1ff",
-                    "initials":"JS",
-                    "email":"jcardenas@gearplug.io",
-                    "profilePicture":"None"
-                    }
-                ],
-                "watchers":[
-
-                ],
-                "checklists":[
-
-                ],
-                "tags":[
-
-                ],
-                "parent":"None",
-                "priority":"None",
-                "due_date":"None",
-                "start_date":"None",
-                "points":"None",
-                "time_estimate":"None",
-                "custom_fields":[
-
-                ],
-                "dependencies":[
-
-                ],
-                "linked_tasks":[
-
-                ],
-                "team_id":"31016756",
-                "url":"https://app.clickup.com/t/25d7z4v",
-                "permission_level":"create",
-                "list":{
-                    "id":"175125718",
-                    "name":"List",
-                    "access":true
-                },
-                "project":{
-                    "id":"103039546",
-                    "name":"folder 1",
-                    "hidden":false,
-                    "access":true
-                },
-                "folder":{
-                    "id":"103039546",
-                    "name":"folder 1",
-                    "hidden":false,
-                    "access":true
-                },
-                "space":{
-                    "id":"49179567"
-                }
-            }
-        ]
-        }
-        Args:
-            list_id (_type_): _description_
-
-        Returns:
-            dict: task
-        """
-
-        response = self._get(self.TASKS.format(list_id=list_id))
-        return response
-
-    def create_task(self, list_id, data: dict):
-        """assignees is an array of the assignees' user ids to be added to this task. You can view the available user ids using the Get Teams (Workspaces) call.
-        example:
-        {
-            "name": "New Task Name",
-            "description": "New Task Description",
-            "assignees": [
-            183
-            ],
-            "tags": [
-            "tag name 1"
-            ],
-            "status": "Open",
-            "priority": 3,
-            "due_date": 1508369194377,
-            "due_date_time": false,
-            "time_estimate": 8640000,
-            "start_date": 1567780450202,
-            "start_date_time": false,
-            "notify_all": true,
-            "parent": null,
-            "links_to": null,
-            "check_required_custom_fields": true,
-            "custom_fields": [
-            {
-                "id": "0a52c486-5f05-403b-b4fd-c512ff05131c",
-                "value": 23
-            },
-            {
-                "id": "03efda77-c7a0-42d3-8afd-fd546353c2f5",
-                "value": "Text field input"
-            }
-            ]
-        }
-        Args:
-            data (dict): _description_
-
-        Returns:
-            _type_: _description_
-        """
-        url = self.TASKS.format(list_id=list_id)
-        data = json.dumps(data)
-        response = self._post(url=url, data=data)
-        return response
-
-    def update_task(self, task_id: str, status: str):
-        url = self.BASE_URL + self.VERSION + "/task/" + task_id
-
-        data = json.dumps({"status": status})
-        response = self._put(url=url, data=data)
-        return response
-
-    def create_webhook(self, task_id: str, team_id: str, endpoint: str, event: str) -> bool:
-        """Creates a webhook based on task changes
-        {
-            {
-            "event": "taskStatusUpdated",
-            "history_items": [
-                {
-                "id": "2861433902084941958",
-                "type": 1,
-                "date": "1646350890907",
-                "field": "status",
-                "parent_id": "175125718",
-                "data": {
-                    "status_type": "custom"
-                },
-                "source": null,
-                "user": {
-                    "id": 42901062,
-                    "username": "Johann Sebastián",
-                    "email": "jcardenas@gearplug.io",
-                    "color": "#81b1ff",
-                    "initials": "JS",
-                    "profilePicture": null
-                },
-                "before": {
-                    "status": "complete",
-                    "color": "#6bc950",
-                    "orderindex": 2,
-                    "type": "closed"
-                },
-                "after": {
-                    "status": "progress",
-                    "color": "#3397dd",
-                    "orderindex": 1,
-                    "type": "custom"
-                }
-                }
-            ],
-            "task_id": "25d7z4v",
-            "webhook_id": "b578c57f-051b-4e58-8c1d-0b3378f681c8"
-        }
-
-        Args:
-            task_id (_type_): _description_
-
-        Returns:
-            bool: _description_
-        """
-        payload = json.dumps({"endpoint": endpoint, "events": [event], "task_id": task_id})
-        response = self._post(url=self.WEBHOOK.format(team_id=team_id), data=payload)
-        return response
-
-    def delete_webhook(self, webhook_id: str) -> bool:
-        """Deletes webhook using ID
-
-        Args:
-            webhook_id (str): _description_
-
-        Returns:
-            bool: _description_
-        """
-        response = self._delete(url=self.DEL_WEBHOOK.format(webhook_id=webhook_id))
-        return response
-
-    def _get(self, url, **kwargs) -> Response:
-        response = self._do_get(url, **kwargs)
-        return response
-
-    def _do_get(self, url, **kwargs) -> Response:
-        return self._request("GET", url, **kwargs)
-
-    def _post(self, url, **kwargs):
-        return self._request("POST", url, **kwargs)
-
-    def _put(self, url, **kwargs):
-        return self._request("PUT", url, **kwargs)
-
-    def _patch(self, url, **kwargs):
-        return self._request("PATCH", url, **kwargs)
-
-    def _delete(self, url, **kwargs):
-        return self._request("DELETE", url, **kwargs)
-
-    def _request(self, method, url, headers=None, **kwargs) -> Response:
-        _headers = {
-            "Authorization": "Bearer {}".format(self.token),
-            "Accept": "application/json",
-            "Content-Type": "application/json",
-        }
-        if headers:
-            _headers.update(headers)
-        return self._parse(requests.request(method, url, headers=_headers, **kwargs))
-
-    def _parse(self, response) -> Response:
-
-        status_code = response.status_code
-
-        if "Content-Type" in response.headers and "application/json" in response.headers["Content-Type"]:
-            r = response.json()
-        else:
-            r = response.content
-
-        if status_code in (200, 201, 202, 204, 206):
-            return r
-        elif status_code == 400:
-            raise exceptions.BadRequest(r)
-        elif status_code == 401:
-            raise exceptions.Unauthorized(r)
-        elif status_code == 403:
-            raise exceptions.Forbidden(r)
-        elif status_code == 404:
-            raise exceptions.NotFound(r)
-        elif status_code == 405:
-            raise exceptions.MethodNotAllowed(r)
-        elif status_code == 406:
-            raise exceptions.NotAcceptable(r)
-        elif status_code == 409:
-            raise exceptions.Conflict(r)
-        elif status_code == 410:
-            raise exceptions.Gone(r)
-        elif status_code == 411:
-            raise exceptions.LengthRequired(r)
-        elif status_code == 412:
-            raise exceptions.PreconditionFailed(r)
-        elif status_code == 413:
-            raise exceptions.RequestEntityTooLarge(r)
-        elif status_code == 415:
-            raise exceptions.UnsupportedMediaType(r)
-        elif status_code == 416:
-            raise exceptions.RequestedRangeNotSatisfiable(r)
-        elif status_code == 422:
-            raise exceptions.UnprocessableEntity(r)
-        elif status_code == 429:
-            raise exceptions.TooManyRequests(r)
-        elif status_code == 500:
-            raise exceptions.InternalServerError(r)
-        elif status_code == 501:
-            raise exceptions.NotImplemented(r)
-        elif status_code == 503:
-            raise exceptions.ServiceUnavailable(r)
-        elif status_code == 504:
-            raise exceptions.GatewayTimeout(r)
-        elif status_code == 507:
-            raise exceptions.InsufficientStorage(r)
-        elif status_code == 509:
-            raise exceptions.BandwidthLimitExceeded(r)
-        else:
-            if r["error"]["innerError"]["code"] == "lockMismatch":
-                # File is currently locked due to being open in the web browser
-                # while attempting to reupload a new version to the drive.
-                # Thus temporarily unavailable.
-                raise exceptions.ServiceUnavailable(r)
-            raise exceptions.UnknownError(r)
+import json
+from clickup import exceptions
+from clickup.response import Response
+from urllib.parse import urlencode
+
+import requests
+
+
+class Client(object):
+    BASE_URL = "https://api.clickup.com/api/"
+    AUTH_URL = "https://app.clickup.com/api"
+    VERSION = "v2"
+
+    WORKSPACE = BASE_URL + VERSION + "/team"
+    SPACE = BASE_URL + VERSION + "/team/{team_id}/space"
+    FOLDER = BASE_URL + VERSION + "/space/{space_id}/folder"
+    LIST = BASE_URL + VERSION + "/folder/{folder_id}/list"
+    TASKS = BASE_URL + VERSION + "/list/{list_id}/task"
+    MEMBERS = BASE_URL + VERSION + "/list/{list_id}/member"
+    CUSTOM_FIELDS = BASE_URL + VERSION + "/list/{list_id}/field"
+    TASK = BASE_URL + VERSION + "/task/{task_id}"
+    WEBHOOK = BASE_URL + VERSION + "/team/{team_id}/webhook"
+    DEL_WEBHOOK = BASE_URL + VERSION + "/webhook/{webhook_id}"
+    REQUEST_TOKEN = BASE_URL + VERSION + "/oauth/token"
+
+    EVENTS = [
+        "taskCreated",
+        "taskUpdated",
+        "taskDeleted",
+        "taskPriorityUpdated",
+        "taskStatusUpdated",
+        "taskAssigneeUpdated",
+        "taskDueDateUpdated",
+        "taskTagUpdated",
+        "taskMoved",
+        "taskCommentPosted",
+        "taskCommentUpdated",
+        "taskTimeEstimateUpdated",
+        "taskTimeTrackedUpdated",
+        "listCreated",
+        "listUpdated",
+        "listDeleted",
+        "folderCreated",
+        "folderUpdated",
+        "folderDeleted",
+        "spaceCreated",
+        "spaceUpdated",
+        "spaceDeleted",
+        "goalCreated",
+        "goalUpdated",
+        "goalDeleted",
+        "keyResultCreated",
+        "keyResultUpdated",
+        "keyResultDeleted",
+    ]
+
+    def __init__(self, client_id: str, client_secret: str) -> None:
+        self.token = None
+        self.client_id = client_id
+        self.client_secret = client_secret
+
+    def authorization_url(self, redirect_uri: str) -> str:
+        params = {"client_id": self.client_id, "client_secret": self.client_secret, "redirect_uri": redirect_uri}
+        url = self.AUTH_URL + "?" + urlencode(params)
+        return url
+
+    def exchange_code(self, code: str) -> Response:
+        """_summary_
+        example:
+        {
+            "access_token": "42901062_76970dae7a8efa65bf8b9ddea7106aefb5a81008"
+        }
+        Args:
+            code (str): _description_
+
+        Returns:
+            Response: _description_
+        """
+        data = json.dumps({"client_id": self.client_id, "client_secret": self.client_secret, "code": code})
+        response = self._post(self.REQUEST_TOKEN, data=data)
+        # response = self._parse(requests.request(method, url, headers=_headers, **kwargs))
+        return response
+
+    def set_token(self, token: str) -> None:
+        """Sets the access_token for its use in this library.
+        Args:
+            token (str): access_token data.
+        """
+        self.token = token
+
+    def get_workspace(self) -> dict:
+        """Return Team ID
+        {
+            "teams":[
+                {
+                    "id":"31016756",
+                    "name":"Gearplug Test",
+                    "color":"#ff4081",
+                    "avatar":"None",
+                    "members":[
+                        {
+                        "user":{
+                            "id":42901062,
+                            "username":"Johann Sebastián",
+                            "email":"jcardenas@gearplug.io",
+                            "color":"#81b1ff",
+                            "profilePicture":"None",
+                            "initials":"JS",
+                            "role":1,
+                            "custom_role":"None",
+                            "last_active":"1646340664585",
+                            "date_joined":"1646059972931",
+                            "date_invited":"1646059972931"
+                        }
+                        }
+                    ]
+                }
+            ]
+            }
+        Returns:
+            dict: _description_
+        """
+        response = self._get(self.WORKSPACE)
+        return response
+
+    def get_spaces(self, team_id: str) -> dict:
+        """Return the spaces list
+        {
+        "spaces":[
+            {
+                "id":"49179567",
+                "name":"Gearplug Test Space 2",
+                "private":false,
+                "statuses":[
+                    {
+                    "id":"p49179567_MCAIkheF",
+                    "status":"to do",
+                    "type":"open",
+                    "orderindex":0,
+                    "color":"#d3d3d3"
+                    },
+                    {
+                    "id":"p49179567_Z1xfhaQK",
+                    "status":"progress",
+                    "type":"custom",
+                    "orderindex":1,
+                    "color":"#3397dd"
+                    },
+                    {
+                    "id":"p49179567_saAGakZL",
+                    "status":"complete",
+                    "type":"closed",
+                    "orderindex":2,
+                    "color":"#6bc950"
+                    }
+                ],
+                "multiple_assignees":true,
+                "features":{
+                    "due_dates":{
+                    "enabled":true,
+                    "start_date":true,
+                    "remap_due_dates":false,
+                    "remap_closed_due_date":false
+                    },
+                    "sprints":{
+                    "enabled":false
+                    },
+                    "time_tracking":{
+                    "enabled":true,
+                    "harvest":false,
+                    "rollup":false
+                    },
+                    "points":{
+                    "enabled":false
+                    },
+                    "custom_items":{
+                    "enabled":false
+                    },
+                    "priorities":{
+                    "enabled":true,
+                    "priorities":[
+                        {
+                            "id":"1",
+                            "priority":"urgent",
+                            "color":"#f50000",
+                            "orderindex":"1"
+                        },
+                        {
+                            "id":"2",
+                            "priority":"high",
+                            "color":"#ffcc00",
+                            "orderindex":"2"
+                        },
+                        {
+                            "id":"3",
+                            "priority":"normal",
+                            "color":"#6fddff",
+                            "orderindex":"3"
+                        },
+                        {
+                            "id":"4",
+                            "priority":"low",
+                            "color":"#d8d8d8",
+                            "orderindex":"4"
+                        }
+                    ]
+                    },
+                    "tags":{
+                    "enabled":true
+                    },
+                    "check_unresolved":{
+                    "enabled":true,
+                    "subtasks":"None",
+                    "checklists":"None",
+                    "comments":"None"
+                    },
+                    "zoom":{
+                    "enabled":false
+                    },
+                    "milestones":{
+                    "enabled":false
+                    },
+                    "custom_fields":{
+                    "enabled":true
+                    },
+                    "dependency_warning":{
+                    "enabled":true
+                    },
+                    "multiple_assignees":{
+                    "enabled":true
+                    }
+                },
+                "archived":false
+            }
+        ]
+        }
+        Args:
+            team_id (_type_): _description_
+
+        Returns:
+            dict: spaces
+        """
+
+        response = self._get(self.SPACE.format(team_id=team_id))
+        return response
+
+    def get_folder(self, space_id: str) -> dict:
+        """Return the folders list
+        {
+        "folders":[
+            {
+                "id":"103039546",
+                "name":"folder 1",
+                "orderindex":1,
+                "override_statuses":false,
+                "hidden":false,
+                "space":{
+                    "id":"49179567",
+                    "name":"Gearplug Test Space 2"
+                },
+                "task_count":"1",
+                "archived":false,
+                "statuses":[
+
+                ],
+                "lists":[
+                    {
+                    "id":"175125718",
+                    "name":"List",
+                    "orderindex":0,
+                    "status":"None",
+                    "priority":"None",
+                    "assignee":"None",
+                    "task_count":1,
+                    "due_date":"None",
+                    "start_date":"None",
+                    "space":{
+                        "id":"49179567",
+                        "name":"Gearplug Test Space 2",
+                        "access":true
+                    },
+                    "archived":false,
+                    "override_statuses":"None",
+                    "statuses":[
+                        {
+                            "id":"p49179567_MCAIkheF",
+                            "status":"to do",
+                            "orderindex":0,
+                            "color":"#d3d3d3",
+                            "type":"open"
+                        },
+                        {
+                            "id":"p49179567_Z1xfhaQK",
+                            "status":"progress",
+                            "orderindex":1,
+                            "color":"#3397dd",
+                            "type":"custom"
+                        },
+                        {
+                            "id":"p49179567_saAGakZL",
+                            "status":"complete",
+                            "orderindex":2,
+                            "color":"#6bc950",
+                            "type":"closed"
+                        }
+                    ],
+                    "permission_level":"create"
+                    }
+                ],
+                "permission_level":"create"
+                }
+            ]
+        }
+        Args:
+            space_id (_type_): _description_
+
+        Returns:
+            dict: folders
+        """
+
+        response = self._get(self.FOLDER.format(space_id=space_id))
+        return response
+
+    def get_list(self, folder_id: str) -> dict:
+        """Return lists of list
+        {
+        "lists":[
+            {
+                "id":"175125718",
+                "name":"List",
+                "orderindex":0,
+                "status":"None",
+                "priority":"None",
+                "assignee":"None",
+                "task_count":1,
+                "due_date":"None",
+                "start_date":"None",
+                "folder":{
+                    "id":"103039546",
+                    "name":"folder 1",
+                    "hidden":false,
+                    "access":true
+                },
+                "space":{
+                    "id":"49179567",
+                    "name":"Gearplug Test Space 2",
+                    "access":true
+                },
+                "archived":false,
+                "override_statuses":"None",
+                "permission_level":"create"
+            }
+        ]
+        }
+        Args:
+            folder_id (_type_): _description_
+
+        Returns:
+            list: dict of lists
+        """
+
+        response = self._get(self.LIST.format(folder_id=folder_id))
+        return response
+
+    def get_task(self, task_id: str) -> dict:
+        """Return single task
+
+        Args:
+            task_id (_type_): _description_
+
+        Returns:
+            dict: task
+        """
+
+        response = self._get(self.TASK.format(task_id=task_id))
+        return response
+
+    def get_tasks(self, list_id: str, params: list = None) -> dict:
+        """Return the list of the current task inside of a list
+        {
+        "tasks":[
+            {
+                "id":"25d7z4v",
+                "custom_id":"None",
+                "name":"task 1",
+                "text_content":"None",
+                "description":"None",
+                "status":{
+                    "status":"to do",
+                    "color":"#d3d3d3",
+                    "type":"open",
+                    "orderindex":0
+                },
+                "orderindex":"7221303.00017640000000000000000000000000",
+                "date_created":"1646261029519",
+                "date_updated":"1646261044142",
+                "date_closed":"None",
+                "archived":false,
+                "creator":{
+                    "id":42901062,
+                    "username":"Johann Sebastián",
+                    "color":"#81b1ff",
+                    "email":"jcardenas@gearplug.io",
+                    "profilePicture":"None"
+                },
+                "assignees":[
+                    {
+                    "id":42901062,
+                    "username":"Johann Sebastián",
+                    "color":"#81b1ff",
+                    "initials":"JS",
+                    "email":"jcardenas@gearplug.io",
+                    "profilePicture":"None"
+                    }
+                ],
+                "watchers":[
+
+                ],
+                "checklists":[
+
+                ],
+                "tags":[
+
+                ],
+                "parent":"None",
+                "priority":"None",
+                "due_date":"None",
+                "start_date":"None",
+                "points":"None",
+                "time_estimate":"None",
+                "custom_fields":[
+
+                ],
+                "dependencies":[
+
+                ],
+                "linked_tasks":[
+
+                ],
+                "team_id":"31016756",
+                "url":"https://app.clickup.com/t/25d7z4v",
+                "permission_level":"create",
+                "list":{
+                    "id":"175125718",
+                    "name":"List",
+                    "access":true
+                },
+                "project":{
+                    "id":"103039546",
+                    "name":"folder 1",
+                    "hidden":false,
+                    "access":true
+                },
+                "folder":{
+                    "id":"103039546",
+                    "name":"folder 1",
+                    "hidden":false,
+                    "access":true
+                },
+                "space":{
+                    "id":"49179567"
+                }
+            }
+        ]
+        }
+        Args:
+            list_id (_type_): _description_
+            params (list): list of params
+
+        Returns:
+            dict: task
+        """
+
+        if params:
+            response = self._get(self.TASKS.format(list_id=list_id) + f"?custom_fields={json.dumps(params)}")
+        else:
+            response = self._get(self.TASKS.format(list_id=list_id))
+        return response
+
+    def get_members(self, list_id: str) -> dict:
+        """Return the list of the current members inside of a list
+        {
+          'members': [
+            {
+              'id': 84869277,
+              'username': 'Jhon Doe',
+              'email': 'Jhon@gmail.com',
+              'color': '',
+              'initials': 'JD',
+              'profilePicture': None,
+              'profileInfo': {
+                'display_profile': None,
+                'verified_ambassador': None,
+                'verified_consultant': None,
+                'top_tier_user': None,
+                'viewed_verified_ambassador': None,
+                'viewed_verified_consultant': None,
+                'viewed_top_tier_user': None
+              }
+            }
+          ]
+        }
+        Args:
+            list_id (_type_): _description_
+
+        Returns:
+            dict: members
+        """
+        response = self._get(self.MEMBERS.format(list_id=list_id))
+        return response
+
+    def get_custom_fields(self, list_id: str) -> dict:
+        """Return the list of the current task inside of a list
+        {
+          'fields': [
+            {
+              'id': '624e56f6-62b8-4593-be83-f1ed4cd147dc',
+              'name': 'Jhon Doe',
+              'type': 'drop_down',
+              'type_config': {
+                'options': [
+                  {
+                    'id': '97d85961-1437-4e17-881c-1db1501ccb9a',
+                    'name': 'Algo 1',
+                    'color': None,
+                    'orderindex': 0
+                  },
+                  {
+                    'id': '8ea9498e-1f0c-4264-b0c9-49565bc08fb3',
+                    'name': 'Algo 2',
+                    'color': None,
+                    'orderindex': 1
+                  }
+                ]
+              },
+              'date_created': '1712686424346',
+              'hide_from_guests': False,
+              'required': False
+            }
+          ]
+        }
+        Args:
+            list_id (_type_): _description_
+
+        Returns:
+            dict: task
+        """
+
+        response = self._get(self.CUSTOM_FIELDS.format(list_id=list_id))
+        return response
+
+    def create_task(self, list_id, data: dict):
+        """assignees is an array of the assignees' user ids to be added to this task. You can view the available user ids using the Get Teams (Workspaces) call.
+        example:
+        {
+            "name": "New Task Name",
+            "description": "New Task Description",
+            "assignees": [
+            183
+            ],
+            "tags": [
+            "tag name 1"
+            ],
+            "status": "Open",
+            "priority": 3,
+            "due_date": 1508369194377,
+            "due_date_time": false,
+            "time_estimate": 8640000,
+            "start_date": 1567780450202,
+            "start_date_time": false,
+            "notify_all": true,
+            "parent": null,
+            "links_to": null,
+            "check_required_custom_fields": true,
+            "custom_fields": [
+            {
+                "id": "0a52c486-5f05-403b-b4fd-c512ff05131c",
+                "value": 23
+            },
+            {
+                "id": "03efda77-c7a0-42d3-8afd-fd546353c2f5",
+                "value": "Text field input"
+            }
+            ]
+        }
+        Args:
+            data (dict): _description_
+
+        Returns:
+            _type_: _description_
+        """
+        url = self.TASKS.format(list_id=list_id)
+        data = json.dumps(data)
+        response = self._post(url=url, data=data)
+        return response
+
+    def update_task(self, task_id: str, status: str):
+        url = self.BASE_URL + self.VERSION + "/task/" + task_id
+
+        data = json.dumps({"status": status})
+        response = self._put(url=url, data=data)
+        return response
+
+    def create_webhook(self, task_id: str, team_id: str, endpoint: str, event: str) -> bool:
+        """Creates a webhook based on task changes
+        {
+            {
+            "event": "taskStatusUpdated",
+            "history_items": [
+                {
+                "id": "2861433902084941958",
+                "type": 1,
+                "date": "1646350890907",
+                "field": "status",
+                "parent_id": "175125718",
+                "data": {
+                    "status_type": "custom"
+                },
+                "source": null,
+                "user": {
+                    "id": 42901062,
+                    "username": "Johann Sebastián",
+                    "email": "jcardenas@gearplug.io",
+                    "color": "#81b1ff",
+                    "initials": "JS",
+                    "profilePicture": null
+                },
+                "before": {
+                    "status": "complete",
+                    "color": "#6bc950",
+                    "orderindex": 2,
+                    "type": "closed"
+                },
+                "after": {
+                    "status": "progress",
+                    "color": "#3397dd",
+                    "orderindex": 1,
+                    "type": "custom"
+                }
+                }
+            ],
+            "task_id": "25d7z4v",
+            "webhook_id": "b578c57f-051b-4e58-8c1d-0b3378f681c8"
+        }
+
+        Args:
+            task_id (_type_): _description_
+
+        Returns:
+            bool: _description_
+        """
+        payload = json.dumps({"endpoint": endpoint, "events": [event], "task_id": task_id})
+        response = self._post(url=self.WEBHOOK.format(team_id=team_id), data=payload)
+        return response
+
+    def delete_webhook(self, webhook_id: str) -> bool:
+        """Deletes webhook using ID
+
+        Args:
+            webhook_id (str): _description_
+
+        Returns:
+            bool: _description_
+        """
+        response = self._delete(url=self.DEL_WEBHOOK.format(webhook_id=webhook_id))
+        return response
+
+    def _get(self, url, **kwargs) -> Response:
+        response = self._do_get(url, **kwargs)
+        return response
+
+    def _do_get(self, url, **kwargs) -> Response:
+        return self._request("GET", url, **kwargs)
+
+    def _post(self, url, **kwargs):
+        return self._request("POST", url, **kwargs)
+
+    def _put(self, url, **kwargs):
+        return self._request("PUT", url, **kwargs)
+
+    def _patch(self, url, **kwargs):
+        return self._request("PATCH", url, **kwargs)
+
+    def _delete(self, url, **kwargs):
+        return self._request("DELETE", url, **kwargs)
+
+    def _request(self, method, url, headers=None, **kwargs) -> Response:
+        _headers = {
+            "Authorization": "Bearer {}".format(self.token),
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+        }
+        if headers:
+            _headers.update(headers)
+        return self._parse(requests.request(method, url, headers=_headers, **kwargs))
+
+    def _parse(self, response) -> Response:
+
+        status_code = response.status_code
+
+        if "Content-Type" in response.headers and "application/json" in response.headers["Content-Type"]:
+            r = response.json()
+        else:
+            r = response.content
+
+        if status_code in (200, 201, 202, 204, 206):
+            return r
+        elif status_code == 400:
+            raise exceptions.BadRequest(r)
+        elif status_code == 401:
+            raise exceptions.Unauthorized(r)
+        elif status_code == 403:
+            raise exceptions.Forbidden(r)
+        elif status_code == 404:
+            raise exceptions.NotFound(r)
+        elif status_code == 405:
+            raise exceptions.MethodNotAllowed(r)
+        elif status_code == 406:
+            raise exceptions.NotAcceptable(r)
+        elif status_code == 409:
+            raise exceptions.Conflict(r)
+        elif status_code == 410:
+            raise exceptions.Gone(r)
+        elif status_code == 411:
+            raise exceptions.LengthRequired(r)
+        elif status_code == 412:
+            raise exceptions.PreconditionFailed(r)
+        elif status_code == 413:
+            raise exceptions.RequestEntityTooLarge(r)
+        elif status_code == 415:
+            raise exceptions.UnsupportedMediaType(r)
+        elif status_code == 416:
+            raise exceptions.RequestedRangeNotSatisfiable(r)
+        elif status_code == 422:
+            raise exceptions.UnprocessableEntity(r)
+        elif status_code == 429:
+            raise exceptions.TooManyRequests(r)
+        elif status_code == 500:
+            raise exceptions.InternalServerError(r)
+        elif status_code == 501:
+            raise exceptions.NotImplemented(r)
+        elif status_code == 503:
+            raise exceptions.ServiceUnavailable(r)
+        elif status_code == 504:
+            raise exceptions.GatewayTimeout(r)
+        elif status_code == 507:
+            raise exceptions.InsufficientStorage(r)
+        elif status_code == 509:
+            raise exceptions.BandwidthLimitExceeded(r)
+        else:
+            if r["error"]["innerError"]["code"] == "lockMismatch":
+                # File is currently locked due to being open in the web browser
+                # while attempting to reupload a new version to the drive.
+                # Thus temporarily unavailable.
+                raise exceptions.ServiceUnavailable(r)
+            raise exceptions.UnknownError(r)
```

### Comparing `clickup_python-1.0.2/clickup/exceptions.py` & `clickup_python-1.0.3/clickup/exceptions.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-class BaseError(Exception):
-    pass
-
-
-class UnknownError(BaseError):
-    pass
-
-
-class TokenRequired(BaseError):
-    pass
-
-
-class BadRequest(BaseError):
-    pass
-
-
-class Unauthorized(BaseError):
-    pass
-
-
-class Forbidden(BaseError):
-    pass
-
-
-class NotFound(BaseError):
-    pass
-
-
-class MethodNotAllowed(BaseError):
-    pass
-
-
-class NotAcceptable(BaseError):
-    pass
-
-
-class Conflict(BaseError):
-    pass
-
-
-class Gone(BaseError):
-    pass
-
-
-class LengthRequired(BaseError):
-    pass
-
-
-class PreconditionFailed(BaseError):
-    pass
-
-
-class RequestEntityTooLarge(BaseError):
-    pass
-
-
-class UnsupportedMediaType(BaseError):
-    pass
-
-
-class RequestedRangeNotSatisfiable(BaseError):
-    pass
-
-
-class UnprocessableEntity(BaseError):
-    pass
-
-
-class TooManyRequests(BaseError):
-    pass
-
-
-class InternalServerError(BaseError):
-    pass
-
-
-class NotImplemented(BaseError):
-    pass
-
-
-class ServiceUnavailable(BaseError):
-    pass
-
-
-class GatewayTimeout(BaseError):
-    pass
-
-
-class InsufficientStorage(BaseError):
-    pass
-
-
-class BandwidthLimitExceeded(BaseError):
+class BaseError(Exception):
+    pass
+
+
+class UnknownError(BaseError):
+    pass
+
+
+class TokenRequired(BaseError):
+    pass
+
+
+class BadRequest(BaseError):
+    pass
+
+
+class Unauthorized(BaseError):
+    pass
+
+
+class Forbidden(BaseError):
+    pass
+
+
+class NotFound(BaseError):
+    pass
+
+
+class MethodNotAllowed(BaseError):
+    pass
+
+
+class NotAcceptable(BaseError):
+    pass
+
+
+class Conflict(BaseError):
+    pass
+
+
+class Gone(BaseError):
+    pass
+
+
+class LengthRequired(BaseError):
+    pass
+
+
+class PreconditionFailed(BaseError):
+    pass
+
+
+class RequestEntityTooLarge(BaseError):
+    pass
+
+
+class UnsupportedMediaType(BaseError):
+    pass
+
+
+class RequestedRangeNotSatisfiable(BaseError):
+    pass
+
+
+class UnprocessableEntity(BaseError):
+    pass
+
+
+class TooManyRequests(BaseError):
+    pass
+
+
+class InternalServerError(BaseError):
+    pass
+
+
+class NotImplemented(BaseError):
+    pass
+
+
+class ServiceUnavailable(BaseError):
+    pass
+
+
+class GatewayTimeout(BaseError):
+    pass
+
+
+class InsufficientStorage(BaseError):
+    pass
+
+
+class BandwidthLimitExceeded(BaseError):
     pass
```

### Comparing `clickup_python-1.0.2/PKG-INFO` & `clickup_python-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: clickup-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: API wrapper for ClickUp written in Python
 License: MIT
-Author: Miguel Ferrer
-Author-email: ingferrermiguel@gmail.com
+Author: Gearplug Team
+Author-email: apps@gearplug.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # clickup-python
 ClickUp API wrapper written in python
 
 ## Installing
```

