# Comparing `tmp/lifelike-1.0.7.tar.gz` & `tmp/lifelike-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifelike-1.0.7.tar", last modified: Thu May 25 21:55:48 2023, max compression
+gzip compressed data, was "lifelike-1.0.9.tar", last modified: Thu May 25 22:05:24 2023, max compression
```

## Comparing `lifelike-1.0.7.tar` & `lifelike-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 21:55:48.640902 lifelike-1.0.7/
--rw-r--r--   0 mustafa    (501) staff       (20)     1073 2023-05-25 21:53:12.000000 lifelike-1.0.7/LICENSE.txt
--rw-r--r--   0 mustafa    (501) staff       (20)      270 2023-05-25 21:55:48.640971 lifelike-1.0.7/PKG-INFO
--rw-r--r--   0 mustafa    (501) staff       (20)     2758 2023-05-25 21:53:12.000000 lifelike-1.0.7/README.md
-drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 21:55:48.639105 lifelike-1.0.7/lifelike/
-drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 21:55:48.640718 lifelike-1.0.7/lifelike/StateManager/
--rw-r--r--   0 mustafa    (501) staff       (20)        0 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/StateManager/__init__.py
--rw-r--r--   0 mustafa    (501) staff       (20)    15743 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/StateManager/base_game_tree.py
--rw-r--r--   0 mustafa    (501) staff       (20)      962 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/StateManager/knowledge_tree.py
--rw-r--r--   0 mustafa    (501) staff       (20)     2131 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/StateManager/sequence_tree.py
--rw-r--r--   0 mustafa    (501) staff       (20)        0 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/__init__.py
--rw-r--r--   0 mustafa    (501) staff       (20)     8371 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/brain.py
--rw-r--r--   0 mustafa    (501) staff       (20)      499 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/state.py
-drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 21:55:48.639983 lifelike-1.0.7/lifelike.egg-info/
--rw-r--r--   0 mustafa    (501) staff       (20)      270 2023-05-25 21:55:48.000000 lifelike-1.0.7/lifelike.egg-info/PKG-INFO
--rw-r--r--   0 mustafa    (501) staff       (20)      409 2023-05-25 21:55:48.000000 lifelike-1.0.7/lifelike.egg-info/SOURCES.txt
--rw-r--r--   0 mustafa    (501) staff       (20)        1 2023-05-25 21:55:48.000000 lifelike-1.0.7/lifelike.egg-info/dependency_links.txt
--rw-r--r--   0 mustafa    (501) staff       (20)       10 2023-05-25 21:55:48.000000 lifelike-1.0.7/lifelike.egg-info/requires.txt
--rw-r--r--   0 mustafa    (501) staff       (20)        9 2023-05-25 21:55:48.000000 lifelike-1.0.7/lifelike.egg-info/top_level.txt
--rw-r--r--   0 mustafa    (501) staff       (20)       79 2023-05-25 21:55:48.641235 lifelike-1.0.7/setup.cfg
--rw-r--r--   0 mustafa    (501) staff       (20)      393 2023-05-25 21:55:42.000000 lifelike-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:05:24.549062 lifelike-1.0.9/
+-rw-rw-rw-   0        0        0     1094 2023-05-23 10:53:00.000000 lifelike-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      277 2023-05-25 22:05:24.549062 lifelike-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2797 2023-05-23 10:53:00.000000 lifelike-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 22:05:24.499449 lifelike-1.0.9/lifelike/
+drwxrwxrwx   0        0        0        0 2023-05-25 22:05:24.544804 lifelike-1.0.9/lifelike/StateManager/
+-rw-rw-rw-   0        0        0        0 2023-05-25 21:49:28.000000 lifelike-1.0.9/lifelike/StateManager/__init__.py
+-rw-rw-rw-   0        0        0    16100 2023-05-25 22:00:42.000000 lifelike-1.0.9/lifelike/StateManager/base_game_tree.py
+-rw-rw-rw-   0        0        0      983 2023-05-25 21:49:28.000000 lifelike-1.0.9/lifelike/StateManager/knowledge_tree.py
+-rw-rw-rw-   0        0        0     2172 2023-05-25 21:49:28.000000 lifelike-1.0.9/lifelike/StateManager/sequence_tree.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 10:53:00.000000 lifelike-1.0.9/lifelike/__init__.py
+-rw-rw-rw-   0        0        0     8615 2023-05-25 21:49:28.000000 lifelike-1.0.9/lifelike/brain.py
+-rw-rw-rw-   0        0        0      511 2023-05-23 10:53:00.000000 lifelike-1.0.9/lifelike/state.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:05:24.533237 lifelike-1.0.9/lifelike.egg-info/
+-rw-rw-rw-   0        0        0      277 2023-05-25 22:05:24.000000 lifelike-1.0.9/lifelike.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-05-25 22:05:24.000000 lifelike-1.0.9/lifelike.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 22:05:24.000000 lifelike-1.0.9/lifelike.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 22:05:24.000000 lifelike-1.0.9/lifelike.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 22:05:24.000000 lifelike-1.0.9/lifelike.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-25 22:05:24.560740 lifelike-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      406 2023-05-25 22:05:02.000000 lifelike-1.0.9/setup.py
```

### Comparing `lifelike-1.0.7/README.md` & `lifelike-1.0.9/README.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# lifelike
-A toolkit that allows for the creation of "lifelike" characters that you can interact with and change how they behave towards you
-
-
-## Brain Useage
-Install the package: `pip install git+https://github.com/lifelike-toolkit/lifelike.git`
-
-Then import it with `from lifelike import brain`
-
-The `Characters` class requires a file path to a JSON file where the characters data will be saved. To create a `Characters` object, initialize it as follows:
-```python
-from lifelike import brain
-characters = brain.Characters("/path/to/your/characters.json")
-```
-Once the object is initialized, the following methods can be used:
-- `add(self, name: str, background: str) -> None: ` adds a character to the character class. Needs a unique name and background written in natural language.
-- `get(self, name: str) -> str: ` returns the background of a character.
-- `update(self, name: str, background: str) -> None: ` updates the background of a character.
-- `delete(self, name) -> None: ` removes a character from the Characters class
-- `save(self) -> None: ` saves all characters to path specified in initiailization
-
-The `Conversations` class requires a file path to a JSON file where the conversations data will be saved, a `Characters` object ss well as a `langchain.llms` object. Initiailize it as follows:
-```python
-# using 'characters' and 'import brain' from above.
-from langchain.llms import LlamaCpp
-llm = LlamaCpp(model_path='ggml-model-q4_0.bin') # Can be any LLM
-
-conversations = brain.Conversations("/path/to/your/conversations.json",
-                                    characters,
-                                    llm)
-```
-Once the object is initialized, the following methods can be used:
-- `new(self, context: str, participants: Set[str]) -> None: ` with a unique context and participants creates a new conversation in Conversations.
-- `get(self, context: str) -> Dict[str, any]:` returns the participants and log of a conversation in the structure of `{"participants":set, "log":[]}` from a conversation with context
-- `update(self, context: str, participants: Set[str], log: List[List[str]]) -> None: ` with a unique context update the participants (set) and log (list of [character, utterance] in sequential order)
-- `delete(self, context: str) -> None: ` deletes a conversation from Conversations
-- `append(self, context: str, speaker: str, utterance: str) -> None:` add utterance from speaker in conversation with unique context
-- `generate(self, context: str, muted: Set[str]) -> List[str]:` given a conversations context and muted characters have an unmuted character say something and add it to the conversation. returns `[speaker, utterance]`
-- `save(self) -> None: ` saves all conversations to a path specialized in initialization
+# lifelike
+A toolkit that allows for the creation of "lifelike" characters that you can interact with and change how they behave towards you
+
+
+## Brain Useage
+Install the package: `pip install git+https://github.com/lifelike-toolkit/lifelike.git`
+
+Then import it with `from lifelike import brain`
+
+The `Characters` class requires a file path to a JSON file where the characters data will be saved. To create a `Characters` object, initialize it as follows:
+```python
+from lifelike import brain
+characters = brain.Characters("/path/to/your/characters.json")
+```
+Once the object is initialized, the following methods can be used:
+- `add(self, name: str, background: str) -> None: ` adds a character to the character class. Needs a unique name and background written in natural language.
+- `get(self, name: str) -> str: ` returns the background of a character.
+- `update(self, name: str, background: str) -> None: ` updates the background of a character.
+- `delete(self, name) -> None: ` removes a character from the Characters class
+- `save(self) -> None: ` saves all characters to path specified in initiailization
+
+The `Conversations` class requires a file path to a JSON file where the conversations data will be saved, a `Characters` object ss well as a `langchain.llms` object. Initiailize it as follows:
+```python
+# using 'characters' and 'import brain' from above.
+from langchain.llms import LlamaCpp
+llm = LlamaCpp(model_path='ggml-model-q4_0.bin') # Can be any LLM
+
+conversations = brain.Conversations("/path/to/your/conversations.json",
+                                    characters,
+                                    llm)
+```
+Once the object is initialized, the following methods can be used:
+- `new(self, context: str, participants: Set[str]) -> None: ` with a unique context and participants creates a new conversation in Conversations.
+- `get(self, context: str) -> Dict[str, any]:` returns the participants and log of a conversation in the structure of `{"participants":set, "log":[]}` from a conversation with context
+- `update(self, context: str, participants: Set[str], log: List[List[str]]) -> None: ` with a unique context update the participants (set) and log (list of [character, utterance] in sequential order)
+- `delete(self, context: str) -> None: ` deletes a conversation from Conversations
+- `append(self, context: str, speaker: str, utterance: str) -> None:` add utterance from speaker in conversation with unique context
+- `generate(self, context: str, muted: Set[str]) -> List[str]:` given a conversations context and muted characters have an unmuted character say something and add it to the conversation. returns `[speaker, utterance]`
+- `save(self) -> None: ` saves all conversations to a path specialized in initialization
```

### Comparing `lifelike-1.0.7/lifelike/StateManager/base_game_tree.py` & `lifelike-1.0.9/lifelike/StateManager/base_game_tree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,351 +1,351 @@
-"""
-Meant to be used alongside chromadb, but any vectordb that uses KNN will work too.
-Tunes sequence embeddings to allow the game to more accurately predict player's intentions.
-For now, requires chromadb
-"""
-import numpy
-import json
-import uuid
-
-from langchain.schema import BaseRetriever
-from langchain.vectorstores import Chroma
-from langchain.embeddings.base import Embeddings # TODO: Make all embedding_function Embeddings interface
-
-class EdgeEmbedding:
-    """Edge embedding dictionary that stores, calculate and allows for retrieval of different preset embeddings"""
-    def __init__(self, name: str, embedding_function: Embeddings=None, current_embedding: list=None, current_weight: int=0) -> None:
-        """
-        Constructor. If loading from dict, use from_dict() instead. 
-        Params:
-            - name: identifier
-            - embedding_function: the function that takes a batch of responses and returns the corresponding batch of embeddings. If not provided, the embedding is marked as Final (no tuning allowed).
-            - current_embedding: the current embedding loaded from json, or pre-determined to bypass tuning. Defaulted to None.
-            - current_weight: the current weight loaded from json (use 1 to bypass tuning). If current_weight is 0, the current_embedding will be ignored. Defaulted to 0.
-        """
-        if not name:
-            raise Exception("edge embedding name cannot be None")
-
-        self.name = name
-        self._final = False # Whether tuning is disabled on this embedding
-
-        if embedding_function is None:
-            if current_embedding is None:
-                raise Exception("EdgeEmbedding {} was initialized with no embedding".format(name))
-            self._final = True # Activate Final flag
-        
-        self.embed = embedding_function
-
-        self.embedding = current_embedding
-
-        self.weight = current_weight # The number of responses this embedding represents
-
-    @classmethod
-    def from_dict(cls:'EdgeEmbedding', embedding_dict: dict, embedding_function: Embeddings=None) -> 'EdgeEmbedding':
-        """
-        Generate up a edge Embedding instance. DO NOT USE TO MAKE DEEP COPY, use copy() instead
-        Params:
-            - embedding_dict: the result of edgeEmbedding.to_dict() instance method, or a dict with the same format
-            - embedding_function: the function that takes a batch of responses and returns the corresponding batch of embeddings. Set to None if no tuning is required
-        """
-        name = embedding_dict["name"]
-        embedding = embedding_dict["embedding"]
-        weight = embedding_dict["weight"]
-        return cls(name, embedding_function, embedding, weight)
-
-    def get_embedding(self) -> list:
-        """
-        Getter function for embedding attribute. Defaulted to all 0s if no responses have been added.
-        """
-        return self.embedding
-
-    def tune_prompts(self, prompts: list) -> list:
-        """
-        Add prompts to the embedding and calculates new embedding using weighted average. Tunes embedding of SequenceEvent.
-        Potentially suffers from density bias. Good response choices will depend on choice of embedding function.
-        Params:
-            -  prompts: the list of prompts that should be matched to this edge_embedding instance
-
-        Returns: The new embedding
-        """
-        if self._final:
-            print("The Embedding is marked as Final. Cannot be tuned.")
-            return None
-
-        new_embeddings = self.embed.embed_documents(prompts)
-
-        # Update weighted average
-        self.embedding = numpy.average([self.embedding] + new_embeddings, 0, [self.weight]+[1]*len(prompts)).tolist()
-
-        # Update weights
-        self.weight += len(prompts)
-        return self.embedding
-
-    def to_dict(self) -> dict:
-        """
-        Used to save to json as part of configuration, as well as make a copy
-        Returns: a dict of the form {'name': ..., 'embedding': ..., 'weight': ...} 
-        """
-        return {
-            'name': self.name,
-            'embedding': self.embedding,
-            'weight': self.weight
-        }
-
-    def copy(self, new_name: str) -> 'EdgeEmbedding':
-        """
-        Return a deep copy of this edgeEmbedding instance.
-        Params:
-            - new_name: Give new name. Ensure it is unique in the game to avoid unexpected behaviours.
-        """
-        embedding_dict = self.to_dict()
-        embedding_dict["name"] = new_name
-        return EdgeEmbedding.from_dict(embedding_dict, self.embed)
-
-
-class GameNode:
-    """Wrapper for a document in Database"""
-    def __init__(self, id: str, context: str, metadata: str) -> None:
-        """
-        Constructor. To build the event from dict, use .from_dict()
-        Params:
-            - id: self-explanatory
-            - context: also self-explanatory
-            - metadata: the text prompts given as response to player speech.
-        """
-        self.id = id
-        self.context = context
-        self.metadata = metadata # Future proofing
-
-    def to_dict(self) -> dict:
-        """Saves tree to a dictionary that can be serialized with json"""
-        return {
-            'id': self.id,
-            'context': self.context,
-            'metadata': self.metadata
-        }
-
-    @staticmethod
-    def from_dict(node_dict: dict) -> 'GameNode':
-        """Rebuild tree using a dictionary to resume progress (expects json deserialization higher up in the process)"""
-        return GameNode(node_dict["id"], node_dict["context"], node_dict["metadata"])
-
-
-class BaseGameTree:
-    """
-    Provides methods that supports building out a Game Tree and acts as an interface for Database.
-    Only Constructor can exit to support retries.
-    Technically a graph, not a tree.
-    """
-    def __init__(self, name: str, embedding_function: Embeddings=None) -> None:
-        """
-        Constructor.
-        Params:
-            - name: Name of the story (Must be chromadb friendly)
-            - embedding_function: Takes input and returns embedding. If not provided, the Tree is marked as Final (cannot be changed)
-        """
-        self.name = name
-        self._final = False # Final flag, determines if any change can be made to the tree
-        # if flag is False, embedding_function will be used to determine embedding using document text
-
-        if embedding_function is None:
-            print('Tree {} was initialized in final mode'.format(name)) # TODO Final Mode might be excessive in constructor
-            self._final = True # Activate Final flag
-        
-        self.embed = embedding_function # TODO Rename this, Embeddings is not a function
-
-        # TODO add persistent option and metadata preset
-        self.vectorstore = Chroma(name, self.embed) # Preset to Chroma TODO make this work with all vectorstore
-
-        # Currently, if there are 2 ways to reach an event, a copy with a new unique id must be made
-        self.node_dict = {} # id - SequenceEvent. Mostly for lookup
-
-        self.embedding_template_dict = {} # All Embedding template must be copied using .copy() to be used or risk unexpected behaviour
-
-        # Provides edge look up for custom edge embedding. Format: {(SequenceEvent left, SequenceEvent right): edgeEmbedding embedding}
-        # Where left is start event, right is end event, and embedding is the required embedding to go from left to right
-        self.edge_dict = {} 
-
-    def add_texts(self, texts, metadatas = None, ids = None, custom_embeddings = None):
-        """
-        Create GameNode and add to GameTree using add_node().
-        Must be overriden if a child of GameNode is used.
-        """
-        if ids is None: # If id not provided, generate it
-            ids = [str(uuid.uuid1()) for _ in texts]
-
-        if custom_embeddings is None:
-            embeddings = self.embed.embed_documents(texts)
-
-        # Text to tree. Does not allow for custom edges
-        for i in range(len(texts)):
-            node = GameNode(ids[i], texts[i], metadatas[i])
-            edge = EdgeEmbedding(ids[i], self.embed, embeddings[i], 20) # Tunable embedding with default weight of 20
-            self.add_node(node)
-            self.add_edge('_', node.id, ids[i], edge)
-
-        return ids
-
-    def add_node(self, node: GameNode) -> bool:
-        """
-        Add a GameNode to the GameTree. 
-        Params:
-            - node: a GameNode instance
-        """
-        if self._final:
-            print("Game Tree was marked as Final. No change can be made to it")
-            return False
-
-        event_id = node.id
-
-        if event_id in self.node_dict:
-            print("Sequence Event id {} already exists. If there is a second way to reach this event, create a copy with a unique id and retry")
-            return False
-        else:
-            self.node_dict[event_id] = node
-            return True
-
-    def add_embedding_template(self, edge_embedding: EdgeEmbedding) -> bool:
-        """
-        Add embedding template.
-        Params:
-            - name: the name for the template
-            - prompts: the initial prompts to tune the template. If None, consider using the "default" template instead.
-        """
-        if self._final:
-            print("Game Tree was marked as Final. No change can be made to it")
-            return False
-
-        name = edge_embedding.name
-
-        if name in self.embedding_template_dict:
-            print("Embedding template {} already exists. Use a new unique name")
-            return False
-        else:
-            self.embedding_template_dict[name] = edge_embedding
-            return True
-
-    def add_edge(self, start_id: str, end_id: str, embedding_name: str, embedding_template: EdgeEmbedding) -> bool:
-        """
-        Add edge to the tree and assign a premade embedding template. 
-        Most of the time, you only have to override validate_edge() to modify behaviour.
-        Params:
-            - start_id: The id of the start event. Must exists in event_dict.
-            - end_id: The id of the end event. Must exists in event_dict.
-            - embedding_name: Rename the embedding class. Ensure it is unique to avoid unexpected behaviours.
-            - embedding_template: The EdgeEmbedding object to use as a template. For saved templates, use get_template().
-        """
-        if self.validate_edge(start_id, end_id, embedding_template.name):
-            # Assigns to edge_dict
-            self.edge_dict[(start_id, end_id)] = embedding_template.copy(embedding_name)
-            return True
-
-    def validate_edge(self, start_id: str, end_id: str, embedding_template_name: str="default") -> bool:
-        """Validates new edge_dict entry. Only contains basic validation, should be overidden to prevent undesireable behaviour"""
-        if self._final:
-            print("Game Tree was marked as Final. No change can be made to it")
-            return False
-        elif end_id not in self.node_dict: # Allows for a setup like (_, end_id) where any node can reach end_id
-            print("Either start_id or end_id does not exist in event_dict. Must be 2 of {}.".format(self.node_dict.keys()))
-            return False
-        elif embedding_template_name not in self.embedding_template_dict:
-            print("Invalid template: Embedding Template must be one of {}. Create one with add_embedding_template() or use the default template".format(self.embedding_template_dict.keys()))
-            return False
-        elif (start_id, end_id) in self.edge_dict:
-            print("Invalid edge: edge {} already exists".format(start_id + '-' + end_id))
-            return False
-        else:
-            return True
-
-    def tune_edge(self, edge_id: tuple, prompts: list) -> bool:
-        """
-        Tune the chosen embedding with extra prompts.
-        Params:
-            - edge_id: Identifier for edge, is a tuple of form (start_event, end_event)
-            - prompts: List of prompts for tuning
-        """
-        if self._final:
-            print("Game Tree was marked as Final. No change can be made to it")
-            return False
-
-        if edge_id not in self.edge_dict:
-            print("edge {} does not exists".format(edge_id))
-            return False
-        self.edge_dict[edge_id].tune_prompts(prompts)
-        return True
-
-    def get_template_options(self) -> list:
-        """Get the name of all stored templates"""
-        return self.embedding_template_dict.keys()
-
-    def get_template(self, name) -> EdgeEmbedding:
-        if name not in self.get_template_options():
-            print("No embedding with name {} found".format(name))
-            return None
-
-        return self.embedding_template_dict[name]
-
-    @classmethod
-    def build_from_json(cls:'BaseGameTree', edge_to_json: str, embedding_function: Embeddings=None) -> 'BaseGameTree':
-        """
-        Rebuild tree from JSON file. May cause unexpected behaviour if the JSON file was built using derived GameNode and EdgeEmbedding classes.
-        Params:
-            - edge_to_json: The string that signifies the edge to the jsonified tree
-            - embedding_function: Takes input and returns embedding. If not provided, the Tree is marked as Final (cannot be changed)
-        """
-        tree_dict = {}
-        with open(edge_to_json, "r") as f:
-            tree_dict = json.load(f)
-
-        tree = cls(tree_dict["name"], embedding_function)
-        for (template_name, template_dict) in tree_dict["embedding_template_dict"].items():
-            tree.embedding_template_dict[template_name] = EdgeEmbedding.from_dict(template_dict, embedding_function)
-
-        for (event_id, event_dict) in tree_dict["event_dict"].items():
-            tree.node_dict[event_id] = GameNode.from_dict(event_dict)
-
-        for (edge_string, embedding_dict) in tree_dict["edge_dict"].items():
-            edge = edge_string.split(" ") # Split by " "
-            tree.edge_dict[edge] = EdgeEmbedding.from_dict(embedding_dict, embedding_function)
-        
-        return tree
-
-    def to_dict(self) -> dict:
-        """Return the instance in dictionary form to be saved to json"""
-        return {
-            "name": self.name,
-            "embedding_template_dict": {template_id: template.to_dict() for (template_id, template) in self.embedding_template_dict.items()}, # Kinda optional here
-            "event_dict": {event_id: event.to_dict() for (event_id, event) in self.node_dict.items()},
-            "edge_dict": {edge[0]+" "+edge[1]: embedding.to_dict() for (edge, embedding) in self.edge_dict.items()}
-        }
-
-    def to_json(self, edge_to_json: str) -> None:
-        """Saves current Tree configuration to json"""
-        with open(edge_to_json, "w") as f:
-            json.dump(self.to_dict(), f, indent=4)
-
-    def write_db(self):
-        """Write current tree to a ChromaDB collection."""
-        # Only need to add the following nodes to chroma, as the starting state does not need to be defined
-        embeddings = []
-        documents = []
-        metadatas=[]
-        ids=[]
-
-        for (edge, embedding) in self.edge_dict.items():
-            target_node_id = edge[1]
-            target_node = self.node_dict[target_node_id]
-
-            embeddings.append(embedding.get_embedding())
-            documents.append(target_node.context)
-            ids.append(target_node_id)
-            metadatas.append(target_node.metadata)
-
-        self.vectorstore._collection.add(ids=ids, embeddings=embeddings, metadatas=metadatas, documents=documents)
-
-    def get_retriever(self, **kwargs) -> BaseRetriever:
-        """
-        Some possible arguments:
-            - search_type
-            - search_kwargs: {"k": Number of returned results}
-        """
-        return self.vectorstore.as_retriever(**kwargs) # Adding some options
+"""
+Meant to be used alongside chromadb, but any vectordb that uses KNN will work too.
+Tunes sequence embeddings to allow the game to more accurately predict player's intentions.
+For now, requires chromadb
+"""
+import numpy
+import json
+import uuid
+
+from langchain.schema import BaseRetriever
+from langchain.vectorstores import Chroma
+from langchain.embeddings.base import Embeddings # TODO: Make all embedding_function Embeddings interface
+
+class EdgeEmbedding:
+    """Edge embedding dictionary that stores, calculate and allows for retrieval of different preset embeddings"""
+    def __init__(self, name: str, embedding_function: Embeddings=None, current_embedding: list=None, current_weight: int=0) -> None:
+        """
+        Constructor. If loading from dict, use from_dict() instead. 
+        Params:
+            - name: identifier
+            - embedding_function: the function that takes a batch of responses and returns the corresponding batch of embeddings. If not provided, the embedding is marked as Final (no tuning allowed).
+            - current_embedding: the current embedding loaded from json, or pre-determined to bypass tuning. Defaulted to None.
+            - current_weight: the current weight loaded from json (use 1 to bypass tuning). If current_weight is 0, the current_embedding will be ignored. Defaulted to 0.
+        """
+        if not name:
+            raise Exception("edge embedding name cannot be None")
+
+        self.name = name
+        self._final = False # Whether tuning is disabled on this embedding
+
+        if embedding_function is None:
+            if current_embedding is None:
+                raise Exception("EdgeEmbedding {} was initialized with no embedding".format(name))
+            self._final = True # Activate Final flag
+        
+        self.embed = embedding_function
+
+        self.embedding = current_embedding
+
+        self.weight = current_weight # The number of responses this embedding represents
+
+    @classmethod
+    def from_dict(cls:'EdgeEmbedding', embedding_dict: dict, embedding_function: Embeddings=None) -> 'EdgeEmbedding':
+        """
+        Generate up a edge Embedding instance. DO NOT USE TO MAKE DEEP COPY, use copy() instead
+        Params:
+            - embedding_dict: the result of edgeEmbedding.to_dict() instance method, or a dict with the same format
+            - embedding_function: the function that takes a batch of responses and returns the corresponding batch of embeddings. Set to None if no tuning is required
+        """
+        name = embedding_dict["name"]
+        embedding = embedding_dict["embedding"]
+        weight = embedding_dict["weight"]
+        return cls(name, embedding_function, embedding, weight)
+
+    def get_embedding(self) -> list:
+        """
+        Getter function for embedding attribute. Defaulted to all 0s if no responses have been added.
+        """
+        return self.embedding
+
+    def tune_prompts(self, prompts: list) -> list:
+        """
+        Add prompts to the embedding and calculates new embedding using weighted average. Tunes embedding of SequenceEvent.
+        Potentially suffers from density bias. Good response choices will depend on choice of embedding function.
+        Params:
+            -  prompts: the list of prompts that should be matched to this edge_embedding instance
+
+        Returns: The new embedding
+        """
+        if self._final:
+            print("The Embedding is marked as Final. Cannot be tuned.")
+            return None
+
+        new_embeddings = self.embed.embed_documents(prompts)
+
+        # Update weighted average
+        self.embedding = numpy.average([self.embedding] + new_embeddings, 0, [self.weight]+[1]*len(prompts)).tolist()
+
+        # Update weights
+        self.weight += len(prompts)
+        return self.embedding
+
+    def to_dict(self) -> dict:
+        """
+        Used to save to json as part of configuration, as well as make a copy
+        Returns: a dict of the form {'name': ..., 'embedding': ..., 'weight': ...} 
+        """
+        return {
+            'name': self.name,
+            'embedding': self.embedding,
+            'weight': self.weight
+        }
+
+    def copy(self, new_name: str) -> 'EdgeEmbedding':
+        """
+        Return a deep copy of this edgeEmbedding instance.
+        Params:
+            - new_name: Give new name. Ensure it is unique in the game to avoid unexpected behaviours.
+        """
+        embedding_dict = self.to_dict()
+        embedding_dict["name"] = new_name
+        return EdgeEmbedding.from_dict(embedding_dict, self.embed)
+
+
+class GameNode:
+    """Wrapper for a document in Database"""
+    def __init__(self, id: str, context: str, metadata: str) -> None:
+        """
+        Constructor. To build the event from dict, use .from_dict()
+        Params:
+            - id: self-explanatory
+            - context: also self-explanatory
+            - metadata: the text prompts given as response to player speech.
+        """
+        self.id = id
+        self.context = context
+        self.metadata = metadata # Future proofing
+
+    def to_dict(self) -> dict:
+        """Saves tree to a dictionary that can be serialized with json"""
+        return {
+            'id': self.id,
+            'context': self.context,
+            'metadata': self.metadata
+        }
+
+    @staticmethod
+    def from_dict(node_dict: dict) -> 'GameNode':
+        """Rebuild tree using a dictionary to resume progress (expects json deserialization higher up in the process)"""
+        return GameNode(node_dict["id"], node_dict["context"], node_dict["metadata"])
+
+
+class BaseGameTree:
+    """
+    Provides methods that supports building out a Game Tree and acts as an interface for Database.
+    Only Constructor can exit to support retries.
+    Technically a graph, not a tree.
+    """
+    def __init__(self, name: str, embedding_function: Embeddings=None) -> None:
+        """
+        Constructor.
+        Params:
+            - name: Name of the story (Must be chromadb friendly)
+            - embedding_function: Takes input and returns embedding. If not provided, the Tree is marked as Final (cannot be changed)
+        """
+        self.name = name
+        self._final = False # Final flag, determines if any change can be made to the tree
+        # if flag is False, embedding_function will be used to determine embedding using document text
+
+        if embedding_function is None:
+            print('Tree {} was initialized in final mode'.format(name)) # TODO Final Mode might be excessive in constructor
+            self._final = True # Activate Final flag
+        
+        self.embed = embedding_function # TODO Rename this, Embeddings is not a function
+
+        # TODO add persistent option and metadata preset
+        self.vectorstore = Chroma(name, self.embed) # Preset to Chroma TODO make this work with all vectorstore
+
+        # Currently, if there are 2 ways to reach an event, a copy with a new unique id must be made
+        self.node_dict = {} # id - SequenceEvent. Mostly for lookup
+
+        self.embedding_template_dict = {} # All Embedding template must be copied using .copy() to be used or risk unexpected behaviour
+
+        # Provides edge look up for custom edge embedding. Format: {(SequenceEvent left, SequenceEvent right): edgeEmbedding embedding}
+        # Where left is start event, right is end event, and embedding is the required embedding to go from left to right
+        self.edge_dict = {} 
+
+    def add_texts(self, texts, metadatas = None, ids = None, custom_embeddings = None):
+        """
+        Create GameNode and add to GameTree using add_node().
+        Must be overriden if a child of GameNode is used.
+        """
+        if ids is None: # If id not provided, generate it
+            ids = [str(uuid.uuid1()) for _ in texts]
+
+        if custom_embeddings is None:
+            embeddings = self.embed.embed_documents(texts)
+
+        # Text to tree. Does not allow for custom edges
+        for i in range(len(texts)):
+            node = GameNode(ids[i], texts[i], metadatas[i])
+            edge = EdgeEmbedding(ids[i], self.embed, embeddings[i], 20) # Tunable embedding with default weight of 20
+            self.add_node(node)
+            self.add_edge('_', node.id, ids[i], edge)
+
+        return ids
+
+    def add_node(self, node: GameNode) -> bool:
+        """
+        Add a GameNode to the GameTree. 
+        Params:
+            - node: a GameNode instance
+        """
+        if self._final:
+            print("Game Tree was marked as Final. No change can be made to it")
+            return False
+
+        event_id = node.id
+
+        if event_id in self.node_dict:
+            print("Sequence Event id {} already exists. If there is a second way to reach this event, create a copy with a unique id and retry")
+            return False
+        else:
+            self.node_dict[event_id] = node
+            return True
+
+    def add_embedding_template(self, edge_embedding: EdgeEmbedding) -> bool:
+        """
+        Add embedding template.
+        Params:
+            - name: the name for the template
+            - prompts: the initial prompts to tune the template. If None, consider using the "default" template instead.
+        """
+        if self._final:
+            print("Game Tree was marked as Final. No change can be made to it")
+            return False
+
+        name = edge_embedding.name
+
+        if name in self.embedding_template_dict:
+            print("Embedding template {} already exists. Use a new unique name")
+            return False
+        else:
+            self.embedding_template_dict[name] = edge_embedding
+            return True
+
+    def add_edge(self, start_id: str, end_id: str, embedding_name: str, embedding_template: EdgeEmbedding) -> bool:
+        """
+        Add edge to the tree and assign a premade embedding template. 
+        Most of the time, you only have to override validate_edge() to modify behaviour.
+        Params:
+            - start_id: The id of the start event. Must exists in event_dict.
+            - end_id: The id of the end event. Must exists in event_dict.
+            - embedding_name: Rename the embedding class. Ensure it is unique to avoid unexpected behaviours.
+            - embedding_template: The EdgeEmbedding object to use as a template. For saved templates, use get_template().
+        """
+        if self.validate_edge(start_id, end_id, embedding_template.name):
+            # Assigns to edge_dict
+            self.edge_dict[(start_id, end_id)] = embedding_template.copy(embedding_name)
+            return True
+
+    def validate_edge(self, start_id: str, end_id: str, embedding_template_name: str="default") -> bool:
+        """Validates new edge_dict entry. Only contains basic validation, should be overidden to prevent undesireable behaviour"""
+        if self._final:
+            print("Game Tree was marked as Final. No change can be made to it")
+            return False
+        elif end_id not in self.node_dict: # Allows for a setup like (_, end_id) where any node can reach end_id
+            print("Either start_id or end_id does not exist in event_dict. Must be 2 of {}.".format(self.node_dict.keys()))
+            return False
+        # elif embedding_template_name not in self.embedding_template_dict:
+        #     print("Invalid template: Embedding Template must be one of {}. Create one with add_embedding_template() or use the default template".format(self.embedding_template_dict.keys()))
+        #     return False
+        elif (start_id, end_id) in self.edge_dict:
+            print("Invalid edge: edge {} already exists".format(start_id + '-' + end_id))
+            return False
+        else:
+            return True
+
+    def tune_edge(self, edge_id: tuple, prompts: list) -> bool:
+        """
+        Tune the chosen embedding with extra prompts.
+        Params:
+            - edge_id: Identifier for edge, is a tuple of form (start_event, end_event)
+            - prompts: List of prompts for tuning
+        """
+        if self._final:
+            print("Game Tree was marked as Final. No change can be made to it")
+            return False
+
+        if edge_id not in self.edge_dict:
+            print("edge {} does not exists".format(edge_id))
+            return False
+        self.edge_dict[edge_id].tune_prompts(prompts)
+        return True
+
+    def get_template_options(self) -> list:
+        """Get the name of all stored templates"""
+        return self.embedding_template_dict.keys()
+
+    def get_template(self, name) -> EdgeEmbedding:
+        if name not in self.get_template_options():
+            print("No embedding with name {} found".format(name))
+            return None
+
+        return self.embedding_template_dict[name]
+
+    @classmethod
+    def build_from_json(cls:'BaseGameTree', edge_to_json: str, embedding_function: Embeddings=None) -> 'BaseGameTree':
+        """
+        Rebuild tree from JSON file. May cause unexpected behaviour if the JSON file was built using derived GameNode and EdgeEmbedding classes.
+        Params:
+            - edge_to_json: The string that signifies the edge to the jsonified tree
+            - embedding_function: Takes input and returns embedding. If not provided, the Tree is marked as Final (cannot be changed)
+        """
+        tree_dict = {}
+        with open(edge_to_json, "r") as f:
+            tree_dict = json.load(f)
+
+        tree = cls(tree_dict["name"], embedding_function)
+        for (template_name, template_dict) in tree_dict["embedding_template_dict"].items():
+            tree.embedding_template_dict[template_name] = EdgeEmbedding.from_dict(template_dict, embedding_function)
+
+        for (event_id, event_dict) in tree_dict["event_dict"].items():
+            tree.node_dict[event_id] = GameNode.from_dict(event_dict)
+
+        for (edge_string, embedding_dict) in tree_dict["edge_dict"].items():
+            edge = edge_string.split(" ") # Split by " "
+            tree.edge_dict[edge] = EdgeEmbedding.from_dict(embedding_dict, embedding_function)
+        
+        return tree
+
+    def to_dict(self) -> dict:
+        """Return the instance in dictionary form to be saved to json"""
+        return {
+            "name": self.name,
+            "embedding_template_dict": {template_id: template.to_dict() for (template_id, template) in self.embedding_template_dict.items()}, # Kinda optional here
+            "event_dict": {event_id: event.to_dict() for (event_id, event) in self.node_dict.items()},
+            "edge_dict": {edge[0]+" "+edge[1]: embedding.to_dict() for (edge, embedding) in self.edge_dict.items()}
+        }
+
+    def to_json(self, edge_to_json: str) -> None:
+        """Saves current Tree configuration to json"""
+        with open(edge_to_json, "w") as f:
+            json.dump(self.to_dict(), f, indent=4)
+
+    def write_db(self):
+        """Write current tree to a ChromaDB collection."""
+        # Only need to add the following nodes to chroma, as the starting state does not need to be defined
+        embeddings = []
+        documents = []
+        metadatas=[]
+        ids=[]
+
+        for (edge, embedding) in self.edge_dict.items():
+            target_node_id = edge[1]
+            target_node = self.node_dict[target_node_id]
+
+            embeddings.append(embedding.get_embedding())
+            documents.append(target_node.context)
+            ids.append(target_node_id)
+            metadatas.append(target_node.metadata)
+
+        self.vectorstore._collection.add(ids=ids, embeddings=embeddings, metadatas=metadatas, documents=documents)
+
+    def get_retriever(self, **kwargs) -> BaseRetriever:
+        """
+        Some possible arguments:
+            - search_type
+            - search_kwargs: {"k": Number of returned results}
+        """
+        return self.vectorstore.as_retriever(**kwargs) # Adding some options
```

### Comparing `lifelike-1.0.7/lifelike/StateManager/knowledge_tree.py` & `lifelike-1.0.9/lifelike/StateManager/knowledge_tree.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""
-Inherits from BaseGameTree. Demonstrates a GameTree for knowledge-based games
-"""
-import uuid
-
-from langchain.vectorstores import Chroma
-from langchain.embeddings.base import Embeddings
-
-from lifelike.StateManager.base_game_tree import BaseGameTree
-
-class KnowledgeTree(BaseGameTree):
-    """Allows for loading the tree from a pre-defined list of contextual texts"""
-    @classmethod
-    def from_texts(cls: BaseGameTree, name:str, texts: list[str], embedding_function: Embeddings, metadatas: list[dict]=None, ids: list[str]=None) -> 'KnowledgeTree':
-        """For now, must know the embedding dimension."""
-        if ids is None: # If id not provided, generate it
-            ids = [str(uuid.uuid1()) for _ in texts]
-
-        tree = cls(name, embedding_function)
-        # TODO: Currently bypasses building tree. Tree is essentially non-functional
-        tree.vectorstore = Chroma.from_texts(texts, embedding_function, metadatas, ids)
+"""
+Inherits from BaseGameTree. Demonstrates a GameTree for knowledge-based games
+"""
+import uuid
+
+from langchain.vectorstores import Chroma
+from langchain.embeddings.base import Embeddings
+
+from lifelike.StateManager.base_game_tree import BaseGameTree
+
+class KnowledgeTree(BaseGameTree):
+    """Allows for loading the tree from a pre-defined list of contextual texts"""
+    @classmethod
+    def from_texts(cls: BaseGameTree, name:str, texts: list[str], embedding_function: Embeddings, metadatas: list[dict]=None, ids: list[str]=None) -> 'KnowledgeTree':
+        """For now, must know the embedding dimension."""
+        if ids is None: # If id not provided, generate it
+            ids = [str(uuid.uuid1()) for _ in texts]
+
+        tree = cls(name, embedding_function)
+        # TODO: Currently bypasses building tree. Tree is essentially non-functional
+        tree.vectorstore = Chroma.from_texts(texts, embedding_function, metadatas, ids)
         return tree
```

### Comparing `lifelike-1.0.7/lifelike/StateManager/sequence_tree.py` & `lifelike-1.0.9/lifelike/StateManager/sequence_tree.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-Inherits from GameNode. Meant for linear games with branching story paths.
-Good example of simple GameTree object.
-"""
-from lifelike.StateManager.base_game_tree import GameNodeRetriever, BaseGameTree, GameNode, EdgeEmbedding
-
-PathEmbedding = EdgeEmbedding
-
-class SequenceEvent(GameNode):
-    """Wrapper for an event document in Database. The game can only see 1 at a time."""
-    def __init__(self, id: str, context: str, metadata: dict={}, reachable: list[str]=[]) -> None:
-        """
-        Constructor. To build the event from dict, use .from_dict()
-        Params:
-            - id: self-explanatory
-            - context: also self-explanatory
-            - metadata: the text prompts given as response to player speech.
-            - reachable: list of ids for sequence event that this specific event can reach. This behaviour can be customized via SequenceEventRetriever
-        """
-        super().__init__(id, context, metadata)
-        self.metadata["reachable"] = reachable # Internal metadata
-
-
-class SequenceTree(BaseGameTree):
-    """
-    Technically a graph. Only used during Database setup. 
-    Provides methods that supports building out a sequence tree and acts as an interface for Database.
-    Only Constructor can exit to support retries.
-    """
-    def validate_edge(self, start_id: str, end_id: str, embedding_name: str, embedding_template: str = "default") -> bool:
-        """Validates new edge_dict entry. All node in an edge must exist."""
-        if not super().validate_edge(start_id, end_id, embedding_name, embedding_template):
-            return False
-        elif start_id not in self.node_dict or end_id not in self.node_dict:
-            print("Either start_id or end_id does not exist in event_dict. Must be 2 of {}.".format(self.node_dict.keys()))
-            return False
-        else:
-            return True
-
-    def add_edge(self, start_id: str, end_id: str, embedding_name: str, embedding_template: str = "default") -> bool:
-        if super().add_edge(start_id, end_id, embedding_name, embedding_template):
+"""
+Inherits from GameNode. Meant for linear games with branching story paths.
+Good example of simple GameTree object.
+"""
+from lifelike.StateManager.base_game_tree import GameNodeRetriever, BaseGameTree, GameNode, EdgeEmbedding
+
+PathEmbedding = EdgeEmbedding
+
+class SequenceEvent(GameNode):
+    """Wrapper for an event document in Database. The game can only see 1 at a time."""
+    def __init__(self, id: str, context: str, metadata: dict={}, reachable: list[str]=[]) -> None:
+        """
+        Constructor. To build the event from dict, use .from_dict()
+        Params:
+            - id: self-explanatory
+            - context: also self-explanatory
+            - metadata: the text prompts given as response to player speech.
+            - reachable: list of ids for sequence event that this specific event can reach. This behaviour can be customized via SequenceEventRetriever
+        """
+        super().__init__(id, context, metadata)
+        self.metadata["reachable"] = reachable # Internal metadata
+
+
+class SequenceTree(BaseGameTree):
+    """
+    Technically a graph. Only used during Database setup. 
+    Provides methods that supports building out a sequence tree and acts as an interface for Database.
+    Only Constructor can exit to support retries.
+    """
+    def validate_edge(self, start_id: str, end_id: str, embedding_name: str, embedding_template: str = "default") -> bool:
+        """Validates new edge_dict entry. All node in an edge must exist."""
+        if not super().validate_edge(start_id, end_id, embedding_name, embedding_template):
+            return False
+        elif start_id not in self.node_dict or end_id not in self.node_dict:
+            print("Either start_id or end_id does not exist in event_dict. Must be 2 of {}.".format(self.node_dict.keys()))
+            return False
+        else:
+            return True
+
+    def add_edge(self, start_id: str, end_id: str, embedding_name: str, embedding_template: str = "default") -> bool:
+        if super().add_edge(start_id, end_id, embedding_name, embedding_template):
             self.node_dict[start_id].metadata["reachable"].append(end_id)
```

### Comparing `lifelike-1.0.7/lifelike/brain.py` & `lifelike-1.0.9/lifelike/brain.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-"""
-This file contains the interface to manage characters and conversations
-"""
-import json
-import os
-import random
-from typing import List, Dict, Set
-from langchain import PromptTemplate, LLMChain
-
-
-class Characters:
-    """
-    This class is an interface to manage characters.
-    """
-    def __init__(self, path: str) -> None:
-        """
-        @param path: path to the json file
-        @return: None, initializes Characters
-        """
-        self.path = path
-        self.characters = {}
-        if os.path.exists(path):
-            self.characters = json.load(open(path, 'r', encoding='utf-8'))
-
-    def is_out(self, name: str) -> ValueError:
-        """
-        @param name: unique name of the character
-        @return: ValueError if character does not exist
-        """
-        if name not in self.characters:
-            raise ValueError(f"Character {name} does not exist.")
-
-    def is_in(self, name: str) -> ValueError:
-        """
-        @param name: unique name of the character
-        @return: ValueError if character exists
-        """
-        if name in self.characters:
-            raise ValueError(f"Character {name} already exists.")
-
-    def get(self, name: str) -> str:
-        """
-        @param name: unique name of the character
-        @return: background of the character
-        """
-        self.is_out(name)
-        return self.characters[name]
-
-    def add(self, name: str, background: str) -> None:
-        """
-        @param name: unique name of the character
-        @param background: background of the character
-        @return: None, adds character to Characters
-        """
-        self.is_in(name)
-        self.characters[name] = background
-
-    def update(self, name: str, background: str) -> None:
-        """
-        @param new_name: name of the character
-        @param background: new background of the character
-        @return: None, updates character in Characters
-        """
-        self.is_out(name)
-        self.characters[name] = background
-
-    def delete(self, name) -> None:
-        """
-        @param name: unique name of the character
-        @return: None, deletes character from Characters
-        """
-        self.is_out(name)
-        self.characters.pop(name)
-
-    def __str__(self) -> str:
-        """
-        @return: string representation of Characters
-        """
-        return str(self.characters)
-
-    def save(self) -> None:
-        """
-        @return: None, saves Characters to json file
-        """
-        json.dump(self.characters, open(self.path, 'w', encoding='utf-8'))
-
-
-class Conversations:
-    """
-    This class is an interface to manage conversations
-    """
-    def __init__(self, path: str, characters: Characters, llm) -> None:
-        """
-        @param path: path to the json file
-        @param characters: Characters object
-        @param llm: langchain llm object
-        @return: None, initializes Conversations
-        """
-        # TODO: Allow for custom prompt template
-        self.path = path
-        self.valid = characters
-        self.llm = llm
-        self.conversations = {}
-        if os.path.exists(path):
-            self.conversations = json.load(open(path, 'r', encoding='utf-8'))
-
-    def context_out(self, context: str) -> ValueError:
-        """
-        @param context: unique context of the conversation
-        @return: ValueError if context does not exist
-        """
-        if context not in self.conversations:
-            raise ValueError(f"Conversation {context} does not exist.")
-
-    def context_in(self, context: str) -> ValueError:
-        """
-        @param context: unique context of the conversation
-        @return: ValueError if context exists
-        """
-        if context in self.conversations:
-            raise ValueError(f"Conversation {context} already exists.")
-
-    def valid_participants(self, participants: Set[str]) -> ValueError:
-        """
-        @param context: unique context of the conversation
-        @param participants: list of character names
-        @return: ValueError if participants are invalid
-        """
-        invalid = participants - set(self.valid.characters)
-        if invalid:
-            raise ValueError(f"The participants in {invalid} do not exist.")
-
-    def get(self, context: str) -> Dict[str, any]:
-        """
-        @param context: unique context of the conversation
-        @return: participants and log of the conversation
-        """
-        self.context_out(context)
-        return self.conversations[context]
-
-    def new(self, context: str, participants: Set[str]) -> None:
-        """
-        @param context: unique context of the conversation
-        @param participants: list of character names
-        @return: None, creates new conversation
-        """
-        self.valid_participants(participants)
-        self.context_in(context)
-        self.conversations[context] = {"participants": participants, "log": []}
-
-    def update(self, context: str, participants: Set[str], log: List[List[str]]) -> None:
-        """
-        @param context: unique context of the conversation
-        @param participants: list of character names
-        @param log: list of [speaker, utterance]
-        @return: None, updates conversation
-        """
-        self.valid_participants(participants)
-        self.context_out(context)
-        self.conversations[context] = {"participants": participants, "log": log}
-
-    def delete(self, context: str) -> None:
-        """
-        @param context: unique context of the conversation
-        @return: None, deletes conversation
-        """
-        self.context_out(context)
-        self.conversations.pop(context)
-
-    def append(self, context: str, speaker: str, utterance: str) -> None:
-        """
-        @param context: unique context of the conversation
-        @param speaker: name of the speaker
-        @param utterance: utterance of the speaker
-        @return: None, appends utterance to the conversation
-        """
-        self.valid_participants({speaker})
-        self.context_out(context)
-        self.conversations[context]["log"].append([speaker, utterance])
-
-    def generate(self, context: str, history: str, muted: Set[str]) -> List[str]:
-        """
-        @param context: unique context of the conversation
-        @param muted: list of muted characters
-        @return: speaker and generated utterance
-        """
-        #TODO: find a smarter way to choose next character
-        #TODO: Find a smarter way to get a single response.
-        #TODO: memory for conversation log overflow
-        #TODO: memory for the context
-        #TODO: memory for the character background
-        self.valid_participants(muted)
-
-        convo = self.get(context)
-
-        convo_speakers = convo["participants"]
-        unmuted = convo_speakers.difference(muted)
-        next_speaker = random.sample(unmuted, 1)[0]
-        bg = self.valid.get(next_speaker)
-
-        convo_log = convo["log"]
-        log_str = '\n'.join([f"{speaker}: {utterance}" for speaker, utterance in convo_log])
-        # get last 3 lines of log
-        try:
-            log_str = '\n'.join(log_str.split('\n')[-3:])
-        except IndexError:
-            pass
-
-        template = "Context:\n"\
-        "{context}\n"\
-        "\n"\
-        "Background:\n"\
-        "{background}\n"\
-        "\n"\
-        "Relevant pieces of information:\n"\
-        "{history}\n"\
-        "(Only use if relevant to the conversation)\n"\
-        "\n"\
-        "Conversation:\n"\
-        "{log}\n"\
-        "{speaker}:"
-
-        prompt = PromptTemplate(template=template,
-                                input_variables=["context", "background",
-                                "history", "log", "speaker"])
-        chain = LLMChain(prompt=prompt, llm=self.llm)
-
-        output = chain.run({"context": context, "background": bg, "history": history, "log": log_str, "speaker": next_speaker})
-        if output != "":
-            output = output.split('\n')[0].lstrip()
-        self.append(context, next_speaker, output)
-        return [next_speaker, output]
-
-    def __str__(self) -> str:
-        """
-        @return: string representation of Conversations
-        """
-        return str(self.conversations)
-
-    def save(self) -> None:
-        """
-        @return: None, saves Conversations to json file
-        """
-        json.dump(self.conversations, open(self.path, 'w', encoding='utf-8'))
+"""
+This file contains the interface to manage characters and conversations
+"""
+import json
+import os
+import random
+from typing import List, Dict, Set
+from langchain import PromptTemplate, LLMChain
+
+
+class Characters:
+    """
+    This class is an interface to manage characters.
+    """
+    def __init__(self, path: str) -> None:
+        """
+        @param path: path to the json file
+        @return: None, initializes Characters
+        """
+        self.path = path
+        self.characters = {}
+        if os.path.exists(path):
+            self.characters = json.load(open(path, 'r', encoding='utf-8'))
+
+    def is_out(self, name: str) -> ValueError:
+        """
+        @param name: unique name of the character
+        @return: ValueError if character does not exist
+        """
+        if name not in self.characters:
+            raise ValueError(f"Character {name} does not exist.")
+
+    def is_in(self, name: str) -> ValueError:
+        """
+        @param name: unique name of the character
+        @return: ValueError if character exists
+        """
+        if name in self.characters:
+            raise ValueError(f"Character {name} already exists.")
+
+    def get(self, name: str) -> str:
+        """
+        @param name: unique name of the character
+        @return: background of the character
+        """
+        self.is_out(name)
+        return self.characters[name]
+
+    def add(self, name: str, background: str) -> None:
+        """
+        @param name: unique name of the character
+        @param background: background of the character
+        @return: None, adds character to Characters
+        """
+        self.is_in(name)
+        self.characters[name] = background
+
+    def update(self, name: str, background: str) -> None:
+        """
+        @param new_name: name of the character
+        @param background: new background of the character
+        @return: None, updates character in Characters
+        """
+        self.is_out(name)
+        self.characters[name] = background
+
+    def delete(self, name) -> None:
+        """
+        @param name: unique name of the character
+        @return: None, deletes character from Characters
+        """
+        self.is_out(name)
+        self.characters.pop(name)
+
+    def __str__(self) -> str:
+        """
+        @return: string representation of Characters
+        """
+        return str(self.characters)
+
+    def save(self) -> None:
+        """
+        @return: None, saves Characters to json file
+        """
+        json.dump(self.characters, open(self.path, 'w', encoding='utf-8'))
+
+
+class Conversations:
+    """
+    This class is an interface to manage conversations
+    """
+    def __init__(self, path: str, characters: Characters, llm) -> None:
+        """
+        @param path: path to the json file
+        @param characters: Characters object
+        @param llm: langchain llm object
+        @return: None, initializes Conversations
+        """
+        # TODO: Allow for custom prompt template
+        self.path = path
+        self.valid = characters
+        self.llm = llm
+        self.conversations = {}
+        if os.path.exists(path):
+            self.conversations = json.load(open(path, 'r', encoding='utf-8'))
+
+    def context_out(self, context: str) -> ValueError:
+        """
+        @param context: unique context of the conversation
+        @return: ValueError if context does not exist
+        """
+        if context not in self.conversations:
+            raise ValueError(f"Conversation {context} does not exist.")
+
+    def context_in(self, context: str) -> ValueError:
+        """
+        @param context: unique context of the conversation
+        @return: ValueError if context exists
+        """
+        if context in self.conversations:
+            raise ValueError(f"Conversation {context} already exists.")
+
+    def valid_participants(self, participants: Set[str]) -> ValueError:
+        """
+        @param context: unique context of the conversation
+        @param participants: list of character names
+        @return: ValueError if participants are invalid
+        """
+        invalid = participants - set(self.valid.characters)
+        if invalid:
+            raise ValueError(f"The participants in {invalid} do not exist.")
+
+    def get(self, context: str) -> Dict[str, any]:
+        """
+        @param context: unique context of the conversation
+        @return: participants and log of the conversation
+        """
+        self.context_out(context)
+        return self.conversations[context]
+
+    def new(self, context: str, participants: Set[str]) -> None:
+        """
+        @param context: unique context of the conversation
+        @param participants: list of character names
+        @return: None, creates new conversation
+        """
+        self.valid_participants(participants)
+        self.context_in(context)
+        self.conversations[context] = {"participants": participants, "log": []}
+
+    def update(self, context: str, participants: Set[str], log: List[List[str]]) -> None:
+        """
+        @param context: unique context of the conversation
+        @param participants: list of character names
+        @param log: list of [speaker, utterance]
+        @return: None, updates conversation
+        """
+        self.valid_participants(participants)
+        self.context_out(context)
+        self.conversations[context] = {"participants": participants, "log": log}
+
+    def delete(self, context: str) -> None:
+        """
+        @param context: unique context of the conversation
+        @return: None, deletes conversation
+        """
+        self.context_out(context)
+        self.conversations.pop(context)
+
+    def append(self, context: str, speaker: str, utterance: str) -> None:
+        """
+        @param context: unique context of the conversation
+        @param speaker: name of the speaker
+        @param utterance: utterance of the speaker
+        @return: None, appends utterance to the conversation
+        """
+        self.valid_participants({speaker})
+        self.context_out(context)
+        self.conversations[context]["log"].append([speaker, utterance])
+
+    def generate(self, context: str, history: str, muted: Set[str]) -> List[str]:
+        """
+        @param context: unique context of the conversation
+        @param muted: list of muted characters
+        @return: speaker and generated utterance
+        """
+        #TODO: find a smarter way to choose next character
+        #TODO: Find a smarter way to get a single response.
+        #TODO: memory for conversation log overflow
+        #TODO: memory for the context
+        #TODO: memory for the character background
+        self.valid_participants(muted)
+
+        convo = self.get(context)
+
+        convo_speakers = convo["participants"]
+        unmuted = convo_speakers.difference(muted)
+        next_speaker = random.sample(unmuted, 1)[0]
+        bg = self.valid.get(next_speaker)
+
+        convo_log = convo["log"]
+        log_str = '\n'.join([f"{speaker}: {utterance}" for speaker, utterance in convo_log])
+        # get last 3 lines of log
+        try:
+            log_str = '\n'.join(log_str.split('\n')[-3:])
+        except IndexError:
+            pass
+
+        template = "Context:\n"\
+        "{context}\n"\
+        "\n"\
+        "Background:\n"\
+        "{background}\n"\
+        "\n"\
+        "Relevant pieces of information:\n"\
+        "{history}\n"\
+        "(Only use if relevant to the conversation)\n"\
+        "\n"\
+        "Conversation:\n"\
+        "{log}\n"\
+        "{speaker}:"
+
+        prompt = PromptTemplate(template=template,
+                                input_variables=["context", "background",
+                                "history", "log", "speaker"])
+        chain = LLMChain(prompt=prompt, llm=self.llm)
+
+        output = chain.run({"context": context, "background": bg, "history": history, "log": log_str, "speaker": next_speaker})
+        if output != "":
+            output = output.split('\n')[0].lstrip()
+        self.append(context, next_speaker, output)
+        return [next_speaker, output]
+
+    def __str__(self) -> str:
+        """
+        @return: string representation of Conversations
+        """
+        return str(self.conversations)
+
+    def save(self) -> None:
+        """
+        @return: None, saves Conversations to json file
+        """
+        json.dump(self.conversations, open(self.path, 'w', encoding='utf-8'))
```

