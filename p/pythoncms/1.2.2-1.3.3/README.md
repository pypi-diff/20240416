# Comparing `tmp/pythoncms-1.2.2.tar.gz` & `tmp/pythoncms-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncms-1.2.2.tar", last modified: Sun Feb  5 19:40:28 2023, max compression
+gzip compressed data, was "pythoncms-1.3.3.tar", last modified: Tue Apr 16 10:53:51 2024, max compression
```

## Comparing `pythoncms-1.2.2.tar` & `pythoncms-1.3.3.tar`

### file list

```diff
@@ -1,527 +1,541 @@
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.451896 pythoncms-1.2.2/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      296 2023-02-05 19:07:54.000000 pythoncms-1.2.2/MANIFEST.in
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2681 2023-02-05 19:40:28.451896 pythoncms-1.2.2/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1954 2023-02-05 19:39:54.000000 pythoncms-1.2.2/README.md
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      186 2023-01-31 20:11:30.000000 pythoncms-1.2.2/dev_requirements.txt
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.287897 pythoncms-1.2.2/pythoncms/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      199 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/.test.prod.env
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     6270 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/CHANGELOG.md
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       80 2023-02-05 19:40:23.000000 pythoncms-1.2.2/pythoncms/__init__.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.291897 pythoncms-1.2.2/pythoncms/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      332 2023-02-05 19:40:27.000000 pythoncms-1.2.2/pythoncms/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     6165 2023-02-04 07:47:13.000000 pythoncms-1.2.2/pythoncms/__pycache__/app.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1572 2023-02-05 19:10:31.000000 pythoncms-1.2.2/pythoncms/__pycache__/cli.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2574 2023-02-04 07:47:13.000000 pythoncms-1.2.2/pythoncms/__pycache__/config.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      962 2023-02-04 07:47:13.000000 pythoncms-1.2.2/pythoncms/__pycache__/init.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1963 2023-02-04 07:47:15.000000 pythoncms-1.2.2/pythoncms/__pycache__/shopyo_admin.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     9091 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/app.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      482 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/autoapp.py.example
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1638 2023-02-05 19:10:25.000000 pythoncms-1.2.2/pythoncms/cli.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      278 2023-02-03 06:49:29.000000 pythoncms-1.2.2/pythoncms/config.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3000 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/config.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      278 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/config_demo.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     7242 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/conftest.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      987 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/init.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      275 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/manage.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.291897 pythoncms-1.2.2/pythoncms/modules/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/__init__.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.291897 pythoncms-1.2.2/pythoncms/modules/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      150 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.291897 pythoncms-1.2.2/pythoncms/modules/box__default/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.291897 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/__init__.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.291897 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      172 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      939 2023-02-05 12:30:24.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/__pycache__/admin.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     5486 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/__pycache__/view.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      601 2023-02-05 12:26:49.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/admin.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      394 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/models.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.295897 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/static/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      429 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/static/icon.svg
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.267897 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.295897 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/appadmin/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2777 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/appadmin/add.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.295897 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/appadmin/blocks/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      268 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/appadmin/blocks/sidebar.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3045 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/appadmin/edit.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2546 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/appadmin/index.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1812 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/appadmin/roles.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.295897 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/tests/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    15217 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/tests/test_admin.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/tests/test_models.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     6167 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/view.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.295897 pythoncms-1.2.2/pythoncms/modules/box__default/auth/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.295897 pythoncms-1.2.2/pythoncms/modules/box__default/auth/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      700 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/__pycache__/decorators.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2148 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/__pycache__/forms.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4475 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4054 2023-02-05 12:30:24.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/__pycache__/view.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      379 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/decorators.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1990 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/forms.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      158 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3997 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/models.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.299897 pythoncms-1.2.2/pythoncms/modules/box__default/auth/static/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      126 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/static/style.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.267897 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.299897 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.299897 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/blocks/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1024 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/blocks/login_form.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1483 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/blocks/register_form.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.299897 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/emails/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      468 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/emails/activate_user.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      249 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/emails/activate_user.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    11666 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/login.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      928 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/register.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      443 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/shop_login.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      750 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/unconfirmed.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.299897 pythoncms-1.2.2/pythoncms/modules/box__default/auth/tests/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      994 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/tests/conftest.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1116 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/tests/factories.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       28 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/tests/test_auth_forms.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    10645 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/tests/test_auth_functional.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     8924 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/tests/test_auth_models.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      563 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/upload.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4808 2023-02-05 12:26:49.000000 pythoncms-1.2.2/pythoncms/modules/box__default/auth/view.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.303897 pythoncms-1.2.2/pythoncms/modules/box__default/base/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.303897 pythoncms-1.2.2/pythoncms/modules/box__default/base/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      490 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/base/__pycache__/view.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      172 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/base/info.json
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.267897 pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.303897 pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.303897 pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/blocks/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       34 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/blocks/default_styles.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      219 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/blocks/flashed_messages.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      376 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/blocks/footer.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      218 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/blocks/macros.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1030 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/blocks/resources.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      399 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/main_base.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2611 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/module_base.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1337 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/nav_base.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      759 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/base/view.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      176 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/box_info.json
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.307897 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.307897 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      279 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/__pycache__/global.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1244 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/__pycache__/helpers.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1002 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/__pycache__/view.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      132 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/global.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2032 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/helpers.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      207 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/info.json
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.271897 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/templates/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.307897 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/templates/dashboard/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1102 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/templates/dashboard/index.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/templates/dashboard/nav.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.307897 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/tests/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1503 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/tests/test_dashboard.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      747 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/view.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.307897 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.307897 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      351 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/__pycache__/global.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      785 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/__pycache__/helpers.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      550 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1050 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/__pycache__/view.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/forms.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      541 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/global.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      274 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/helpers.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      255 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      231 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/models.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.271897 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/templates/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.307897 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/templates/i18n/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.311897 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/templates/i18n/blocks/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/templates/i18n/blocks/sidebar.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      366 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/templates/i18n/dashboard.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.311897 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/tests/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       49 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/tests/test_i18n_functional.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       45 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/tests/test_i18n_models.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1298 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/i18n/view.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.311897 pythoncms-1.2.2/pythoncms/modules/box__default/page/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.311897 pythoncms-1.2.2/pythoncms/modules/box__default/page/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1109 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/__pycache__/forms.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      238 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/__pycache__/global.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      382 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/__pycache__/helpers.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2503 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3265 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/__pycache__/view.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      952 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/forms.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       73 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/global.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      105 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/helpers.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      549 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2245 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/models.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.271897 pythoncms-1.2.2/pythoncms/modules/box__default/page/templates/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.315897 pythoncms-1.2.2/pythoncms/modules/box__default/page/templates/page/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      564 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/templates/page/all_pages.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.315897 pythoncms-1.2.2/pythoncms/modules/box__default/page/templates/page/blocks/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      160 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/templates/page/blocks/sidebar.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3481 2023-02-05 12:26:49.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/templates/page/dashboard.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-02-04 07:33:35.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/templates/page/dashboard_edit.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4391 2023-02-05 12:26:49.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/templates/page/view_page_dashboard.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3683 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/page/view.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.315897 pythoncms-1.2.2/pythoncms/modules/box__default/settings/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/__init__.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.319897 pythoncms-1.2.2/pythoncms/modules/box__default/settings/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      172 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      244 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/__pycache__/global.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      747 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/__pycache__/helpers.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1056 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      168 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/__pycache__/view.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       76 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/global.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      461 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/helpers.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      198 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      438 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/models.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.271897 pythoncms-1.2.2/pythoncms/modules/box__default/settings/templates/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.319897 pythoncms-1.2.2/pythoncms/modules/box__default/settings/templates/settings/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      823 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/templates/settings/edit.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      777 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/templates/settings/index.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      121 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/templates/settings/nav.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      642 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/upload.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/settings/view.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.319897 pythoncms-1.2.2/pythoncms/modules/box__default/theme/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.323897 pythoncms-1.2.2/pythoncms/modules/box__default/theme/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      456 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/theme/__pycache__/global.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1978 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/theme/__pycache__/helpers.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2329 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/box__default/theme/__pycache__/view.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/theme/forms.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      445 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/theme/global.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1509 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/theme/helpers.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      335 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/theme/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/theme/models.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.271897 pythoncms-1.2.2/pythoncms/modules/box__default/theme/templates/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.323897 pythoncms-1.2.2/pythoncms/modules/box__default/theme/templates/theme/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.323897 pythoncms-1.2.2/pythoncms/modules/box__default/theme/templates/theme/blocks/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      118 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/theme/templates/theme/blocks/sidebar.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3263 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/box__default/theme/templates/theme/index.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3239 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/box__default/theme/view.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.323897 pythoncms-1.2.2/pythoncms/modules/contact/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.323897 pythoncms-1.2.2/pythoncms/modules/contact/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      776 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/contact/__pycache__/forms.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      354 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/contact/__pycache__/global.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1086 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/contact/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1875 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/contact/__pycache__/view.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      736 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/contact/forms.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      149 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/contact/global.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      333 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/contact/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      561 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/contact/models.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.275897 pythoncms-1.2.2/pythoncms/modules/contact/templates/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.327896 pythoncms-1.2.2/pythoncms/modules/contact/templates/contact/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.327896 pythoncms-1.2.2/pythoncms/modules/contact/templates/contact/blocks/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      172 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/contact/templates/contact/blocks/sidebar.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1564 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/contact/templates/contact/contact_form.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2477 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/contact/templates/contact/dashboard.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.327896 pythoncms-1.2.2/pythoncms/modules/contact/tests/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3637 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/contact/tests/test_contact.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1754 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/contact/view.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.327896 pythoncms-1.2.2/pythoncms/modules/resource/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.327896 pythoncms-1.2.2/pythoncms/modules/resource/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1346 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/resource/__pycache__/view.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/resource/forms.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      262 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/resource/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1855 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/resource/models.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.275897 pythoncms-1.2.2/pythoncms/modules/resource/templates/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.275897 pythoncms-1.2.2/pythoncms/modules/resource/templates/resource/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.327896 pythoncms-1.2.2/pythoncms/modules/resource/templates/resource/blocks/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/resource/templates/resource/blocks/sidebar.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4345 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/resource/view.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.327896 pythoncms-1.2.2/pythoncms/modules/www/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.327896 pythoncms-1.2.2/pythoncms/modules/www/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      279 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/www/__pycache__/global.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      921 2023-02-04 07:47:16.000000 pythoncms-1.2.2/pythoncms/modules/www/__pycache__/view.cpython-310.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/www/forms.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      191 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/www/global.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      324 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/modules/www/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/www/models.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.275897 pythoncms-1.2.2/pythoncms/modules/www/templates/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.331896 pythoncms-1.2.2/pythoncms/modules/www/templates/www/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.331896 pythoncms-1.2.2/pythoncms/modules/www/templates/www/blocks/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/www/templates/www/blocks/sidebar.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      550 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/www/templates/www/index.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1414 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/modules/www/view.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1379 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/shopyo_admin.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.335896 pythoncms-1.2.2/pythoncms/static/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    34244 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/static/bootstrap-grid.min.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3937 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/static/bootstrap-reboot.min.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    78636 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/static/bootstrap.bundle.min.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   144878 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/static/bootstrap.min.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4291 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/static/box.svg
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.335896 pythoncms-1.2.2/pythoncms/static/css/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     5330 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/static/css/b4vtabs.min.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      964 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/static/css/simple_sidebar.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.339896 pythoncms-1.2.2/pythoncms/static/default/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   213806 2023-01-31 20:11:30.000000 pythoncms-1.2.2/pythoncms/static/default/default_product.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)  3753798 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/default/default_subcategory.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    15406 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/favicon.ico
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.347896 pythoncms-1.2.2/pythoncms/static/fontawesome/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1548 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/LICENSE.txt
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.355896 pythoncms-1.2.2/pythoncms/static/fontawesome/css/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    68243 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/all.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    54457 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/all.min.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      528 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/brands.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      476 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/brands.min.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    66628 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/fontawesome.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    53030 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/fontawesome.min.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      547 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/regular.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      491 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/regular.min.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      540 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/solid.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      483 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/solid.min.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     7270 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/svg-with-js.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4689 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/svg-with-js.min.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    41032 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/v4-shims.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    26441 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/css/v4-shims.min.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.367896 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   125320 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-brands-400.eot
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   659641 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-brands-400.svg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   125016 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-brands-400.ttf
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    84568 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-brands-400.woff
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    72148 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-brands-400.woff2
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    34388 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-regular-400.eot
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   144371 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-regular-400.svg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    34092 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-regular-400.ttf
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    16812 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-regular-400.woff
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    13608 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-regular-400.woff2
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   186512 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-solid-900.eot
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   815282 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-solid-900.svg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   186228 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-solid-900.ttf
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    96248 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-solid-900.woff
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    74320 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-solid-900.woff2
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    86659 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/jquery_3.2.1.min.js
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.371896 pythoncms-1.2.2/pythoncms/static/js/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1237 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/js/python.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    14499 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/logo.png
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    11020 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/logo.svg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     8789 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/shopyo.png
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    11538 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/shopyo.svg
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.279897 pythoncms-1.2.2/pythoncms/static/themes/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.275897 pythoncms-1.2.2/pythoncms/static/themes/back/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.371896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.279897 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.371896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/css/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2650 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/css/demo.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.375896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      741 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/config.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    15694 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/dashboards-analytics.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1118 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/extended-ui-perfect-scrollbar.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      199 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/form-basic-inputs.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3964 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/main.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      881 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/pages-account-settings-account.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1101 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/ui-modals.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      456 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/ui-popover.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1344 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/ui-toasts.js
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.279897 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.379896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   981701 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/core.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.379896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      531 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-account-settings.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    36140 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-auth.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1518 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-icons.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      769 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-misc.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    71012 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/theme-default.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.383896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.391896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   292572 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.eot
--rw-rw-r--   0 appinv    (1000) appinv    (1000)  1125138 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.svg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   292404 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.ttf
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   292480 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.woff
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   102988 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.woff2
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    79999 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.395896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/js/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   842421 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/js/bootstrap.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   105344 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/js/helpers.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    81752 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/js/menu.js
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.279897 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.395896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/apex-charts/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    17622 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/apex-charts/apex-charts.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)  1251190 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/apex-charts/apexcharts.js
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.403896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       61 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/highlight-github.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1268 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/highlight.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)  2964866 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/highlight.js
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.411896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/jquery/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   832987 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/jquery/jquery.js
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.411896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/masonry/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   178166 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/masonry/masonry.js
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.411896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/perfect-scrollbar/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     5008 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/perfect-scrollbar/perfect-scrollbar.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)   108756 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/perfect-scrollbar/perfect-scrollbar.js
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.415896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/popper/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    57765 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/popper/popper.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3473 2023-02-05 12:26:49.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/authbase.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    14071 2023-02-05 12:26:49.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/base.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       64 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/index.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       55 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2349 2023-02-05 12:26:49.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/login.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2205 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/register.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.415896 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/sections/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    23793 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/sections/dashboard_elements.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1233 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/sections/resource_end_body.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1235 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/sections/resource_head.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1418 2023-02-04 07:38:05.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/styles.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      705 2023-02-05 12:26:49.000000 pythoncms-1.2.2/pythoncms/static/themes/back/sneat/unconfirmed.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.279897 pythoncms-1.2.2/pythoncms/static/themes/front/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.419896 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    17128 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/LICENSE.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      821 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/README.txt
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.279897 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.419896 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/css/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    59402 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/css/fontawesome-all.min.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    61737 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/css/main.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.419896 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/js/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2439 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/js/breakpoints.min.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2051 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/js/browser.min.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    89501 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/js/jquery.min.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     5969 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/js/main.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    12434 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/js/util.js
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.419896 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.419896 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/base/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1025 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/base/_page.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1570 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/base/_reset.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3123 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/base/_typography.scss
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.423896 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1092 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_actions.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      516 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_box.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1758 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_button.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      761 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_contact.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2920 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_features.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3925 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_form.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      483 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_icon.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      425 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_icons.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1108 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_image.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      893 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_list.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      578 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_mini-posts.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1311 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_pagination.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3087 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_posts.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      631 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_row.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      772 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_section.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1292 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_table.scss
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.423896 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1522 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_banner.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      297 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_footer.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      905 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_header.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      994 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_main.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1956 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_menu.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4410 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_sidebar.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      302 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_wrapper.scss
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.427896 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4578 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_breakpoints.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1958 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_functions.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2841 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_html-grid.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2219 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_mixins.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      836 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_vars.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     7356 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_vendor.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1618 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/main.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1363 2023-02-05 12:26:49.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/base.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1363 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/contact.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    25374 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/elements.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    10955 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/generic.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.427896 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    20660 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic01.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    20986 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic02.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    21127 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic03.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    21412 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic04.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    21497 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic05.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    21564 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic06.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    10854 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic07.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    10934 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic08.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    10350 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic09.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    70746 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic10.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    99292 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic11.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4258 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/index.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       55 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1151 2023-02-05 12:26:49.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/page.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       45 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/render_demo.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.431896 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/sections/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/sections/footer.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/sections/nav.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/sections/resources.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4142 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/sections/sidebar.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      727 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/editorial/styles.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.431896 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    17128 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/LICENSE.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1129 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/README.txt
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.283897 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.435896 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/css/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    59402 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/css/fontawesome-all.min.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.435896 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/css/images/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      863 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/css/images/intro.svg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    69467 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/css/main.css
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      900 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/css/noscript.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.439896 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2439 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/breakpoints.min.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2051 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/browser.min.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    89501 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/jquery.min.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2258 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/jquery.scrollex.min.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      832 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/jquery.scrolly.min.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4062 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/main.js
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    12434 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/util.js
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.439896 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.439896 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/base/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      989 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/base/_page.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1571 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/base/_reset.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3437 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/base/_typography.scss
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.443896 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1790 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_actions.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      533 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_box.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2085 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_button.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      313 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_contact.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2002 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_features.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     5209 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_form.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1211 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_icon.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      424 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_icons.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      887 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_image.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      910 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_list.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      610 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_menu.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      632 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_row.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      745 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_section.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1491 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_split.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2471 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_spotlights.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1399 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_table.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2410 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_wrapper.scss
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.443896 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/layout/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      619 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_footer.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1593 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_header.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      628 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_intro.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3772 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_sidebar.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      523 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_wrapper.scss
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.447896 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4578 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_breakpoints.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1958 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_functions.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2841 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_html-grid.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2219 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_mixins.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1041 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_vars.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     7356 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_vendor.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1368 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/main.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      917 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/noscript.scss
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1730 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/base.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1590 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/contact.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    16635 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/elements.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1538 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/generic.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.447896 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     6953 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic01.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     5767 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic02.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     6828 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic03.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    12171 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic04.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2527 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic05.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2798 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic06.jpg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     5976 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/index.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       55 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/info.json
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      278 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/page.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       45 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/render_demo.html
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.447896 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/sections/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/sections/footer.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/sections/nav.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/sections/resources.html
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      727 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/styles.css
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.447896 pythoncms-1.2.2/pythoncms/tests/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      545 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/tests/conftest.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2122 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/tests/test_configs.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      707 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/tests/test_dunder_main.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      200 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/tests/test_manage.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1133 2023-01-31 20:11:31.000000 pythoncms-1.2.2/pythoncms/wsgi.py.example
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-02-05 19:40:28.287897 pythoncms-1.2.2/pythoncms.egg-info/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2681 2023-02-05 19:40:28.000000 pythoncms-1.2.2/pythoncms.egg-info/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    23431 2023-02-05 19:40:28.000000 pythoncms-1.2.2/pythoncms.egg-info/SOURCES.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        1 2023-02-05 19:40:28.000000 pythoncms-1.2.2/pythoncms.egg-info/dependency_links.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       48 2023-02-05 19:40:28.000000 pythoncms-1.2.2/pythoncms.egg-info/entry_points.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       33 2023-02-05 19:40:28.000000 pythoncms-1.2.2/pythoncms.egg-info/requires.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       10 2023-02-05 19:40:28.000000 pythoncms-1.2.2/pythoncms.egg-info/top_level.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       33 2023-01-31 20:11:31.000000 pythoncms-1.2.2/requirements.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       38 2023-02-05 19:40:28.451896 pythoncms-1.2.2/setup.cfg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3136 2023-02-04 07:44:14.000000 pythoncms-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.980569 pythoncms-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-16 10:53:47.000000 pythoncms-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-16 10:53:51.980569 pythoncms-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-16 10:53:47.000000 pythoncms-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-16 10:53:47.000000 pythoncms-1.3.3/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.892568 pythoncms-1.3.3/pythoncms/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/.env_demo
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/.test.prod.env
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.892568 pythoncms-1.3.3/pythoncms/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-16 10:53:51.000000 pythoncms-1.3.3/pythoncms/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/autoapp.py.example
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/config_demo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.892568 pythoncms-1.3.3/pythoncms/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.892568 pythoncms-1.3.3/pythoncms/modules/box__default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.892568 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.892568 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/static/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.880568 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.896568 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/appadmin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/appadmin/add.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.896568 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/appadmin/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/appadmin/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/appadmin/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/appadmin/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/appadmin/roles.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.896568 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.896568 pythoncms-1.3.3/pythoncms/modules/box__default/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.896568 pythoncms-1.3.3/pythoncms/modules/box__default/auth/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.880568 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.896568 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.896568 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/blocks/login_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/blocks/register_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.896568 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/emails/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/emails/activate_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/emails/activate_user.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/register.html
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/shop_login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/unconfirmed.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.900568 pythoncms-1.3.3/pythoncms/modules/box__default/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/tests/test_auth_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/tests/test_auth_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/tests/test_auth_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/auth/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.900568 pythoncms-1.3.3/pythoncms/modules/box__default/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/base/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/base/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.880568 pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.900568 pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.900568 pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/blocks/default_styles.html
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/blocks/flashed_messages.html
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/blocks/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/blocks/macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/blocks/resources.html
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/main_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/module_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/nav_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/base/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/box_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.900568 pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.880568 pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.900568 pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/templates/dashboard/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/templates/dashboard/nav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.900568 pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.900568 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.880568 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.900568 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/templates/i18n/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.904568 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/templates/i18n/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/templates/i18n/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/templates/i18n/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.904568 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/tests/test_i18n_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/tests/test_i18n_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/i18n/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.904568 pythoncms-1.3.3/pythoncms/modules/box__default/info/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/info/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/info/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/info/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/info/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/info/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.880568 pythoncms-1.3.3/pythoncms/modules/box__default/info/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.904568 pythoncms-1.3.3/pythoncms/modules/box__default/info/templates/info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/info/templates/info/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/info/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.904568 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.880568 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.904568 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/templates/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/templates/settings/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/templates/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/templates/settings/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.904568 pythoncms-1.3.3/pythoncms/modules/box__default/page/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/page/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/page/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/page/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/page/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/page/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.880568 pythoncms-1.3.3/pythoncms/modules/box__default/page/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.908568 pythoncms-1.3.3/pythoncms/modules/box__default/page/templates/page/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/page/templates/page/all_pages.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.908568 pythoncms-1.3.3/pythoncms/modules/box__default/page/templates/page/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/page/templates/page/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/page/templates/page/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/page/templates/page/dashboard_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/page/templates/page/view_page_dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/page/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.908568 pythoncms-1.3.3/pythoncms/modules/box__default/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/theme/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/theme/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/theme/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/theme/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/theme/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.880568 pythoncms-1.3.3/pythoncms/modules/box__default/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.908568 pythoncms-1.3.3/pythoncms/modules/box__default/theme/templates/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.908568 pythoncms-1.3.3/pythoncms/modules/box__default/theme/templates/theme/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/theme/templates/theme/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/theme/templates/theme/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/box__default/theme/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.908568 pythoncms-1.3.3/pythoncms/modules/contact/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/contact/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/contact/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/contact/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/contact/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.880568 pythoncms-1.3.3/pythoncms/modules/contact/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.908568 pythoncms-1.3.3/pythoncms/modules/contact/templates/contact/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.908568 pythoncms-1.3.3/pythoncms/modules/contact/templates/contact/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/contact/templates/contact/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/contact/templates/contact/contact_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/contact/templates/contact/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.908568 pythoncms-1.3.3/pythoncms/modules/contact/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/contact/tests/test_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/contact/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.908568 pythoncms-1.3.3/pythoncms/modules/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/resource/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/resource/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/resource/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.884568 pythoncms-1.3.3/pythoncms/modules/resource/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.884568 pythoncms-1.3.3/pythoncms/modules/resource/templates/resource/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.908568 pythoncms-1.3.3/pythoncms/modules/resource/templates/resource/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/resource/templates/resource/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/resource/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.912568 pythoncms-1.3.3/pythoncms/modules/www/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/www/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/www/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/www/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/www/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.884568 pythoncms-1.3.3/pythoncms/modules/www/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.912568 pythoncms-1.3.3/pythoncms/modules/www/templates/www/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.912568 pythoncms-1.3.3/pythoncms/modules/www/templates/www/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/www/templates/www/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/www/templates/www/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/modules/www/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/shopyo_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.912568 pythoncms-1.3.3/pythoncms/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    34244 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    78636 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   144878 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/box.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.912568 pythoncms-1.3.3/pythoncms/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/css/b4vtabs.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/css/simple_sidebar.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.912568 pythoncms-1.3.3/pythoncms/static/default/
+-rw-r--r--   0 runner    (1001) docker     (127)   213806 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/default/default_product.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  3753798 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/default/default_subcategory.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.920568 pythoncms-1.3.3/pythoncms/static/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.920568 pythoncms-1.3.3/pythoncms/static/fontawesome/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    68243 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/all.css
+-rw-r--r--   0 runner    (1001) docker     (127)    54457 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/brands.css
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/brands.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    66628 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/fontawesome.css
+-rw-r--r--   0 runner    (1001) docker     (127)    53030 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/regular.css
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/regular.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/solid.css
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/solid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/svg-with-js.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/svg-with-js.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    41032 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/v4-shims.css
+-rw-r--r--   0 runner    (1001) docker     (127)    26441 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/css/v4-shims.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.924568 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   125320 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   659641 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   125016 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    84568 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    72148 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34388 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144371 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   186512 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   815282 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   186228 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    96248 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    74320 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/jquery_3.2.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.928568 pythoncms-1.3.3/pythoncms/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/js/python.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/shopyo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/shopyo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.888568 pythoncms-1.3.3/pythoncms/static/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.884568 pythoncms-1.3.3/pythoncms/static/themes/back/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.928568 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/authbase.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.928568 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   211157 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/css/sb-admin-2.css
+-rw-r--r--   0 runner    (1001) docker     (127)   170737 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/css/sb-admin-2.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    42782 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.928568 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.928568 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/js/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/js/demo/chart-area-demo.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/js/demo/chart-bar-demo.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/js/demo/chart-pie-demo.js
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/js/demo/datatables-demo.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/js/sb-admin-2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/js/sb-admin-2.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/register.html
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/unconfirmed.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.884568 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.884568 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.932568 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   236864 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   409586 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    84378 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   316181 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   144033 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)   254480 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    63467 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   192479 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.936568 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/chart.js/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   593984 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/chart.js/Chart.bundle.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)   226496 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/chart.js/Chart.bundle.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)   443106 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/chart.js/Chart.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)   173077 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/chart.js/Chart.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.936568 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/datatables/
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/datatables/dataTables.bootstrap4.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/datatables/dataTables.bootstrap4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/datatables/dataTables.bootstrap4.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/datatables/dataTables.bootstrap4.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   450383 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/datatables/jquery.dataTables.js
+-rw-r--r--   0 runner    (1001) docker     (127)    83602 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/datatables/jquery.dataTables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.940568 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery/
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   137960 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.min.map
+-rw-r--r--   0 runner    (1001) docker     (127)   235341 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.slim.js
+-rw-r--r--   0 runner    (1001) docker     (127)    72372 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.slim.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   110315 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.slim.min.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.940568 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery-easing/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1656 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery-easing/jquery.easing.compatibility.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4047 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery-easing/jquery.easing.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2532 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery-easing/jquery.easing.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.940568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.884568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.940568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/css/demo.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.940568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15694 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/dashboards-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/extended-ui-perfect-scrollbar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/form-basic-inputs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/pages-account-settings-account.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/ui-modals.js
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/ui-popover.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/ui-toasts.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.884568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.944568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   981701 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/core.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.944568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-account-settings.css
+-rw-r--r--   0 runner    (1001) docker     (127)    36140 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-auth.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-misc.css
+-rw-r--r--   0 runner    (1001) docker     (127)    71012 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/theme-default.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.944568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.948568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/
+-rw-r--r--   0 runner    (1001) docker     (127)   292572 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)  1125138 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   292404 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   292480 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   102988 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    79999 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.948568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   842421 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)   105344 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/js/helpers.js
+-rw-r--r--   0 runner    (1001) docker     (127)    81752 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/js/menu.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.888568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.948568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/apex-charts/
+-rw-r--r--   0 runner    (1001) docker     (127)    17622 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/apex-charts/apex-charts.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1251190 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/apex-charts/apexcharts.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.952568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/highlight-github.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/highlight.css
+-rw-r--r--   0 runner    (1001) docker     (127)  2964866 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/highlight.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.956568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/jquery/
+-rw-r--r--   0 runner    (1001) docker     (127)   832987 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/jquery/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.956568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/masonry/
+-rw-r--r--   0 runner    (1001) docker     (127)   178166 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/masonry/masonry.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.956568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/perfect-scrollbar/
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/perfect-scrollbar/perfect-scrollbar.css
+-rw-r--r--   0 runner    (1001) docker     (127)   108756 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/perfect-scrollbar/perfect-scrollbar.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.956568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/popper/
+-rw-r--r--   0 runner    (1001) docker     (127)    57765 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/popper/popper.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/authbase.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14074 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/register.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.960568 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)    23793 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/sections/dashboard_elements.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/sections/resource_end_body.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/sections/resource_head.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/back/sneat/unconfirmed.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.888568 pythoncms-1.3.3/pythoncms/static/themes/front/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.960568 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.888568 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.960568 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    59402 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/css/fontawesome-all.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    61737 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.960568 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/js/breakpoints.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/js/browser.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/js/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.960568 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.964568 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/base/_page.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/base/_reset.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/base/_typography.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.964568 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_actions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_box.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_button.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_contact.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_features.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_form.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_icon.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_list.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_mini-posts.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_posts.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_row.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_section.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_table.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.968568 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_banner.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_main.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_menu.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_sidebar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_wrapper.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.968568 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_breakpoints.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_functions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_html-grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_vars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_vendor.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/main.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/contact.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/elements.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/generic.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.968568 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic01.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    20986 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic02.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    21127 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic03.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    21412 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic04.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    21497 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic05.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    21564 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic06.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic07.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic08.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic09.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    70746 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic10.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    99292 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic11.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/render_demo.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.972568 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/sections/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/sections/resources.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/sections/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/editorial/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.972568 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.888568 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.972568 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    59402 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/css/fontawesome-all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.972568 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/css/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/css/images/intro.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    69467 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/css/noscript.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.972568 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/breakpoints.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/browser.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/jquery.scrollex.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/jquery.scrolly.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.976569 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.976569 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/base/_page.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/base/_reset.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/base/_typography.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.976569 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_actions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_box.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_button.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_contact.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_features.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_form.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_icon.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_list.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_menu.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_row.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_section.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_split.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_spotlights.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_table.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_wrapper.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.976569 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_intro.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_sidebar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_wrapper.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.980569 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_breakpoints.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_functions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_html-grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_vars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_vendor.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/main.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/noscript.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/contact.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16635 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/elements.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/generic.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.980569 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic01.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic02.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic03.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic04.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic05.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic06.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/render_demo.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.980569 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/sections/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/sections/resources.html
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.980569 pythoncms-1.3.3/pythoncms/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/tests/test_dunder_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-16 10:53:47.000000 pythoncms-1.3.3/pythoncms/wsgi.py.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:53:51.980569 pythoncms-1.3.3/pythoncms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-16 10:53:51.000000 pythoncms-1.3.3/pythoncms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24077 2024-04-16 10:53:51.000000 pythoncms-1.3.3/pythoncms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:53:51.000000 pythoncms-1.3.3/pythoncms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 10:53:51.000000 pythoncms-1.3.3/pythoncms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 10:53:51.000000 pythoncms-1.3.3/pythoncms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 10:53:51.000000 pythoncms-1.3.3/pythoncms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 10:53:47.000000 pythoncms-1.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:53:51.980569 pythoncms-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-16 10:53:47.000000 pythoncms-1.3.3/setup.py
```

### Comparing `pythoncms-1.2.2/PKG-INFO` & `pythoncms-1.3.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: pythoncms
-Version: 1.2.2
+Version: 1.3.3
 Home-page: 
 Author: Abdur-Rahmaan Janhangeer
 Author-email: arj.python@gmail.com
 Project-URL: Bug Reports, https://github.com/shopyo/pythoncms/issues
 Project-URL: Source, https://github.com/shopyo/pythoncms
 Keywords: cms
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: shopyo==4.8.6
+Requires-Dist: SQLAlchemy==1.4.46
+Requires-Dist: python-dotenv
+
 
 <div align="center">
 
 
 
 <img src="https://github.com/shopyo/pythoncms/raw/main/assets/logo.png" width="200"/>
 
@@ -46,14 +51,25 @@
 pip install pythoncms
 pythoncms start mysite
 cd mysite
 shopyo initialise
 flask --debug run
 ```
 
+If .env file not created, create .env file with content
+
+```.env
+ACTIVE_FRONT_THEME = 'editorial'
+ACTIVE_BACK_THEME = 'sneat'
+APP_NAME = 'Demo'
+ACTIVE_ICONSET = 'boxicons'
+SITE_TITLE = 'Site title'
+SITE_DESCRIPTION = 'Site title'
+```
+
 ## Local dev
 
 Install package
 
 ! Important: Please create and activate a virtual environment.
 
 ```
@@ -87,21 +103,26 @@
 http://127.0.0.1:5000/dashboard/
 ```
 
 ## Theme
 
 Themes are located at '/static/themes/'
 
-Each theme must have
+Each front theme must have
 
 ```
 index.html
-base.html
 contact.html
 page.html
+```
+
+Each back theme must have
+
+```
+base.html
 login.html
 register.html
 unconfirmed.html
 ```
 
 - info.json
```

### Comparing `pythoncms-1.2.2/README.md` & `pythoncms-1.3.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 <div align="center">
 
 
 
 <img src="https://github.com/shopyo/pythoncms/raw/main/assets/logo.png" width="200"/>
 
 <br><br>
@@ -26,14 +27,25 @@
 pip install pythoncms
 pythoncms start mysite
 cd mysite
 shopyo initialise
 flask --debug run
 ```
 
+If .env file not created, create .env file with content
+
+```.env
+ACTIVE_FRONT_THEME = 'editorial'
+ACTIVE_BACK_THEME = 'sneat'
+APP_NAME = 'Demo'
+ACTIVE_ICONSET = 'boxicons'
+SITE_TITLE = 'Site title'
+SITE_DESCRIPTION = 'Site title'
+```
+
 ## Local dev
 
 Install package
 
 ! Important: Please create and activate a virtual environment.
 
 ```
@@ -67,21 +79,26 @@
 http://127.0.0.1:5000/dashboard/
 ```
 
 ## Theme
 
 Themes are located at '/static/themes/'
 
-Each theme must have
+Each front theme must have
 
 ```
 index.html
-base.html
 contact.html
 page.html
+```
+
+Each back theme must have
+
+```
+base.html
 login.html
 register.html
 unconfirmed.html
 ```
 
 - info.json
```

### Comparing `pythoncms-1.2.2/pythoncms/app.py` & `pythoncms-1.3.3/pythoncms/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,48 +19,61 @@
 from flask_admin.menu import MenuLink
 from flask_login import current_user
 from shopyo.api.assets import get_static
 from shopyo.api.assets import register_devstatic
 from shopyo.api.debug import is_yo_debug
 from shopyo.api.file import trycopy
 
+import sqlalchemy
+
 
 base_path = os.path.dirname(os.path.abspath(__file__))
 sys.path.insert(0, base_path)
 from config import app_config
 
 # from init import db
 from init import load_extensions
 from init import modules_path
 from init import installed_packages
 
 
 from shopyo_admin import MyAdminIndexView
+from shopyo_admin import DefaultModelView
+from modules.box__default.keyvalue.models import KeyValue
+from modules.box__default.keyvalue.helpers import set_value
+from init import db
+
 
+from dotenv import load_dotenv
+
+load_dotenv()
 
 def create_app(config_name="development"):
 
     global_template_variables = {}
     global_configs = {}
     app = Flask(
         __name__,
         instance_path=os.path.join(base_path, "instance"),
         instance_relative_config=True,
     )
 
+    
+
     load_plugins(app, global_template_variables, global_configs, config_name)
     load_config_from_obj(app, config_name)
     load_config_from_instance(app, config_name)
     create_config_json()
     load_extensions(app)
     setup_flask_admin(app)
     register_devstatic(app, modules_path)
     load_blueprints(app, config_name, global_template_variables, global_configs)
     setup_theme_paths(app)
     inject_global_vars(app, global_template_variables)
+    sync_keyvalue_envvar(app)
     return app
 
 
 def load_plugins(app, global_template_variables, global_configs, config_name):
     for plugin in installed_packages:
         if plugin not in ["shopyo_admin"]:
             try:
@@ -134,15 +147,15 @@
 def setup_flask_admin(app):
     admin = Admin(
         app,
         name="My App",
         template_mode="bootstrap4",
         index_view=MyAdminIndexView(),
     )
-    # admin.add_view(DefaultModelView(Settings, db.session))
+    admin.add_view(DefaultModelView(KeyValue, db.session))
     admin.add_link(MenuLink(name="Logout", category="", url="/auth/logout?next=/admin"))
 
 
 def load_blueprints(app, config_name, global_template_variables, global_configs):
     """
     - Registers blueprints
     - Adds global template objects from modules
@@ -251,18 +264,47 @@
             )
             app.jinja_loader = my_loader
 
 
 def inject_global_vars(app, global_template_variables):
     @app.context_processor
     def inject_global_vars():
-        APP_NAME = "dwdwefw"
-
+        APP_NAME = os.environ.get('APP_NAME', 'Demo')
+        def get_setting(env_var):
+            return os.environ.get(env_var)
+        
         base_context = {
             "APP_NAME": APP_NAME,
             "len": len,
             "current_user": current_user,
             "get_static": get_static,
+            "get_setting": get_setting
         }
         base_context.update(global_template_variables)
 
         return base_context
+    
+
+def sync_keyvalue_envvar(app):
+    with app.app_context():
+        try:
+            set_value(
+                'ACTIVE_FRONT_THEME',os.environ.get('ACTIVE_FRONT_THEME', 'editorial')
+            )
+            set_value(
+                'ACTIVE_BACK_THEME',os.environ.get('ACTIVE_BACK_THEME', 'sneat')
+            )
+            set_value(
+                'SITE_TITLE',os.environ.get('SITE_TITLE', 'Site Info')
+            )
+            set_value(
+                'SITE_DESCRIPTION',os.environ.get('SITE_DESCRIPTION', 'Site Description')
+            )
+            set_value(
+                'APP_NAME',os.environ.get('APP_NAME', 'Default App Name')
+            )
+            set_value(
+                'ACTIVE_ICONSET',os.environ.get('ACTIVE_ICONSET', 'boxicons')
+            )
+        except sqlalchemy.exc.OperationalError as e: # on shopyo initialise command
+            if os.environ.get('FLASK_DEBUG', False):
+                print(e)
```

### Comparing `pythoncms-1.2.2/pythoncms/cli.py` & `pythoncms-1.3.3/pythoncms/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -58,8 +58,12 @@
     New project
     """
     dest = os.getcwd() + f"/{name}"
 
     trycopytree(str(path.parent.absolute()), dest)
     tryrmfile(dest + "/cli.py")
     trymkfile(dest + "/requirements.txt", reqs)
+    try:
+        os.rename('.env_demo', '.env')
+    except Exception as e:
+        print(e)
     click.echo(f"🍭  Pythoncms project {name} is ready to go!")
```

### Comparing `pythoncms-1.2.2/pythoncms/config.py` & `pythoncms-1.3.3/pythoncms/config.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/conftest.py` & `pythoncms-1.3.3/pythoncms/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import pytest
 from app import create_app
 from flask import url_for
 from flask_login import current_user as _current_user
 from init import db as _db
 from modules.box__default.auth.models import User
-from modules.box__default.settings.models import Settings
+from modules.box__default.keyvalue.models import Settings
 from sqlalchemy import event
 
 # run in shopyo/shopyo
 # python -m pytest . or python -m pytest -v
 
 if os.path.exists("testing.db"):
     os.remove("testing.db")
```

### Comparing `pythoncms-1.2.2/pythoncms/init.py` & `pythoncms-1.3.3/pythoncms/init.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/admin.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/admin.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/appadmin/add.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/appadmin/add.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/appadmin/edit.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/appadmin/edit.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/appadmin/index.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/appadmin/index.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/templates/appadmin/roles.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/templates/appadmin/roles.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/tests/test_admin.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/appadmin/view.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/appadmin/view.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/forms.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/forms.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/models.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/models.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/blocks/login_form.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/blocks/login_form.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/blocks/register_form.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/blocks/register_form.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/login.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/login.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/register.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/register.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/templates/auth/unconfirmed.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/templates/auth/unconfirmed.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/tests/conftest.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/tests/factories.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/tests/factories.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/tests/test_auth_functional.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/tests/test_auth_functional.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/tests/test_auth_models.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/tests/test_auth_models.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/upload.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/upload.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/auth/view.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/auth/view.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/blocks/resources.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/blocks/resources.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/module_base.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/module_base.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/base/templates/base/nav_base.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/base/templates/base/nav_base.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% set active_page = active_page|default('none') %}
 
 <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
     <!-- Brand/logo -->
     <a class="navbar-brand" href="#">
         <img src="/static/shopyo.svg" width="35" height="30">
-        {{OUR_APP_NAME}} | {{active_page.capitalize()}}
+        {{APP_NAME}} | {{active_page.capitalize()}}
     </a>
     <!-- Nav Links Left Aligned -->
     <ul class="navbar-nav">
         <li class="nav-item">
             <a class="nav-link" href="{{url_for('dashboard.index')}}" title="Main Page">
                 <i class="yo-admin-nav-icon fas fa-home"></i>
             </a>
```

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/base/view.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/base/view.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/helpers.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/helpers.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/templates/dashboard/index.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/templates/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/tests/test_dashboard.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/dashboard/view.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/dashboard/view.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/i18n/global.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/i18n/global.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/i18n/view.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/i18n/view.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/page/forms.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/page/forms.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/page/info.json` & `pythoncms-1.3.3/pythoncms/modules/box__default/page/info.json`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/page/models.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/page/models.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/page/templates/page/all_pages.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/page/templates/page/all_pages.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/page/templates/page/dashboard.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/page/templates/page/dashboard.html`

 * *Files 21% similar despite different names*

```diff
@@ -8,49 +8,48 @@
 <br>
 <div class="container">
     <div class="card">
         <div class="card-body">
             <h3>New page</h3>
             <form action="{{url_for('{}.check_pagecontent'.format(module_name))}}" method="POST">
                 {{ form.title.label }}
-                <div class="input-group mb-3">
+
                     {{ form.title }}
-                    <span id="error" type="text" vissiblity='hidden'></span>
-                </div>
+
+
                 {{ form.slug.label }}
-                <div class="input-group mb-3">
+
                     {{ form.slug }}
-                    <span id="error" type="text" vissiblity='hidden'></span>
-                </div>
-                <div class="field">
+
+
                     {{ form.lang.label }} <br>
-                    <div class="input-group mb-3">
+
                         {{ form.lang }}
-                    </div>
-                </div>
-                <div class="field">
+
+
+
                     {{ form.content.label }} <br>
-                    <div class="input-group mb-3">
+
                         {{ form.content }}
-                    </div>
-                </div>
+
+
 
 
                 <input type="hidden" name="csrf_token" value="{{csrf_token()}}">
                 <input type="submit" class="btn btn-info" value="submit">
             </form>
         </div>
     </div>
 </div>
-<script src="https://cdnjs.cloudflare.com/ajax/libs/tinymce/6.3.1/tinymce.min.js" integrity="sha512-eV68QXP3t5Jbsf18jfqT8xclEJSGvSK5uClUuqayUbF5IRK8e2/VSXIFHzEoBnNcvLBkHngnnd3CY7AFpUhF7w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+<script src="https://cdnjs.cloudflare.com/ajax/libs/tinymce/6.8.3/tinymce.min.js" integrity="sha512-eV68QXP3t5Jbsf18jfqT8xclEJSGvSK5uClUuqayUbF5IRK8e2/VSXIFHzEoBnNcvLBkHngnnd3CY7AFpUhF7w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script type="text/javascript">
 tinymce.init({
     selector: '#content',
-    plugins: `advlist autolink link image imagetools lists
-                charmap print preview hr anchor pagebreak
+    plugins: `advlist autolink link image  lists
+                charmap print preview  anchor pagebreak
         searchreplace wordcount visualblocks visualchars code
         fullscreen insertdatetime media nonbreaking
         save table directionality template paste
         codesample`
     ,
     imagetools_toolbar: "rotateleft rotateright | flipv fliph | editimage imageoptions",
     toolbar: 'insertfile undo redo | styleselect | bold italic | alignleft aligncenter alignright alignjustify | bullist numlist outdent indent | link image | print preview media fullpage | forecolor backcolor emoticons | codesample | table tabledelete | tableprops tablerowprops tablecellprops | tableinsertrowbefore tableinsertrowafter tabledeleterow | tableinsertcolbefore tableinsertcolafter tabledeletecol',
```

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/page/templates/page/view_page_dashboard.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/page/templates/page/view_page_dashboard.html`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     <div class="card">
         <div class="card-body">
             <a href="{{ url_for('page.index') }}">
                 <button type="button" class="btn rounded-pill btn-icon btn-primary">
                     <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" style="fill: rgb(255, 255, 255);transform: ;msFilter:;"><path d="M21 11H6.414l5.293-5.293-1.414-1.414L2.586 12l7.707 7.707 1.414-1.414L6.414 13H21z"></path></svg>
                   </button>
             </a>
+            <a class="btn btn-lnk btn-primary" target="_blank" href="{{ url_for('page.view_page', slug=page.slug) }}">view</a>
             <br><br>
             <form action="{{url_for('{}.edit_pagecontent'.format(module_name))}}" method="POST">
                 {{ form.title.label }}
                 <div class="input-group mb-3">
 
                     {{ form.title }}
                     <span id="error" type="text" vissiblity='hidden'></span>
@@ -45,15 +46,15 @@
                 <input type="hidden" name="page_id" value="{{page.id}}">
                 <input type="hidden" name="csrf_token" value="{{csrf_token()}}">
                 <input type="submit" class="btn btn-info" value="submit">
             </form>
         </div>
     </div>
 </div>
-<script src="https://cdnjs.cloudflare.com/ajax/libs/tinymce/6.3.1/tinymce.min.js" integrity="sha512-eV68QXP3t5Jbsf18jfqT8xclEJSGvSK5uClUuqayUbF5IRK8e2/VSXIFHzEoBnNcvLBkHngnnd3CY7AFpUhF7w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+<script src="https://cdnjs.cloudflare.com/ajax/libs/tinymce/6.8.3/tinymce.min.js" integrity="sha512-eV68QXP3t5Jbsf18jfqT8xclEJSGvSK5uClUuqayUbF5IRK8e2/VSXIFHzEoBnNcvLBkHngnnd3CY7AFpUhF7w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script type="text/javascript">
 tinymce.init({
     selector: '#content',
     plugins: `advlist autolink link image imagetools lists
                 charmap print preview hr anchor pagebreak
         searchreplace wordcount visualblocks visualchars code
         fullscreen insertdatetime media nonbreaking
```

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/page/view.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/page/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     form.content = page.get_content(lang=lang_arg)
     form.lang.data = lang_arg
 
     context.update({"page": page, "form": form})
     return render_template("page/view_page_dashboard.html", **context)
 
 
-@module_blueprint.route("/s/<slug>", methods=["GET"])
+@module_blueprint.route("/<slug>", methods=["GET"])
 def view_page(slug):
     context = {}
     page = Page.query.filter(Page.slug == slug).first()
     context.update({"page": page})
 
     return render_template(f"{get_active_front_theme()}/page.html", **context)
     # return render_template("page/view_page.html", **context)
```

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/settings/templates/settings/edit.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/templates/settings/edit.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/settings/templates/settings/index.html` & `pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/templates/settings/index.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/settings/upload.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/keyvalue/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
 from init import db
-from modules.box__default.settings.models import Settings
+from modules.box__default.keyvalue.models import Settings
 
 
 def add_setting(name, value):
     if Settings.query.filter_by(setting=name).first():
         s = Settings.query.get(name)
         s.value = value
         db.session.commit()
```

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/theme/helpers.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/theme/helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import json
 import os
 
 from flask import url_for
 from init import themes_path
-from modules.box__default.settings.helpers import get_setting
-
+from modules.box__default.keyvalue.helpers import get_value
 
 def get_front_theme_dir():
-    theme_dir = os.path.join(themes_path, "front", get_setting("ACTIVE_FRONT_THEME"))
+    theme_dir = os.path.join(themes_path, "front", get_value('ACTIVE_FRONT_THEME'))
     return theme_dir
 
 
 def get_front_theme_info_data():
     info_path = os.path.join(get_front_theme_dir(), "info.json")
     with open(info_path) as f:
         info_data = json.load(f)
     return info_data
 
 
 def get_active_front_theme():
-    return get_setting("ACTIVE_FRONT_THEME")
+    return get_value('ACTIVE_FRONT_THEME')
 
 
 def get_active_front_theme_version():
     return get_front_theme_info_data()["version"]
 
 
 def get_active_front_theme_styles_url():
@@ -31,27 +30,27 @@
         "resource.active_front_theme_css",
         active_theme=get_active_front_theme(),
         v=get_active_front_theme_version(),
     )
 
 
 def get_back_theme_dir():
-    theme_dir = os.path.join(themes_path, "back", get_setting("ACTIVE_BACK_THEME"))
+    theme_dir = os.path.join(themes_path, "back", get_value('ACTIVE_BACK_THEME'))
     return theme_dir
 
 
 def get_back_theme_info_data():
     info_path = os.path.join(get_back_theme_dir(), "info.json")
     with open(info_path) as f:
         info_data = json.load(f)
     return info_data
 
 
 def get_active_back_theme():
-    return get_setting("ACTIVE_BACK_THEME")
+    return get_value('ACTIVE_BACK_THEME')
 
 
 def get_active_back_theme_version():
     return get_back_theme_info_data()["version"]
 
 
 def get_active_back_theme_styles_url():
```

### Comparing `pythoncms-1.2.2/pythoncms/modules/box__default/theme/view.py` & `pythoncms-1.3.3/pythoncms/modules/box__default/theme/view.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 
 from flask import Blueprint
 from flask import current_app
 from flask import redirect
 from flask import render_template
 from flask import url_for
 from flask_login import login_required
-from modules.box__default.settings.helpers import get_setting
-from modules.box__default.settings.helpers import set_setting
 from shopyo.api.file import get_folders
 
 # from flask import flash
 # from flask import request
 # from shopyo.api.html import notify_success
 # from init import db
 
-# from modules.box__default.settings.models import Settings
+from modules.box__default.keyvalue.helpers import get_value
+from modules.box__default.keyvalue.helpers import set_value
 
 # from shopyo.api.forms import flash_errors
 
 
 dirpath = os.path.dirname(os.path.abspath(__file__))
 module_info = {}
 
@@ -63,47 +62,60 @@
     back_theme_folders = get_folders(back_themes_path)
     for folder in back_theme_folders:
         theme_path = os.path.join(back_themes_path, folder)
         info_path = os.path.join(theme_path, "info.json")
         with open(info_path) as f:
             all_back_info[folder] = json.load(f)
 
-    active_front_theme = get_setting("ACTIVE_FRONT_THEME")
-    active_back_theme = get_setting("ACTIVE_BACK_THEME")
+    active_front_theme = get_value('ACTIVE_FRONT_THEME')
+    active_back_theme = get_value('ACTIVE_BACK_THEME')
+    active_iconset = get_value('ACTIVE_ICONSET')
 
     context.update(
         {
             "all_front_info": all_front_info,
             "all_back_info": all_back_info,
             "active_front_theme": active_front_theme,
             "active_back_theme": active_back_theme,
+            "active_iconset": active_iconset
         }
     )
     context.update(module_settings)
 
     return render_template(
         "{}/index.html".format(module_info["module_name"]), **context
     )
 
 
 @module_blueprint.route("/activate/front/<theme_name>")
 @login_required
 def activate_front_theme(theme_name):
-    set_setting("ACTIVE_FRONT_THEME", theme_name)
+    set_value('ACTIVE_FRONT_THEME', theme_name)
 
     # with app.app_context():
 
     # current_app.jinja_loader,
     # print(current_app.jinja_loader.list_templates())
     return redirect(url_for("{}.index".format(module_info["module_name"])))
 
 
 @module_blueprint.route("/activate/back/<theme_name>")
 @login_required
 def activate_back_theme(theme_name):
-    set_setting("ACTIVE_BACK_THEME", theme_name)
+    set_value('ACTIVE_BACK_THEME', theme_name)
+
+    # with app.app_context():
+
+    # current_app.jinja_loader,
+    # print(current_app.jinja_loader.list_templates())
+    return redirect(url_for("{}.index".format(module_info["module_name"])))
+
+@module_blueprint.route("/activate/inconset/<name>")
+@login_required
+def activate_iconset(name):
+    set_value('ACTIVE_ICONSET', name) # fa, boxicons
 
     # with app.app_context():
 
     # current_app.jinja_loader,
     # print(current_app.jinja_loader.list_templates())
     return redirect(url_for("{}.index".format(module_info["module_name"])))
```

### Comparing `pythoncms-1.2.2/pythoncms/modules/contact/forms.py` & `pythoncms-1.3.3/pythoncms/modules/contact/forms.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/contact/models.py` & `pythoncms-1.3.3/pythoncms/modules/contact/models.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/contact/templates/contact/contact_form.html` & `pythoncms-1.3.3/pythoncms/modules/contact/templates/contact/contact_form.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/contact/templates/contact/dashboard.html` & `pythoncms-1.3.3/pythoncms/modules/contact/templates/contact/dashboard.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/contact/tests/test_contact.py` & `pythoncms-1.3.3/pythoncms/modules/contact/tests/test_contact.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/contact/view.py` & `pythoncms-1.3.3/pythoncms/modules/contact/view.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/resource/models.py` & `pythoncms-1.3.3/pythoncms/modules/resource/models.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/resource/view.py` & `pythoncms-1.3.3/pythoncms/modules/resource/view.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # from flask import redirect
 
 # from flask import url_for
 
 # from flask_login import login_required
 # from PIL import Image as PILimage
 
-# from shopyo.api.enhance import get_setting
 # from shopyo.api.file import delete_file
 
 # from modules.box__ecommerce.product.models import Product
 # from modules.resource.models import Image
 
 # from modules.resource.models import Resource
```

### Comparing `pythoncms-1.2.2/pythoncms/modules/www/templates/www/index.html` & `pythoncms-1.3.3/pythoncms/modules/www/templates/www/index.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/modules/www/view.py` & `pythoncms-1.3.3/pythoncms/modules/www/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,33 +7,32 @@
 # from flask import redirect
 # from flask import flash
 # from flask import request
 #
 # from shopyo.api.html import notify_success
 # from shopyo.api.forms import flash_errors
 # from shopyo.api.enhance import get_active_theme_dir
-# from shopyo.api.enhance import get_setting
 # from modules.box__ecommerce.shop.helpers import get_cart_data
 
 mhelp = ModuleHelp(__file__, __name__)
 globals()[mhelp.blueprint_str] = mhelp.blueprint
 module_blueprint = globals()[mhelp.blueprint_str]
 
 
 @module_blueprint.route("/")
 def index():
     # cant be defined above but must be manually set each time
     # active_theme_dir = os.path.join(
-    #     dirpath, "..", "..", "themes", get_setting("ACTIVE_FRONT_THEME")
+    #     dirpath, "..", "..", "themes", os.environ.get('ACTIVE_FRONT_THEME")
     # )
     # module_blueprint.template_folder = active_theme_dir
 
     # return str(module_blueprint.template_folder)
 
-    # return render_template(get_setting("ACTIVE_FRONT_THEME") + "/index.html")
+    # return render_template(os.environ.get('ACTIVE_FRONT_THEME") + "/index.html")
 
     return render_template(
         f"{get_active_front_theme()}/index.html", get_static=get_static
     )
 
 
 from shopyo.api.assets import get_static
```

### Comparing `pythoncms-1.2.2/pythoncms/shopyo_admin.py` & `pythoncms-1.3.3/pythoncms/shopyo_admin.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/bootstrap-grid.min.css` & `pythoncms-1.3.3/pythoncms/static/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/bootstrap-reboot.min.css` & `pythoncms-1.3.3/pythoncms/static/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/bootstrap.bundle.min.js` & `pythoncms-1.3.3/pythoncms/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/bootstrap.min.css` & `pythoncms-1.3.3/pythoncms/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/box.svg` & `pythoncms-1.3.3/pythoncms/static/box.svg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/css/b4vtabs.min.css` & `pythoncms-1.3.3/pythoncms/static/css/b4vtabs.min.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/css/simple_sidebar.css` & `pythoncms-1.3.3/pythoncms/static/css/simple_sidebar.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/default/default_product.jpg` & `pythoncms-1.3.3/pythoncms/static/default/default_product.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/default/default_subcategory.jpg` & `pythoncms-1.3.3/pythoncms/static/default/default_subcategory.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/favicon.ico` & `pythoncms-1.3.3/pythoncms/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/LICENSE.txt` & `pythoncms-1.3.3/pythoncms/static/fontawesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/css/all.css` & `pythoncms-1.3.3/pythoncms/static/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/css/all.min.css` & `pythoncms-1.3.3/pythoncms/static/fontawesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/css/brands.css` & `pythoncms-1.3.3/pythoncms/static/fontawesome/css/brands.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/css/fontawesome.css` & `pythoncms-1.3.3/pythoncms/static/fontawesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/css/fontawesome.min.css` & `pythoncms-1.3.3/pythoncms/static/fontawesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/css/regular.css` & `pythoncms-1.3.3/pythoncms/static/fontawesome/css/regular.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/css/solid.css` & `pythoncms-1.3.3/pythoncms/static/fontawesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/css/svg-with-js.css` & `pythoncms-1.3.3/pythoncms/static/fontawesome/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/css/svg-with-js.min.css` & `pythoncms-1.3.3/pythoncms/static/fontawesome/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/css/v4-shims.css` & `pythoncms-1.3.3/pythoncms/static/fontawesome/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/css/v4-shims.min.css` & `pythoncms-1.3.3/pythoncms/static/fontawesome/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-brands-400.eot` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-brands-400.svg` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-brands-400.ttf` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-brands-400.woff` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-brands-400.woff2` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-regular-400.eot` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-regular-400.svg` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-regular-400.ttf` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-regular-400.woff` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-regular-400.woff2` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-solid-900.eot` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-solid-900.svg` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-solid-900.ttf` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-solid-900.woff` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/fontawesome/webfonts/fa-solid-900.woff2` & `pythoncms-1.3.3/pythoncms/static/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/jquery_3.2.1.min.js` & `pythoncms-1.3.3/pythoncms/static/jquery_3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/js/python.js` & `pythoncms-1.3.3/pythoncms/static/js/python.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/logo.png` & `pythoncms-1.3.3/pythoncms/static/logo.png`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/logo.svg` & `pythoncms-1.3.3/pythoncms/static/logo.svg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/shopyo.png` & `pythoncms-1.3.3/pythoncms/static/shopyo.png`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/shopyo.svg` & `pythoncms-1.3.3/pythoncms/static/shopyo.svg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/css/demo.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/css/demo.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/config.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/config.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/dashboards-analytics.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/dashboards-analytics.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/extended-ui-perfect-scrollbar.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/extended-ui-perfect-scrollbar.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/main.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/main.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/pages-account-settings-account.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/pages-account-settings-account.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/ui-modals.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/ui-modals.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/js/ui-toasts.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/js/ui-toasts.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/core.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/core.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-account-settings.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-account-settings.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-auth.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-auth.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-icons.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-icons.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-misc.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/pages/page-misc.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/css/theme-default.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/css/theme-default.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.eot` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.eot`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.svg` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.svg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.ttf` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.ttf`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.woff` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.woff`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.woff2` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons/boxicons.woff2`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/fonts/boxicons.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/js/bootstrap.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/js/helpers.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/js/helpers.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/js/menu.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/js/menu.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/apex-charts/apex-charts.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/apex-charts/apex-charts.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/apex-charts/apexcharts.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/apex-charts/apexcharts.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/highlight.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/highlight.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/highlight.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/highlight/highlight.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/jquery/jquery.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/masonry/masonry.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/masonry/masonry.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/perfect-scrollbar/perfect-scrollbar.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/perfect-scrollbar/perfect-scrollbar.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/perfect-scrollbar/perfect-scrollbar.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/perfect-scrollbar/perfect-scrollbar.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/assets/vendor/libs/popper/popper.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/assets/vendor/libs/popper/popper.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/authbase.html` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/authbase.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/base.html` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -123,30 +123,30 @@
 
               {%if menu_type == 'no-menu'%}
                 <li class="menu-item {{'active' if get_url_prefix() == moduleinfo['url_prefix']}}">
                   <a href="{{link}}" class="menu-link">
                     {%if 'file' in moduleinfo['icons']%}
                     <img class="menu-icon" src="{{get_static(moduleinfo['static_name'], moduleinfo['icons']['file'])}}">
                     {%else%}
-                      {%if get_setting('ACTIVE_ICONSET') == 'fa'%}
-                      <i class="menu-icon {{moduleinfo['icons']['fa']}}"></i>
+                      {%if get_value('ACTIVE_ICONSET') == 'fa'%}
+                      <i class="{{moduleinfo['icons']['fa']}}"></i>
                       {%else%}
                       <i class="menu-icon tf-icons {{moduleinfo['icons']['boxicons']}}"></i>
                       {%endif%}
                     {%endif%}
                     <div data-i18n="{{moduleinfo['display_string']}}">{{moduleinfo['display_string']}}</div>
                   </a>
                 </li>
               {%elif menu_type == 'show-menu'%}
                 <li class="menu-item {{'open active' if get_url_prefix() == moduleinfo['url_prefix']}}">
                   <a href="javascript:void(0);" class="menu-link menu-toggle">
                     {%if 'file' in moduleinfo['icons']%}
                       <img class="menu-icon" src="{{get_static(moduleinfo['static_name'], moduleinfo['icons']['file'])}}">
                     {%else%}
-                      {%if get_setting('ACTIVE_ICONSET') == 'fa'%}
+                      {%if get_value('ACTIVE_ICONSET') == 'fa'%}
                       <i class="menu-icon {{moduleinfo['icons']['fa']}}"></i>
                       {%else%}
                       <i class="menu-icon tf-icons {{moduleinfo['icons']['boxicons']}}"></i>
                       {%endif%}
                     {%endif%}
                     <div data-i18n="{{moduleinfo['display_string']}}">{{moduleinfo['display_string']}}</div>
                   </a>
@@ -287,15 +287,15 @@
             <!-- Content -->
             <div>
                 {%block content%}
 
                 {%endblock%}
             </div>
             <!-- / Content -->
-
+            <br/>
             <!-- Footer -->
             <footer class="content-footer footer bg-footer-theme">
               <div class="container-xxl d-flex flex-wrap justify-content-between py-2 flex-md-row flex-column">
                 <div class="mb-2 mb-md-0">
                   ©
                   <script>
                     document.write(new Date().getFullYear());
```

#### html2text {}

```diff
@@ -17,31 +17,32 @@
       link = all_info[info]['url_prefix'] + all_info[info]['dashboard'] %}
       {%else%} {% set link = all_info[info]['url_prefix'] %} {%endif%} {%if
       'menu-type' not in moduleinfo %} {%set menu_type="no-menu"%} {%endif%}
       {%if 'menu' in moduleinfo%} {%set menu_type='show-menu'%} {%endif%} {%if
       'menu-type' in moduleinfo %} {%set menu_type=all_info['menu-type']%}
       {%endif%} {%if menu_type == 'no-menu'%}
     * _{_%_i_f_ _'_f_i_l_e_'_ _i_n_ _m_o_d_u_l_e_i_n_f_o_[_'_i_c_o_n_s_'_]_%_}_ _[_{_{_g_e_t___s_t_a_t_i_c_(_m_o_d_u_l_e_i_n_f_o
-      _[_'_s_t_a_t_i_c___n_a_m_e_'_]_,_ _m_o_d_u_l_e_i_n_f_o_[_'_i_c_o_n_s_'_]_[_'_f_i_l_e_'_]_)_}_}_]_{_%_e_l_s_e_%_}_ _{_%_i_f_ _g_e_t___s_e_t_t_i_n_g
+      _[_'_s_t_a_t_i_c___n_a_m_e_'_]_,_ _m_o_d_u_l_e_i_n_f_o_[_'_i_c_o_n_s_'_]_[_'_f_i_l_e_'_]_)_}_}_]_{_%_e_l_s_e_%_}_ _{_%_i_f_ _g_e_t___v_a_l_u_e
       _(_'_A_C_T_I_V_E___I_C_O_N_S_E_T_'_)_ _=_=_ _'_f_a_'_%_}_ _{_%_e_l_s_e_%_}_ _{_%_e_n_d_i_f_%_}_ _{_%_e_n_d_i_f_%_}
       _{_{_m_o_d_u_l_e_i_n_f_o_[_'_d_i_s_p_l_a_y___s_t_r_i_n_g_'_]_}_}
     * {%elif menu_type == 'show-menu'%}
     * _{_%_i_f_ _'_f_i_l_e_'_ _i_n_ _m_o_d_u_l_e_i_n_f_o_[_'_i_c_o_n_s_'_]_%_}_ _[_{_{_g_e_t___s_t_a_t_i_c_(_m_o_d_u_l_e_i_n_f_o
-      _[_'_s_t_a_t_i_c___n_a_m_e_'_]_,_ _m_o_d_u_l_e_i_n_f_o_[_'_i_c_o_n_s_'_]_[_'_f_i_l_e_'_]_)_}_}_]_{_%_e_l_s_e_%_}_ _{_%_i_f_ _g_e_t___s_e_t_t_i_n_g
+      _[_'_s_t_a_t_i_c___n_a_m_e_'_]_,_ _m_o_d_u_l_e_i_n_f_o_[_'_i_c_o_n_s_'_]_[_'_f_i_l_e_'_]_)_}_}_]_{_%_e_l_s_e_%_}_ _{_%_i_f_ _g_e_t___v_a_l_u_e
       _(_'_A_C_T_I_V_E___I_C_O_N_S_E_T_'_)_ _=_=_ _'_f_a_'_%_}_ _{_%_e_l_s_e_%_}_ _{_%_e_n_d_i_f_%_}_ _{_%_e_n_d_i_f_%_}
       _{_{_m_o_d_u_l_e_i_n_f_o_[_'_d_i_s_p_l_a_y___s_t_r_i_n_g_'_]_}_}
           o {%for menu in moduleinfo['menu'] %} {%set menuname = menu%} {%set
             menulink = moduleinfo['menu'][menu]%} {%set subprefix = moduleinfo
             ['url_prefix'] + menulink%}
           o _{_{_m_e_n_u_n_a_m_e_}_}
           o {%endfor%}
     * {%endif%} {% endif %} {% endfor %}
 [                    ]
     * _S_t_a_r
     *     o _J_o_h_n_ _D_o_e_ _A_d_m_i_n
           o _M_y_ _P_r_o_f_i_l_e
     * _L_o_g_ _O_u_t
 {%block content%} {%endblock%}
+
 ©
 , made with ❤️ by _T_h_e_m_e_S_e_l_e_c_t_i_o_n
 _L_i_c_e_n_s_e _M_o_r_e_ _T_h_e_m_e_s _D_o_c_u_m_e_n_t_a_t_i_o_n _S_u_p_p_o_r_t
 {%include 'sneat/sections/resource_end_body.html' %}
```

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/login.html` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/login.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/register.html` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/register.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/sections/dashboard_elements.html` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/sections/dashboard_elements.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/sections/resource_end_body.html` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/sections/resource_end_body.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/sections/resource_head.html` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/sections/resource_head.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/styles.css` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/styles.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/back/sneat/unconfirmed.html` & `pythoncms-1.3.3/pythoncms/static/themes/back/sneat/unconfirmed.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/LICENSE.txt` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/README.txt` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/README.txt`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/css/fontawesome-all.min.css` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/css/main.css` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/css/main.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/js/breakpoints.min.js` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/js/breakpoints.min.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/js/browser.min.js` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/js/browser.min.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/js/jquery.min.js` & `pythoncms-1.3.3/pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/js/main.js` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/js/main.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/js/util.js` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/js/util.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/base/_page.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/base/_page.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/base/_reset.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/base/_reset.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/base/_typography.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/base/_typography.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_actions.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_actions.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_box.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_box.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_button.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_button.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_contact.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_contact.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_features.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_features.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_form.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_form.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_image.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_image.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_list.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_list.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_mini-posts.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_mini-posts.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_pagination.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_pagination.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_posts.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_posts.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_row.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_row.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_section.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_section.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/components/_table.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/components/_table.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_banner.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_banner.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_header.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_header.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_main.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_main.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_menu.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_menu.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/layout/_sidebar.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/layout/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_breakpoints.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_functions.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_functions.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_html-grid.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_html-grid.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_mixins.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_mixins.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_vars.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_vars.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/libs/_vendor.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/libs/_vendor.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/assets/sass/main.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/sass/main.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/base.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!--
 	Editorial by HTML5 UP
 	html5up.net | @ajlkn
 	Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)
 -->
 <html>
 	<head>
-		<title>Editorial by HTML5 UP</title>
+		<title>{{get_setting('SITE_TITLE')}}</title>
 		<meta charset="utf-8" />
 		<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no" />
 		<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css" integrity="sha512-MV7K8+y+gLIBoVD59lQIYicR65iaqukzvf/nwasF0nqhPay5w/9lJmVM2hMDcnK1OnMGCdVK+iQrJ7lzPJQd1w==" crossorigin="anonymous" referrerpolicy="no-referrer" />
 		<link rel="stylesheet" href="{{url_for('static', filename='themes/front/editorial/assets/css/main.css')}}" />
 	</head>
 	<body class="is-preload">
         {%block body%}
```

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/contact.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/contact.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/elements.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/elements.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/generic.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/generic.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic01.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic01.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic02.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic02.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic03.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic03.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic04.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic04.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic05.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic05.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic06.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic06.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic07.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic07.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic08.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic08.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic09.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic09.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic10.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic10.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/images/pic11.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/images/pic11.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/index.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -22,30 +22,29 @@
 								</ul>
 							</header>
 
 						<!-- Banner -->
 							<section id="banner">
 								<div class="content">
 									<header>
-										<h1>Hi, I’m Editorial<br />
-										by HTML5 UP</h1>
-										<p>A free and fully responsive site template</p>
+										<h1>{{get_value('SITE_TITLE')}}</h1>
+										<p>{{get_value('SITE_DESCRIPTION')}}</p>
 									</header>
 									<p>Aenean ornare velit lacus, ac varius enim ullamcorper eu. Proin aliquam facilisis ante interdum congue. Integer mollis, nisl amet convallis, porttitor magna ullamcorper, amet egestas mauris. Ut magna finibus nisi nec lacinia. Nam maximus erat id euismod egestas. Pellentesque sapien ac quam. Lorem ipsum dolor sit nullam.</p>
 									<ul class="actions">
 										<li><a href="#" class="button big">Learn More</a></li>
 									</ul>
 								</div>
 								<span class="image object">
 									<img src="{{url_for('static', filename='themes/front/editorial/images/pic10.jpg')}}" alt="" />
 								</span>
 							</section>
 
 						<!-- Section -->
-							<section>
+							<!-- <section>
 								<header class="major">
 									<h2>Erat lacinia</h2>
 								</header>
 								<div class="features">
 									<article>
 										<span class="icon fa-gem"></span>
 										<div class="content">
@@ -71,27 +70,27 @@
 										<span class="icon solid fa-signal"></span>
 										<div class="content">
 											<h3>Sed magna finibus</h3>
 											<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
 										</div>
 									</article>
 								</div>
-							</section>
+							</section> -->
 
 						<!-- Section -->
 							<section>
 								<header class="major">
 									<h2>Posts</h2>
 								</header>
 								<div class="posts">
 									{%for page in get_pages()%}
 									<article>
 										<a href="#" class="image"><img src="{{url_for('static', filename='themes/front/editorial/images/pic01.jpg')}}" alt="" /></a>
 										<h3>{{page.title}}</h3>
-										<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
+										
 										<ul class="actions">
 											<li><a href="{{page.get_url()}}" class="button">More</a></li>
 										</ul>
 									</article>
 									{%endfor%}
 								</div>
 							</section>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,38 +1,22 @@
 {%extends 'editorial/base.html'%} {%block body%}
 _EE_dd_ii_tt_oo_rr_ii_aa_ll_ _b_y_ _H_T_M_L_5_ _U_P
     * _T_w_i_t_t_e_r
     * _F_a_c_e_b_o_o_k
     * _S_n_a_p_c_h_a_t
     * _I_n_s_t_a_g_r_a_m
     * _M_e_d_i_u_m
-************ HHii,, II?â??mm EEddiittoorriiaall
-bbyy HHTTMMLL55 UUPP ************
-A free and fully responsive site template
+************ {{{{ggeett__vvaalluuee((''SSIITTEE__TTIITTLLEE''))}}}} ************
+{{get_value('SITE_DESCRIPTION')}}
 Aenean ornare velit lacus, ac varius enim ullamcorper eu. Proin aliquam
 facilisis ante interdum congue. Integer mollis, nisl amet convallis, porttitor
 magna ullamcorper, amet egestas mauris. Ut magna finibus nisi nec lacinia. Nam
 maximus erat id euismod egestas. Pellentesque sapien ac quam. Lorem ipsum dolor
 sit nullam.
     * _L_e_a_r_n_ _M_o_r_e
-********** EErraatt llaacciinniiaa **********
-******** PPoorrttiittoorr uullllaammccoorrppeerr ********
-Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin
-aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.
-******** SSaappiieenn vveerrooeerrooss ********
-Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin
-aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.
-******** QQuuaamm lloorreemm iippssuumm ********
-Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin
-aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.
-******** SSeedd mmaaggnnaa ffiinniibbuuss ********
-Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin
-aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.
 ********** PPoossttss **********
 {%for page in get_pages()%}
 ******** {{{{ppaaggee..ttiittllee}}}} ********
-Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin
-aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.
     * _M_o_r_e
 {%endfor%}
 {%include 'editorial/sections/sidebar.html'%}
 {%endblock%}
```

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/page.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/page.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/sections/sidebar.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/sections/sidebar.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/editorial/styles.css` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/styles.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/LICENSE.txt` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/README.txt` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/README.txt`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/css/fontawesome-all.min.css` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/css/images/intro.svg` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/css/images/intro.svg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/css/main.css` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/css/main.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/css/noscript.css` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/css/noscript.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/breakpoints.min.js` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/breakpoints.min.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/browser.min.js` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/browser.min.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/jquery.min.js` & `pythoncms-1.3.3/pythoncms/static/themes/front/editorial/assets/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/jquery.scrollex.min.js` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/jquery.scrollex.min.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/jquery.scrolly.min.js` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/jquery.scrolly.min.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/main.js` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/main.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/js/util.js` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/js/util.js`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/base/_page.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/base/_page.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/base/_reset.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/base/_reset.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/base/_typography.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/base/_typography.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_actions.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_actions.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_box.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_box.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_button.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_button.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_features.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_features.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_form.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_form.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_icon.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_icon.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_image.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_image.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_list.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_list.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_menu.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_menu.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_row.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_row.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_section.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_section.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_split.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_split.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_spotlights.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_spotlights.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_table.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_table.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/components/_wrapper.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/components/_wrapper.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_footer.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_footer.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_header.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_header.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_intro.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_intro.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_sidebar.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_wrapper.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/layout/_wrapper.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_breakpoints.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_functions.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_functions.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_html-grid.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_html-grid.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_mixins.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_mixins.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_vars.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_vars.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_vendor.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/libs/_vendor.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/main.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/main.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/assets/sass/noscript.scss` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/assets/sass/noscript.scss`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/base.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/base.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/contact.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/contact.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/elements.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/elements.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/generic.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/generic.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic01.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic01.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic02.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic02.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic03.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic03.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic04.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic04.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic05.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic05.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/images/pic06.jpg` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/images/pic06.jpg`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/index.html` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/index.html`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/static/themes/front/hyperspace/styles.css` & `pythoncms-1.3.3/pythoncms/static/themes/front/hyperspace/styles.css`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/tests/conftest.py` & `pythoncms-1.3.3/pythoncms/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/tests/test_configs.py` & `pythoncms-1.3.3/pythoncms/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/tests/test_dunder_main.py` & `pythoncms-1.3.3/pythoncms/tests/test_dunder_main.py`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms/wsgi.py.example` & `pythoncms-1.3.3/pythoncms/wsgi.py.example`

 * *Files identical despite different names*

### Comparing `pythoncms-1.2.2/pythoncms.egg-info/PKG-INFO` & `pythoncms-1.3.3/pythoncms.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: pythoncms
-Version: 1.2.2
+Version: 1.3.3
 Home-page: 
 Author: Abdur-Rahmaan Janhangeer
 Author-email: arj.python@gmail.com
 Project-URL: Bug Reports, https://github.com/shopyo/pythoncms/issues
 Project-URL: Source, https://github.com/shopyo/pythoncms
 Keywords: cms
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: shopyo==4.8.6
+Requires-Dist: SQLAlchemy==1.4.46
+Requires-Dist: python-dotenv
+
 
 <div align="center">
 
 
 
 <img src="https://github.com/shopyo/pythoncms/raw/main/assets/logo.png" width="200"/>
 
@@ -46,14 +51,25 @@
 pip install pythoncms
 pythoncms start mysite
 cd mysite
 shopyo initialise
 flask --debug run
 ```
 
+If .env file not created, create .env file with content
+
+```.env
+ACTIVE_FRONT_THEME = 'editorial'
+ACTIVE_BACK_THEME = 'sneat'
+APP_NAME = 'Demo'
+ACTIVE_ICONSET = 'boxicons'
+SITE_TITLE = 'Site title'
+SITE_DESCRIPTION = 'Site title'
+```
+
 ## Local dev
 
 Install package
 
 ! Important: Please create and activate a virtual environment.
 
 ```
@@ -87,21 +103,26 @@
 http://127.0.0.1:5000/dashboard/
 ```
 
 ## Theme
 
 Themes are located at '/static/themes/'
 
-Each theme must have
+Each front theme must have
 
 ```
 index.html
-base.html
 contact.html
 page.html
+```
+
+Each back theme must have
+
+```
+base.html
 login.html
 register.html
 unconfirmed.html
 ```
 
 - info.json
```

### Comparing `pythoncms-1.2.2/pythoncms.egg-info/SOURCES.txt` & `pythoncms-1.3.3/pythoncms.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,54 @@
 MANIFEST.in
 README.md
 dev_requirements.txt
 requirements.txt
 setup.py
+pythoncms/.env_demo
 pythoncms/.test.prod.env
 pythoncms/CHANGELOG.md
 pythoncms/__init__.py
 pythoncms/app.py
 pythoncms/autoapp.py.example
 pythoncms/cli.py
-pythoncms/config.json
 pythoncms/config.py
 pythoncms/config_demo.json
 pythoncms/conftest.py
 pythoncms/init.py
 pythoncms/manage.py
 pythoncms/shopyo_admin.py
 pythoncms/wsgi.py.example
 pythoncms.egg-info/PKG-INFO
 pythoncms.egg-info/SOURCES.txt
 pythoncms.egg-info/dependency_links.txt
 pythoncms.egg-info/entry_points.txt
 pythoncms.egg-info/requires.txt
 pythoncms.egg-info/top_level.txt
-pythoncms/__pycache__/__init__.cpython-310.pyc
-pythoncms/__pycache__/app.cpython-310.pyc
-pythoncms/__pycache__/cli.cpython-310.pyc
-pythoncms/__pycache__/config.cpython-310.pyc
-pythoncms/__pycache__/init.cpython-310.pyc
-pythoncms/__pycache__/shopyo_admin.cpython-310.pyc
+pythoncms/__pycache__/__init__.cpython-312.pyc
 pythoncms/modules/__init__.py
-pythoncms/modules/__pycache__/__init__.cpython-310.pyc
 pythoncms/modules/box__default/box_info.json
 pythoncms/modules/box__default/appadmin/__init__.py
 pythoncms/modules/box__default/appadmin/admin.py
 pythoncms/modules/box__default/appadmin/info.json
 pythoncms/modules/box__default/appadmin/models.py
 pythoncms/modules/box__default/appadmin/view.py
-pythoncms/modules/box__default/appadmin/__pycache__/__init__.cpython-310.pyc
-pythoncms/modules/box__default/appadmin/__pycache__/admin.cpython-310.pyc
-pythoncms/modules/box__default/appadmin/__pycache__/view.cpython-310.pyc
 pythoncms/modules/box__default/appadmin/static/icon.svg
 pythoncms/modules/box__default/appadmin/templates/appadmin/add.html
 pythoncms/modules/box__default/appadmin/templates/appadmin/edit.html
 pythoncms/modules/box__default/appadmin/templates/appadmin/index.html
 pythoncms/modules/box__default/appadmin/templates/appadmin/roles.html
 pythoncms/modules/box__default/appadmin/templates/appadmin/blocks/sidebar.html
 pythoncms/modules/box__default/appadmin/tests/test_admin.py
 pythoncms/modules/box__default/appadmin/tests/test_models.py
 pythoncms/modules/box__default/auth/decorators.py
 pythoncms/modules/box__default/auth/forms.py
 pythoncms/modules/box__default/auth/info.json
 pythoncms/modules/box__default/auth/models.py
 pythoncms/modules/box__default/auth/upload.py
 pythoncms/modules/box__default/auth/view.py
-pythoncms/modules/box__default/auth/__pycache__/decorators.cpython-310.pyc
-pythoncms/modules/box__default/auth/__pycache__/forms.cpython-310.pyc
-pythoncms/modules/box__default/auth/__pycache__/models.cpython-310.pyc
-pythoncms/modules/box__default/auth/__pycache__/view.cpython-310.pyc
 pythoncms/modules/box__default/auth/static/style.css
 pythoncms/modules/box__default/auth/templates/auth/login.html
 pythoncms/modules/box__default/auth/templates/auth/register.html
 pythoncms/modules/box__default/auth/templates/auth/shop_login.html
 pythoncms/modules/box__default/auth/templates/auth/unconfirmed.html
 pythoncms/modules/box__default/auth/templates/auth/blocks/login_form.html
 pythoncms/modules/box__default/auth/templates/auth/blocks/register_form.html
@@ -69,116 +56,96 @@
 pythoncms/modules/box__default/auth/templates/auth/emails/activate_user.txt
 pythoncms/modules/box__default/auth/tests/conftest.py
 pythoncms/modules/box__default/auth/tests/factories.py
 pythoncms/modules/box__default/auth/tests/test_auth_forms.py
 pythoncms/modules/box__default/auth/tests/test_auth_functional.py
 pythoncms/modules/box__default/auth/tests/test_auth_models.py
 pythoncms/modules/box__default/base/info.json
+pythoncms/modules/box__default/base/models.py
 pythoncms/modules/box__default/base/view.py
-pythoncms/modules/box__default/base/__pycache__/view.cpython-310.pyc
 pythoncms/modules/box__default/base/templates/base/main_base.html
 pythoncms/modules/box__default/base/templates/base/module_base.html
 pythoncms/modules/box__default/base/templates/base/nav_base.html
 pythoncms/modules/box__default/base/templates/base/blocks/default_styles.html
 pythoncms/modules/box__default/base/templates/base/blocks/flashed_messages.html
 pythoncms/modules/box__default/base/templates/base/blocks/footer.html
 pythoncms/modules/box__default/base/templates/base/blocks/macros.html
 pythoncms/modules/box__default/base/templates/base/blocks/resources.html
 pythoncms/modules/box__default/dashboard/global.py
 pythoncms/modules/box__default/dashboard/helpers.py
 pythoncms/modules/box__default/dashboard/info.json
 pythoncms/modules/box__default/dashboard/view.py
-pythoncms/modules/box__default/dashboard/__pycache__/global.cpython-310.pyc
-pythoncms/modules/box__default/dashboard/__pycache__/helpers.cpython-310.pyc
-pythoncms/modules/box__default/dashboard/__pycache__/view.cpython-310.pyc
 pythoncms/modules/box__default/dashboard/templates/dashboard/index.html
 pythoncms/modules/box__default/dashboard/templates/dashboard/nav.html
 pythoncms/modules/box__default/dashboard/tests/test_dashboard.py
 pythoncms/modules/box__default/i18n/forms.py
 pythoncms/modules/box__default/i18n/global.py
 pythoncms/modules/box__default/i18n/helpers.py
 pythoncms/modules/box__default/i18n/info.json
 pythoncms/modules/box__default/i18n/models.py
 pythoncms/modules/box__default/i18n/view.py
-pythoncms/modules/box__default/i18n/__pycache__/global.cpython-310.pyc
-pythoncms/modules/box__default/i18n/__pycache__/helpers.cpython-310.pyc
-pythoncms/modules/box__default/i18n/__pycache__/models.cpython-310.pyc
-pythoncms/modules/box__default/i18n/__pycache__/view.cpython-310.pyc
 pythoncms/modules/box__default/i18n/templates/i18n/dashboard.html
 pythoncms/modules/box__default/i18n/templates/i18n/blocks/sidebar.html
 pythoncms/modules/box__default/i18n/tests/test_i18n_functional.py
 pythoncms/modules/box__default/i18n/tests/test_i18n_models.py
+pythoncms/modules/box__default/info/forms.py
+pythoncms/modules/box__default/info/global.py
+pythoncms/modules/box__default/info/helpers.py
+pythoncms/modules/box__default/info/info.json
+pythoncms/modules/box__default/info/models.py
+pythoncms/modules/box__default/info/view.py
+pythoncms/modules/box__default/info/templates/info/dashboard.html
+pythoncms/modules/box__default/keyvalue/__init__.py
+pythoncms/modules/box__default/keyvalue/global.py
+pythoncms/modules/box__default/keyvalue/helpers.py
+pythoncms/modules/box__default/keyvalue/info.json
+pythoncms/modules/box__default/keyvalue/models.py
+pythoncms/modules/box__default/keyvalue/upload.py
+pythoncms/modules/box__default/keyvalue/view.py
+pythoncms/modules/box__default/keyvalue/templates/settings/edit.html
+pythoncms/modules/box__default/keyvalue/templates/settings/index.html
+pythoncms/modules/box__default/keyvalue/templates/settings/nav.html
 pythoncms/modules/box__default/page/forms.py
 pythoncms/modules/box__default/page/global.py
 pythoncms/modules/box__default/page/helpers.py
 pythoncms/modules/box__default/page/info.json
 pythoncms/modules/box__default/page/models.py
 pythoncms/modules/box__default/page/view.py
-pythoncms/modules/box__default/page/__pycache__/forms.cpython-310.pyc
-pythoncms/modules/box__default/page/__pycache__/global.cpython-310.pyc
-pythoncms/modules/box__default/page/__pycache__/helpers.cpython-310.pyc
-pythoncms/modules/box__default/page/__pycache__/models.cpython-310.pyc
-pythoncms/modules/box__default/page/__pycache__/view.cpython-310.pyc
 pythoncms/modules/box__default/page/templates/page/all_pages.html
 pythoncms/modules/box__default/page/templates/page/dashboard.html
 pythoncms/modules/box__default/page/templates/page/dashboard_edit.html
 pythoncms/modules/box__default/page/templates/page/view_page_dashboard.html
 pythoncms/modules/box__default/page/templates/page/blocks/sidebar.html
-pythoncms/modules/box__default/settings/__init__.py
-pythoncms/modules/box__default/settings/global.py
-pythoncms/modules/box__default/settings/helpers.py
-pythoncms/modules/box__default/settings/info.json
-pythoncms/modules/box__default/settings/models.py
-pythoncms/modules/box__default/settings/upload.py
-pythoncms/modules/box__default/settings/view.py
-pythoncms/modules/box__default/settings/__pycache__/__init__.cpython-310.pyc
-pythoncms/modules/box__default/settings/__pycache__/global.cpython-310.pyc
-pythoncms/modules/box__default/settings/__pycache__/helpers.cpython-310.pyc
-pythoncms/modules/box__default/settings/__pycache__/models.cpython-310.pyc
-pythoncms/modules/box__default/settings/__pycache__/view.cpython-310.pyc
-pythoncms/modules/box__default/settings/templates/settings/edit.html
-pythoncms/modules/box__default/settings/templates/settings/index.html
-pythoncms/modules/box__default/settings/templates/settings/nav.html
 pythoncms/modules/box__default/theme/forms.py
 pythoncms/modules/box__default/theme/global.py
 pythoncms/modules/box__default/theme/helpers.py
 pythoncms/modules/box__default/theme/info.json
 pythoncms/modules/box__default/theme/models.py
 pythoncms/modules/box__default/theme/view.py
-pythoncms/modules/box__default/theme/__pycache__/global.cpython-310.pyc
-pythoncms/modules/box__default/theme/__pycache__/helpers.cpython-310.pyc
-pythoncms/modules/box__default/theme/__pycache__/view.cpython-310.pyc
 pythoncms/modules/box__default/theme/templates/theme/index.html
 pythoncms/modules/box__default/theme/templates/theme/blocks/sidebar.html
 pythoncms/modules/contact/forms.py
 pythoncms/modules/contact/global.py
 pythoncms/modules/contact/info.json
 pythoncms/modules/contact/models.py
 pythoncms/modules/contact/view.py
-pythoncms/modules/contact/__pycache__/forms.cpython-310.pyc
-pythoncms/modules/contact/__pycache__/global.cpython-310.pyc
-pythoncms/modules/contact/__pycache__/models.cpython-310.pyc
-pythoncms/modules/contact/__pycache__/view.cpython-310.pyc
 pythoncms/modules/contact/templates/contact/contact_form.html
 pythoncms/modules/contact/templates/contact/dashboard.html
 pythoncms/modules/contact/templates/contact/blocks/sidebar.html
 pythoncms/modules/contact/tests/test_contact.py
 pythoncms/modules/resource/forms.py
 pythoncms/modules/resource/info.json
 pythoncms/modules/resource/models.py
 pythoncms/modules/resource/view.py
-pythoncms/modules/resource/__pycache__/view.cpython-310.pyc
 pythoncms/modules/resource/templates/resource/blocks/sidebar.html
 pythoncms/modules/www/forms.py
 pythoncms/modules/www/global.py
 pythoncms/modules/www/info.json
 pythoncms/modules/www/models.py
 pythoncms/modules/www/view.py
-pythoncms/modules/www/__pycache__/global.cpython-310.pyc
-pythoncms/modules/www/__pycache__/view.cpython-310.pyc
 pythoncms/modules/www/templates/www/index.html
 pythoncms/modules/www/templates/www/blocks/sidebar.html
 pythoncms/static/bootstrap-grid.min.css
 pythoncms/static/bootstrap-reboot.min.css
 pythoncms/static/bootstrap.bundle.min.js
 pythoncms/static/bootstrap.min.css
 pythoncms/static/box.svg
@@ -219,14 +186,59 @@
 pythoncms/static/fontawesome/webfonts/fa-regular-400.woff2
 pythoncms/static/fontawesome/webfonts/fa-solid-900.eot
 pythoncms/static/fontawesome/webfonts/fa-solid-900.svg
 pythoncms/static/fontawesome/webfonts/fa-solid-900.ttf
 pythoncms/static/fontawesome/webfonts/fa-solid-900.woff
 pythoncms/static/fontawesome/webfonts/fa-solid-900.woff2
 pythoncms/static/js/python.js
+pythoncms/static/themes/back/sbadmin/.gitignore
+pythoncms/static/themes/back/sbadmin/404.html
+pythoncms/static/themes/back/sbadmin/LICENSE
+pythoncms/static/themes/back/sbadmin/authbase.html
+pythoncms/static/themes/back/sbadmin/base.html
+pythoncms/static/themes/back/sbadmin/index.html
+pythoncms/static/themes/back/sbadmin/info.json
+pythoncms/static/themes/back/sbadmin/login.html
+pythoncms/static/themes/back/sbadmin/register.html
+pythoncms/static/themes/back/sbadmin/unconfirmed.html
+pythoncms/static/themes/back/sbadmin/css/sb-admin-2.css
+pythoncms/static/themes/back/sbadmin/css/sb-admin-2.min.css
+pythoncms/static/themes/back/sbadmin/js/sb-admin-2.js
+pythoncms/static/themes/back/sbadmin/js/sb-admin-2.min.js
+pythoncms/static/themes/back/sbadmin/js/demo/chart-area-demo.js
+pythoncms/static/themes/back/sbadmin/js/demo/chart-bar-demo.js
+pythoncms/static/themes/back/sbadmin/js/demo/chart-pie-demo.js
+pythoncms/static/themes/back/sbadmin/js/demo/datatables-demo.js
+pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.bundle.js
+pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.bundle.js.map
+pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.bundle.min.js
+pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.js
+pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.js.map
+pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.min.js
+pythoncms/static/themes/back/sbadmin/vendor/bootstrap/js/bootstrap.min.js.map
+pythoncms/static/themes/back/sbadmin/vendor/chart.js/Chart.bundle.js
+pythoncms/static/themes/back/sbadmin/vendor/chart.js/Chart.bundle.min.js
+pythoncms/static/themes/back/sbadmin/vendor/chart.js/Chart.js
+pythoncms/static/themes/back/sbadmin/vendor/chart.js/Chart.min.js
+pythoncms/static/themes/back/sbadmin/vendor/datatables/dataTables.bootstrap4.css
+pythoncms/static/themes/back/sbadmin/vendor/datatables/dataTables.bootstrap4.js
+pythoncms/static/themes/back/sbadmin/vendor/datatables/dataTables.bootstrap4.min.css
+pythoncms/static/themes/back/sbadmin/vendor/datatables/dataTables.bootstrap4.min.js
+pythoncms/static/themes/back/sbadmin/vendor/datatables/jquery.dataTables.js
+pythoncms/static/themes/back/sbadmin/vendor/datatables/jquery.dataTables.min.js
+pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.js
+pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.min.js
+pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.min.map
+pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.slim.js
+pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.slim.min.js
+pythoncms/static/themes/back/sbadmin/vendor/jquery/jquery.slim.min.map
+pythoncms/static/themes/back/sbadmin/vendor/jquery-easing/jquery.easing.compatibility.js
+pythoncms/static/themes/back/sbadmin/vendor/jquery-easing/jquery.easing.js
+pythoncms/static/themes/back/sbadmin/vendor/jquery-easing/jquery.easing.min.js
 pythoncms/static/themes/back/sneat/authbase.html
 pythoncms/static/themes/back/sneat/base.html
 pythoncms/static/themes/back/sneat/index.html
 pythoncms/static/themes/back/sneat/info.json
 pythoncms/static/themes/back/sneat/login.html
 pythoncms/static/themes/back/sneat/register.html
 pythoncms/static/themes/back/sneat/styles.css
```

### Comparing `pythoncms-1.2.2/setup.py` & `pythoncms-1.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         # These classifiers are *not* checked by 'pip install'. See instead
         # 'python_requires' below.
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     keywords="cms",  # Optional
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
```

