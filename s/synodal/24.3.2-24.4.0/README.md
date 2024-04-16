# Comparing `tmp/synodal-24.3.2.tar.gz` & `tmp/synodal-24.4.0.tar.gz`

## Comparing `synodal-24.3.2.tar` & `synodal-24.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    12380 2020-02-02 00:00:00.000000 synodal-24.3.2/synodal.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 synodal-24.3.2/tasks.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 synodal-24.3.2/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 synodal-24.3.2/COPYING
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 synodal-24.3.2/README.rst
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 synodal-24.3.2/pyproject.toml
--rw-r--r--   0        0        0    44701 2020-02-02 00:00:00.000000 synodal-24.3.2/PKG-INFO
+-rw-r--r--   0        0        0    13635 2020-02-02 00:00:00.000000 synodal-24.4.0/synodal.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 synodal-24.4.0/tasks.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 synodal-24.4.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 synodal-24.4.0/COPYING
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 synodal-24.4.0/README.rst
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 synodal-24.4.0/pyproject.toml
+-rw-r--r--   0        0        0    44679 2020-02-02 00:00:00.000000 synodal-24.4.0/PKG-INFO
```

### Comparing `synodal-24.3.2/synodal.py` & `synodal-24.4.0/synodal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
-# code generated 2024-03-19 14:39:23.585016 by make_code.py script of synodal
+# code generated 2024-04-16 08:42:25.569834 by make_code.py script of synodal
 # yapf: disable
 
 
 from collections import namedtuple
 
 repo_fields = ("nickname", "package_name", "git_repo", "settings_module",
     "front_end", "extra_deps", "public_url", "verbose_name", "description")
@@ -30,21 +30,25 @@
  Repository(nickname='ug', package_name='', git_repo='https://gitlab.com/lino-framework/ug.git', settings_module='', front_end='', extra_deps=[], public_url='https://using.lino-framework.org/', verbose_name=None, description=None),
  Repository(nickname='hg', package_name='', git_repo='https://gitlab.com/lino-framework/hg.git', settings_module='', front_end='', extra_deps=[], public_url='https://hosting.lino-framework.org/', verbose_name=None, description=None),
  Repository(nickname='lf', package_name='', git_repo='https://gitlab.com/lino-framework/lf.git', settings_module='', front_end='', extra_deps=[], public_url='https://www.lino-framework.org/', verbose_name=None, description=None),
  Repository(nickname='ss', package_name='', git_repo='https://gitlab.com/synodalsoft/ss.git', settings_module='', front_end='', extra_deps=[], public_url='https://www.synodalsoft.net/', verbose_name=None, description=None),
  Repository(nickname='algus', package_name='', git_repo='https://gitlab.com/lino-framework/algus.git', settings_module='', front_end='', extra_deps=[], public_url='', verbose_name=None, description=None),
  Repository(nickname='min1', package_name='', git_repo='', settings_module='lino_book.projects.min1.settings', front_end='', extra_deps=[], public_url='', verbose_name='yet another Lino application', description=None),
  Repository(nickname='min2', package_name='', git_repo='', settings_module='lino_book.projects.min2.settings', front_end='', extra_deps=[], public_url='', verbose_name='yet another Lino application', description=None),
- Repository(nickname='cosi4', package_name='', git_repo='', settings_module='lino_book.projects.cosi4.settings', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/cosi4.html', verbose_name=None, description=None),
- Repository(nickname='cosi5', package_name='', git_repo='', settings_module='lino_book.projects.cosi5.settings', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/cosi5.html', verbose_name=None, description=None),
- Repository(nickname='cosi_ee', package_name='', git_repo='', settings_module='lino_book.projects.cosi_ee.settings', front_end='', extra_deps=[], public_url='', verbose_name='Lino Così', description="Così! That's how we love accounting! A simple accounting application."),
- Repository(nickname='lydia', package_name='', git_repo='', settings_module='lino_book.projects.lydia.settings.demo', front_end='', extra_deps=[], public_url='', verbose_name='Lino Tera', description='A Lino for managing therapeutic centres'),
- Repository(nickname='noi1r', package_name='', git_repo='', settings_module='lino_book.projects.noi1r.settings', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/noi1r.html', verbose_name=None, description=None),
- Repository(nickname='chatter', package_name='', git_repo='', settings_module='lino_book.projects.chatter.settings', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/chatter.html', verbose_name=None, description=None),
- Repository(nickname='polly', package_name='', git_repo='', settings_module='lino_book.projects.polly.settings.demo', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/polly.html', verbose_name=None, description=None),
+ Repository(nickname='cosi4', package_name='', git_repo='', settings_module='lino_book.projects.cosi4.settings', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/cosi4.html', verbose_name=None, description='a Lino Così for Uruguay'),
+ Repository(nickname='cosi5', package_name='', git_repo='', settings_module='lino_book.projects.cosi5.settings', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/cosi5.html', verbose_name=None, description='a Lino Così for Bangladesh'),
+ Repository(nickname='roger', package_name='', git_repo='', settings_module='lino_book.projects.roger.settings.demo', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/roger.html', verbose_name=None, description='A customized Lino Voga site'),
+ Repository(nickname='human', package_name='', git_repo='', settings_module='lino_book.projects.human.settings', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/human.html', verbose_name=None, description='Testing some human properties'),
+ Repository(nickname='cosi_ee', package_name='', git_repo='', settings_module='lino_book.projects.cosi_ee.settings', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/cosi_ee.html', verbose_name=None, description='A Lino Così for Estonia'),
+ Repository(nickname='pierre', package_name='', git_repo='', settings_module='lino_book.projects.pierre.settings.demo', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/pierre.html', verbose_name=None, description='A Lino Così for Belgium (FR)'),
+ Repository(nickname='apc', package_name='', git_repo='', settings_module='lino_book.projects.apc.settings.demo', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/apc.html', verbose_name=None, description='A Lino Così for Belgium (DE)'),
+ Repository(nickname='lydia', package_name='', git_repo='', settings_module='lino_book.projects.lydia.settings.demo', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/lydia.html', verbose_name=None, description='A customized Lino Tera site'),
+ Repository(nickname='noi1r', package_name='', git_repo='', settings_module='lino_book.projects.noi1r.settings', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/noi1r.html', verbose_name=None, description='noi1e with React front end'),
+ Repository(nickname='chatter', package_name='', git_repo='', settings_module='lino_book.projects.chatter.settings', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/chatter.html', verbose_name=None, description='an instant messaging system'),
+ Repository(nickname='polly', package_name='', git_repo='', settings_module='lino_book.projects.polly.settings.demo', front_end='', extra_deps=[], public_url='https://dev.lino-framework.org/projects/polly.html', verbose_name=None, description='A little polls manager'),
  Repository(nickname='std', package_name='', git_repo='', settings_module='lino.projects.std.settings', front_end='', extra_deps=[], public_url='', verbose_name='yet another Lino application', description=None),
  Repository(nickname='amici', package_name='lino-amici', git_repo='https://gitlab.com/lino-framework/amici', settings_module='lino_amici.lib.amici.settings', front_end='', extra_deps=['lino', 'xl'], public_url='', verbose_name='Lino Amici', description='Manage your family contacts'),
  Repository(nickname='avanti', package_name='lino-avanti', git_repo='https://gitlab.com/lino-framework/avanti', settings_module='lino_avanti.lib.avanti.settings', front_end='', extra_deps=['lino', 'xl'], public_url='', verbose_name='Lino Avanti', description='Manage the integration course of immigrants in East Belgium'),
  Repository(nickname='cms', package_name='lino-cms', git_repo='https://gitlab.com/lino-framework/cms', settings_module='lino_cms.lib.cms.settings', front_end='', extra_deps=['lino', 'xl'], public_url='', verbose_name='Lino CMS', description='Manage the content of your website'),
  Repository(nickname='care', package_name='lino-care', git_repo='https://gitlab.com/lino-framework/care', settings_module='lino_care.lib.care.settings', front_end='', extra_deps=['lino', 'xl'], public_url='', verbose_name='Lino Care', description='Manage a network of helpers.'),
  Repository(nickname='cosi', package_name='lino-cosi', git_repo='https://gitlab.com/lino-framework/cosi', settings_module='lino_cosi.lib.cosi.settings', front_end='', extra_deps=['lino', 'xl'], public_url='', verbose_name='Lino Così', description="Così! That's how we love accounting! A simple accounting application."),
  Repository(nickname='mentori', package_name='lino-mentori', git_repo='https://gitlab.com/lino-framework/mentori', settings_module='lino_mentori.lib.mentori.settings', front_end='', extra_deps=['lino', 'xl'], public_url='', verbose_name='Lino Mentori', description=None),
@@ -56,19 +60,19 @@
  Repository(nickname='vilma', package_name='lino-vilma', git_repo='https://gitlab.com/lino-framework/vilma', settings_module='lino_vilma.lib.vilma.settings', front_end='', extra_deps=['lino', 'xl'], public_url='', verbose_name='Lino Vilma', description='Manage contacts, resources and skills of a village community'),
  Repository(nickname='voga', package_name='lino-voga', git_repo='https://gitlab.com/lino-framework/voga', settings_module='lino_voga.lib.voga.settings', front_end='', extra_deps=['lino', 'xl'], public_url='', verbose_name='Lino Voga', description='A Lino Django application for managing courses, participants and meeting rooms'),
  Repository(nickname='weleup', package_name='lino-weleup', git_repo='https://gitlab.com/lino-framework/weleup', settings_module='lino_weleup.settings', front_end='', extra_deps=['lino', 'xl', 'welfare'], public_url='', verbose_name='Lino Welfare Eupen', description='A Lino Django application for the PCSW of Eupen'),
  Repository(nickname='welcht', package_name='lino-welcht', git_repo='https://gitlab.com/lino-framework/welcht', settings_module='lino_welcht.settings', front_end='', extra_deps=['lino', 'xl', 'welfare'], public_url='', verbose_name='Lino Welfare Châtelet', description='A Lino Django application for the PCSW of Châtelet')]
 
 REPOS_DICT = {r.nickname: r for r in REPOS_LIST}
 
-FRONT_ENDS = [a for a in KNOWN_REPOS if a.front_end]
+FRONT_ENDS = {r.front_end: r for r in KNOWN_REPOS if r.front_end}
 
-PUBLIC_SITES = [PublicSite(url='https://voga1r.lino-framework.org', settings_module='lino_voga.lib.voga.settings', default_ui='lino.modlib.extjs'),
- PublicSite(url='https://voga1e.lino-framework.org', settings_module='lino_voga.lib.voga.settings', default_ui='lino_react.react'),
- PublicSite(url='https://cosi1e.lino-framework.org', settings_module='lino_cosi.lib.cosi.settings', default_ui='lino.modlib.extjs'),
+PUBLIC_SITES = [PublicSite(url='https://voga1e.lino-framework.org', settings_module='lino_voga.lib.voga.settings', default_ui='lino.modlib.extjs'),
+ PublicSite(url='https://voga1r.lino-framework.org', settings_module='lino_voga.lib.voga.settings', default_ui='lino_react.react'),
+ PublicSite(url='https://cosi1e.lino-framework.org', settings_module='lino_cosi.lib.cosi.settings', default_ui='lino_react.react'),
  PublicSite(url='https://noi1r.lino-framework.org', settings_module='lino_noi.lib.noi.settings', default_ui='lino_react.react'),
  PublicSite(url='https://weleup1.mylino.net', settings_module='lino_weleup.settings', default_ui='lino.modlib.extjs'),
  PublicSite(url='https://welcht1.mylino.net', settings_module='lino_welcht.settings', default_ui='lino.modlib.extjs')]
 
 SPHINX_EXTLINKS = {'ticket': ('https://jane.mylino.net/#/api/tickets/PublicTickets/%s', '#%s')}
 
 # end of generated code
```

### Comparing `synodal-24.3.2/.gitignore` & `synodal-24.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `synodal-24.3.2/COPYING` & `synodal-24.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `synodal-24.3.2/README.rst` & `synodal-24.4.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,80 +3,81 @@
 =======================
 
 A lightweight Python package with metadata about the code repositories of the
 `Synodalsoft project <https://www.synodalsoft.net>`__.
 
 Source code repository: https://gitlab.com/lino-framework/synodal
 
-Documentation for the maintained: https://dev.lino-framework.org/specs/synodal/index.html
+Documentation for the maintainer:
+https://dev.lino-framework.org/specs/synodal/index.html
 
 Usage examples:
 
 >>> import synodal
->>> # help(synodal.Repository)
 >>> from synodal import KNOWN_REPOS, REPOS_DICT, FRONT_ENDS, PUBLIC_SITES
 >>> r = REPOS_DICT['lino']
 >>> print(r.git_repo)
 https://gitlab.com/lino-framework/lino.git
 
 >>> synodal.Repository._fields
 ('nickname', 'package_name', 'git_repo', 'settings_module', 'front_end', 'extra_deps', 'public_url', 'verbose_name', 'description')
 >>> synodal.PublicSite._fields
 ('url', 'settings_module', 'default_ui')
 
->>> for r in FRONT_ENDS:
+>>> for r in FRONT_ENDS.values():
 ...     print("{r.nickname} : {r.front_end}".format(r=r))
 lino : lino.modlib.extjs
 react : lino_react.react
 openui5 : lino_openui5.openui5
 
-
 >>> from importlib import import_module
 >>> for ps in PUBLIC_SITES:
 ...     m = import_module(ps.settings_module)
 ...     print("{ps.url} : {m.Site.verbose_name} using {ps.default_ui}".format(
 ...        ps=ps, m=m))
-https://voga1r.lino-framework.org : Lino Voga using lino.modlib.extjs
-https://voga1e.lino-framework.org : Lino Voga using lino_react.react
-https://cosi1e.lino-framework.org : Lino Così using lino.modlib.extjs
+https://voga1e.lino-framework.org : Lino Voga using lino.modlib.extjs
+https://voga1r.lino-framework.org : Lino Voga using lino_react.react
+https://cosi1e.lino-framework.org : Lino Così using lino_react.react
 https://noi1r.lino-framework.org : Lino Noi using lino_react.react
 https://weleup1.mylino.net : Lino Welfare Eupen using lino.modlib.extjs
 https://welcht1.mylino.net : Lino Welfare Châtelet using lino.modlib.extjs
 
+
 >>> from lino.utils.code import analyze_rst
 >>> packages = [r.package_name.replace("-","_") for r in KNOWN_REPOS if r.package_name]
 >>> print(analyze_rst(*packages))  #doctest: +SKIP
 ============== ============ =========== =============== ============= =======
  name           code lines   doc lines   comment lines   total lines   files
 -------------- ------------ ----------- --------------- ------------- -------
  atelier        1.1k         847         388             3k            16
  etgen          511          727         300             1.9k          13
  eidreader      88           118         54              307           5
  commondata     7k           25          42              7k            12
- getlino        526          1.2k        245             2k            13
- lino           32k          22k         10k             79k           356
- lino_xl        45k          14k         12k             83k           523
+ getlino        528          1.2k        241             2k            13
+ lino           32k          22k         10k             79k           357
+ lino_xl        45k          14k         12k             83k           514
  lino_welfare   40k          9k          4k              60k           371
- lino_react     907          488         242             1.9k          8
+ lino_react     907          490         244             1.9k          8
  lino_openui5   222          668         235             1.4k          19
- lino_book      23k          3k          2k              32k           643
+ lino_book      23k          3k          2k              32k           639
  lino_amici     6k           238         393             7k            109
  lino_avanti    1.2k         456         562             3k            52
  lino_cms       193          85          77              469           22
- lino_care      849          393         791             2k            41
+ lino_care      849          390         791             2k            41
  lino_cosi      240          138         155             690           36
  lino_mentori   425          293         230             1.2k          37
- lino_noi       1.1k         727         890             3k            52
+ lino_noi       1.1k         724         915             3k            52
  lino_presto    1.0k         614         540             3k            55
  lino_pronto    775          199         143             1.4k          46
  lino_tera      1.7k         674         1.2k            5k            77
  lino_shop      359          148         111             795           21
  lino_vilma     467          204         264             1.1k          14
  lino_voga      2k           1.7k        797             6k            59
- lino_weleup    136          144         95              452           9
- lino_welcht    779          206         344             1.7k          27
- total          168k         59k         36k             308k          3k
+ lino_weleup    136          146         95              455           9
+ lino_welcht    781          206         344             1.7k          27
+ total          168k         58k         36k             308k          3k
 ============== ============ =========== =============== ============= =======
 <BLANKLINE>
 
 
+
 Above code snippet is skipped because the values change often.
```

### Comparing `synodal-24.3.2/pyproject.toml` & `synodal-24.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = 'synodal'
-version = '24.3.2'
+version = '24.4.0'
 description = "Metadata about the Synodalsoft project"
 
 install_requires = []
 # scripts=['synodal.py']
 readme = "README.rst"
 # py_modules = ['synodal']
```

### Comparing `synodal-24.3.2/PKG-INFO` & `synodal-24.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: synodal
-Version: 24.3.2
+Version: 24.4.0
 Summary: Metadata about the Synodalsoft project
 Project-URL: Homepage, https://www.synodalsoft.net
 Project-URL: Repository, https://gitlab.com/lino-framework/synodal
 Author-email: Rumma & Ko Ltd <info@lino-framework.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
@@ -681,80 +681,81 @@
 =======================
 
 A lightweight Python package with metadata about the code repositories of the
 `Synodalsoft project <https://www.synodalsoft.net>`__.
 
 Source code repository: https://gitlab.com/lino-framework/synodal
 
-Documentation for the maintained: https://dev.lino-framework.org/specs/synodal/index.html
+Documentation for the maintainer:
+https://dev.lino-framework.org/specs/synodal/index.html
 
 Usage examples:
 
 >>> import synodal
->>> # help(synodal.Repository)
 >>> from synodal import KNOWN_REPOS, REPOS_DICT, FRONT_ENDS, PUBLIC_SITES
 >>> r = REPOS_DICT['lino']
 >>> print(r.git_repo)
 https://gitlab.com/lino-framework/lino.git
 
 >>> synodal.Repository._fields
 ('nickname', 'package_name', 'git_repo', 'settings_module', 'front_end', 'extra_deps', 'public_url', 'verbose_name', 'description')
 >>> synodal.PublicSite._fields
 ('url', 'settings_module', 'default_ui')
 
->>> for r in FRONT_ENDS:
+>>> for r in FRONT_ENDS.values():
 ...     print("{r.nickname} : {r.front_end}".format(r=r))
 lino : lino.modlib.extjs
 react : lino_react.react
 openui5 : lino_openui5.openui5
 
-
 >>> from importlib import import_module
 >>> for ps in PUBLIC_SITES:
 ...     m = import_module(ps.settings_module)
 ...     print("{ps.url} : {m.Site.verbose_name} using {ps.default_ui}".format(
 ...        ps=ps, m=m))
-https://voga1r.lino-framework.org : Lino Voga using lino.modlib.extjs
-https://voga1e.lino-framework.org : Lino Voga using lino_react.react
-https://cosi1e.lino-framework.org : Lino Così using lino.modlib.extjs
+https://voga1e.lino-framework.org : Lino Voga using lino.modlib.extjs
+https://voga1r.lino-framework.org : Lino Voga using lino_react.react
+https://cosi1e.lino-framework.org : Lino Così using lino_react.react
 https://noi1r.lino-framework.org : Lino Noi using lino_react.react
 https://weleup1.mylino.net : Lino Welfare Eupen using lino.modlib.extjs
 https://welcht1.mylino.net : Lino Welfare Châtelet using lino.modlib.extjs
 
+
 >>> from lino.utils.code import analyze_rst
 >>> packages = [r.package_name.replace("-","_") for r in KNOWN_REPOS if r.package_name]
 >>> print(analyze_rst(*packages))  #doctest: +SKIP
 ============== ============ =========== =============== ============= =======
  name           code lines   doc lines   comment lines   total lines   files
 -------------- ------------ ----------- --------------- ------------- -------
  atelier        1.1k         847         388             3k            16
  etgen          511          727         300             1.9k          13
  eidreader      88           118         54              307           5
  commondata     7k           25          42              7k            12
- getlino        526          1.2k        245             2k            13
- lino           32k          22k         10k             79k           356
- lino_xl        45k          14k         12k             83k           523
+ getlino        528          1.2k        241             2k            13
+ lino           32k          22k         10k             79k           357
+ lino_xl        45k          14k         12k             83k           514
  lino_welfare   40k          9k          4k              60k           371
- lino_react     907          488         242             1.9k          8
+ lino_react     907          490         244             1.9k          8
  lino_openui5   222          668         235             1.4k          19
- lino_book      23k          3k          2k              32k           643
+ lino_book      23k          3k          2k              32k           639
  lino_amici     6k           238         393             7k            109
  lino_avanti    1.2k         456         562             3k            52
  lino_cms       193          85          77              469           22
- lino_care      849          393         791             2k            41
+ lino_care      849          390         791             2k            41
  lino_cosi      240          138         155             690           36
  lino_mentori   425          293         230             1.2k          37
- lino_noi       1.1k         727         890             3k            52
+ lino_noi       1.1k         724         915             3k            52
  lino_presto    1.0k         614         540             3k            55
  lino_pronto    775          199         143             1.4k          46
  lino_tera      1.7k         674         1.2k            5k            77
  lino_shop      359          148         111             795           21
  lino_vilma     467          204         264             1.1k          14
  lino_voga      2k           1.7k        797             6k            59
- lino_weleup    136          144         95              452           9
- lino_welcht    779          206         344             1.7k          27
- total          168k         59k         36k             308k          3k
+ lino_weleup    136          146         95              455           9
+ lino_welcht    781          206         344             1.7k          27
+ total          168k         58k         36k             308k          3k
 ============== ============ =========== =============== ============= =======
 <BLANKLINE>
 
 
+
 Above code snippet is skipped because the values change often.
```

