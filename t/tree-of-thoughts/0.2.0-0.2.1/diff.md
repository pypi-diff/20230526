# Comparing `tmp/tree-of-thoughts-0.2.0.tar.gz` & `tmp/tree-of-thoughts-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.2.0.tar", last modified: Thu May 25 23:46:13 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.2.1.tar", last modified: Fri May 26 16:42:57 2023, max compression
```

## Comparing `tree-of-thoughts-0.2.0.tar` & `tree-of-thoughts-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:46:13.909988 tree-of-thoughts-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 23:46:00.000000 tree-of-thoughts-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-25 23:46:13.909988 tree-of-thoughts-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14194 2023-05-25 23:46:00.000000 tree-of-thoughts-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 23:46:13.909988 tree-of-thoughts-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-25 23:46:00.000000 tree-of-thoughts-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:46:13.909988 tree-of-thoughts-0.2.0/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 23:46:00.000000 tree-of-thoughts-0.2.0/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32181 2023-05-25 23:46:00.000000 tree-of-thoughts-0.2.0/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:46:13.909988 tree-of-thoughts-0.2.0/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-25 23:46:13.000000 tree-of-thoughts-0.2.0/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-25 23:46:13.000000 tree-of-thoughts-0.2.0/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 23:46:13.000000 tree-of-thoughts-0.2.0/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 23:46:13.000000 tree-of-thoughts-0.2.0/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 23:46:13.000000 tree-of-thoughts-0.2.0/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:42:57.097295 tree-of-thoughts-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 16:42:44.000000 tree-of-thoughts-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 16:42:57.097295 tree-of-thoughts-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-05-26 16:42:44.000000 tree-of-thoughts-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:42:57.097295 tree-of-thoughts-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-26 16:42:44.000000 tree-of-thoughts-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:42:57.097295 tree-of-thoughts-0.2.1/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-26 16:42:44.000000 tree-of-thoughts-0.2.1/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41686 2023-05-26 16:42:44.000000 tree-of-thoughts-0.2.1/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:42:57.097295 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 16:42:57.000000 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 16:42:57.000000 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:42:57.000000 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:42:57.000000 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:42:57.000000 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.2.0/LICENSE` & `tree-of-thoughts-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.0/PKG-INFO` & `tree-of-thoughts-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.2.0/README.md` & `tree-of-thoughts-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -28,66 +28,75 @@
 Navigate to the repository folder: ```cd tree-of-thoughts```
 
 ```pip install openai```
 
 Create a Python script (e.g., example.py) and import the necessary classes:
 
 ``` python
-from tree_of_thoughts.treeofthoughts import OpenAILanguageModel, CustomLanguageModel, TreeofThoughts, OptimizedOpenAILanguageModel, OptimizedTreeofThoughts
+from tree_of_thoughts.treeofthoughts import OpenAILanguageModel, CustomLanguageModel, TreeofThoughts, OptimizedOpenAILanguageModel, OptimizedTreeofThoughts, HuggingLanguageModel
 
 use_v2 = False
 api_key=""
 api_base= "" # leave it blank if you simply use default openai api url
 
 if not use_v2:
     #v1
     model = OpenAILanguageModel(api_key=api_key, api_base=api_base # api_model="gpt4" # for higher performance base model is not smart
     ) 
 else:
     #v2 parallel execution, caching, adaptive temperature
     model = OptimizedOpenAILanguageModel(api_key=api_key, api_base=api_base, # api_model="gpt4" # for higher performance base model is not smart
     )
 
+#huggingface
+# model_name="gpt2"
+# model = HuggingLanguageModel(model_name)
+
+
 #choose search algorithm('BFS' or 'DFS')
 search_algorithm = "BFS"
 
 #cot or propose
 strategy="cot"
 
 # value or vote
 evaluation_strategy = "value"
 
 if not use_v2:
     #create an instance of the tree of thoughts class v1
     tree_of_thoughts = TreeofThoughts(model, search_algorithm)
 else:
-    #or v2 -> dynamic beam width -< adjust the beam width [b] dynamically based on the search depth quality of the generated thoughts
+    #or v2 -> dynamic beam width -< adjust the beam width [b] dynamically based on the search depth quality of the generated thoughts # does not work now use regular tree of thoughts
     tree_of_thoughts= OptimizedTreeofThoughts(model, search_algorithm)
 
 input_problem = "use 4 numbers and basic arithmetic operations (+-*/) to obtain 24" #note for super intelligent responses you'll have to be more explicit in your prompt and select a better model
     
-k = 5
-T = 3
-b = 5
-vth = 0.5
-timeout = 10
-confidence = 1.0 #cmodel is confident on performance
-max_iterations = 40 #tree branch nodes 
-convergence_threshold = 0.01
-convergence_count = 5
 
 
+input_problem = "What are the best reasoning methods to advance Large Language Models"
+k = 5 #number of thoughts to input
+T = 3 # maximum depth of the search tree
+b = 5 # branching factor -< number of child nodes for each branch
+vth = 0.5 # pruning state -> any evaluated thought below this is eliminated
+timeout = 10 #10 seconds timeout before stop
+confidence = 0.8 #cmodel is confident on performance
+max_iterations = 40 #tree branh nodes 
+convergence_threshold = 0.01 #determining when the search process has converged
+convergence_count = 5 # number of searchers to be considered converged
+#read documentation for more
 
+#call the solve emthod with the input problem and other params
+solution = tree_of_thoughts.solve(input_problem, k, T, b, vth, timeout, confidence, max_iterations, convergence_threshold, convergence_count)
 
-solution = tree_of_thoughts.solve(input_problem, k, T, b, vth, timeout, confidence_threshold=confidence, max_iterations=max_iterations, convergence_threshold=convergence_threshold, convergence_count=convergence_count)
     
 
-#use the solution in your production environment
-print(f'solution {solution}')
 
+# Save the tree and metrics to a JSON file
+file_name = "logs/tree_of_thoughts_output.json"
+tree_of_thoughts.save_tree_to_json(file_name)
 
 ```
 
 Or Integrate your own custom language model:
 
 ```python
 
@@ -172,16 +181,69 @@
 ## Usage Examples
 
 ### OpenAI API
 
 To use Tree of Thoughts with OpenAI's API, create a custom model class that inherits from `AbstractLanguageModel` and implements the required methods using OpenAI's API. Then, create an instance of the `TreeOfThoughts` class with the custom model and the desired search algorithm ('BFS' or 'DFS').
 
 ### Hugging Face Transformers
+To run huggingface transformers
+``` 
+git clone https://github.com/kyegomez/tree-of-thoughts
+cd tree-of-thoughts
+python3 huggingfaceExample.py
+```
+
+```python
+from tree_of_thoughts import HuggingLanguageModel
+
+model_name="gpt2"
+model_tokenizer="your tokenizer"
+
+huggingface_model = HuggingLanguageModel(model_name, model_tokenizer)
+```
+
+
+
+```python
+class HuggingLanguageModel(AbstractLanguageModel):
+    def __init__(self, model_name):
+        self.model = AutoModelForCausalLM.from_pretrained(model_name)
+        self.tokenizer = AutoTokenizer.from_pretrained(model_name)
+
+    def generate_thoughts(self, state, k):
+        state_text = ' '.join(state)
+        prompt = f"Given the current state of reasoning: '{state_text}', generate {k} coherent thoughts to achieve the reasoning process:"
+
+        inputs = self.tokenizer(prompt, return_tensors="pt")
+        outputs = self.model.generate(**inputs, num_return_sequences=k)
+        thoughts = [self.tokenizer.decode(output, skip_special_tokens=True) for output in outputs]
+
+        return thoughts
 
-To use Tree of Thoughts with Hugging Face Transformers, create a custom model class that inherits from `AbstractLanguageModel` and implements the required methods using Hugging Face Transformers. Then, create an instance of the `TreeOfThoughts` class with the custom model and the desired search algorithm ('BFS' or 'DFS').
+    def evaluate_states(self, states, inital_prompt):
+        state_values = {}
+        for state in states:
+            state_text = ' '.join(state)
+            prompt = f"Given the current state of reasoning: '{state_text}', pessimitically evaluate its value as a float between 0 and 1 based on it's potential to achieve {inital_prompt}"
+
+            inputs = self.tokenizer(prompt, return_tensors="pt")
+            outputs = self.model.generate(**inputs, num_return_sequences=1)
+            value_text = self.tokenizer.decode(outputs[0], skip_special_tokens=True)
+
+            try:
+                value = float(value_text)
+            except ValueError:
+                value = 0  # Assign a default value if the conversion fails
+
+            state_values[state] = value
+
+        return state_values
+
+
+```
 
 
 # Contributing
 This algorithm is still infant yet it's potential remains unimaginable, let's advance the reasoning of AI's together under this banner.
 
 # Share With Your Network
 
@@ -251,58 +313,36 @@
 3. Develop a method for combining different modalities in the search tree, allowing the algorithm to reason across different data types.
 4. Implement and test the multi-modal Tree of Thoughts algorithm with various problems and datasets.
 5. Optimize the algorithm for performance and resource usage, ensuring it scales well with large multi-modal datasets.
 6. Publish the results and gather feedback from the community to further improve the multi-modal Tree of Thoughts algorithm.
 
 Join us on this exciting journey to advance the Tree of Thoughts algorithm to multi-modality superintelligence! 🚀
 
-# The Compiler
-
-[Utilizing Tree of Thoughts for optimal program synthesis](https://github.com/kyegomez/the-compiler)
-
-![the compiler banner](https://github.com/kyegomez/the-compiler/raw/main/the-compiler.png)
-
-Welcome to _The Compiler_, a novel child project under the Tree of Thoughts (ToT) paradigm. This project is crafted with the intent of making autonomous programming not just a reality, but an effortless task for you. 
-
-In essence, _The Compiler_ allows you to "grow" any program you can dream of. By providing a high-level specification of the product you would like, you can sit back and let _The Compiler_ do the heavy lifting. 
-
-## Overview 
-
-_The Compiler_ leverages the ToT framework and large language models (LLMs) to handle the programming process, from abstract specifications to a working program. 
-
-Here's a basic breakdown of the workflow:
-
-1. **Input**: You provide an abstract specification for the product you would like.
-2. **Unit Tests Generation**: We use an LLM on ToT to produce a suite of unit tests for the code.
-3. **Run ToT**: We run the Tree of Thoughts LLM on the given specification, using the generated unit tests as the evaluation score.
-4. **Output**: Ready to use program!
+# Here's the documentation for the inputs of the optimized Tree of Thoughts model:
 
-## Architecture
+x (str): The initial problem statement or prompt for which the Tree of Thoughts algorithm will generate a solution.
 
-The Compiler, leveraging the Tree of Thoughts paradigm, consists of several primary components, including the Specification Parser, Thought Decomposer, Thought Generator, State Evaluator, and the Search Algorithm. 
+k (int, default=5): The number of thoughts to generate at each state. A higher value of k will result in more thoughts being generated, potentially leading to a more diverse set of solutions. However, increasing k may also increase the computational complexity and time required to find a solution.
 
-1. **Specification Parser**: This interprets your high-level input specifications and translates them into a format that the Thought Decomposer can understand and work with.
+T (int, default=3): The maximum depth of the search tree. A higher value of T allows the algorithm to explore deeper states, potentially leading to better solutions. However, increasing T may also increase the computational complexity and time required to find a solution.
 
-2. **Thought Decomposer**: This component breaks down the programming problem into manageable "thoughts" or steps.
+b (int, default=5): The branching factor of the search tree, which determines the maximum number of child nodes for each parent node. A higher value of b allows the algorithm to explore more states, potentially leading to better solutions. However, increasing b may also increase the computational complexity and time required to find a solution.
 
-3. **Thought Generator**: It generates potential thoughts or steps from the current state using two strategies, either sampling thoughts independently or proposing thoughts sequentially.
+vth (float, default=0.5): The value threshold for pruning states. States with a value below this threshold will be discarded, reducing the search space. A higher value of vth will result in a more aggressive pruning strategy, potentially speeding up the search process. However, setting vth too high may cause the algorithm to discard promising states, leading to suboptimal solutions.
 
-4. **State Evaluator**: It evaluates the progress of different states towards solving the programming problem, acting as a heuristic for the Search Algorithm.
+timeout (int, default=10): The maximum time (in seconds) allowed for the search process. If the search process exceeds this time limit, the algorithm will return the best solution found so far.
 
-5. **Search Algorithm**: This module determines which states to keep exploring and in which order. It employs either Breadth-First Search (BFS) or Depth-First Search (DFS), depending on the nature of the problem.
+confidence_threshold (float, default=0.8): The confidence threshold for determining when a solution is satisfactory. If the algorithm finds a solution with a confidence value above this threshold, it will return the solution immediately.
 
-## Share The Compiler
+max_iterations (int, default=40): The maximum number of iterations allowed for the search process. If the search process exceeds this number of iterations, the algorithm will return the best solution found so far.
 
-If you find this project exciting and think others might benefit from it, feel free to share it. Use the buttons below to share it on various social media platforms:
+convergence_threshold (float, default=0.01): The convergence threshold for determining when the search process has converged. If the difference in confidence values between consecutive iterations is below this threshold for a specified number of iterations (convergence_count), the algorithm will return the best solution found so far.
 
-- [Share on Twitter](http://twitter.com/share?text=Check%20out%20The%20Compiler%20project%20on%20GitHub!%20It%20allows%20you%20to%20autonomously%20create%20programs%20using%20abstract%20specifications.&url=https://github.com/kyegomez/the-compiler)
-- [Share on LinkedIn](http://www.linkedin.com/shareArticle?mini=true&url=https://github.com/kyegomez/the-compiler&title=The%20Compiler%20Project&summary=This%20project%20is%20a%20revolution%20in%20autonomous%20programming!%20Check%20it%20out%20on%20GitHub.)
-- [Share on Facebook](http://www.facebook.com/sharer.php?u=https://github.com/kyegomez/the-compiler)
+convergence_count (int, default=5): The number of consecutive iterations required for the search process to be considered converged. If the difference in confidence values between consecutive iterations is below the convergence_threshold for this number of iterations, the algorithm will return the best solution found so far.
 
-Let's revolutionize the world of programming together with _The Compiler_!
 
 
 
 # Acknowledgements
 
 Thanks to: Shunyu Yao Princeton University, Dian Yu Google DeepMind, Jeffrey Zhao, Google DeepMind, Izhak Shafran Google DeepMind, Thomas L. Griffiths, Princeton University, Yuan Cao Google DeepMind, Karthik Narasimha, Princeton University for sharing this amazing work with the world!
```

### Comparing `tree-of-thoughts-0.2.0/setup.py` & `tree-of-thoughts-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.2.0',
+  version = '0.2.1',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.2.0/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

