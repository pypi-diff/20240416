# Comparing `tmp/django_admin_background_task-0.1.0.tar.gz` & `tmp/django_admin_background_task-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_admin_background_task-0.1.0.tar", max compression
+gzip compressed data, was "django_admin_background_task-0.2.0.tar", max compression
```

## Comparing `django_admin_background_task-0.1.0.tar` & `django_admin_background_task-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
--rw-r--r--   0        0        0    11357 2024-03-08 11:29:40.116270 django_admin_background_task-0.1.0/LICENSE
--rw-r--r--   0        0        0      597 2024-03-08 15:18:31.249786 django_admin_background_task-0.1.0/README.md
--rw-r--r--   0        0        0     6148 2024-03-08 11:30:13.720132 django_admin_background_task-0.1.0/bgtask/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-08 11:30:13.723481 django_admin_background_task-0.1.0/bgtask/__init__.py
--rw-r--r--   0        0        0      854 2024-03-08 11:30:13.730142 django_admin_background_task-0.1.0/bgtask/admin.py
--rw-r--r--   0        0        0      144 2024-03-08 11:30:13.729684 django_admin_background_task-0.1.0/bgtask/apps.py
--rw-r--r--   0        0        0     2013 2024-03-08 11:30:13.719326 django_admin_background_task-0.1.0/bgtask/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-08 11:30:13.714396 django_admin_background_task-0.1.0/bgtask/migrations/__init__.py
--rw-r--r--   0        0        0     7683 2024-03-08 12:25:51.787186 django_admin_background_task-0.1.0/bgtask/models.py
--rw-r--r--   0        0        0      231 2024-03-08 11:30:13.721685 django_admin_background_task-0.1.0/bgtask/stack_contexts.py
--rw-r--r--   0        0        0      746 2024-03-08 11:30:13.732726 django_admin_background_task-0.1.0/bgtask/static/bgtask/js/bgtask-once.js
--rw-r--r--   0        0        0    12636 2024-03-08 11:30:13.733294 django_admin_background_task-0.1.0/bgtask/static/bgtask/js/bgtask.js
--rw-r--r--   0        0        0      852 2024-03-08 11:30:13.734974 django_admin_background_task-0.1.0/bgtask/templates/bgtask/bg_changelist_status_column.html
--rw-r--r--   0        0        0        1 2024-03-08 11:30:13.737691 django_admin_background_task-0.1.0/bgtask/templates/bgtask/bgtask_templates.html
--rw-r--r--   0        0        0     1845 2024-03-08 11:30:13.736549 django_admin_background_task-0.1.0/bgtask/templates/bgtask/bgtask_view.html
--rw-r--r--   0        0        0      166 2024-03-08 11:30:13.735684 django_admin_background_task-0.1.0/bgtask/templates/bgtask/progress.html
--rw-r--r--   0        0        0        0 2024-03-08 11:30:13.710598 django_admin_background_task-0.1.0/bgtask/templatetags/__init__.py
--rw-r--r--   0        0        0      413 2024-03-08 11:30:13.710386 django_admin_background_task-0.1.0/bgtask/templatetags/bgtask.py
--rw-r--r--   0        0        0     1090 2024-03-08 11:30:13.723311 django_admin_background_task-0.1.0/bgtask/tests/test_bgtask.py
--rw-r--r--   0        0        0      161 2024-03-08 11:30:13.738363 django_admin_background_task-0.1.0/bgtask/urls.py
--rw-r--r--   0        0        0     1983 2024-03-08 11:58:17.670993 django_admin_background_task-0.1.0/bgtask/views.py
--rw-r--r--   0        0        0     1706 2024-03-08 15:18:15.181380 django_admin_background_task-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 django_admin_background_task-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-08 11:29:40.116270 django_admin_background_task-0.2.0/LICENSE
+-rw-r--r--   0        0        0      597 2024-03-08 15:24:11.483284 django_admin_background_task-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-08 11:30:13.723481 django_admin_background_task-0.2.0/bgtask/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-16 15:31:09.755506 django_admin_background_task-0.2.0/bgtask/admin.py
+-rw-r--r--   0        0        0      144 2024-03-08 11:30:13.729684 django_admin_background_task-0.2.0/bgtask/apps.py
+-rw-r--r--   0        0        0       57 2024-03-10 23:21:32.768101 django_admin_background_task-0.2.0/bgtask/backends/__init__.py
+-rw-r--r--   0        0        0      304 2024-03-10 23:20:51.665708 django_admin_background_task-0.2.0/bgtask/backends/thread_pool.py
+-rw-r--r--   0        0        0     1119 2024-04-16 15:15:56.816234 django_admin_background_task-0.2.0/bgtask/decorators.py
+-rw-r--r--   0        0        0     2013 2024-03-08 11:30:13.719326 django_admin_background_task-0.2.0/bgtask/migrations/0001_initial.py
+-rw-r--r--   0        0        0      968 2024-04-16 14:59:49.149350 django_admin_background_task-0.2.0/bgtask/migrations/0002_backgroundtask_namespace_alter_backgroundtask_name.py
+-rw-r--r--   0        0        0        0 2024-03-08 11:30:13.714396 django_admin_background_task-0.2.0/bgtask/migrations/__init__.py
+-rw-r--r--   0        0        0     2925 2024-04-16 15:13:30.710650 django_admin_background_task-0.2.0/bgtask/model_admin.py
+-rw-r--r--   0        0        0     9184 2024-04-16 15:32:37.932296 django_admin_background_task-0.2.0/bgtask/models.py
+-rw-r--r--   0        0        0      231 2024-03-08 11:30:13.721685 django_admin_background_task-0.2.0/bgtask/stack_contexts.py
+-rw-r--r--   0        0        0      746 2024-03-08 11:30:13.732726 django_admin_background_task-0.2.0/bgtask/static/bgtask/js/bgtask-once.js
+-rw-r--r--   0        0        0    13151 2024-03-12 15:54:33.635207 django_admin_background_task-0.2.0/bgtask/static/bgtask/js/bgtask.js
+-rw-r--r--   0        0        0     1062 2024-04-14 14:54:44.154777 django_admin_background_task-0.2.0/bgtask/templates/bgtask/admin/change_list.html
+-rw-r--r--   0        0        0      978 2024-03-12 15:14:21.911729 django_admin_background_task-0.2.0/bgtask/templates/bgtask/bg_changelist_status_column.html
+-rw-r--r--   0        0        0        1 2024-03-08 11:30:13.737691 django_admin_background_task-0.2.0/bgtask/templates/bgtask/bgtask_templates.html
+-rw-r--r--   0        0        0     1845 2024-03-08 11:30:13.736549 django_admin_background_task-0.2.0/bgtask/templates/bgtask/bgtask_view.html
+-rw-r--r--   0        0        0      166 2024-03-08 11:30:13.735684 django_admin_background_task-0.2.0/bgtask/templates/bgtask/progress.html
+-rw-r--r--   0        0        0        0 2024-03-08 11:30:13.710598 django_admin_background_task-0.2.0/bgtask/templatetags/__init__.py
+-rw-r--r--   0        0        0      413 2024-03-08 11:30:13.710386 django_admin_background_task-0.2.0/bgtask/templatetags/bgtask.py
+-rw-r--r--   0        0        0     1090 2024-03-08 11:30:13.723311 django_admin_background_task-0.2.0/bgtask/tests/test_bgtask.py
+-rw-r--r--   0        0        0      161 2024-03-08 11:30:13.738363 django_admin_background_task-0.2.0/bgtask/urls.py
+-rw-r--r--   0        0        0     1765 2024-03-12 15:30:59.663003 django_admin_background_task-0.2.0/bgtask/views.py
+-rw-r--r--   0        0        0     1706 2024-03-12 15:36:09.621880 django_admin_background_task-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 django_admin_background_task-0.2.0/PKG-INFO
```

### Comparing `django_admin_background_task-0.1.0/LICENSE` & `django_admin_background_task-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.1.0/README.md` & `django_admin_background_task-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```
 INSTALLED_APPS = [
     ...
     "bgtask",
 ]
 ```
 
-And mount the amdin monitoring URLs:
+And mount the admin monitoring URLs:
 
 ```
 urlpatterns = [
     # You should be able to mount them anywhere but I put them here
     path(r"admin/background-task/", include("bgtask.urls")),
     path("admin", admin.site.urls),
 ]
```

### Comparing `django_admin_background_task-0.1.0/bgtask/admin.py` & `django_admin_background_task-0.2.0/bgtask/admin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from django.contrib import admin
 from django.template.loader import render_to_string
 
 from .models import BackgroundTask
-from .views import task_dict
 
 
 def background_task_status(obj):
     if isinstance(obj, BackgroundTask):
         bgtask = obj
     else:
         bgtasks = BackgroundTask.objects.filter(acted_on_object_id=obj.id).order_by("-created")
 
         # for now just pick the most recent
         bgtask = bgtasks.first()
 
     output = render_to_string(
-        "bgtask/bg_changelist_status_column.html", {"bgtask": bgtask and task_dict(bgtask)}
+        "bgtask/bg_changelist_status_column.html", {"bgtask": bgtask and bgtask.task_dict}
     )
     return output
 
 
 background_task_status.__name__ = "Task Status"
 
 
 @admin.register(BackgroundTask)
 class BackgroundTaskAdmin(admin.ModelAdmin):
-    list_filter = ["state", "result"]
-    list_display = ("created", background_task_status, "result", "completed_at")
+    list_filter = ["state", "namespace", "name"]
+    list_display = ("created", "namespace_name", background_task_status, "result", "completed_at")
     ordering = ["-created"]
+
+    def namespace_name(self, bgtask):
+        return ".".join(f for f in [bgtask.namespace, bgtask.name] if f)
```

### Comparing `django_admin_background_task-0.1.0/bgtask/migrations/0001_initial.py` & `django_admin_background_task-0.2.0/bgtask/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.1.0/bgtask/models.py` & `django_admin_background_task-0.2.0/bgtask/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 import functools
 import logging
 import os
 import time
 import traceback
 import uuid
+from contextlib import contextmanager
 
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.db import models, transaction
+from django.forms.models import model_to_dict
 from django.utils import timezone
 
 from model_utils import Choices
 
 
 log = logging.getLogger(__name__)
 
 
 def locked(meth):
     @functools.wraps(meth)
     def _locked_meth(self, *args, **kwargs):
+        if getattr(self, "_locked", False):
+            return meth(self, *args, **kwargs)
+
         with transaction.atomic():
             BackgroundTask.objects.filter(id=self.id).select_for_update().only("id").get()
-            return meth(self, *args, **kwargs)
+            self.refresh_from_db()
+
+            # Mark as locked in case we are called recursively
+            self._locked = True
+            try:
+                return meth(self, *args, **kwargs)
+            finally:
+                self._locked = False
 
     return _locked_meth
 
 
 def only_if_state(state):
     def only_if_state_decorator(meth):
         def only_if_state_wrapper(self, *args, **kwargs):
@@ -37,22 +49,32 @@
             return meth(self, *args, **kwargs)
 
         return only_if_state_wrapper
 
     return only_if_state_decorator
 
 
-class CreatedUpdatedMixin(models.Model):
-    class Meta:
-        abstract = True
-
-
-class BackgroundTask(CreatedUpdatedMixin):
+class BackgroundTask(models.Model):
     id = models.UUIDField(primary_key=True, editable=False, default=uuid.uuid4)
-    name = models.CharField(max_length=1000)
+    name = models.CharField(
+        max_length=1000,
+        help_text=(
+            "Name (or type) of this task, is not unique "
+            "per task instance but generally per task functionality"
+        ),
+    )
+    namespace = models.CharField(
+        max_length=1000,
+        default="",
+        blank=True,
+        help_text=(
+            "Optional namespace that can be used to avoid having to make names unique across an "
+            "entire codebase, allowing them to be shorter and human readable"
+        ),
+    )
 
     STATES = Choices("not_started", "running", "success", "partial_success", "failed")
     state = models.CharField(max_length=16, default=STATES.not_started, choices=STATES)
     steps_to_complete = models.PositiveIntegerField(
         null=True, blank=True, help_text="The number of steps in the task for it to be completed."
     )
     steps_completed = models.PositiveIntegerField(
@@ -76,21 +98,44 @@
     created = models.DateTimeField(auto_now_add=True)
     updated = models.DateTimeField(auto_now=True)
 
     class Meta:
         ordering = ["created", "id"]
 
     @property
+    def task_dict(self):
+        task_dict = model_to_dict(self)
+        return {"id": str(self.id), "updated": self.updated.isoformat(), **task_dict}
+
+    @property
     def num_failed_steps(self):
         return sum(error.get("num_failed_steps", 0) for error in self.errors)
 
     @property
     def incomplete(self):
         return self.state in [self.STATES.not_started, self.STATES.running]
 
+    @contextmanager
+    def runs_single_step(self):
+        try:
+            yield
+        except Exception as exc:
+            self.steps_failed(1, error=exc)
+        else:
+            self.add_successful_steps(1)
+
+    @contextmanager
+    def finishes(self):
+        try:
+            yield
+        except Exception as exc:
+            self.fail(exc)
+        else:
+            self.succeed()
+
     @locked
     @only_if_state(STATES.not_started)
     def start(self):
         log.info("%s starting", self)
         self.state = self.STATES.running
         self.started_at = timezone.now()
         self.save()
@@ -105,60 +150,61 @@
         self.errors.append(
             {"datetime": self.completed_at.isoformat(), **self._error_dict_for_error(exc)},
         )
         self.save()
 
     @locked
     @only_if_state(STATES.running)
-    def succeed(self, result):
+    def succeed(self, result=None):
         log.info("%s succeeded.", self)
         self.state = self.STATES.success
-        self.completion = 1
+        self.steps_completed = self.steps_to_complete
         self.completed_at = timezone.now()
         self.result = self.serialize_result(result)
         self.save()
 
     @locked
     @only_if_state(STATES.running)
     def finish(self):
         """Mark task as finished, automatically deducing the final state."""
         if not self.errors:
             log.info("Finishing as success with no errors")
             self.state = self.STATES.success
         elif self.steps_to_complete is None:
-            log.info("Finishing as failure with no steps to complete configured")
-            self.state = self.STATES.failed
+            log.info("Finishing as success with no steps to complete configured")
+            self.state = self.STATES.success
         elif self.num_failed_steps == self.steps_to_complete:
             log.info("Finishing as failure with all steps failed")
             self.state = self.STATES.failed
         else:
             log.info("Finishing as partial success with some steps failed")
             self.state = self.STATES.partial_success
 
+        self.completed_at = timezone.now()
+        self.save()
+
     @locked
     def add_successful_steps(self, num_steps):
         self.steps_completed += num_steps
-        self._maybe_finish()
-        self.save()
+        self._finish_or_save()
 
     @locked
     def steps_failed(self, num_steps, steps_identifier=None, error=None):
         self.steps_completed += num_steps
         error_dict = {
             "datetime": timezone.now().isoformat(),
             "num_failed_steps": num_steps,
         }
         if steps_identifier:
             error_dict["steps_identifier"] = steps_identifier
 
         error_dict.update(self._error_dict_for_error(error))
 
         self.errors.append(error_dict)
-        self._maybe_finish()
-        self.save()
+        self._finish_or_save()
 
     def dispatch(self):
         # double fork to avoid zombies
         pid = os.fork()
 
         if pid != 0:
             log.info("Waiting for child %d", pid)
@@ -223,13 +269,16 @@
 
         if hasattr(error, "__traceback__"):
             error_dict["traceback"] = "".join(
                 traceback.format_list(traceback.extract_tb(error.__traceback__))
             )
         return error_dict
 
-    def _maybe_finish(self):
-        if self.steps_to_complete is None:
-            return
-
-        if self.steps_completed >= self.steps_to_complete:
+    def _finish_or_save(self):
+        if (
+            self.steps_to_complete is not None
+            and self.steps_completed is not None
+            and self.steps_completed >= self.steps_to_complete
+        ):
             self.finish()
+        else:
+            self.save()
```

### Comparing `django_admin_background_task-0.1.0/bgtask/static/bgtask/js/bgtask-once.js` & `django_admin_background_task-0.2.0/bgtask/static/bgtask/js/bgtask-once.js`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.1.0/bgtask/static/bgtask/js/bgtask.js` & `django_admin_background_task-0.2.0/bgtask/static/bgtask/js/bgtask.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -23,15 +23,15 @@
         max
     } = {
         value: null,
         max: null
     }) {
         this.element = element;
 
-        this.timerId = null;
+        this.animationFrameRequestId = null;
 
         this.max = max;
         // set it immediately initially
         this.progEle.value = value;
     }
 
     update({
@@ -62,64 +62,69 @@
         return this.progEle.value;
     }
     set value(value) {
         // we're going to start the timer again if it was already running.
         this._cancelTimer();
         const currentValue = this.progEle.value || 0;
         if (value === null || value === undefined) {
+            // console.info("null value");
             this.progEle.removeAttribute("value");
-            this._clearState();
             return
         }
         if (value >= this.max) {
+            // console.info("greater than max", value, this.max);
             this.progEle.value = this.max;
-            this._clearState();
             return;
         }
         if (currentValue === value) {
-            this._clearState();
+            // console.info("already at value", currentValue, value);
             return;
         }
 
         // completion due in the refresh period plus a bit so that we don't get there too soon
         // and cause a visible stop: we would rather the next update arrived before we reached the
         // target value
-        const completionDue = new Date(new Date().getTime() + REFRESH_PERIOD_MS + 500);
-        const initialMSToCompletion = completionDue - new Date();
+        const now = new Date();
+        const completionDue = new Date(now.getTime() + REFRESH_PERIOD_MS + PROGRESS_REFRESH_MS);
+        const initialMSToCompletion = completionDue - now;
+        const completionDueHighRes = performance.now() + initialMSToCompletion;
         const previousValue = currentValue;
 
-        const updateProgress = () => {
-            const now = new Date();
-            if (completionDue <= now) {
-                this.progEle.value = value;
-                this._cancelTimer();
-                this._clearState();
+        let startTimestamp = null;
+
+        const updateProgressStep = (now) => {
+            if (startTimestamp === null) {
+                startTimestamp = now;
+                this.animationFrameRequestId = window.requestAnimationFrame(updateProgressStep);
                 return;
             }
-
-            const msRemaining = completionDue - now;
-
+            const msRemaining = completionDueHighRes - now;
             const newValue = previousValue + (
                 ((initialMSToCompletion - msRemaining) / initialMSToCompletion) *
                 (value - previousValue)
             );
+
+            if (completionDue <= now || Math.abs((value - newValue) / this.progEle.max) < 0.001) {
+                this.progEle.value = value;
+                return;
+            }
+
             this.progEle.value = newValue;
-        };
+            this.animationFrameRequestId = window.requestAnimationFrame(updateProgressStep);
+        }
 
-        this.timerId = setInterval(updateProgress, PROGRESS_REFRESH_MS);
+        this.animationFrameRequestId = window.requestAnimationFrame(updateProgressStep);
     }
 
     _cancelTimer() {
-        if (this.timerId !== null) {
-            clearInterval(this.timerId);
+        if (this.animationFrameRequestId !== null) {
+            window.cancelAnimationFrame(this.animationFrameRequestId)
         }
-        this.timerId = null;
+        this.animationFrameRequestId = null;
     }
-
-    _clearState() {}
 }
 
 // -------------------------------------------------------------------------------------------------
 // Manage the progress div (what's in the column the admin list view of a taskable model).
 // -------------------------------------------------------------------------------------------------
 class TaskProgressDiv {
     constructor(divOrId, task) {
```

### Comparing `django_admin_background_task-0.1.0/bgtask/templates/bgtask/bg_changelist_status_column.html` & `django_admin_background_task-0.2.0/bgtask/templates/bgtask/bg_changelist_status_column.html`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 {% if not bgtask %}
 -
 {% else %}
 {% with initialTasksJsonId="initialTasksJson-"|add:bgtask.id %}
 {{ bgtask|json_script:initialTasksJsonId }}
 {% endwith %}
 <script src="{% static 'bgtask/js/bgtask-once.js' %}"></script>
+{% if bgtask.acted_on_object_id %}
 <a href="{% url 'bgtask:tasks' %}?object_id={{bgtask.acted_on_object_id}}">
+{% else %}
+<a href="{% url 'admin:bgtask_backgroundtask_change' bgtask.id %}">
+{% endif %}
     <div id="bgtask-column-{{ bgtask.id }}">
         {% include 'bgtask/progress.html' %}
     </div>
 </a>
 <script>
 (() => {
     const poller = BGTaskPoller.sharedInstance("{% url 'bgtask:tasks' %}");
```

#### html2text {}

```diff
@@ -1,5 +1,8 @@
 {% load static %} {% if not bgtask %} - {% else %} {% with
 initialTasksJsonId="initialTasksJson-"|add:bgtask.id %} {{ bgtask|json_script:
 initialTasksJsonId }} {% endwith %}
+{% if bgtask.acted_on_object_id %}
+_{_%_ _e_l_s_e_ _%_}
+_{_%_ _e_n_d_i_f_ _%_}
 _{_%_ _i_n_c_l_u_d_e_ _'_b_g_t_a_s_k_/_p_r_o_g_r_e_s_s_._h_t_m_l_'_ _%_}
 {% endif %}
```

### Comparing `django_admin_background_task-0.1.0/bgtask/templates/bgtask/bgtask_view.html` & `django_admin_background_task-0.2.0/bgtask/templates/bgtask/bgtask_view.html`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.1.0/bgtask/tests/test_bgtask.py` & `django_admin_background_task-0.2.0/bgtask/tests/test_bgtask.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.1.0/bgtask/views.py` & `django_admin_background_task-0.2.0/bgtask/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,16 @@
 
 from .models import BackgroundTask
 
 
 Q_NONE = Q(pk__in=[])
 
 
-def task_dict(task):
-    task_dict = model_to_dict(task)
-    if "stack_context" in task_dict:
-        del task_dict["stack_context"]
-    return {"id": str(task.id), "updated": task.updated.isoformat(), **task_dict}
-
-
 def _tasks_dict(tasks):
-    td = {str(task.id): task_dict(task) for task in tasks}
+    td = {str(task.id): task.task_dict for task in tasks}
     return td
 
 
 def background_tasks_view_html(request, task):
     return render(
         request,
         "bgtask/bgtask_view.html",
```

### Comparing `django_admin_background_task-0.1.0/pyproject.toml` & `django_admin_background_task-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-admin-background-task"
-version = "0.1.0"
+version = "0.2.0"
 description = "A set of tools for django apps to persist and monitor the status of background tasks"
 authors = [
     "David Park <david@greenparksoftware.co.uk>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/daphtdazz/django-bgtask"
```

### Comparing `django_admin_background_task-0.1.0/PKG-INFO` & `django_admin_background_task-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-background-task
-Version: 0.1.0
+Version: 0.2.0
 Summary: A set of tools for django apps to persist and monitor the status of background tasks
 Home-page: https://github.com/daphtdazz/django-bgtask
 License: Apache-2.0
 Author: David Park
 Author-email: david@greenparksoftware.co.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -37,15 +37,15 @@
 ```
 INSTALLED_APPS = [
     ...
     "bgtask",
 ]
 ```
 
-And mount the amdin monitoring URLs:
+And mount the admin monitoring URLs:
 
 ```
 urlpatterns = [
     # You should be able to mount them anywhere but I put them here
     path(r"admin/background-task/", include("bgtask.urls")),
     path("admin", admin.site.urls),
 ]
```

