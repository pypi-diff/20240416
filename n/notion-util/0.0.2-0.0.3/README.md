# Comparing `tmp/notion-util-0.0.2.tar.gz` & `tmp/notion-util-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-util-0.0.2.tar", last modified: Sun Feb 18 03:49:30 2024, max compression
+gzip compressed data, was "notion-util-0.0.3.tar", last modified: Tue Apr 16 09:46:09 2024, max compression
```

## Comparing `notion-util-0.0.2.tar` & `notion-util-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 03:49:30.940809 notion-util-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-02-18 03:49:30.940809 notion-util-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-18 03:49:19.000000 notion-util-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 03:49:30.940809 notion-util-0.0.2/notion/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-18 03:49:19.000000 notion-util-0.0.2/notion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18073 2024-02-18 03:49:19.000000 notion-util-0.0.2/notion/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 03:49:30.940809 notion-util-0.0.2/notion_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-02-18 03:49:30.000000 notion-util-0.0.2/notion_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-18 03:49:30.000000 notion-util-0.0.2/notion_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 03:49:30.000000 notion-util-0.0.2/notion_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-18 03:49:30.000000 notion-util-0.0.2/notion_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-18 03:49:30.000000 notion-util-0.0.2/notion_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-18 03:49:30.940809 notion-util-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-02-18 03:49:19.000000 notion-util-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:46:09.056647 notion-util-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-16 09:46:09.056647 notion-util-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-16 09:45:55.000000 notion-util-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:46:09.056647 notion-util-0.0.3/notion/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 09:45:55.000000 notion-util-0.0.3/notion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19367 2024-04-16 09:45:55.000000 notion-util-0.0.3/notion/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:46:09.056647 notion-util-0.0.3/notion_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-16 09:46:08.000000 notion-util-0.0.3/notion_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-16 09:46:09.000000 notion-util-0.0.3/notion_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:46:08.000000 notion-util-0.0.3/notion_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 09:46:08.000000 notion-util-0.0.3/notion_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 09:46:08.000000 notion-util-0.0.3/notion_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:46:09.056647 notion-util-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 09:45:55.000000 notion-util-0.0.3/setup.py
```

### Comparing `notion-util-0.0.2/PKG-INFO` & `notion-util-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-util
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial Python API client for Notion.so
 Home-page: https://github.com/tatsu-i/notion-util
 Author: tatsu-i
 License: UNKNOWN
 Description: # Notion Util
         
         このプロジェクトは、Notion.soの非公式Python APIクライアントです。
```

### Comparing `notion-util-0.0.2/README.md` & `notion-util-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `notion-util-0.0.2/notion/util.py` & `notion-util-0.0.3/notion/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import os
 import re
 import csv
 import logging
 import requests
 from tempfile import mkdtemp
 
-# 環境変数からNotionのAPIキーを取得する
-NOTION_SECRET = os.getenv("NOTION_SECRET")
-
 
 def extract_notion_page_id(url):
     # Find URLs that starts with "https://www.notion.so" and extracts the UUID
     patterns = [
         r"https://www\.notion\.so/[^/]+/[^/]+-([a-f0-9]{32})",
         r"https://www\.notion\.so/[^/]+/([a-f0-9]{32})",
         r"https://www\.notion\.so/[^/]+-([a-f0-9]{32})",
@@ -21,23 +18,14 @@
     for pattern in patterns:
         match = re.search(pattern, url)
         if match:
             return match.group(1)
     return None
 
 
-# Notion APIのバージョン
-
-NOTION_HEADERS = {
-    "Authorization": f"Bearer {NOTION_SECRET}",
-    "Notion-Version": "2022-06-28",
-    "Content-Type": "application/json",
-}
-
-
 def extract_notion_page_ids(message):
     # "https://www.notion.so"で始まるURLを見つけてUUIDを抽出します
     patterns = [
         r"https://www\.notion\.so/[^/]+/[^/]+-([a-f0-9]{32})",
         r"https://www\.notion\.so/[^/]+/([a-f0-9]{32})",
         r"https://www\.notion\.so/[^/]+-([a-f0-9]{32})",
         r"https://www\.notion\.so/([a-f0-9]{32})",
@@ -47,269 +35,29 @@
     for pattern in patterns:
         matches = re.findall(pattern, message)
         if matches:
             page_ids.extend(matches)
     return page_ids
 
 
-# text content helper function
-def get_text_content(rich_text, recursive, depth):
-    text_content = ""
-    for element in rich_text:
-        text = element["plain_text"]
-        if element["type"] == "text":
-            # テキスト要素にリンクがある場合、Markdownリンク形式に変換
-            if element["text"]["link"] is not None:
-                url = element["text"]["link"]["url"]
-                if url is not None:
-                    text = f"[{text}]({url})\n"
-                    if recursive and depth <= 3:
-                        text += get_page_markdown(url, recursive, depth)
-        elif element["type"] == "mention" and element["href"]:
-            # メンションタイプの要素に対する処理（ページへのリンクなど）
-            url = element["href"]
-            text = f"[{text}]({url})\n"
-            if recursive and depth <= 3:
-                text += get_page_markdown(url, recursive, depth)
-        text_content += text
-    return text_content.strip()
-
-
-# 特定のブロックをMarkdownに変換する関数
-def block_to_markdown(block, recursive, depth):
-    block_type = block["type"]
-    content = ""
-
-    if block_type == "paragraph":
-        content = (
-            get_text_content(
-                block.get("paragraph", {}).get("rich_text", []), recursive, depth
-            )
-            + "\n"
-        )
-    elif block_type == "heading_1":
-        content = f"# {get_text_content(block.get('heading_1', {}).get('rich_text', []), recursive, depth)}\n"
-    elif block_type == "heading_2":
-        content = f"## {get_text_content(block.get('heading_2', {}).get('rich_text', []), recursive, depth)}\n"
-    elif block_type == "heading_3":
-        content = f"### {get_text_content(block.get('heading_3', {}).get('rich_text', []), recursive, depth)}\n"
-    elif block_type == "bulleted_list_item":
-        content = f"* {get_text_content(block.get('bulleted_list_item', {}).get('rich_text', []), recursive, depth)}\n"
-    elif block_type == "numbered_list_item":
-        content = f"1. {get_text_content(block.get('numbered_list_item', {}).get('rich_text', []), recursive, depth)}\n"
-    elif block_type == "quote":
-        content = f"> {get_text_content(block.get('quote', {}).get('rich_text', []), recursive, depth)}\n"
-    # コードブロックタイプの処理
-    elif block_type == "code":
-        code_content = get_text_content(
-            block.get("code", {}).get("rich_text", []), recursive, depth
-        )
-        language = block["code"].get("language", "")
-        content = f"```{language}\n{code_content}\n```\n"
-    # `table`ブロックタイプの処理
-    elif block_type == "table_row":
-        # テーブルの行を処理
-        row_cells = block["table_row"]["cells"]
-        row_content = []
-        for cell in row_cells:
-            cell_content = get_text_content(cell, recursive, depth)
-            row_content.append(cell_content)
-        content = f"| {' | '.join(row_content)} |\n"
-    # 他のブロックタイプの処理をここに追加...
-
-    return content
-
-
-# ブロックを取得してMarkdownに変換する関数
-def retrieve_blocks(page_id, recursive, level=0, depth=0):
-    read_url = f"https://api.notion.com/v1/blocks/{page_id}/children"
-    markdown_content = ""
-    while True:
-        response = requests.get(read_url, headers=NOTION_HEADERS)
-        if response.status_code != 200:
-            logging.error(
-                f"Failed to read blocks with status code {response.status_code}: {response.text} {read_url}"
-            )
-            break
-
-        data = response.json()
-        blocks = data.get("results", [])
-        for block in blocks:
-            markdown_content += "  " * level
-            markdown_content += block_to_markdown(block, recursive, depth)
-            if block.get("has_children", False):
-                markdown_content += retrieve_blocks(
-                    block["id"], recursive, level + 1, depth
-                )
-
-        # 'has_more'と'next_cursor'をチェックして全てのブロックを読み込む
-        if not data.get("has_more", False):
-            break
-        read_url = f"{read_url}&start_cursor={data.get('next_cursor')}"
-
-    return markdown_content
-
-
-def get_page_markdown(url, recursive=False, depth=0):
-    if url.find("https://www.notion.so") == -1:
-        return ""
-    page_id = extract_notion_page_id(url)
-    response = requests.get(
-        f"https://api.notion.com/v1/pages/{page_id}", headers=NOTION_HEADERS
-    )
-    page_info = response.json()
-
-    if page_info.get("object") == "error":
-        logging.error(page_info)
-        return ""
-
-    else:
-        return retrieve_blocks(page_id, recursive, 0, depth + 1).strip()
-
-
-def get_page_database(url):
-    if url.find("https://www.notion.so") == -1:
-        return ""
-    database_id = extract_notion_page_id(url)
-
-    response = requests.post(
-        f"https://api.notion.com/v1/databases/{database_id}/query",
-        headers=NOTION_HEADERS,
-    )
-    data = response.json()
-
-    # ヘッダーの抽出
-    headers = set()
-    if data.get("object") == "error":
-        logging.error(data)
-        return ""
-
-    for page in data["results"]:
-        headers.update(page["properties"].keys())
-
-    # ヘッダーをリストに変換し、ソート
-    headers = sorted(list(headers))
-
-    # 各レコードのデータを取得
-    table_data = []
-
-    for page in data["results"]:
-        row = []
-        for header in headers:
-            property = page["properties"].get(header)
-            if property:
-                property_type = property.get("type")
-                if property_type == "title":
-                    title_list = property.get("title", [])
-                    title = title_list[0].get("plain_text", "") if title_list else ""
-                    url = page["url"]
-                    row.append(f"[{title}]({url})")
-                elif property_type == "multi_select":
-                    tags = [tag["name"] for tag in property.get("multi_select", [])]
-                    row.append(",".join(tags))
-                elif property_type in ["last_edited_time", "created_time"]:
-                    user_info = property.get(property.get("type", ""), "") or ""
-                    row.append(user_info)
-                elif property_type in ["last_edited_by", "created_by"]:
-                    user_info = property.get(property.get("type", ""), {}) or {}
-                    row.append(f'user_{user_info["id"]}')
-                elif property_type == "select":
-                    select_info = property.get("select", {}) or {}
-                    row.append(select_info.get("name") or "")
-                elif property_type == "relation":
-                    relation_info = ", ".join(
-                        [f"user_{rel['id']}" for rel in property.get("relation", [])]
-                    )
-                    row.append(relation_info)
-                elif property_type == "url":
-                    url_info = property.get("url", "") or ""
-                    row.append(url_info)
-                elif property_type == "status":
-                    status_info = property.get("status", {}).get("name", "") or ""
-                    row.append(status_info)
-                elif property_type == "people":
-                    people = property.get("people", [])
-                    if people:
-                        peoples = [f"user_{p['id']}" for p in people]
-                        row.append(",".join(peoples))
-                elif property_type == "date":
-                    pdate = property.get("date", {})
-                    if pdate:
-                        start = pdate.get("start", "")
-                        end = pdate.get("end", "")
-                        row.append(f"start:{start} end:{end}")
-                elif property_type == "rich_text":
-                    rich_text = property.get("plain_text", "")
-                    row.append(rich_text)
-                else:
-                    # print(property_type, property)
-                    row.append("")
-            else:
-                row.append(str(property.get(property.get("type", ""), "")))
-
-        table_data.append(row)
-
-    # 一時ディレクトリを作成
-    temp_dir = mkdtemp()
-    csv_file_path = os.path.join(temp_dir, f"notion-database-{database_id}.csv")
-
-    with open(csv_file_path, "w", newline="") as csvfile:
-        writer = csv.writer(csvfile)
-        writer.writerow(headers)
-        for row in table_data:
-            writer.writerow(row)
-
-    return csv_file_path
-
-
-def create_notion_page(database_id, page_title, properties={}):
-    create_url = "https://api.notion.com/v1/pages"
-
-    # ページのタイトルを設定
-    data = {
-        "parent": {"database_id": database_id},
-        "properties": {
-            "Name": {"title": [{"text": {"content": page_title}}]},
-            **properties,
-        },
-        "children": [],
-    }
-
-    response = requests.post(create_url, headers=NOTION_HEADERS, json=data)
-    if response.status_code != 200:
-        raise Exception(
-            f"Failed to create page with status code {response.status_code}: {response.text}"
-        )
-
-    return response.json()
-
-
-def append_blocks_to_page(page_id, blocks):
-    append_url = f"https://api.notion.com/v1/blocks/{page_id}/children"
-
-    data = {"children": blocks}
-
-    response = requests.patch(append_url, headers=NOTION_HEADERS, json=data)
-    if response.status_code != 200:
-        message = f"Failed to append blocks with status code {response.status_code}: {response.text}"
-        logging.error(f"{message}\n{data}")
-        raise Exception(message)
-
-
 def markdown_to_notion_blocks(markdown_text):
     lines = markdown_text.split("\n")
     blocks = []
     current_indent_level = 0
-    list_item_stack = [[] for _ in range(10)]  # 10レベルのネストに対応するスタックを用意
+    list_item_stack = [
+        [] for _ in range(10)
+    ]  # 10レベルのネストに対応するスタックを用意
     code_block_open = False
     code_language = ""
     code_content = []
 
     for line in lines:
-        if line.strip() == "" and not code_block_open:  # 空行はスキップ（コードブロック外）
+        if (
+            line.strip() == "" and not code_block_open
+        ):  # 空行はスキップ（コードブロック外）
             continue
 
         # コードブロックの処理
         if line.startswith("```"):
             if code_block_open:  # コードブロックの終わり
                 block = {
                     "object": "block",
@@ -472,7 +220,261 @@
             if (
                 "children" in block.get("bulleted_list_item", {})
                 and not block["bulleted_list_item"]["children"]
             ):
                 del block["bulleted_list_item"]["children"]
 
     return blocks
+
+
+class Notion:
+    def __init__(self, notion_secret=os.getenv("NOTION_SECRET")):
+        # 環境変数からNotionのAPIキーを取得する
+        self.notion_secret = notion_secret
+        # Notion APIのバージョン
+        self.notion_headers = {
+            "Authorization": f"Bearer {self.notion_secret}",
+            "Notion-Version": "2022-06-28",
+            "Content-Type": "application/json",
+        }
+
+    # ブロックを取得してMarkdownに変換する関数
+    def retrieve_blocks(self, page_id, recursive, level=0, depth=0):
+        read_url = f"https://api.notion.com/v1/blocks/{page_id}/children"
+        markdown_content = ""
+        while True:
+            response = requests.get(read_url, headers=self.notion_headers)
+            if response.status_code != 200:
+                logging.error(
+                    f"Failed to read blocks with status code {response.status_code}: {response.text} {read_url}"
+                )
+                break
+
+            data = response.json()
+            blocks = data.get("results", [])
+            for block in blocks:
+                markdown_content += "  " * level
+                markdown_content += self.block_to_markdown(block, recursive, depth)
+                if block.get("has_children", False):
+                    markdown_content += self.retrieve_blocks(
+                        block["id"], recursive, level + 1, depth
+                    )
+
+            # 'has_more'と'next_cursor'をチェックして全てのブロックを読み込む
+            if not data.get("has_more", False):
+                break
+            read_url = f"{read_url}&start_cursor={data.get('next_cursor')}"
+
+        return markdown_content
+
+    def get_page_markdown(self, url, recursive=False, depth=0):
+        if url.find("https://www.notion.so") == -1:
+            return ""
+        page_id = extract_notion_page_id(url)
+        response = requests.get(
+            f"https://api.notion.com/v1/pages/{page_id}", headers=self.notion_headers
+        )
+        page_info = response.json()
+
+        if page_info.get("object") == "error":
+            logging.error(page_info)
+            return ""
+
+        else:
+            return self.retrieve_blocks(page_id, recursive, 0, depth + 1).strip()
+
+    def get_page_database(self, url):
+        if url.find("https://www.notion.so") == -1:
+            return ""
+        database_id = extract_notion_page_id(url)
+
+        response = requests.post(
+            f"https://api.notion.com/v1/databases/{database_id}/query",
+            headers=self.notion_headers,
+        )
+        data = response.json()
+
+        # ヘッダーの抽出
+        headers = set()
+        if data.get("object") == "error":
+            logging.error(data)
+            return ""
+
+        for page in data["results"]:
+            headers.update(page["properties"].keys())
+
+        # ヘッダーをリストに変換し、ソート
+        headers = sorted(list(headers))
+
+        # 各レコードのデータを取得
+        table_data = []
+
+        for page in data["results"]:
+            row = []
+            for header in headers:
+                property = page["properties"].get(header)
+                if property:
+                    property_type = property.get("type")
+                    if property_type == "title":
+                        title_list = property.get("title", [])
+                        title = (
+                            title_list[0].get("plain_text", "") if title_list else ""
+                        )
+                        url = page["url"]
+                        row.append(f"[{title}]({url})")
+                    elif property_type == "multi_select":
+                        tags = [tag["name"] for tag in property.get("multi_select", [])]
+                        row.append(",".join(tags))
+                    elif property_type in ["last_edited_time", "created_time"]:
+                        user_info = property.get(property.get("type", ""), "") or ""
+                        row.append(user_info)
+                    elif property_type in ["last_edited_by", "created_by"]:
+                        user_info = property.get(property.get("type", ""), {}) or {}
+                        row.append(f'user_{user_info["id"]}')
+                    elif property_type == "select":
+                        select_info = property.get("select", {}) or {}
+                        row.append(select_info.get("name") or "")
+                    elif property_type == "relation":
+                        relation_info = ", ".join(
+                            [
+                                f"user_{rel['id']}"
+                                for rel in property.get("relation", [])
+                            ]
+                        )
+                        row.append(relation_info)
+                    elif property_type == "url":
+                        url_info = property.get("url", "") or ""
+                        row.append(url_info)
+                    elif property_type == "status":
+                        status_info = property.get("status", {}).get("name", "") or ""
+                        row.append(status_info)
+                    elif property_type == "people":
+                        people = property.get("people", [])
+                        if people:
+                            peoples = [f"user_{p['id']}" for p in people]
+                            row.append(",".join(peoples))
+                    elif property_type == "date":
+                        pdate = property.get("date", {})
+                        if pdate:
+                            start = pdate.get("start", "")
+                            end = pdate.get("end", "")
+                            row.append(f"start:{start} end:{end}")
+                    elif property_type == "rich_text":
+                        rich_text = property.get("plain_text", "")
+                        row.append(rich_text)
+                    else:
+                        # print(property_type, property)
+                        row.append("")
+                else:
+                    row.append(str(property.get(property.get("type", ""), "")))
+
+            table_data.append(row)
+
+        # 一時ディレクトリを作成
+        temp_dir = mkdtemp()
+        csv_file_path = os.path.join(temp_dir, f"notion-database-{database_id}.csv")
+
+        with open(csv_file_path, "w", newline="") as csvfile:
+            writer = csv.writer(csvfile)
+            writer.writerow(headers)
+            for row in table_data:
+                writer.writerow(row)
+
+        return csv_file_path
+
+    def create_notion_page(self, database_id, page_title, properties={}):
+        create_url = "https://api.notion.com/v1/pages"
+
+        # ページのタイトルを設定
+        data = {
+            "parent": {"database_id": database_id},
+            "properties": {
+                "Name": {"title": [{"text": {"content": page_title}}]},
+                **properties,
+            },
+            "children": [],
+        }
+
+        response = requests.post(create_url, headers=self.notion_headers, json=data)
+        if response.status_code != 200:
+            raise Exception(
+                f"Failed to create page with status code {response.status_code}: {response.text}"
+            )
+
+        return response.json()
+
+    def append_blocks_to_page(self, page_id, blocks):
+        append_url = f"https://api.notion.com/v1/blocks/{page_id}/children"
+
+        data = {"children": blocks}
+
+        response = requests.patch(append_url, headers=self.notion_headers, json=data)
+        if response.status_code != 200:
+            message = f"Failed to append blocks with status code {response.status_code}: {response.text}"
+            logging.error(f"{message}\n{data}")
+            raise Exception(message)
+
+    # text content helper function
+    def get_text_content(self, rich_text, recursive, depth):
+        text_content = ""
+        for element in rich_text:
+            text = element["plain_text"]
+            if element["type"] == "text":
+                # テキスト要素にリンクがある場合、Markdownリンク形式に変換
+                if element["text"]["link"] is not None:
+                    url = element["text"]["link"]["url"]
+                    if url is not None:
+                        text = f"[{text}]({url})\n"
+                        if recursive and depth <= 3:
+                            text += self.get_page_markdown(url, recursive, depth)
+            elif element["type"] == "mention" and element["href"]:
+                # メンションタイプの要素に対する処理（ページへのリンクなど）
+                url = element["href"]
+                text = f"[{text}]({url})\n"
+                if recursive and depth <= 3:
+                    text += self.get_page_markdown(url, recursive, depth)
+            text_content += text
+        return text_content.strip()
+
+    # 特定のブロックをMarkdownに変換する関数
+    def block_to_markdown(self, block, recursive, depth):
+        block_type = block["type"]
+        content = ""
+
+        if block_type == "paragraph":
+            content = (
+                self.get_text_content(
+                    block.get("paragraph", {}).get("rich_text", []), recursive, depth
+                )
+                + "\n"
+            )
+        elif block_type == "heading_1":
+            content = f"# {self.get_text_content(block.get('heading_1', {}).get('rich_text', []), recursive, depth)}\n"
+        elif block_type == "heading_2":
+            content = f"## {self.get_text_content(block.get('heading_2', {}).get('rich_text', []), recursive, depth)}\n"
+        elif block_type == "heading_3":
+            content = f"### {self.get_text_content(block.get('heading_3', {}).get('rich_text', []), recursive, depth)}\n"
+        elif block_type == "bulleted_list_item":
+            content = f"* {self.get_text_content(block.get('bulleted_list_item', {}).get('rich_text', []), recursive, depth)}\n"
+        elif block_type == "numbered_list_item":
+            content = f"1. {self.get_text_content(block.get('numbered_list_item', {}).get('rich_text', []), recursive, depth)}\n"
+        elif block_type == "quote":
+            content = f"> {self.get_text_content(block.get('quote', {}).get('rich_text', []), recursive, depth)}\n"
+        # コードブロックタイプの処理
+        elif block_type == "code":
+            code_content = self.get_text_content(
+                block.get("code", {}).get("rich_text", []), recursive, depth
+            )
+            language = block["code"].get("language", "")
+            content = f"```{language}\n{code_content}\n```\n"
+        # `table`ブロックタイプの処理
+        elif block_type == "table_row":
+            # テーブルの行を処理
+            row_cells = block["table_row"]["cells"]
+            row_content = []
+            for cell in row_cells:
+                cell_content = self.get_text_content(cell, recursive, depth)
+                row_content.append(cell_content)
+            content = f"| {' | '.join(row_content)} |\n"
+        # 他のブロックタイプの処理をここに追加...
+
+        return content
```

### Comparing `notion-util-0.0.2/notion_util.egg-info/PKG-INFO` & `notion-util-0.0.3/notion_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-util
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial Python API client for Notion.so
 Home-page: https://github.com/tatsu-i/notion-util
 Author: tatsu-i
 License: UNKNOWN
 Description: # Notion Util
         
         このプロジェクトは、Notion.soの非公式Python APIクライアントです。
```

### Comparing `notion-util-0.0.2/setup.py` & `notion-util-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return reqs
 
 
 install_requires = get_requirements("requirements.txt")
 
 setuptools.setup(
     name="notion-util",
-    version="0.0.2",
+    version="0.0.3",
     author="tatsu-i",
     description="Unofficial Python API client for Notion.so",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tatsu-i/notion-util",
     install_requires=install_requires,
     include_package_data=True,
```

