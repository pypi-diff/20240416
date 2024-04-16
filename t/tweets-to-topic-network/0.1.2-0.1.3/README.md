# Comparing `tmp/tweets_to_topic_network-0.1.2.tar.gz` & `tmp/tweets_to_topic_network-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweets_to_topic_network-0.1.2.tar", max compression
+gzip compressed data, was "tweets_to_topic_network-0.1.3.tar", max compression
```

## Comparing `tweets_to_topic_network-0.1.2.tar` & `tweets_to_topic_network-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2024-04-11 12:12:13.477841 tweets_to_topic_network-0.1.2/LICENSE
--rw-r--r--   0        0        0     9420 2024-04-11 13:51:27.446268 tweets_to_topic_network-0.1.2/README.md
--rw-r--r--   0        0        0      717 2024-04-11 14:04:33.327689 tweets_to_topic_network-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 12:12:13.484112 tweets_to_topic_network-0.1.2/tweets_to_topic_network/__init__.py
--rw-r--r--   0        0        0     7973 2024-04-11 13:29:07.797058 tweets_to_topic_network-0.1.2/tweets_to_topic_network/data.py
--rw-r--r--   0        0        0    10831 2024-04-11 12:12:13.484495 tweets_to_topic_network-0.1.2/tweets_to_topic_network/network.py
--rw-r--r--   0        0        0     6743 2024-04-11 13:56:57.706709 tweets_to_topic_network-0.1.2/tweets_to_topic_network/topic.py
--rw-r--r--   0        0        0    10302 1970-01-01 00:00:00.000000 tweets_to_topic_network-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-11 12:12:13.477841 tweets_to_topic_network-0.1.3/LICENSE
+-rw-r--r--   0        0        0    13264 2024-04-16 17:38:24.238044 tweets_to_topic_network-0.1.3/README.md
+-rw-r--r--   0        0        0      738 2024-04-16 17:41:26.586531 tweets_to_topic_network-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-16 17:41:11.397030 tweets_to_topic_network-0.1.3/tweets_to_topic_network/__init__.py
+-rw-r--r--   0        0        0     8171 2024-04-16 15:33:49.288519 tweets_to_topic_network-0.1.3/tweets_to_topic_network/data.py
+-rw-r--r--   0        0        0    10831 2024-04-11 12:12:13.484495 tweets_to_topic_network-0.1.3/tweets_to_topic_network/network.py
+-rw-r--r--   0        0        0     8697 2024-04-16 16:14:51.525205 tweets_to_topic_network-0.1.3/tweets_to_topic_network/topic.py
+-rw-r--r--   0        0        0    14188 1970-01-01 00:00:00.000000 tweets_to_topic_network-0.1.3/PKG-INFO
```

### Comparing `tweets_to_topic_network-0.1.2/LICENSE` & `tweets_to_topic_network-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tweets_to_topic_network-0.1.2/pyproject.toml` & `tweets_to_topic_network-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tweets-to-topic-network"
-version = "0.1.2"
+version = "0.1.3"
 description = "start from a set of tweets and create a multilayer network where each layer is a topic"
 authors = ["alessiogandelli <alessiogandelli99@gmail.com>"]
 readme = "README.md"
 packages = [{include = "tweets_to_topic_network"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
@@ -14,14 +14,15 @@
 bertopic = "^0.16.0"
 openai = "^1.17.0"
 typing-extensions = "^4.11.0"
 qdrant-client = "^1.8.2"
 uunet = "^2.1.1"
 networkx = "^3.3"
 igraph = "^0.11.4"
+fastembed = "^0.2.6"
 
 
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 
 [build-system]
```

### Comparing `tweets_to_topic_network-0.1.2/tweets_to_topic_network/data.py` & `tweets_to_topic_network-0.1.3/tweets_to_topic_network/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
         self.n_cop = None
 
         # paths and name
         self.name = self.file_tweets.split('/')[-1].split('.')[0]
 
         self.folder = '/'.join(file_tweets.split('/')[:-1])
         self.path_cache = os.path.join(self.folder, 'cache')
-        self.tweets_file = os.path.join(self.path_cache,'tweets_'+self.name)
-        self.users_file = os.path.join(self.path_cache,'users_'+self.name)
-        self.labeled_file = os.path.join(self.path_cache,'retweet_labeled_'+self.name)
+        self.tweets_file = os.path.join(self.path_cache,'data','tweets_'+self.name)
+        self.users_file = os.path.join(self.path_cache,'data','users_'+self.name)
+        self.labeled_file = os.path.join(self.path_cache,'data', 'retweet_labeled_'+self.name)
 
         # dataframes
         self.df_tweets = None
         self.df_original = None
         self.df_original_influencers = None
         self.df_retweets = None
         self.df_quotes = None
@@ -63,16 +63,19 @@
         self.df_original = df_tweets[df_tweets['referenced_type'].isna()] # The handwritten tweets
         self.df_retweets = df_tweets[df_tweets['referenced_type'] == 'retweeted']
         self.df_quotes = df_tweets[df_tweets['referenced_type'] == 'quoted']
         self.df_reply = df_tweets[df_tweets['referenced_type'] == 'replied_to']
     
     def _is_cached(self):
        
-        if not os.path.exists(self.path_cache):
+        if not os.path.exists(self.path_cache): # mkdir cache
             os.makedirs(self.path_cache)
+        
+        if not os.path.exists(os.path.join(self.path_cache, 'data')): # mkdir cache/data
+            os.makedirs(os.path.join(self.path_cache, 'data'))
 
         return os.path.exists(self.tweets_file+'.pkl') and os.path.exists(self.users_file+'.pkl')
 
     def _load_json(self):
         if self.file_user is not None:
             df_user = self._load_users_json()
         else :
```

### Comparing `tweets_to_topic_network-0.1.2/tweets_to_topic_network/network.py` & `tweets_to_topic_network-0.1.3/tweets_to_topic_network/network.py`

 * *Files identical despite different names*

### Comparing `tweets_to_topic_network-0.1.2/PKG-INFO` & `tweets_to_topic_network-0.1.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: tweets-to-topic-network
-Version: 0.1.2
-Summary: start from a set of tweets and create a multilayer network where each layer is a topic
-Author: alessiogandelli
-Author-email: alessiogandelli99@gmail.com
-Requires-Python: >=3.10,<3.12
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bertopic (>=0.16.0,<0.17.0)
-Requires-Dist: igraph (>=0.11.4,<0.12.0)
-Requires-Dist: jsonlines (>=4.0.0,<5.0.0)
-Requires-Dist: networkx (>=3.3,<4.0)
-Requires-Dist: openai (>=1.17.0,<2.0.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
-Requires-Dist: qdrant-client (>=1.8.2,<2.0.0)
-Requires-Dist: sentence-transformers (>=2.6.1,<3.0.0)
-Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
-Requires-Dist: uunet (>=2.1.1,<3.0.0)
-Description-Content-Type: text/markdown
-
 # tweets-to-network
 ```bash
 pip install tweets-to-topic-network
 ```
 
 This repository contains the code to 
 - create networks from a set of tweets in json format (as they come from the API (RIP))
@@ -32,37 +10,77 @@
 from a set of tweets it is possibile to generate multiple networks:
 - *retweet network*:  a network where the nodes are the users and the edges are the retweets
 - *retweet network multilayer*: a network where the nodes are the users and the edges are the retweets, but the edges are divided in layers based on the topic of the tweet
 - *temporal text network*: a bipartite network where the nodes are the tweets and the users and the edges are the interactions between them
 
 #  Usage
 
+import the classes
 ```python
 from tweets_to_topic_network.data import Data_processor 
 from tweets_to_topic_network.topic import Topic_modeler
 from tweets_to_topic_network.network import Network_creator
+```
 
+load the json files and process them
+```python
 data = Data_processor(file_tweets, file_user, '22')
 data.process_json() # this process the data and creates several dataframes useful for the next steps
+```
+
+Run topic modeling, takes as parameters
+- dataframe: only requirement is the column 'text', 
+- name: name of the dataset
+- embeddedder_name: the supported embedding models are all the sentence transfers models, you can find them [here](https://www.sbert.net/docs/pretrained_models.html), and openai `text-embedding-ada-002` , `text-embedding-3-large` `text-embedding-3-small`
+- path_cache: the path where to save the labeled dataframe and the model in safetensor format
 
+returns the input dataframe with a new column with the topic of the tweet
+
+```python
 tm = Topic_modeler(data.df_original, name = data.name, embedder_name='all-MiniLM-L6-v2', path_cache = data.path_cache)
 df_labeled = tm.get_topics() # this creates a new column in the dataframe with the topic of the tweet
+```
+Update the dataframe with the labeled topics
 
-
+```python
 df_retweet_labeled = data.update_df(df_labeled) # this updates the dataframe with the labeled topics
-
+```
+create the networks 
+```python
 nw = Network_creator(df_retweet_labeled, name = data.name, path = data.folder)
-nw.create_retweet_network() # this creates the retweet network
-nw.create_ttnetwork()   # this creates the temporal text network
-nw.create_retweet_ml()  # this creates the multilayer network
+rt_network = nw.create_retweet_network() # this creates the retweet network
+rt_network_ml = nw.create_retweet_ml()   # this creates the multilayer network
+tt_network = nw.create_ttnetwork()       # this creates the temporal text network
+```
+
+## Qdrant integration
+
+you have the opportunity to store the embeddings in a [qdrant](https://qdrant.tech/documentation/quick-start/) instance, you need docker, if you do not do it, nothing happens
+
+```shell
+docker pull qdrant/qdrant
+
+```
+
+this will create a set of folders in your current directory, to explore the embeddings stored go on [http://localhost:6333/dashboard](http://localhost:6333/dashboard)
+
+```shell
+docker run -p 6333:6333 -p 6334:6334  -v $(pwd)/qdrant_storage:/qdrant/storage:z qdrant/qdrant
+
+```
+create a dotenv file with the following variables 
+
+```shell
+OPENAI_API_KEY=your-api-key
+QDRANT_URL=http://localhost:6333
 ```
 
 
 # Input 
-Th input is in [jsonl](https://jsonlines.org/) format, so one JSON per line representing or a user or a tweet depending on the file. You can find an example in [this](https://github.com/alessiogandelli/tweets-to-topic-network/blob/main/data/toy.json) file. This format is the one you can get querying the Twitter API. make sure your input file is in this format.
+The input is in [jsonl](https://jsonlines.org/) format, so one JSON per line representing or a user or a tweet depending on the file. You can find an example in [this](https://github.com/alessiogandelli/tweets-to-topic-network/blob/main/data/toy.json) file. This format is the one you can get querying the Twitter API. make sure your input file is in this format.
 
 ## JSON tweets file 
 The JSON tweets file contains information about all tweets involved in the conversation. Each tweet is represented as a JSON object with the following fields:
 
 - `author`: The ID of the tweet author.
 - `text`: The content of the tweet.
 - `created_at`: The timestamp when the tweet was created.
@@ -77,56 +95,101 @@
 ## JSON users file (optional)
 The user's file is used to get the username of the author of the tweet. 
 
 - `id`: The ID of the user.
 - `username`: The username of the user.
 
 
+# Files created: cache and networks
+
+## Cache
+When the data is processed it will be saved in a cache folder to avoid processing the same data multiple times. The cache folder will be in the same folder as the file you are processing, i suggest you to create a folder for each set of tweets you want to process. Pickle files are for machines, csv files are for humans.
+The cache folder will contain the following structure:
+
+```shell
+cache
+├── data
+│   ├── tweets_cop22.csv        # this is the dataframe of the tweets 
+│   ├── tweets_cop22.pkl
+│   ├── tweets_cop22_topics.pkl # this is the labeled dataframe with topics
+│   ├── users_cop22.csv         # this is the dataframe of the users
+│   └── users_cop22.pkl
+└── tm
+    └── all-MiniLM-L6-v2            # the folder for this embedding model
+        ├── embeddings_cop22.pkl    # the embeddings of the tweets 
+        ├── model_cop22             # the model in safetensor format
+        │   ├── config.json
+        │   ├── ctfidf.safetensors
+        │   ├── ctfidf_config.json
+        │   ├── topic_embeddings.safetensors
+        │   └── topics.json
+        └── topics_cop22.csv    # topics, keyworkds and representative tweets
+
+```
+
+## Networks
+The networks will be saved in the networks folder in the same folder as the file you are processing. Note that there are two different retweet network, one is generated from the temporal text network, the other directly from the tweets, there could be differences like self edges, still have to figure out which one is better. The networks folder will contain the following structure:
+
+```shell
+├── networks
+│   ├── cop22_retweet.gml                   # retweet network
+│   ├── cop22_retweet_ml.gml                # retweet network multilayer
+│   ├── cop22_retweet_network_ml.gml       # retweet network multilayer from projection
+│   ├── cop22_ttt.gml                   # temporal text network
+│   └── projected                   # each layer (topic) of the multilayer network
+│       ├── cop22__prj_-1.0.gml
+│       ├── cop22__prj_0.0.gml
+│       ├── cop22__prj_1.0.gml
+│       ├── cop22__prj_10.0.gml
+│       ├── cop22__prj_11.0.gml
+
+
+```
 
 # Classes
 The pipeline is divided into three classes, each of them is independent and can be used separately.
 
-- dataProcessor: takes the two json files and creates a pandas dataframe with all the tweets in english. It also creates a cache of the dataframe in csv and pickle format.
+- *Data_processor*: takes the two json files (or just one) and creates a pandas dataframe with all the tweets in english. It also creates a cache of the dataframe in csv and pickle format.
 
-- TopicModeler: takes a dataframe and labels the tweets with a topic using BERTopic. It also creates a cache of the labeled dataframe in csv and pickle format.
+- *Topic_modeler*: takes a dataframe and labels the tweets with a topic using BERTopic. It also creates a cache of the labeled dataframe in csv and pickle format.
 
-- NetworkCreator: takes a dataframe of tweets and creates a network from it. It can create a retweet network, a temporal text network, and a multilayer network. The networks are saved in gml format.
+- *Network_creator*: takes a dataframe of tweets and creates a network from it. It can create a retweet network, a temporal text network, and a multilayer network. The networks are saved in gml format.
 
 
 ## Data Processor
-The first step is to initialize the pipeline class giving the two files as input and the name of the COP.
+The first step is to initialize the pipeline class giving the two files as input and the name of the COP. (file_user is optional, if not present the username will be the user id)
 
 ```python
-data = Data_processor(file_tweets, file_user, name)
+data = Data_processor(file_tweets=file_tweets, file_user=file_user, n_cop='22')
 data.process_json()
 
 ```
 ### Under the hood
-Let's see what happen when you run the process_json() function, firstly, if the files are present in the cache folder, it loads them, otherwise, it follows this pipeline:.
+Let's see what happen when you run the`process_json()` function, firstly, if the files are present in the cache folder, it loads them, otherwise, it follows this pipeline:.
 - load_users_json: loads the json file of the users into a dataframe 
 - load_tweets_json: loads the json file of the tweets into a dataframe discarding the tweets with attachments
 - save dataframes: both in pickle (for machines) and csv(for humans) format in the cache folder
 
-### after the topic modeling
-There is the possibility to update the dataframe with the labeled topic, so that the object data contains all the data needed, it gets the labeled dataframe of the original tweets ( the topic modeling is not run on retweets to save save time and energy), and propagate the topic also to the retweets of the original tweets.
+### After the topic modeling
+There is the possibility to update the dataframe with the labeled topic, so that the object data contains all the data needed, it gets the labeled dataframe of the original tweets (the topic modeling is not run on retweets to save save time and energy), and propagate the topic also to the retweets of the original tweets.
 
 ```python  
 df_retweet_labeled = data.update_df(df_labeled)
 
 ```
 ## Topic Modeler
-Then we can get the topics of the tweets using BERTopic, this creates a new column in the dataframe with the topic of the tweet. The topics are saved in a pickle file for caching. In [this](https://github.com/alessiogandelli/topic-modeling-evaluation) repository I conclude that BERTopic is the best topic modeling algorithm for this scenario. You can choose the embedder you prefer
+Then we can get the topics of the tweets using BERTopic, this creates a new column in the dataframe with the topic of the tweet. The topics are saved in a pickle file for caching. In [this](https://github.com/alessiogandelli/topic-modeling-eval) repository I conclude that BERTopic is the best topic modeling algorithm for this scenario. You can choose the embedder you prefer
 
 ```python
 tm = Topic_modeler(data.df_original, name = data.name, embedder_name='all-MiniLM-L6-v2', path_cache = data.path_cache)
 df_labeled = tm.get_topics()
 
 
 ```
-### label topics 
+### label topics (todo)
 we use openai gpt3.5turbo model to label the topic using the putput of the cTFIDF and some representative tweets. 
 
 ## Network Creator
 Finally we can create the networks using the full dataframe with topic labels. there are 3 possible types of network you can create
 
 ```python
 nw = Network_creator(df_retweet_labeled, name = data.name, path = data.folder)
@@ -180,15 +243,15 @@
 
 
 
 
 
 #  How to run it
 
-suggestion: create a folder for each set of tweets you want to process, in our case one for each COP. Inside this folder there should be the two jsonl files, one for the tweets and one for the users. After running the main script( either using make or just running main.py) in that folder you will find the following folders:
+suggestion: create a folder for each set of tweets you want to process, in our case one for each COP. Inside this folder there should be the two jsonl files, one for the tweets and one for the users. The script will create the following directories:
 
 - `cache`: contains the csv and pickle files of the intermediate steps of the pipeline, from the cleaned dataset in csv to the label of the topics.
 
 - `networks`: contains the gml files of the temporal text network
 
 
 
@@ -209,8 +272,7 @@
 - csv/pkl tweets: 1.79 GB
 - temporal text network: 900 MB
 - projected multilayer: 84 MB
 
 2 h for processing the json file 
 4 h for extracting topics 
 18 h for creating the networks 
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

