# Comparing `tmp/wtforms-widgets-1.0.7.tar.gz` & `tmp/wtforms_widgets-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtforms-widgets-1.0.7.tar", last modified: Sun Mar  7 14:58:30 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `wtforms-widgets-1.0.7.tar` & `wtforms_widgets-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,15 @@
-drwxr-xr-x   0 ibot3     (1000) ibot3     (1000)        0 2021-03-07 14:58:30.433351 wtforms-widgets-1.0.7/
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)      759 2021-03-07 14:58:30.433351 wtforms-widgets-1.0.7/PKG-INFO
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)     1695 2021-03-07 14:47:32.000000 wtforms-widgets-1.0.7/README.md
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)       38 2021-03-07 14:58:30.433351 wtforms-widgets-1.0.7/setup.cfg
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)     1080 2021-03-07 14:57:50.000000 wtforms-widgets-1.0.7/setup.py
-drwxr-xr-x   0 ibot3     (1000) ibot3     (1000)        0 2021-03-07 14:58:30.430018 wtforms-widgets-1.0.7/wtforms_widgets/
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)        0 2021-01-07 15:37:13.000000 wtforms-widgets-1.0.7/wtforms_widgets/__init__.py
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)      484 2021-01-07 15:37:13.000000 wtforms-widgets-1.0.7/wtforms_widgets/base_form.py
-drwxr-xr-x   0 ibot3     (1000) ibot3     (1000)        0 2021-03-07 14:58:30.433351 wtforms-widgets-1.0.7/wtforms_widgets/fields/
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)       24 2021-01-07 15:37:13.000000 wtforms-widgets-1.0.7/wtforms_widgets/fields/__init__.py
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)     7808 2021-01-07 15:37:13.000000 wtforms-widgets-1.0.7/wtforms_widgets/fields/core.py
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)     5895 2021-03-07 14:47:32.000000 wtforms-widgets-1.0.7/wtforms_widgets/fields/custom.py
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)      250 2021-01-07 15:37:13.000000 wtforms-widgets-1.0.7/wtforms_widgets/fields/filters.py
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)     1151 2021-03-07 14:47:32.000000 wtforms-widgets-1.0.7/wtforms_widgets/fields/validators.py
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)    10273 2021-01-07 15:37:13.000000 wtforms-widgets-1.0.7/wtforms_widgets/widgets.py
-drwxr-xr-x   0 ibot3     (1000) ibot3     (1000)        0 2021-03-07 14:58:30.433351 wtforms-widgets-1.0.7/wtforms_widgets.egg-info/
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)      759 2021-03-07 14:58:30.000000 wtforms-widgets-1.0.7/wtforms_widgets.egg-info/PKG-INFO
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)      504 2021-03-07 14:58:30.000000 wtforms-widgets-1.0.7/wtforms_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)        1 2021-03-07 14:58:30.000000 wtforms-widgets-1.0.7/wtforms_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)        1 2021-01-07 16:49:37.000000 wtforms-widgets-1.0.7/wtforms_widgets.egg-info/not-zip-safe
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)       49 2021-03-07 14:58:30.000000 wtforms-widgets-1.0.7/wtforms_widgets.egg-info/requires.txt
--rw-r--r--   0 ibot3     (1000) ibot3     (1000)       16 2021-03-07 14:58:30.000000 wtforms-widgets-1.0.7/wtforms_widgets.egg-info/top_level.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/.git
+-rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/distribute.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/wtforms_widgets/__init__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/wtforms_widgets/base_form.py
+-rw-r--r--   0        0        0    10237 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/wtforms_widgets/widgets.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/wtforms_widgets/fields/__init__.py
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/wtforms_widgets/fields/core.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/wtforms_widgets/fields/custom.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/wtforms_widgets/fields/filters.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/wtforms_widgets/fields/validators.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/README.md
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 wtforms_widgets-1.0.9/PKG-INFO
```

### Comparing `wtforms-widgets-1.0.7/wtforms_widgets/fields/core.py` & `wtforms_widgets-1.0.9/wtforms_widgets/fields/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,127 +1,126 @@
 import re
+import typing as t
 from datetime import datetime
 from itertools import chain
 
 import wtforms
-import wtforms.ext.sqlalchemy
-import wtforms.ext.sqlalchemy.fields
 
 from ..widgets import decorate_field, BootstrapFormControlDecorator, \
-    BootstrapStandardDecorator, BootstrapFormGroupDecorator, \
+    BootstrapStandardDecorator, \
     BootstrapRadioDecorator, BootstrapCheckboxDecorator, \
     BootstrapFieldListWidget, BootstrapFormFieldWidget, \
-    BootstrapDatepickerWidget, MoneyFieldDecorator, decorate
+    BootstrapDatepickerWidget, MoneyFieldDecorator, decorate, \
+    BootstrapFormSelectDecorator
 
 
 class SelectField(wtforms.fields.SelectField):
     widget = decorate_field(
         wtforms.fields.SelectField,
         BootstrapFormControlDecorator,
+        BootstrapFormSelectDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
 class SelectMultipleField(wtforms.fields.SelectMultipleField):
     widget = decorate_field(
         wtforms.fields.SelectMultipleField,
         BootstrapFormControlDecorator,
+        BootstrapFormSelectDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
 class RadioField(wtforms.fields.RadioField):
     widget = BootstrapFieldListWidget()
     option_widget = decorate(
         wtforms.widgets.RadioInput(),
         BootstrapRadioDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
 class StringField(wtforms.fields.StringField):
     widget = decorate_field(
         wtforms.fields.StringField,
         BootstrapFormControlDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
 class TextField(StringField):
     pass
 
 
 class IntegerField(wtforms.fields.IntegerField):
     widget = decorate_field(
         wtforms.fields.IntegerField,
         BootstrapFormControlDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
 class DecimalField(wtforms.fields.DecimalField):
     widget = decorate_field(
         wtforms.fields.DecimalField,
         BootstrapFormControlDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
 class MoneyField(wtforms.fields.DecimalField):
     widget = decorate_field(
         wtforms.fields.DecimalField,
         MoneyFieldDecorator,
         BootstrapFormControlDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
     def process_formdata(self, valuelist):
         if valuelist:
             valuelist[0] = valuelist[0].replace(",", ".")
         return super(MoneyField, self).process_formdata(valuelist)
 
 
 class FloatField(wtforms.fields.FloatField):
     widget = decorate_field(
         wtforms.fields.FloatField,
         BootstrapFormControlDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
 class BooleanField(wtforms.fields.BooleanField):
     widget = decorate_field(
         wtforms.fields.BooleanField,
         BootstrapCheckboxDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
 class DateTimeField(wtforms.fields.DateTimeField):
     widget = decorate(
         BootstrapDatepickerWidget(),
         BootstrapFormControlDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
+    )
+
+
+class TimeField(wtforms.fields.TimeField):
+    widget = decorate_field(
+        wtforms.fields.TimeField,
+        BootstrapFormControlDecorator,
+        BootstrapStandardDecorator,
     )
 
 
 class DateField(wtforms.fields.DateField):
     widget = decorate(
         BootstrapDatepickerWidget(),
         BootstrapFormControlDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
     supported_directives = {
         'd': 'dd',
         'm': 'mm',
         'a': 'D',
         'A': 'DD',
         'b': 'M',
@@ -187,66 +186,74 @@
 
 
 class TextAreaField(wtforms.fields.TextAreaField):
     widget = decorate_field(
         wtforms.fields.TextAreaField,
         BootstrapFormControlDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
 class PasswordField(wtforms.fields.PasswordField):
     widget = decorate_field(
         wtforms.fields.PasswordField,
         BootstrapFormControlDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
 class FileField(wtforms.fields.FileField):
     widget = decorate_field(
         wtforms.fields.FileField,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
 # No need to decorate wtforms.fields.HiddenField
 HiddenField = wtforms.fields.HiddenField
 
 
 class SubmitField(wtforms.fields.SubmitField):
     widget = decorate_field(
         wtforms.fields.SubmitField,
-        BootstrapFormGroupDecorator
-    )
-
-
-class QuerySelectField(
-    wtforms.ext.sqlalchemy.fields.QuerySelectField
-):
-    widget = decorate_field(
-        wtforms.ext.sqlalchemy.fields.QuerySelectField,
-        BootstrapFormControlDecorator,
-        BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
 
-class QuerySelectMultipleField(
-    wtforms.ext.sqlalchemy.fields.QuerySelectMultipleField
-):
-    widget = decorate_field(
-        wtforms.ext.sqlalchemy.fields.QuerySelectMultipleField,
-        BootstrapFormControlDecorator,
-        BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
-    )
+try:
+    import wtforms_sqlalchemy.fields
+except ImportError:
+    def __getattr__(name: str) -> t.Any:
+        if name in ("QuerySelectField", "QuerySelectmultipleField"):
+            raise AttributeError(
+                f"To use the {name!r}, install `wtforms_sqalalchemy`"
+                " via the `[sql]` optional dependency group"
+                " (`pip install wtforms-widgets[sql]`)"
+            )
+        raise AttributeError(f"module {__name__!r} has on attribute {name!r}!")
+else:
+    class QuerySelectField(
+        wtforms_sqlalchemy.fields.QuerySelectField
+    ):
+        widget = decorate_field(
+            wtforms_sqlalchemy.fields.QuerySelectField,
+            BootstrapFormControlDecorator,
+            BootstrapFormSelectDecorator,
+            BootstrapStandardDecorator,
+        )
+
+
+    class QuerySelectMultipleField(
+        wtforms_sqlalchemy.fields.QuerySelectMultipleField
+    ):
+        widget = decorate_field(
+            wtforms_sqlalchemy.fields.QuerySelectMultipleField,
+            BootstrapFormControlDecorator,
+            BootstrapFormSelectDecorator,
+            BootstrapStandardDecorator,
+        )
 
 
 class FieldList(wtforms.fields.FieldList):
     widget = BootstrapFieldListWidget()
 
 
 class FormField(wtforms.fields.FormField):
```

### Comparing `wtforms-widgets-1.0.7/wtforms_widgets/fields/custom.py` & `wtforms_widgets-1.0.9/wtforms_widgets/fields/custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from wtforms import fields
 from wtforms.validators import ValidationError
 
 from . import core
 from ..widgets import LazyLoadSelectWidget, \
     BootstrapFormControlDecorator, BootstrapStandardDecorator, \
-    BootstrapFormGroupDecorator, decorate, BootstrapStaticFieldWidget, \
-    decorators, decorate_field, Disabler, MacFieldDecorator
+    decorate, BootstrapStaticFieldWidget, \
+    decorators, decorate_field, Disabler, MacFieldDecorator, \
+    BootstrapFormSelectDecorator
 
 
 def static(field):
     widget = field.kwargs.get("widget", field.field_class.widget)
     field.kwargs["widget"] = decorate(
         BootstrapStaticFieldWidget(),
         *reversed(list(decorators(widget)))
@@ -75,16 +76,16 @@
     :param conditions: The names of the fields this one depends on as a List.
     :param data_endpoint: The name of the endpoint that provides the data.
     """
 
     widget = decorate(
         LazyLoadSelectWidget(),
         BootstrapFormControlDecorator,
+        BootstrapFormSelectDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
     def __init__(self, *args, **kwargs):
         self.conditions = kwargs.pop("conditions")
         self.data_endpoint = kwargs.pop("data_endpoint")
 
         super(LazyLoadSelectField, self).__init__(*args, **kwargs)
@@ -159,18 +160,19 @@
     """A MacField """
 
     widget = decorate_field(
         fields.StringField,
         MacFieldDecorator,
         BootstrapFormControlDecorator,
         BootstrapStandardDecorator,
-        BootstrapFormGroupDecorator
     )
 
     def __init__(self, *args, **kwargs):
+        kwargs.setdefault('render_kw', {})
+        kwargs['render_kw'].setdefault('placeholder', '00:de:ad:be:ef:00')
         super(MacField, self).__init__(*args, **kwargs)
 
     def __call__(self, **kwargs):
         return super(MacField, self).__call__(
             data_role='mac-address-input',
             **kwargs
         )
```

### Comparing `wtforms-widgets-1.0.7/wtforms_widgets/fields/validators.py` & `wtforms_widgets-1.0.9/wtforms_widgets/fields/validators.py`

 * *Files identical despite different names*

### Comparing `wtforms-widgets-1.0.7/wtforms_widgets/widgets.py` & `wtforms_widgets-1.0.9/wtforms_widgets/widgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,28 @@
 from functools import reduce
 from itertools import chain
 
 import wtforms.fields
 from flask import url_for
-from markupsafe import escape
-from wtforms.widgets.core import html_params, HTMLString
+from markupsafe import escape, Markup as HTMLString
+from wtforms.widgets.core import html_params
 
 
 class WidgetDecorator(object):
     """Decorate widgets."""
 
     def __init__(self, widget):
         """
         :param widget: Original widget to be decorated.
         """
         if widget is None:
             raise ValueError('Parameter widget may not be None.')
         self.widget = widget
 
 
-class BootstrapFormGroupDecorator(WidgetDecorator):
-    """
-    Wraps a widget inside a Bootstrap form-group and prints errors.
-
-    The widget's output is wrapped in a Bootstrap form-group. Any field errors
-    are displayed in Bootstrap help-blocks after the widget.
-    """
-
-    def __call__(self, field, **kwargs):
-        classes = [u'form-group']
-        if field.errors:
-            classes.append(u'text-danger')
-        return HTMLString(u''.join([
-            Markup(u'<div class="{0}" id="form-group-' + field.name + '">')
-                .format(u' '.join(classes)),
-            self.widget(field, **kwargs),
-            u'</div>']))
-
-
 class BootstrapFormControlDecorator(WidgetDecorator):
     """Adds the Bootstrap form-control class to a widget."""
 
     def __call__(self, field, **kwargs):
         if 'class_' in kwargs:
             kwargs['class_'] = u'form-control ' + kwargs['class_']
         else:
@@ -58,28 +39,37 @@
     Renders a field in horizontal layout.
 
     Horizontal layout is a two column layout, where the label is placed in the
     left column and the field is placed right next to it.
     """
 
     def render_horizontal(self, field, **kwargs):
-        html = ['<div class="row">',
+        error_html = [
+            Markup('<div class="invalid-feedback">{0}</div>').format(e)
+            for e in field.errors
+        ]
+        desc_html = []
+        if field.description:
+            desc_html.append(
+                Markup('<div class="col-sm-12"><span class="form-text">{0}</span></div>')
+                    .format(field.description)
+            )
+        label_classes = ['col-form-label']
+        if field.errors:
+            label_classes.append('text-danger')
+        html = [f'<div class="row" id="form-group-{field.name}">',
                 '<div class="col-sm-4">',
-                field.label(class_=u'col-form-label'),
+                field.label(class_=' '.join(label_classes)),
+                *desc_html,
                 '</div>',
                 '<div class="col-sm-4">',
                 self.widget(field, **kwargs),
+                *error_html,
                 '</div>',
                 '</div>']
-        help_block = Markup(u'<div class="col-sm-12">'
-                            u'<span class="form-text">{0}</span>'
-                            u'</div>')
-        if field.description:
-            html.append(help_block.format(field.description))
-        html.extend(help_block.format(e) for e in field.errors)
         return HTMLString(u''.join(html))
 
     def render_inline(self, field, **kwargs):
         return HTMLString(u''.join([
             field.label(class_=u'sr-only'),
             self.widget(field, placeholder=field.label.text, **kwargs),
         ]))
@@ -112,54 +102,50 @@
 
     Horizontal layout is a two column layout, where the label is placed in the
     left column and the field is placed right next to it.
     """
     wrapper_class = None
 
     def _render(self, field, **kwargs):
+
+        # we need:
+        input_classes = kwargs.get('class_', '').split()
+        kwargs['class_'] = ' '.join(input_classes + ['form-check-input'])
         return HTMLString(u''.join([
-            # TODO fix that: we now have the following schema
-            # https://getbootstrap.com/docs/4.0/components/forms/#horizontal-form
-            u'<div class="',
-            self.wrapper_class,
-            u'">',
-            field.label(
-                u"{0} {1}".format(
-                    self.widget(field, **kwargs),
-                    escape(field.label.text)
-                )),
+            u'<div class="form-check">',
+            self.widget(field, **kwargs),
+            field.label(escape(field.label.text), class_='form-check-label'),
             u'</div>',
         ]))
 
     def render_basic(self, field, **kwargs):
         return self._render(field, **kwargs)
 
     def render_horizontal(self, field, **kwargs):
         return HTMLString(u''.join([
-            u'<div class="offset-sm-4 col-sm-4">',
+            f'<div class="row" id="form-group-{field.name}"><div class="offset-sm-4 col-sm-4">',
             self._render(field, **kwargs),
-            u'</div>',
+            u'</div></div>',
         ]))
 
     def render_inline(self, field, **kwargs):
         return field.label(u"{0} {1}".format(
             self.widget(field, **kwargs),
             escape(field.label.text)
         ), class_=self.wrapper_class + "-inline")
 
     def __call__(self, field, **kwargs):
         render_mode = kwargs.pop("render_mode", "horizontal")
         if render_mode == "basic":
             return self.render_basic(field, **kwargs)
-        elif render_mode == "horizontal":
+        if render_mode == "horizontal":
             return self.render_horizontal(field, **kwargs)
-        elif render_mode == "inline":
+        if render_mode == "inline":
             return self.render_inline(field, **kwargs)
-        else:
-            raise ValueError("Unknown render mode: {0}".format(render_mode))
+        raise ValueError(f"Unknown render mode: {render_mode}")
 
 
 class BootstrapRadioDecorator(BootstrapRadioCheckboxDecorator):
     wrapper_class = u"radio"
 
 
 class BootstrapCheckboxDecorator(BootstrapRadioCheckboxDecorator):
@@ -261,14 +247,21 @@
                 options['checked'] = 'checked'
             html.append(u'<input {}>'.format(html_params(**options)))
             html.append(label)
             html.append(u'</label>')
         return u''.join(html)
 
 
+class BootstrapFormSelectDecorator(WidgetDecorator):
+    def __call__(self, field, **kwargs):
+        classes = kwargs.get('class_', '').split()
+        kwargs['class_'] = ' '.join(classes + ['form-select'])
+        return self.widget(field, **kwargs)
+
+
 class LazyLoadSelectWidget(wtforms.widgets.Select):
     """This is the widget for the LazyLoadSelectField
 
     Please look at web.form.fields.LazyLoadSelectField for more information.
     """
 
     def __call__(self, field, **kwargs):
@@ -289,17 +282,21 @@
 
 
 class MoneyFieldDecorator(WidgetDecorator):
     """Adds the Bootstrap form-control class to a widget."""
 
     def __call__(self, field, **kwargs):
         kwargs['class_'] += ' money-amount'
-        return ('<div class="input-group">' + self.widget(field, **kwargs) +
-                '<span class="input-group-append input-group-text">€</span></div>')
+        group_cls = 'input-group' + (' is-invalid' if field.errors else '')
+        return Markup(
+            '<div class="{}">{}<span class="input-group-text">€</span></div>'
+        ).format(group_cls, self.widget(field, **kwargs))
 
 
 class MacFieldDecorator(WidgetDecorator):
     """Adds an addon which shows the vendor."""
 
     def __call__(self, field, **kwargs):
-        return ('<div class="input-group">' + self.widget(field, **kwargs) +
-                '<div class="input-group-append input-group-text mac-manufacturer">?</div></div>')
+        group_cls = 'input-group' + (' is-invalid' if field.errors else '')
+        return Markup(
+            '<div class="{}">{}<div class="input-group-text mac-manufacturer">?</div></div>'
+        ).format(group_cls, self.widget(field, **kwargs))
```

