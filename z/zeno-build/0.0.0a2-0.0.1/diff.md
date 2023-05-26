# Comparing `tmp/zeno_build-0.0.0a2.tar.gz` & `tmp/zeno_build-0.0.1.tar.gz`

## Comparing `zeno_build-0.0.0a2.tar` & `zeno_build-0.0.1.tar`

### file list

```diff
@@ -1,34 +1,39 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/__init__.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/cache_utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/version.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/evaluation/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/evaluation/classification_metrics.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/evaluation/text_features/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/evaluation/text_features/exact_match.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/evaluation/text_features/length.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/evaluation/text_metrics/__init__.py
--rw-r--r--   0        0        0    15356 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/evaluation/text_metrics/critique.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/experiments/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/experiments/experiment_run.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/experiments/search_space.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/models/__init__.py
--rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/models/chat_generate.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/models/global_models.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/models/lm_config.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/models/text_generate.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/optimizers/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/optimizers/base.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/optimizers/random.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/optimizers/standard.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/optimizers/vizier.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/prompts/__init__.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/prompts/chat_prompt.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/prompts/prompt_utils.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/reporting/__init__.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/reporting/aggregate_results.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/zeno_build/reporting/visualize.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/LICENSE
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/README.md
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 zeno_build-0.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/__init__.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/cache_utils.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/version.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/text_features/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/text_features/exact_match.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/text_features/length.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/text_metrics/__init__.py
+-rw-r--r--   0        0        0    15356 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/evaluation/text_metrics/critique.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/experiments/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/experiments/experiment_run.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/experiments/search_space.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/__init__.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/chat_generate.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/dataset_config.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/global_models.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/lm_config.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/text_generate.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/providers/__init__.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/providers/cohere_utils.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/providers/huggingface_utils.py
+-rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/models/providers/openai_utils.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/optimizers/__init__.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/optimizers/base.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/optimizers/random.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/optimizers/standard.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/optimizers/vizier.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/prompts/__init__.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/prompts/chat_prompt.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/prompts/prompt_utils.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/reporting/__init__.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/reporting/aggregate_results.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/reporting/reporting_utils.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 zeno_build-0.0.1/zeno_build/reporting/visualize.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 zeno_build-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.1/LICENSE
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 zeno_build-0.0.1/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 zeno_build-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 zeno_build-0.0.1/PKG-INFO
```

### Comparing `zeno_build-0.0.0a2/zeno_build/evaluation/text_features/exact_match.py` & `zeno_build-0.0.1/zeno_build/evaluation/text_features/exact_match.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a2/zeno_build/evaluation/text_features/length.py` & `zeno_build-0.0.1/zeno_build/evaluation/text_features/length.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a2/zeno_build/evaluation/text_metrics/critique.py` & `zeno_build-0.0.1/zeno_build/evaluation/text_metrics/critique.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a2/zeno_build/models/lm_config.py` & `zeno_build-0.0.1/zeno_build/models/lm_config.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a2/zeno_build/models/text_generate.py` & `zeno_build-0.0.1/zeno_build/models/text_generate.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a2/zeno_build/optimizers/base.py` & `zeno_build-0.0.1/zeno_build/optimizers/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
 
 class Optimizer:
     """An optimizer for hyperparameter search."""
 
     def __init__(
         self,
-        space: dict[str, search_space.SearchDimension],
-        constants: dict[str, Any],
+        space: search_space.SearchSpace,
         distill_functions: list[Callable[[DataFrame, ZenoOptions], DistillReturn]],
         metric: Callable[[DataFrame, ZenoOptions], MetricReturn],
+        num_trials: int | None,
     ):
         """Initialize an optimizer."""
         self.space = space
-        self.constants = constants
         self.distill_functions = distill_functions
         self.metric = metric
+        self.num_trials = num_trials
 
     def calculate_metric(
         self, data: list[Any], labels: list[Any], outputs: list[Any]
     ) -> float:
         """Calculate the metric for a set of data, labels, and outputs.
 
         This must be called only once after get_parameters.
@@ -54,7 +54,28 @@
             label_path="",
             output_path="",
         )
         df = DataFrame({"data": data, "labels": labels, "outputs": outputs})
         for distill_function in self.distill_functions:
             df[distill_function.__name__] = distill_function(df, ops).distill_output
         return self.metric(df, ops).metric
+
+    def is_complete(
+        self,
+        output_dir: str,
+        include_in_progress: bool = False,
+    ) -> bool:
+        """Check if the optimizer has completed.
+
+        Args:
+            output_dir: The directory where the results of each trial are stored.
+            include_in_progress: Whether to include trials that are still running.
+
+        Returns:
+            True if the optimizer run has completed.
+        """
+        if self.num_trials is None:
+            return False
+        valid_param_files = self.space.get_valid_param_files(
+            output_dir=output_dir, include_in_progress=include_in_progress
+        )
+        return len(valid_param_files) >= self.num_trials
```

### Comparing `zeno_build-0.0.0a2/zeno_build/optimizers/random.py` & `zeno_build-0.0.1/zeno_build/optimizers/random.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,30 +16,31 @@
 
 
 class RandomOptimizer(Optimizer):
     """An optimizer using random search."""
 
     def __init__(
         self,
-        space: dict[str, search_space.SearchDimension],
-        constants: dict[str, Any],
+        space: search_space.SearchSpace,
         distill_functions: list[Callable[[DataFrame, ZenoOptions], DistillReturn]],
         metric: Callable[[DataFrame, ZenoOptions], MetricReturn],
         seed: int | None = None,
+        num_trials: int | None = None,
     ):
         """Initialize a random optimizer.
 
         Args:
             space: The space to search over.
             constants: The constants to use.
             distill_functions: The distill functions to use.
             metric: The metric to use.
             seed: The random seed to use.
+            num_trials: The maximum number of trials to run.
         """
-        super().__init__(space, constants, distill_functions, metric)
+        super().__init__(space, distill_functions, metric, num_trials)
         # Set state without side-effects (for single thread)
         saved_state = random.getstate()
         random.seed(seed)
         self._state = random.getstate()
         random.setstate(saved_state)
 
     def get_parameters(self) -> dict[str, Any]:
@@ -47,24 +48,29 @@
 
         Args:
             space: The space to randomize.
 
         Returns:
             A dictionary of randomized parameters.
         """
-        saved_state = random.getstate()
-        random.setstate(self._state)
-        params = dict(self.constants)
-        for name, dimension in self.space.items():
-            if isinstance(dimension, search_space.Categorical) or isinstance(
-                dimension, search_space.Discrete
-            ):
-                params[name] = random.choice(dimension.choices)
-            elif isinstance(dimension, search_space.Float):
-                params[name] = random.uniform(dimension.lower, dimension.upper)
-            elif isinstance(dimension, search_space.Int):
-                params[name] = random.randint(dimension.lower, dimension.upper)
-            else:
-                raise ValueError(f"Unknown search dimension: {dimension}")
-        self._state = random.getstate()
-        random.setstate(saved_state)
+        if isinstance(self.space, search_space.CombinatorialSearchSpace):
+            saved_state = random.getstate()
+            random.setstate(self._state)
+            params = {}
+            for name, dimension in self.space.dimensions.items():
+                if isinstance(dimension, search_space.Categorical) or isinstance(
+                    dimension, search_space.Discrete
+                ):
+                    params[name] = random.choice(dimension.choices)
+                elif isinstance(dimension, search_space.Float):
+                    params[name] = random.uniform(dimension.lower, dimension.upper)
+                elif isinstance(dimension, search_space.Int):
+                    params[name] = random.randint(dimension.lower, dimension.upper)
+                elif isinstance(dimension, search_space.Constant):
+                    params[name] = dimension.value
+                else:
+                    raise ValueError(f"Unknown search dimension: {dimension}")
+            self._state = random.getstate()
+            random.setstate(saved_state)
+        else:
+            raise NotImplementedError(f"Unsupported search space {type(self.space)}.")
         return params
```

### Comparing `zeno_build-0.0.0a2/zeno_build/optimizers/vizier.py` & `zeno_build-0.0.1/zeno_build/optimizers/vizier.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,40 +17,44 @@
 
 
 class VizierOptimizer(Optimizer):
     """An optimizer using the Vizier toolkit."""
 
     def __init__(
         self,
-        space: dict[str, search_space.SearchDimension],
-        constants: dict[str, Any],
+        space: search_space.SearchSpace,
         distill_functions: list[Callable[[DataFrame, ZenoOptions], DistillReturn]],
         metric: Callable[[DataFrame, ZenoOptions], MetricReturn],
+        num_trials: int | None = None,
         algorithm: str = "RANDOM_SEARCH",
         owner: str = "zeno-build",
         study_id: str = "zeno-build",
     ):
         """Initialize a Vizier optimizer.
 
         Args:
             space: The space to search over.
             constants: The constants to use.
             distill_functions: The distill functions to use.
             metric: The metric to use.
+            num_trials: The number of trials to run.
             algorithm: The algorithm to use for optimization.
             owner: The owner of the study.
             study_id: The ID of the study.
         """
-        super().__init__(space, constants, distill_functions, metric)
+        if not isinstance(space, search_space.CombinatorialSearchSpace):
+            raise NotImplementedError("Only combinatorial search spaces are supported.")
+
+        super().__init__(space, distill_functions, metric, num_trials)
         self.algorithm = algorithm
         self.owner = owner
         self.study_id = study_id
         # Algorithm, search space, and metrics.
         study_config = vz.StudyConfig(algorithm=self.algorithm)
-        for name, dimension in space.items():
+        for name, dimension in space.dimensions.items():
             if isinstance(dimension, search_space.Categorical):
                 study_config.search_space.root.add_categorical_param(
                     name, dimension.choices
                 )
             elif isinstance(dimension, search_space.Discrete):
                 study_config.search_space.root.add_discrete_param(
                     name, dimension.choices
```

### Comparing `zeno_build-0.0.0a2/zeno_build/prompts/chat_prompt.py` & `zeno_build-0.0.1/zeno_build/prompts/chat_prompt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Specify the prompts you want to use."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Literal
+from typing import Any, Literal
 
 
 @dataclass
 class ChatTurn:
     """A single turn for a chat prompt.
 
     Attributes:
@@ -25,14 +25,35 @@
 
     Attributes:
         messages: A set of messages for the chat turn
     """
 
     messages: list[ChatTurn]
 
+    @staticmethod
+    def from_dict(data: dict[str, Any]) -> ChatMessages:
+        """Create a chat messages object from a dictionary."""
+        return ChatMessages(
+            messages=[
+                ChatTurn(role=x["role"], content=x["content"]) for x in data["messages"]
+            ]
+        )
+
+    def to_dict(self) -> dict[str, Any]:
+        """Convert a chat messages object to a dictionary."""
+        return {
+            "messages": [
+                {
+                    "role": x.role,
+                    "content": x.content,
+                }
+                for x in self.messages
+            ]
+        }
+
     def to_openai_chat_completion_messages(
         self,
         full_context: ChatMessages,
     ) -> list[dict[str, str]]:
         """Build an OpenAI ChatCompletion message.
 
         Args:
```

### Comparing `zeno_build-0.0.0a2/zeno_build/reporting/aggregate_results.py` & `zeno_build-0.0.1/zeno_build/reporting/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a2/zeno_build/reporting/visualize.py` & `zeno_build-0.0.1/zeno_build/reporting/visualize.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,22 +29,15 @@
         functions: List of functions to use in Zeno
         zeno_config: Zeno configuration parameters
     """
     if len(df) != len(labels):
         raise ValueError("Length of data and labels must be equal.")
     if data_column not in df.columns:
         raise ValueError(f"Data column {data_column} not in DataFrame.")
-    model_results: dict[str, ExperimentRun] = {}
-    for i, res in enumerate(results):
-        # TODO(alex): think about how to represent hyperparameter-based model names.
-        name = res.name or "model" + str(i)
-
-        # Prevent duplicate runs being added to Zeno
-        if name not in model_results:
-            model_results[name] = res
+    model_results: dict[str, ExperimentRun] = {x.name: x for x in results}
 
     @model
     def get_model(name):
         mod = model_results[name].predictions
 
         def pred(df, ops):
             return ModelReturn(model_output=itemgetter(*df["index"].to_list())(mod))
```

### Comparing `zeno_build-0.0.0a2/.gitignore` & `zeno_build-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a2/LICENSE` & `zeno_build-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a2/README.md` & `zeno_build-0.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -31,44 +31,40 @@
 
 To get started with `zeno-build`, install the package from PyPI:
 
 ```bash
 pip install zeno-build
 ```
 
-Next, _start building_! Browse the [tasks/](tasks/) directory, where we have a
-bunch of examples of how you can use `zeno-build` for different tasks, such as
-[chatbots](tasks/chatbot/), [text summarization](tasks/summarization/), or [text
-classification](tasks/text_classification/). Check out the [Zeno Build
-Concepts](tasks/CO) doc for more details on the different aspects of the
-library.
+Next, _start building_! Browse to the [docs](docs/) directory to get a
+primer or to the [examples/](examples/) directory, where we
+have a bunch of examples of how you can use `zeno-build` for different tasks,
+such as [chatbots](examples/chatbot/),
+[text summarization](examples/summarization/), or [text
+classification](examples/text_classification/).
 
 Each of the examples include code for running experiments and evaluating the
 results. `zeno-build` will produce a comprehensive report with the
 [Zeno](https://zenoml.com/) ML analysis platform. To give you a flavor of what
 these reports will look like, check out a few of our pre-made reports below:
 
-- [Zeno Chatbot Report](TODO): A report comparing different methods for creating
-  chatbots, including API-based models such as ChatGPT, Claude, and Cohere, with
-  open-source models such as Vicuna, Alpaca, and Flan-T5.
-- [Zeno Summarization Report](TODO): A report comparing different methods for
-  text summarization, including GPT-3, Flan-T5, and Pegasus.
-- [Zeno Sentiment Analysis Report](TODO): A report comparing different
-  pre-trained models for sentiment analysis across a variety of datasets.
+- [Zeno Chatbot Report](examples/chatbot/report/): A report comparing different methods
+  for creating chatbots, including API-based models such as ChatGPT and Cohere,
+  with open-source models such as Vicuna, Alpaca, and MPT.
 
 ## Building Your Own Apps (and Contributing Back)
 
-Each of the examples in the [tasks/](tasks/) directory is specifically designed
+Each of the examples in the [examples/](examples/) directory is specifically designed
 to be self-contained and easy to modify. To get started building your own apps,
 we suggest that you first click into the directory and read the general README,
 find the closest example to what you're trying to do, copy the example to the
 new directory, and start hacking!
 
 If you build something cool, **we'd love for you to contribute it back**. We
-welcome pull requests of both new task examples, new reports for existing tasks,
+welcome pull requests of both new examples, new reports for existing examples,
 and new functionality for the core `zeno_build` library. If this is of interest
 to you, please click through to our [contributing doc](contributing.md) doc to
 learn more.
 
 ## Get in Touch
 
 If you have any questions, feature requests, bug reports, etc., we recommend
```

### Comparing `zeno_build-0.0.0a2/pyproject.toml` & `zeno_build-0.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers = [
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
-dependencies = ["aiolimiter>=1.0.0", "inspiredco>=0.0.2", "zenoml>=0.5.3"]
+dependencies = ["aiolimiter>=1.0.0", "inspiredco>=0.0.2", "zenoml>=0.6.0"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["mypy>=1.2.0", "pre-commit>=3.2.0", "pytest>=6.0.0", "black>=23.3.0"]
 
 [tool.hatch.build]
 include = ["*.py"]
-exclude = ["*_test.py", "tasks/**"]
+exclude = ["*_test.py", "tasks/**", "examples/**"]
 only-packages = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["zeno_build"]
 
 [tool.hatch.version]
 path = "zeno_build/version.py"
```

### Comparing `zeno_build-0.0.0a2/PKG-INFO` & `zeno_build-0.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeno_build
-Version: 0.0.0a2
+Version: 0.0.1
 Summary: A library for comparing multiple llm-based systems.
 Author-email: Ángel Alexander Cabrera <alex.cabrera@gmail.com>, Graham Neubig <neubig@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Zeno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,15 +27,15 @@
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: aiolimiter>=1.0.0
 Requires-Dist: inspiredco>=0.0.2
-Requires-Dist: zenoml>=0.5.3
+Requires-Dist: zenoml>=0.6.0
 Provides-Extra: test
 Requires-Dist: black>=23.3.0; extra == 'test'
 Requires-Dist: mypy>=1.2.0; extra == 'test'
 Requires-Dist: pre-commit>=3.2.0; extra == 'test'
 Requires-Dist: pytest>=6.0.0; extra == 'test'
 Description-Content-Type: text/markdown
 
@@ -72,44 +72,40 @@
 
 To get started with `zeno-build`, install the package from PyPI:
 
 ```bash
 pip install zeno-build
 ```
 
-Next, _start building_! Browse the [tasks/](tasks/) directory, where we have a
-bunch of examples of how you can use `zeno-build` for different tasks, such as
-[chatbots](tasks/chatbot/), [text summarization](tasks/summarization/), or [text
-classification](tasks/text_classification/). Check out the [Zeno Build
-Concepts](tasks/CO) doc for more details on the different aspects of the
-library.
+Next, _start building_! Browse to the [docs](docs/) directory to get a
+primer or to the [examples/](examples/) directory, where we
+have a bunch of examples of how you can use `zeno-build` for different tasks,
+such as [chatbots](examples/chatbot/),
+[text summarization](examples/summarization/), or [text
+classification](examples/text_classification/).
 
 Each of the examples include code for running experiments and evaluating the
 results. `zeno-build` will produce a comprehensive report with the
 [Zeno](https://zenoml.com/) ML analysis platform. To give you a flavor of what
 these reports will look like, check out a few of our pre-made reports below:
 
-- [Zeno Chatbot Report](TODO): A report comparing different methods for creating
-  chatbots, including API-based models such as ChatGPT, Claude, and Cohere, with
-  open-source models such as Vicuna, Alpaca, and Flan-T5.
-- [Zeno Summarization Report](TODO): A report comparing different methods for
-  text summarization, including GPT-3, Flan-T5, and Pegasus.
-- [Zeno Sentiment Analysis Report](TODO): A report comparing different
-  pre-trained models for sentiment analysis across a variety of datasets.
+- [Zeno Chatbot Report](examples/chatbot/report/): A report comparing different methods
+  for creating chatbots, including API-based models such as ChatGPT and Cohere,
+  with open-source models such as Vicuna, Alpaca, and MPT.
 
 ## Building Your Own Apps (and Contributing Back)
 
-Each of the examples in the [tasks/](tasks/) directory is specifically designed
+Each of the examples in the [examples/](examples/) directory is specifically designed
 to be self-contained and easy to modify. To get started building your own apps,
 we suggest that you first click into the directory and read the general README,
 find the closest example to what you're trying to do, copy the example to the
 new directory, and start hacking!
 
 If you build something cool, **we'd love for you to contribute it back**. We
-welcome pull requests of both new task examples, new reports for existing tasks,
+welcome pull requests of both new examples, new reports for existing examples,
 and new functionality for the core `zeno_build` library. If this is of interest
 to you, please click through to our [contributing doc](contributing.md) doc to
 learn more.
 
 ## Get in Touch
 
 If you have any questions, feature requests, bug reports, etc., we recommend
```

