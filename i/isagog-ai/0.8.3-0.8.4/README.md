# Comparing `tmp/isagog_ai-0.8.3.tar.gz` & `tmp/isagog_ai-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isagog_ai-0.8.3.tar", max compression
+gzip compressed data, was "isagog_ai-0.8.4.tar", max compression
```

## Comparing `isagog_ai-0.8.3.tar` & `isagog_ai-0.8.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.3/isagog/__init__.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.3/isagog/client/__init__.py
--rw-r--r--   0        0        0     9327 2024-04-15 08:35:12.556546 isagog_ai-0.8.3/isagog/client/kg_client.py
--rw-r--r--   0        0        0     5971 2024-04-09 14:40:57.250758 isagog_ai-0.8.3/isagog/client/nlp_client.py
--rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.3/isagog/generator/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-10 08:27:28.933122 isagog_ai-0.8.3/isagog/generator/sparql_generator.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.3/isagog/model/__init__.py
--rw-r--r--   0        0        0    18896 2024-04-15 11:50:48.729498 isagog_ai-0.8.3/isagog/model/kg_model.py
--rw-r--r--   0        0        0    27390 2024-04-10 09:06:24.629297 isagog_ai-0.8.3/isagog/model/kg_query.py
--rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.8.3/isagog/model/nlp_model.py
--rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.3/LICENSE
--rw-r--r--   0        0        0      588 2024-04-12 15:52:50.928459 isagog_ai-0.8.3/pyproject.toml
--rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.3/README.md
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.4/isagog/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.4/isagog/client/__init__.py
+-rw-r--r--   0        0        0    10003 2024-04-16 08:17:48.784662 isagog_ai-0.8.4/isagog/client/kg_client.py
+-rw-r--r--   0        0        0     6456 2024-04-16 08:17:48.810054 isagog_ai-0.8.4/isagog/client/nlp_client.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.4/isagog/generator/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-10 08:27:28.933122 isagog_ai-0.8.4/isagog/generator/sparql_generator.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.4/isagog/model/__init__.py
+-rw-r--r--   0        0        0    20405 2024-04-16 06:53:26.703123 isagog_ai-0.8.4/isagog/model/kg_model.py
+-rw-r--r--   0        0        0    26878 2024-04-16 07:29:03.592734 isagog_ai-0.8.4/isagog/model/kg_query.py
+-rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.8.4/isagog/model/nlp_model.py
+-rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.4/LICENSE
+-rw-r--r--   0        0        0      588 2024-04-15 12:25:44.740393 isagog_ai-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.4/README.md
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.8.4/PKG-INFO
```

### Comparing `isagog_ai-0.8.3/isagog/client/kg_client.py` & `isagog_ai-0.8.4/isagog/client/kg_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 load_dotenv()
 
 KG_DEFAULT_TIMEOUT = int(os.getenv('KG_DEFAULT_TIMEOUT', 120))
 
 # Type variable for the Entity hierarchy
 E = TypeVar('E', bound='Entity')
 
+AUTH_TOKEN_KEY = os.getenv('ISAGOG_AUTH_TOKEN_KEY', 'X-Isagog-API-Token')
+AUTH_TOKEN_VALUE = os.getenv('ISAGOG_AUTH_TOKEN_VALUE')
+
 
 class KnowledgeBase(object):
     """
     Interface to knowledge base service
     """
 
     def __init__(self,
@@ -47,15 +50,15 @@
         self.version = version if version else "latest"
         self.logger = logger if logger else logging.getLogger()
         self.logger.info("Isagog KG client (%s) initialized on route %s", hex(id(self)), route)
 
     def get_entity(self,
                    _id: Reference,
                    expand: bool = True,
-                   entity_type: Type[E] = Entity
+                   entity_type: Type[E] = Entity,
                    ) -> E | None:
         """
         Gets the entity by its identifier
         :param _id: the entity identifier
         :param expand: whether to return entity attributes
         :param entity_type: the entity type (default: Entity)
         """
@@ -67,33 +70,38 @@
         if not issubclass(entity_type, Entity):
             raise ValueError(f"{entity_type} not an Entity")
 
         expand = "true" if expand else "false"
 
         params = f"id={_id}&expand={expand}"
 
+        headers = {"Accept": "application/json"}
+
+        if AUTH_TOKEN_VALUE:
+            headers[AUTH_TOKEN_KEY] = AUTH_TOKEN_VALUE
+
         if self.dataset:
             params += f"&dataset={self.dataset}"
 
         res = httpx.get(
             url=self.route,
             params=params,
-            headers={"Accept": "application/json"},
+            headers=headers,
         )
         if res.status_code == 200:
             self.logger.debug("Fetched %s", _id)
             return entity_type(_id, **res.json())
         else:
             self.logger.error("Couldn't fetch %s due to %s", _id, res.text)
             return None
 
     def query_assertions(self,
                          subject: Individual,
                          properties: list[Attribute | Relation],
-                         timeout=KG_DEFAULT_TIMEOUT
+                         timeout=KG_DEFAULT_TIMEOUT,
                          ) -> list[Assertion]:
         """
         Returns specific entity properties
 
         :param timeout:
         :param subject:
         :param properties: the queried properties
@@ -110,20 +118,25 @@
         self.logger.debug("Querying assertions for %s", subject)
 
         query = UnarySelectQuery(subject=subject.id)
 
         for prop in properties:
             query.add_fetch_clause(predicate=str(prop.id))
 
-        query_dict = query.to_dict(self.version)
+        headers = {"Accept": "application/json"}
+
+        if AUTH_TOKEN_VALUE:
+            headers[AUTH_TOKEN_KEY] = AUTH_TOKEN_VALUE
+
+        query_dict = query.to_dict(version=self.version)
 
         res = httpx.post(
             url=self.route,
             json=query_dict,
-            headers={"Accept": "application/json"},
+            headers=headers,
             timeout=timeout
         )
 
         if res.status_code == 200:
             res_list = res.json()
             if len(res_list) == 0:
                 self.logger.warning("Void attribute query")
@@ -142,15 +155,16 @@
         else:
             self.logger.warning("Query of entity %s failed due to %s", subject, res.text)
             return []
 
     def search_individuals(self,
                            kinds: list[Concept] = None,
                            constraints: dict[Attribute, Value] = None,
-                           timeout=KG_DEFAULT_TIMEOUT
+                           timeout=KG_DEFAULT_TIMEOUT,
+                           auth_token=None
                            ) -> list[Individual]:
         """
         Retrieves individuals by string search
         :param timeout: the request timeout
         :param kinds: the kinds to search for
         :param constraints: the search constraints
         :return: a list of matching individuals
@@ -167,86 +181,95 @@
         else:
             search_clause = DisjunctiveClause()
             for attribute, value in constraints.items():
                 search_clause.add_atom(property=attribute, argument=value, method=Comparison.REGEX)
 
         query.add(search_clause)
 
+        headers = {"Accept": "application/json"}
+        if auth_token:
+            headers[AUTH_TOKEN_KEY] = auth_token
+
         res = httpx.post(
             url=self.route,
-            json=query.to_dict(self.version),
-            headers={"Accept": "application/json"},
+            json=query.to_dict(version=self.version),
+            headers=headers,
             timeout=timeout
         )
 
         if res.status_code == 200:
             entities.extend([Individual(r.get('id'), **r) for r in res.json()])
         else:
             self.logger.error("Search individuals failed: code %d, reason %s", res.status_code, res.text)
 
         return entities
 
     def query_individuals(self,
                           query: UnarySelectQuery,
                           kind: Type[E] = Individual,
-                          timeout=KG_DEFAULT_TIMEOUT
+                          timeout=KG_DEFAULT_TIMEOUT,
                           ) -> list[E]:
         """
 
-        :param query:
-        :param kind:
-        :param timeout:
-        :return:
+
+        :param query: the query
+        :param kind: the kind of individuals to return
+        :param timeout: the request timeout
+        :return: a list of individuals of the specified kind
         """
         start_time = time.time()
 
-        req = query.to_dict(self.version)
+        req = query.to_dict(version=self.version)
 
         if self.dataset and (self.version == "latest" or self.version > "v1.0.0"):
             req['dataset'] = self.dataset
 
+        headers = {"Accept": "application/json"}
+
+        if AUTH_TOKEN_VALUE:
+            headers[AUTH_TOKEN_KEY] = AUTH_TOKEN_VALUE
+
         res = httpx.post(
             url=self.route,
             json=req,
-            headers={"Accept": "application/json"},
+            headers=headers,
             timeout=timeout
         )
 
         if res.status_code == 200:
             self.logger.debug("Query individuals done in %d seconds", time.time() - start_time)
             return [kind(r.get('id'), **r) for r in res.json()]
         elif res.status_code < 500:
             self.logger.warning("query individuals return code %d, reason %s", res.status_code, res.text)
         else:
             self.logger.error("query individuals return code code %d, reason %s", res.status_code, res.text)
         return []
 
-    def upsert_individual(self, individual: Individual, auth_token=None) -> bool:
+    def upsert_individual(self, individual: Individual) -> bool:
         """
         Updates an individual or insert it if not present; existing properties are preserved
 
         :param individual: the individual
-        :param assetions: assertions to be updated
-        :param auth_token:
+
         :return:
         """
         if individual.need_update():
 
             self.logger.debug("Updating individual %s", individual.id)
 
             params = {'id': individual.id}
             if self.dataset:
                 params['dataset'] = self.dataset
 
             req = [ass.to_dict() for ass in individual.get_assertions()]
 
             headers = {"Accept": "application/json"}
 
-            if auth_token:
-                headers["Authorization"] = f'Bearer {auth_token}'
+            if AUTH_TOKEN_VALUE:
+                headers[AUTH_TOKEN_KEY] = AUTH_TOKEN_VALUE
 
             try:
                 res = httpx.patch(
                     url=self.route,
                     params=params,
                     json=req,
                     headers=headers
@@ -257,12 +280,11 @@
                     return True
                 else:
                     print(f"upsert failed {res.status_code}")
                     return False
             except Exception as e:
                 raise e
         else:
-            self.logger.debug("Individual %s doesn't need update", individual.id)
-
+            self.logger.warning("Individual %s doesn't need update", individual.id)
 
-    def delete_individual(self, _id: Reference, auth_key=None):
+    def delete_individual(self, _id: Reference, auth_token=None):
         pass
```

### Comparing `isagog_ai-0.8.3/isagog/client/nlp_client.py` & `isagog_ai-0.8.4/isagog/client/nlp_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 (c) Isagog S.r.l. 2024, MIT License
 """
 import logging
 import os
 import time
 import httpx
 
-
 from dotenv import load_dotenv
 
 from isagog.model.nlp_model import Word, NamedEntity
 
 load_dotenv()
 
 NLP_DEFAULT_TIMEOUT = int(os.getenv('NLP_DEFAULT_TIMEOUT', 60))
 
 DEFAULT_LEXICAL_POS = ["NOUN", "VERB", "ADJ", "ADV"]
 DEFAULT_SEARCH_POS = ["NOUN", "VERB", "PROPN"]
 
+AUTH_TOKEN_KEY = os.getenv('ISAGOG_AUTH_TOKEN_KEY', 'X-Isagog-API-Token')
+AUTH_TOKEN_VALUE = os.getenv('ISAGOG_AUTH_TOKEN_VALUE')
+
 
 def truncate(s: str, n=10):
     """
     Truncate a string to the first N characters, adding '...' if the string is longer.
 
     :param s: The string to be truncated.
     :param n: The maximum length of the truncated string.
@@ -88,22 +90,28 @@
         Extract the main N words (keywords) from the supplied text
         :param timeout:
         :param text:
         :param number:
         :return:
         """
         self.logger.debug("Extracting %d keywords from %s", number, truncate(text))
+
+        headers = {"Accept": "application/json"}
+
+        if AUTH_TOKEN_VALUE:
+            headers[AUTH_TOKEN_KEY] = AUTH_TOKEN_VALUE
+
         res = httpx.post(
             url=self.route + "/analyze",
             json={
                 "text": text,
                 "tasks": ["keyword"],
                 "keyword_number": number
             },
-            headers={"Accept": "application/json"},
+            headers=headers,
             timeout=timeout
         )
         if res.status_code == 200:
             res_dict = res.json()
             words = [kwr[0] for kwr in res_dict["keyword"]]
             return words
         else:
@@ -121,21 +129,26 @@
         :param filter_pos: part of speech list
         :return:
         """
         self.logger.debug("Extracting words from %s", truncate(text))
         if not filter_pos:
             filter_pos = DEFAULT_LEXICAL_POS
 
+        headers = {"Accept": "application/json"}
+
+        if AUTH_TOKEN_VALUE:
+            headers[AUTH_TOKEN_KEY] = AUTH_TOKEN_VALUE
+
         res = httpx.post(
             url=self.route + "/analyze",
             json={
                 "text": text,
                 "tasks": ["word"]
             },
-            headers={"Accept": "application/json"},
+            headers=headers,
             timeout=timeout
         )
         if res.status_code == 200:
             res_dict = res.json()
             words = [Word(**{k: v for k, v in r.items() if k in Word._fields}) for r in res_dict["words"]]
             return [w.text for w in words if w.pos in filter_pos]
         else:
@@ -153,21 +166,26 @@
         :param timeout:
         :return:
         """
         self.logger.debug("Extracting words and entities from %s", truncate(text))
         if not filter_pos:
             filter_pos = DEFAULT_LEXICAL_POS
 
+        headers = {"Accept": "application/json"}
+
+        if AUTH_TOKEN_VALUE:
+            headers[AUTH_TOKEN_KEY] = AUTH_TOKEN_VALUE
+
         res = httpx.post(
             url=self.route + "/analyze",
             json={
                 "text": text,
                 "tasks": ["word", "entity"]
             },
-            headers={"Accept": "application/json"},
+            headers=headers,
             timeout=timeout
         )
 
         if res.status_code == 200:
             res_dict = res.json()
             words = list(filter(lambda w: w.pos in filter_pos,
                                 [Word(**{k: v for k, v in r.items() if k in Word._fields}) for r in res_dict["words"]]))
```

### Comparing `isagog_ai-0.8.3/isagog/generator/sparql_generator.py` & `isagog_ai-0.8.4/isagog/generator/sparql_generator.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.3/isagog/model/kg_model.py` & `isagog_ai-0.8.4/isagog/model/kg_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -108,53 +108,62 @@
         self.comment = kwargs.get('comment', "")
         self.ontology = kwargs.get('ontology', "")
         self.parents = kwargs.get('parents', [OWL.Thing])
 
 
 class Attribute(Entity):
     """
-    Assertions ranging on concrete domains
+    Class of assertions ranging on concrete domains
     owl:DatatypeProperties
     """
 
-    def __init__(self, _id: Reference, **kwargs):
+    def __init__(self,
+                 _id: Reference,
+                 domain: Reference = None,
+                 parents: list[Reference] = None,
+                 **kwargs):
         """
 
         :param _id:
         :param kwargs: domain
         """
 
         super().__init__(_id, owl=OWL.DatatypeProperty)
-        self.domain = kwargs.get('domain', OWL.Thing)
-        self.parents = kwargs.get('parents', [OWL.topDataProperty])
-        self.type = kwargs.get('type', "string")
+        self.domain = domain if domain else OWL.Thing
+        self.parents = parents if parents else [OWL.topDataProperty]
+        if 'type' in kwargs:
+            self.__type__ = kwargs.get('type')
 
 
 class Relation(Entity):
     """
-    Assertions ranging on individuals
+    Class of assertions ranging on individuals
     owl:ObjectProperty
     """
 
     def __init__(
             self,
             _id: Reference,
+            domain: Reference = None,
+            range: Reference = None,
+            inverse: Reference = None,
+            parents: list[Reference] = None,
             **kwargs
     ):
         """
         :param _id:
         :param kwargs: inverse, domain, range, label
         """
 
         super().__init__(_id, owl=OWL.ObjectProperty)
-        self.inverse = kwargs.get('inverse')
-        self.domain = kwargs.get('domain', Concept(OWL.Thing))
-        self.range = kwargs.get('range', Concept(OWL.Thing))
+        self.inverse = inverse if inverse else None
+        self.domain = domain if domain else OWL.Thing
+        self.range = range if range else OWL.Thing
         self.label = kwargs.get('label', _uri_label(_id))
-        self.parents = kwargs.get('parents', [OWL.topObjectProperty])
+        self.parents = parents if parents else OWL.topObjectProperty
 
 
 class Assertion(object):
     """
     Assertion axiom of the form: property(subject, values)
     """
 
@@ -166,22 +175,22 @@
         """
 
         :param predicate:
         :param subject:
         :param values:
         """
         if predicate is None:
-            # try to get the predicate from the kwargs, if not present raise an error
+            # try to get the predicate from aliases in kwargs, if not present raise an error
             predicate = kwargs.get('property', kwargs.get('id', None))
             if predicate is None:
                 raise ValueError("missing predicate")
 
         self.predicate = str(predicate).strip("<>")
         self.subject = str(subject).strip("<>") if subject else None
-        self.values = values if values else []
+        self.values = list(values) if values else list()
 
     def to_dict(self) -> dict:
         return _todict(self)
 
     def is_empty(self) -> bool:
         return not self.values
 
@@ -198,16 +207,15 @@
     no super-categories allowed.
     """
 
     def __init__(
             self,
             source: IO[bytes] | TextIO | str,
             publicIRI: str,
-            source_format="turtle",
-            **kwargs
+            source_format="turtle"
     ):
         """
         :param source:  Path to the ontology source file.
         :param publicIRI:  Base IRI for the ontology.
         :param source_format:  Format of the ontology.
 
         """
@@ -277,15 +285,16 @@
 
 
 class AttributeInstance(Assertion):
     """
     Attributive assertion
     """
 
-    def __init__(self, predicate: Reference = None,
+    def __init__(self,
+                 predicate: Reference = None,
                  subject: Reference = None,
                  values: list[str | int | float | bool] = None,
                  **kwargs):
         """
         :param subject: the asserted subject
         :param predicate: the asserted property
         :param values: the asserted values, they can be strings, integers, floats or booleans
@@ -352,15 +361,15 @@
     def first_value(self, default=None) -> str | int | float | bool | None:
         if len(self.values) > 0:
             return self.values[0]
         else:
             return default
 
 
-VOID_ATTRIBUTE = AttributeInstance(predicate='http://isagog.com/attribute#void')
+VOID_ATTRIBUTE = AttributeInstance(predicate='https://isagog.com/attribute#void')
 
 
 class RelationInstance(Assertion):
     """
     Relational assertion
     """
 
@@ -421,15 +430,15 @@
             for kind in individual.kind:
                 if kind not in kind_map:
                     kind_map[kind] = []
                 kind_map[kind].append(individual)
         return kind_map
 
 
-VOID_RELATION = RelationInstance(predicate='http://isagog.com/relation#void')
+VOID_RELATION = RelationInstance(predicate='https://isagog.com/relation#void')
 
 
 class Individual(Entity):
     """
     Individual entity
 
     """
@@ -442,42 +451,27 @@
 
         :param _id: the individual identifier
         :param attributes: the individual attributes
         :param relations: the individual relations
         :param kwargs:
         """
         super().__init__(_id, owl=OWL.NamedIndividual, **kwargs)
-        self.attributes = []
-        self.relations = []
-        # self.label = kwargs.get('label', _uri_label(self.id))
-        # self.add_attribute(AttributeInstance(predicate=RDFS.label, values=[self.label]))
-        #
-        # self.kind = kwargs.get('kind', kwargs.get('kinds', [OWL.Thing]))  # back compatibility w 0.7
-        # if not all(x == OWL.Thing for x in self.kind):
-        #     self.add_attribute(AttributeInstance(predicate=RDF.type, values=self.kind))
-        #
-        # self.comment = kwargs.get('comment', '')
-        # if self.comment:
-        #     self.add_attribute(AttributeInstance(predicate=RDFS.comment, values=[self.comment]))
-
+        self.attributes = list()
+        self.relations = list()
         if attributes:
             for attribute in attributes:
                 if isinstance(attribute, dict):
                     attribute = AttributeInstance(**attribute)
-                self.add_attribute(attribute)
+                self.add_attribute(instance=attribute)
 
-        # self.attributes.extend([AttributeInstance(**a_data) for a_data in
-        #                         kwargs.get('attributes', list[AttributeInstance]())])
         if relations:
             for relation in relations:
                 if isinstance(relation, dict):
                     relation = RelationInstance(**relation)
-                self.add_relation(relation)
-        # self.relations.extend(
-        #     [RelationInstance(**r_data) for r_data in kwargs.get('relations', list[RelationInstance]())])
+                self.add_relation(instance=relation)
         if 'score' in kwargs:
             self.score = float(kwargs.get('score'))
         if self.has_attribute(PROFILE_ATTRIBUTE):
             self.profile = {
                 profile_value.split("=")[0]: int(profile_value.split("=")[1])
                 for profile_value in self.get_attribute(PROFILE_ATTRIBUTE).values
             }
@@ -542,35 +536,73 @@
             return self.score
         else:
             return None
 
     def has_score(self) -> bool:
         return hasattr(self, 'score')
 
-    def add_attribute(self, attribute: AttributeInstance):
+    def add_attribute(self,
+                      predicate: Reference | str = None,
+                      values: list[str | int | float | bool] = None,
+                      instance: AttributeInstance = None):
         """
         Adds an attribute to the individual
-        :param attribute:
+        One of predicate or instance must be provided (but not both: in that case, instance is preferred)
+        :param values:
+        :param predicate:
+        :param instance:
         """
-        if attribute.subject and attribute.subject != self.id:
-            logging.warning("attribute for %s redeclared for %s", attribute.subject, self.id)
-        attribute.subject = self.id
-        self.attributes.append(attribute)
+        if instance:
+            if not isinstance(instance, AttributeInstance):
+                raise ValueError("bad instance")
+            if instance.subject and instance.subject != self.id:
+                logging.warning("attribute for %s redeclared for %s", instance.subject, self.id)
+            instance.subject = self.id
+            existing = self.get_attribute(instance.predicate)
+            if not existing or existing.is_empty():
+                self.attributes.append(instance)
+            else:
+                existing.values.extend([value for value in instance.values if value not in existing.values])
+        else:
+            if not predicate:
+                raise ValueError("missing property")
+            if not isinstance(predicate, (Reference, str)):
+                raise ValueError("bad property")
+            self.add_attribute(instance=AttributeInstance(predicate=predicate, values=values))
         self._refresh = True
 
-    def add_relation(self, relation: RelationInstance):
-        """
-
-        :param relation:
+    def add_relation(self,
+                     predicate: Reference | str = None,
+                     values: list[Reference | str] = None,
+                     instance: RelationInstance = None):
+        """
+        Adds a relation to the individual
+        One of predicate or instance must be provided (but not both: in that case, instance is preferred)
+        :param instance:
+        :param values:
+        :param predicate:
         :return:
         """
-        if relation.subject and relation.subject != self.id:
-            logging.warning("relation for %s redeclared for %s", relation.subject, self.id)
-        relation.subject = self.id
-        self.relations.append(relation)
-        self._refresh = True
+        if instance:
+            if not isinstance(instance, RelationInstance):
+                raise ValueError("bad instance")
+            if instance.subject and instance.subject != self.id:
+                logging.warning("relation for %s redeclared for %s", instance.subject, self.id)
+            instance.subject = self.id
+            existing = self.get_relation(instance.predicate)
+            if not existing or existing.is_empty():
+                self.relations.append(instance)
+            else:
+                existing.values.extend([value for value in instance.values if value not in existing.values])
+            self._refresh = True
+        else:
+            if not predicate:
+                raise ValueError("missing property")
+            if not isinstance(predicate, (Reference, str)):
+                raise ValueError("bad property")
+            self.add_relation(instance=RelationInstance(predicate=predicate, values=values))
 
     def need_update(self):
         return self._refresh
 
     def updated(self):
         self._refresh = False
```

### Comparing `isagog_ai-0.8.3/isagog/model/kg_query.py` & `isagog_ai-0.8.4/isagog/model/kg_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
     A model for knowledge graph queries
     The model is based on a triple query language (subject, property, argument)
     (c) Isagog S.r.l. 2024, MIT License
 """
 from __future__ import annotations
+
 import logging
 import random
 import re
 from enum import Enum
 from typing import Protocol
 from urllib.parse import urlparse
-from rdflib import RDF, RDFS, OWL, URIRef
 
-from isagog.model.kg_model import Assertion
+from rdflib import RDF, RDFS, OWL, URIRef
 
 DEFAULT_PREFIXES = [("rdf", "http://www.w3.org/2000/01/rdf-schema"),
                     ("rdfs", "http://www.w3.org/2001/XMLSchema"),
                     ("text", "http://jena.apache.org/text")]
 
 # don't change this for the sake of back compatibility
 _SUBJVAR = 'i'
@@ -548,26 +548,18 @@
                 if isinstance(c.subject, Variable):
                     _vars.append(c.subject)
         return set(_vars)
 
     def has_return_vars(self) -> bool:
         return len(self.project_vars()) > 0
 
-    # def to_sparql(self) -> str:
-    #     """
-    #     This method is deprecated and will be removed in a future version.
-    #
-    #     Use generate_query with a SPARQL generator instead.
-    #     """
-    #     raise NotImplementedError()
-
     def generate(self, generator: Generator) -> str:
         return generator.generate_query(self)
 
-    def to_dict(self, version: str = None) -> dict:
+    def to_dict(self, **kwargs) -> dict:
         pass
 
 
 class UnarySelectQuery(SelectQuery):
     """
     Select query about a single subject
 
@@ -713,28 +705,21 @@
                     case 'dataset':
                         pass
                     case _:
                         logging.error("Illegal key %s", key)
         except Exception as e:
             raise ValueError(f"Malformed query due to: {e}")
 
-    # def to_sparql(self) -> str:
-    #     """
-    #     Deprecated
-    #     :return:
-    #
-    #     """
-    #     from isagog.generator.sparql_generator import _SPARQLGEN
-    #
-    #     return _SPARQLGEN.generate_query(self)
-
-    def to_dict(self, version=None) -> dict:
+    def to_dict(self, **kwargs) -> dict:
 
         out = {}
-        if version is None or version > "1.0.0":
+
+        version = kwargs.get('version')
+
+        if not version or version > "1.0.0":
             out['subject'] = self.subject
 
         out['clauses'] = [c.to_dict(version=version) for c in self.clauses]
         out['graph'] = self.graph
         out['limit'] = self.limit
         out['lang'] = self.lang
         if self.min_score:
```

### Comparing `isagog_ai-0.8.3/LICENSE` & `isagog_ai-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.3/pyproject.toml` & `isagog_ai-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2269 7361 676f 672d 6169  ame = "isagog-ai
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 302e  "..version = "0.
-00000030: 382e 3322 0d0a 6465 7363 7269 7074 696f  8.3"..descriptio
+00000030: 382e 3422 0d0a 6465 7363 7269 7074 696f  8.4"..descriptio
 00000040: 6e20 3d20 2263 6c69 656e 7420 666f 7220  n = "client for 
 00000050: 6973 6167 6f67 2061 6920 7365 7276 6963  isagog ai servic
 00000060: 6573 220d 0a61 7574 686f 7273 203d 205b  es"..authors = [
 00000070: 2247 7569 646f 2056 6574 6572 6520 3c67  "Guido Vetere <g
 00000080: 2e76 6574 6572 6540 6973 6167 6f67 2e63  .vetere@isagog.c
 00000090: 6f6d 3e22 5d0d 0a72 6561 646d 6520 3d20  om>"]..readme = 
 000000a0: 2252 4541 444d 452e 6d64 220d 0a70 6163  "README.md"..pac
```

### Comparing `isagog_ai-0.8.3/PKG-INFO` & `isagog_ai-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isagog-ai
-Version: 0.8.3
+Version: 0.8.4
 Summary: client for isagog ai services
 Author: Guido Vetere
 Author-email: g.vetere@isagog.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

