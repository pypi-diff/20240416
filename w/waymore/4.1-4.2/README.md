# Comparing `tmp/waymore-4.1.tar.gz` & `tmp/waymore-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waymore-4.1.tar", last modified: Tue Apr  2 16:37:57 2024, max compression
+gzip compressed data, was "waymore-4.2.tar", last modified: Tue Apr 16 12:51:10 2024, max compression
```

## Comparing `waymore-4.1.tar` & `waymore-4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-02 16:37:57.147115 waymore-4.1/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-20 18:00:02.000000 waymore-4.1/LICENSE
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-04-02 16:37:57.135640 waymore-4.1/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    46794 2024-04-02 16:34:35.000000 waymore-4.1/README.md
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-02 16:37:57.148137 waymore-4.1/setup.cfg
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2142 2024-04-01 16:43:41.000000 waymore-4.1/setup.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-02 16:37:56.924503 waymore-4.1/waymore/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-04-02 16:35:08.000000 waymore-4.1/waymore/__init__.py
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)   166754 2024-04-02 16:34:25.000000 waymore-4.1/waymore/waymore.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-02 16:37:57.117277 waymore-4.1/waymore.egg-info/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      253 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/SOURCES.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/dependency_links.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       49 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/entry_points.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       63 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/requires.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        8 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/top_level.txt
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-16 12:51:10.357043 waymore-4.2/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-20 18:00:02.000000 waymore-4.2/LICENSE
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-04-16 12:51:10.338303 waymore-4.2/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    46794 2024-04-16 12:25:53.000000 waymore-4.2/README.md
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-16 12:51:10.359349 waymore-4.2/setup.cfg
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2142 2024-04-01 16:43:41.000000 waymore-4.2/setup.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-16 12:51:10.094560 waymore-4.2/waymore/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-04-16 12:25:47.000000 waymore-4.2/waymore/__init__.py
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)   167332 2024-04-16 12:32:29.000000 waymore-4.2/waymore/waymore.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-16 12:51:10.319250 waymore-4.2/waymore.egg-info/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      253 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       49 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/entry_points.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       63 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/requires.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        8 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/top_level.txt
```

### Comparing `waymore-4.1/LICENSE` & `waymore-4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `waymore-4.1/PKG-INFO` & `waymore-4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waymore
-Version: 4.1
+Version: 4.2
 Summary: Find way more from the Wayback Machine, Common Crawl, Alien Vault OTX, URLScan & VirusTotal!
 Home-page: https://github.com/xnl-h4ck3r/waymore
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
@@ -12,15 +12,15 @@
 Requires-Dist: termcolor
 Requires-Dist: psutil
 Requires-Dist: urlparse3
 Requires-Dist: tldextract
 
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.1
+## About - v4.2
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
```

### Comparing `waymore-4.1/README.md` & `waymore-4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.1
+## About - v4.2
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
```

### Comparing `waymore-4.1/setup.py` & `waymore-4.2/setup.py`

 * *Files identical despite different names*

### Comparing `waymore-4.1/waymore/waymore.py` & `waymore-4.2/waymore/waymore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1776,31 +1776,39 @@
                     return
                 except Exception as e:
                     writerr(colored(getSPACER('[ ERR ] Error getting response for page ' + page + ' - ' + str(e)),'red'))
                     resp = None
                     return
             
             # Get the URLs and MIME types. Each line is a separate JSON string
-            for line in resp.iter_lines():
-                results = line.decode("utf-8")
-                # Only get MIME Types if --verbose option was selected
-                if verbose():
-                    try:
-                        linkMimes.add(str(results).split(' ')[2])
-                    except Exception as e:
-                        if verbose():
-                            writerr(colored(getSPACER('ERROR processWayBackPage 2: Cannot get MIME type from line: ' + str(line)),'red'))
-                            write(resp.text)
-                try:
+            try:
+                for line in resp.iter_lines():
+                    results = line.decode("utf-8")
                     foundUrl = fixArchiveOrgUrl(str(results).split(' ')[1])
-                    linksFoundAdd(foundUrl)
-                except Exception as e:
-                    if verbose():
-                        writerr(colored(getSPACER('ERROR processWayBackPage 3: Cannot get link from line: ' + str(line)),'red'))         
-                        write(resp.text)       
+                    
+                    # Check the URL exclusions
+                    match = re.search(r'('+re.escape(FILTER_URL).replace(',','|')+')', foundUrl, flags=re.IGNORECASE)
+                    if match is None:
+                        # Only get MIME Types if --verbose option was selected
+                        if verbose():
+                            try:
+                                linkMimes.add(str(results).split(' ')[2])
+                            except Exception as e:
+                                if verbose():
+                                    writerr(colored(getSPACER('ERROR processWayBackPage 2: Cannot get MIME type from line: ' + str(line)),'red'))
+                                    write(resp.text)
+                        try:
+                            linksFoundAdd(foundUrl)
+                        except Exception as e:
+                            if verbose():
+                                writerr(colored(getSPACER('ERROR processWayBackPage 3: Cannot get link from line: ' + str(line)),'red'))         
+                                write(resp.text)       
+            except Exception as e:
+                if verbose():
+                    writerr(colored(getSPACER('ERROR processWayBackPage 4: ' + str(line)),'red'))   
         else:
             pass
     except Exception as e:
         if verbose():
             writerr(colored("ERROR processWayBackPage 1: " + str(e), "red"))
     
 def getWaybackUrls():
@@ -2418,20 +2426,20 @@
             
             # Set the collapse parameter value in the archive.org URL. From the Wayback API docs:
             # "A new form of filtering is the option to 'collapse' results based on a field, or a substring of a field.
             # Collapsing is done on adjacent cdx lines where all captures after the first one that are duplicate are filtered out.
             # This is useful for filtering out captures that are 'too dense' or when looking for unique captures."
             if args.capture_interval == 'none': # get all
                 collapse = ''
-            elif args.capture_interval == 'h': # get at most 1 capture per hour
-                collapse = 'timestamp:10'
-            elif args.capture_interval == 'd': # get at most 1 capture per day
-                collapse = 'timestamp:8'
-            elif args.capture_interval == 'm': # get at most 1 capture per month
-                collapse = 'timestamp:6'
+            elif args.capture_interval == 'h': # get at most 1 capture per URL per hour
+                collapse = 'timestamp:10,original'
+            elif args.capture_interval == 'd': # get at most 1 capture per URL per day
+                collapse = 'timestamp:8,original'
+            elif args.capture_interval == 'm': # get at most 1 capture per URL per month
+                collapse = 'timestamp:6,original'
 
             url = WAYBACK_URL.replace('{DOMAIN}',subs + quote(argsInput) + path).replace('{COLLAPSE}',collapse) + filterMIME + filterCode + filterLimit + filterFrom + filterTo + filterKeywords
                 
             if verbose():
                 write(colored('The archive URL requested to get responses: ','magenta')+colored(url+'\n','white'))
             
             if args.check_only:
```

### Comparing `waymore-4.1/waymore.egg-info/PKG-INFO` & `waymore-4.2/waymore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waymore
-Version: 4.1
+Version: 4.2
 Summary: Find way more from the Wayback Machine, Common Crawl, Alien Vault OTX, URLScan & VirusTotal!
 Home-page: https://github.com/xnl-h4ck3r/waymore
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
@@ -12,15 +12,15 @@
 Requires-Dist: termcolor
 Requires-Dist: psutil
 Requires-Dist: urlparse3
 Requires-Dist: tldextract
 
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.1
+## About - v4.2
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
```

