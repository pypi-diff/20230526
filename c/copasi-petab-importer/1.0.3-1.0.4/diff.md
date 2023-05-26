# Comparing `tmp/copasi-petab-importer-1.0.3.tar.gz` & `tmp/copasi-petab-importer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copasi-petab-importer-1.0.3.tar", last modified: Tue Apr 18 05:53:43 2023, max compression
+gzip compressed data, was "copasi-petab-importer-1.0.4.tar", last modified: Fri May 26 07:51:36 2023, max compression
```

## Comparing `copasi-petab-importer-1.0.3.tar` & `copasi-petab-importer-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-04-18 05:53:43.816281 copasi-petab-importer-1.0.3/
--rw-r--r--   0 frank      (501) staff       (20)       64 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/MANIFEST.in
--rw-r--r--   0 frank      (501) staff       (20)      279 2023-04-18 05:53:43.816325 copasi-petab-importer-1.0.3/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)     3253 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/README.md
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-04-18 05:53:43.816634 copasi-petab-importer-1.0.3/copasi_petab_importer/
--rw-r--r--   0 frank      (501) staff       (20)     9163 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/PEtab.py
--rw-r--r--   0 frank      (501) staff       (20)      311 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)      497 2023-04-18 05:53:43.816667 copasi-petab-importer-1.0.3/copasi_petab_importer/_version.py
--rw-r--r--   0 frank      (501) staff       (20)     1899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/convert_all_petab.py
--rw-r--r--   0 frank      (501) staff       (20)     4579 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/convert_benchmark.py
--rw-r--r--   0 frank      (501) staff       (20)    33406 2023-04-17 21:25:19.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/convert_petab.py
--rw-r--r--   0 frank      (501) staff       (20)    12270 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/petab.ui
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-04-18 05:53:43.816031 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/
--rw-r--r--   0 frank      (501) staff       (20)      279 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)      603 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/SOURCES.txt
--rw-r--r--   0 frank      (501) staff       (20)        1 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/dependency_links.txt
--rw-r--r--   0 frank      (501) staff       (20)      138 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/entry_points.txt
--rw-r--r--   0 frank      (501) staff       (20)       62 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/requires.txt
--rw-r--r--   0 frank      (501) staff       (20)       22 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/top_level.txt
--rw-r--r--   0 frank      (501) staff       (20)      243 2023-04-18 05:53:43.816499 copasi-petab-importer-1.0.3/setup.cfg
--rw-r--r--   0 frank      (501) staff       (20)      899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/setup.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-04-18 05:53:43.816140 copasi-petab-importer-1.0.3/test/
--rw-r--r--   0 frank      (501) staff       (20)     1916 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/test/test_importer.py
--rw-r--r--   0 frank      (501) staff       (20)    78254 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/versioneer.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 07:51:36.071087 copasi-petab-importer-1.0.4/
+-rw-r--r--   0 frank      (501) staff       (20)       64 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/MANIFEST.in
+-rw-r--r--   0 frank      (501) staff       (20)      279 2023-05-26 07:51:36.071151 copasi-petab-importer-1.0.4/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)     3714 2023-05-03 06:40:46.000000 copasi-petab-importer-1.0.4/README.md
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 07:51:36.071498 copasi-petab-importer-1.0.4/copasi_petab_importer/
+-rw-r--r--   0 frank      (501) staff       (20)     9163 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/PEtab.py
+-rw-r--r--   0 frank      (501) staff       (20)      351 2023-05-16 13:46:05.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)      497 2023-05-26 07:51:36.071528 copasi-petab-importer-1.0.4/copasi_petab_importer/_version.py
+-rw-r--r--   0 frank      (501) staff       (20)     1899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/convert_all_petab.py
+-rw-r--r--   0 frank      (501) staff       (20)     4579 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/convert_benchmark.py
+-rw-r--r--   0 frank      (501) staff       (20)    39718 2023-05-26 07:45:03.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/convert_petab.py
+-rw-r--r--   0 frank      (501) staff       (20)    12270 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/petab.ui
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 07:51:36.070702 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/
+-rw-r--r--   0 frank      (501) staff       (20)      279 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)      603 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 frank      (501) staff       (20)        1 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 frank      (501) staff       (20)      138 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/entry_points.txt
+-rw-r--r--   0 frank      (501) staff       (20)       62 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/requires.txt
+-rw-r--r--   0 frank      (501) staff       (20)       22 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/top_level.txt
+-rw-r--r--   0 frank      (501) staff       (20)      243 2023-05-26 07:51:36.071372 copasi-petab-importer-1.0.4/setup.cfg
+-rw-r--r--   0 frank      (501) staff       (20)      899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/setup.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 07:51:36.070814 copasi-petab-importer-1.0.4/test/
+-rw-r--r--   0 frank      (501) staff       (20)     2940 2023-05-25 08:44:48.000000 copasi-petab-importer-1.0.4/test/test_importer.py
+-rw-r--r--   0 frank      (501) staff       (20)    78254 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/versioneer.py
```

### Comparing `copasi-petab-importer-1.0.3/README.md` & `copasi-petab-importer-1.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 So this converter 1. reads the SBML file and converts it to the COPASI format, then converts the experimental data so we can use it in COPASI, and provides the mapping to the observables. Once the converter is done, and you run the parameter estimation you will get the current solution displayed. 
 
 The benchmarks are also added as submodule to this repo. So if you do want to use those, be sure to check it out as well, running: 
 
 	git submodule init 
 	git submodule update
 
+### Run PEtab the easy way
+This project is used direclty from [basico](https://basico.rtdf.io), where we directly implement a PetabSimulator. So if you are interested in just running PEtab problems with COPASI, I recommend to 
+
+	pip install copasi-basico[petab]
+	
+and then follow the [basico petab example](https://basico.readthedocs.io/en/latest/notebooks/Working_with_PEtab.html). Otherwise, this project can of course be used on its own as described below. 
 
 ### Setup
 Create a new virtual environment, and then run `pip install -r requirements.txt`. This will install all the dependencies, these are: 
 
 - numpy
 - pandas
 - python-copasi
```

### Comparing `copasi-petab-importer-1.0.3/copasi_petab_importer/PEtab.py` & `copasi-petab-importer-1.0.4/copasi_petab_importer/PEtab.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.3/copasi_petab_importer/convert_all_petab.py` & `copasi-petab-importer-1.0.4/copasi_petab_importer/convert_all_petab.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.3/copasi_petab_importer/convert_benchmark.py` & `copasi-petab-importer-1.0.4/copasi_petab_importer/convert_benchmark.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.3/copasi_petab_importer/convert_petab.py` & `copasi-petab-importer-1.0.4/copasi_petab_importer/convert_petab.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import pandas as pd
 import numpy as np
 import logging
 import libsbml
 
 dm = COPASI.CRootContainer.addDatamodel()
 assert (isinstance(dm, COPASI.CDataModel))
-print("using COPASI: %s" % COPASI.CVersion.VERSION.getVersion())
+
+logger = logging.getLogger(__name__)
+logger.info("using COPASI: %s" % COPASI.CVersion.VERSION.getVersion())
 
 
 class PEtabProblem:
     def __init__(self, dirname=None, model_name=None, condition_file=None, measurement_file=None,
                  parameter_file=None, simulation_file=None, model_file=None, observable_file=None, yaml_file=None):
         self.directory = dirname
         self.model_name = model_name
@@ -90,41 +92,56 @@
 
         for i in range(observable_data.shape[0]):
             current = observable_data.iloc[i]
             id = current.observableId
 
             # ignore invalid ids
             if not libsbml.SyntaxChecker_isValidSBMLSId(id):
-                logging.warning(
+                logger.warning(
                     'Invalid observableId {0} in observable table'.
-                        format(id))
+                    format(id))
                 continue
 
             name = id
 
             # if we have one already, don't add again
             # something ought to be wrong with the table here
             if id in all_ids:
-                logging.warning(
+                logger.warning(
                     'observableId {0} appears already in the model'.
-                        format(id))
+                    format(id))
                 continue
 
             formula = current.observableFormula
             if not isinstance(formula, str):
-                logging.warning(
+                logger.warning(
                     'Invalid observableFormula for observableId {0}'.
-                        format(id))
+                    format(id))
                 continue
 
+            if 'observableTransformation' in current:
+                transformation = current.observableTransformation
+                if not isinstance(transformation, str):
+                    logger.warning(
+                        'Invalid observableTransformation for observableId {0} default to lin'.
+                        format(id))
+                    transformation = 'lin'
+            else:
+                transformation = 'lin'
+
+            if transformation == 'log':
+                formula = 'ln({0})'.format(formula)
+            elif transformation == 'log10':
+                formula = 'log({0})'.format(formula)
+
             math = libsbml.parseL3Formula(formula)
             if math is None:
-                logging.warning(
+                logger.warning(
                     'Invalid observableFormula for observableId {0}'.
-                        format(id))
+                    format(id))
                 continue
 
             self.add_missing_params(model, math)
 
             obs = model.createParameter()
             obs.setId(id)
             obs.setName(name)
@@ -385,14 +402,100 @@
                                 if not current_exp['condition'] in self.ignore_independent:
                                     self.ignore_independent[current_exp['condition']] = {}
                                 self.ignore_independent[current_exp['condition']][col] = \
                                     conditions[col].values[0]
                     output.write('\n')
                     line += 1
 
+    def assign_weight(self, petab, observable, obj_map, i):
+        """ retrieves the weight from the petab problem for the given column
+        """
+
+        noise_formula = petab.observable_data.query('observableId == "' + observable + '"').noiseFormula.values[0]
+
+        # check if it is a number if so use it
+        try:
+            value = float(noise_formula)
+            obj_map.setScale(i, value)
+            return True
+        except ValueError:
+            pass
+
+        # otherwise we search for it in the parameter table
+        parameter = petab.parameter_data.query('parameterId == "' + noise_formula + '"')
+
+        if len(parameter) == 0:
+            # check whether the noise formula is a parameter in the model
+            mv = dm.getModel().getModelValue(noise_formula)
+            if mv is not None:
+                # if so, we use it
+                obj_map.setScale(i, mv.getInitialValue())
+                return True
+
+            # if the noise formula starts with 'noiseParameter' and a number, we should
+            # be taking the value from the noiseParameters column in the measurement
+            # table
+            if noise_formula.startswith('noiseParameter'):
+                # strip the noiseParameter part
+                noise_formula = noise_formula[14:]
+                # find the index until the next '_'
+                index = noise_formula.find('_')
+                if index > 0:
+                    # get the number
+                    number = int(noise_formula[0:index])
+                    # get the observable name
+                    observable_name = noise_formula[index + 1:]
+                    # get the noiseParameters
+                    noise_parameter = petab.measurement_data.query('observableId == "' + observable_name + '"') \
+                                      .noiseParameters.values
+                    if len(noise_parameter) == 0:
+                        return False
+
+                    try:
+                        noise_parameter = noise_parameter[0].split(';')
+                    except AttributeError:
+                        try:
+                            noise_parameter = float(noise_parameter[0])
+                            noise_parameter = [ noise_parameter]
+                        except ValueError:
+                            return False
+
+                    if len(noise_parameter) >= number:
+                        # get the value from the column
+                        noise_parameter = noise_parameter[number - 1]
+                        # now that we have the parameter check whether it is a number
+                        try:
+                            value = float(noise_parameter)
+                            obj_map.setScale(i, value)
+                            return True
+                        except ValueError:
+                            pass
+                        # otherwise look for it in the parameter table
+                        parameter = petab.parameter_data.query('parameterId == "' + noise_parameter + '"')
+                        return self._assign_weight_from_parameter(parameter, noise_parameter, obj_map, i)
+            logger.debug('Unsupported noise formula %s. Ignoring it.' % noise_formula)
+            return False
+
+        return self._assign_weight_from_parameter(parameter, noise_formula, obj_map, i)
+
+    def _assign_weight_from_parameter(self, parameter, noise_formula, obj_map, i):
+        if len(parameter) == 0:
+            return False
+        if parameter.iloc[0].estimate == 1:
+            logger.debug('COPASI cannot estimate the noise parameter %s. Ignoring it.' % noise_formula)
+            return False
+        # take the nominal value
+        try:
+            value = float(parameter.iloc[0].nominalValue)
+            obj_map.setScale(i, value)
+            return True
+        except ValueError:
+            pass
+        return False
+
     def create_mapping(self, experiments, petab):
         task = dm.getTask('Parameter Estimation')
         # mark task as executable, so it can be run by copasi se
         task.setScheduled(True)
         problem = task.getProblem()
         # disable statistics at the end of the runs
         problem.setCalculateStatistics(False)
@@ -460,15 +563,17 @@
                             obj = dm.findObjectByDisplayName(
                                 'Values[' + all_cols[i] + ']')
                         if obj is not None:
                             cn = obj.getValueReference().getCN()
                             role = COPASI.CExperiment.dependent
                             obj_map.setRole(i, role)
                             obj_map.setObjectCN(i, cn)
-                            exp.calculateWeights()
+                            if not self.assign_weight(petab, all_cols[i], obj_map, i):
+                                exp.calculateWeights()
+                            # exp.calculateWeights()
                             continue
                 obj_map.setRole(i, role)
 
             for i in range(num_conditions):
                 role = COPASI.CExperiment.ignore
                 obj = dm.findObjectByDisplayName(
                     'Values[' + cond_cols[i] + ']')
@@ -508,26 +613,37 @@
 
             obs = data.observableId[i]
             cond = data.simulationConditionId[i]
             time = data.time[i]
             value = data.measurement[i]
             params = data.observableParameters[i] \
                 if 'observableParameters' in data else None
-            transformation = data.observableTransformation[i] \
-                if 'observableTransformation' in data else 'lin'
+
+            try:
+                transformation = \
+                petab.observable_data.loc[petab.observable_data.observableId == obs]['observableTransformation'].values[
+                    0]
+                if transformation == 'log':
+                    value = math.log(float(value))
+                elif transformation == 'log10':
+                    value = math.log10(float(value))
+            except IndexError:
+                transformation = data.observableTransformation[i] \
+                    if 'observableTransformation' in data else 'lin'
+                pass
+            except KeyError:
+                transformation = data.observableTransformation[i] \
+                    if 'observableTransformation' in data else 'lin'
+                pass
+
             condition = data.simulationConditionId[i] \
                 if 'simulationConditionId' in data else None
             preequilibrationCondition = data.preequilibrationConditionId[i] \
                 if 'preequilibrationConditionId' in data else None
 
-            # if self.transform_data and transformation == 'log10':
-            #     value = math.pow(10.0, float(value))
-            # elif self.transform_data and transformation == 'log':
-            #     value = math.exp(float(value))
-
             if cond not in experiments.keys():
                 experiments[cond] = {'name': cond,
                                      'columns': {},
                                      'time': [],
                                      'offset': 0,
                                      'condition': condition,
                                      'preequilibrationCondition': preequilibrationCondition}
@@ -607,24 +723,26 @@
             if obj is None:
                 obj = dm.findObjectByDisplayName(str('Values[' + current.parameterName + ']'))
             if estimate == 0:
                 # update the initial value but don't create an item for it
                 if obj is not None:
                     obj.setInitialValue(value)
                 else:
-                    # could not resolve object, look into this
-                    logging.warning('could not resolve object {0} for fit item'.format(name))
+                    # check whether this is used in a noiseFormula
+                    if not self.petab.observable_data.noiseFormula.str.contains(name).any():
+                        # otherwise raise warning since we could not resolve object
+                        logger.warning('could not resolve object {0} for fit item'.format(name))
                 continue
 
             if obj is None:
                 # if there is no such parameter in the model, we might have 
                 # to create it first
                 model = dm.getModel()
                 obj = model.createModelValue(name, value)
-                logging.debug('created model value {0} for fit item'.format(name))
+                logger.debug('created model value {0} for fit item'.format(name))
 
             # update the initial value
             obj.setInitialValue(value)
 
             cn = obj.getInitialValueReference().getCN()
 
             # if we found it, we can get its internal identifier and create
@@ -642,24 +760,24 @@
         for condition in self.ignore_independent:
             for name in self.ignore_independent[condition]:
                 parameterId = self.ignore_independent[condition][name]
                 obj = dm.findObjectByDisplayName(str('Values[' + name + ']'))
                 if obj is None:
                     obj = dm.findObjectByDisplayName(name)
                 if obj is None:
-                    logging.warning(
+                    logger.warning(
                         'No model value for {0} to create fit item for'.
-                            format(name))
+                        format(name))
                     continue
 
                 current = parameters[parameters.parameterId == parameterId]
                 if current.shape[0] == 0:
                     # this should not be happening
-                    logging.warning('No entry for {0} in parameter table'.
-                                    format(parameterId))
+                    logger.warning('No entry for {0} in parameter table'.
+                                   format(parameterId))
                     continue
                 current = current.iloc[0]
                 # if current.parameterScale == 'log10':
                 #     lower = pow(10.0, float(current['lowerBound']))
                 #     upper = pow(10.0, float(current['upperBound']))
                 #     value = pow(10.0, float(current['nominalValue']))
                 # elif current.parameterScale == 'log':
@@ -740,62 +858,83 @@
         assumes, that the problem `petab`, `out_dir` and `out_name` has already been set
 
         :return: None
         """
 
         self.generate_copasi_file(self.petab, self.out_dir, self.out_name)
 
-    def add_transformation_for_params(self, obs, params):
-        # type: (str, str) -> None
+    def add_transformation_for_params(self, obs, params, transformation='lin'):
+        # type: (str, str, str) -> None
         """ add assignment rules to observable parameters """
         count = 0
 
         if params is None:
             return
 
         if np.isreal(params):
             if not np.isnan(params):
-                self.add_value_transform(params, 1, obs)
+                self.add_value_transform(params, 1, obs, transformation)
             return
 
         for param in params.split(';'):
             count += 1
             obj = dm.findObjectByDisplayName('Values[' + param + ']')
             if obj is None:
                 # it could be a value
-                if self.add_value_transform(param, count, obs):
+                if self.add_value_transform(param, count, obs, transformation):
                     continue
                 # otherwise add it as model value and try mapping
                 obj = dm.getModel().createModelValue(param, 1.0)
-                logging.debug('created model value {0} for transformation'.
-                              format(param))
+                logger.debug('created model value {0} for transformation'.
+                             format(param))
 
             obs_param = dm.findObjectByDisplayName(
                 'Values[observableParameter{0}_{1}]'.format(count, obs))
             if obs_param is None or \
                     not isinstance(obs_param, COPASI.CModelValue):
                 continue
             obs_param.setStatus(COPASI.CModelValue.Status_ASSIGNMENT)
-            obs_param.setExpression('<{0}>'.format(obj.getCN()))
+            if transformation == 'log':
+                obs_param.setExpression('ln(<{0}>)'.format(obj.getCN()))
+            elif transformation == 'log10':
+                obs_param.setExpression('log(<{0}>)'.format(obj.getCN()))
+            else:
+                obs_param.setExpression('<{0}>'.format(obj.getCN()))
 
     @staticmethod
-    def add_value_transform(value, index, obs):
+    def add_value_transform(value, index, obs, transformation='lin'):
         if isinstance(value, str):
             try:
                 value = float(value)
             except ValueError:
                 return False
         if np.isreal(value):
             obs_param = dm.findObjectByDisplayName(
                 'Values[observableParameter{0}_{1}]'.format(index, obs))
             if obs_param is None or \
                     not isinstance(obs_param, COPASI.CModelValue):
                 return False
-            obs_param.setValue(float(value))
-            obs_param.setInitialValue(float(value))
+            if transformation == 'log':
+                try:
+                    value = math.log(float(value))
+                except ValueError:
+                    logger.warning('encountered value {0} for log transform for measurement of observable {1}'.format(
+                        value, obs))
+                    value = 0
+            elif transformation == 'log10':
+                try:
+                    value = math.log10(float(value))
+                except ValueError:
+                    logger.warning('encountered value {0} for log transform for measurement of observable {1}'.format(
+                        value, obs))
+                    value = 0
+            else:
+                value = float(value)
+            obs_param.setValue(value)
+            obs_param.setInitialValue(value)
             return True
         return False
 
 
 def main():
     num_args = len(sys.argv)
```

### Comparing `copasi-petab-importer-1.0.3/copasi_petab_importer/petab.ui` & `copasi-petab-importer-1.0.4/copasi_petab_importer/petab.ui`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/SOURCES.txt` & `copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.3/setup.py` & `copasi-petab-importer-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.3/test/test_importer.py` & `copasi-petab-importer-1.0.4/test/test_importer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,72 @@
 import unittest
 
 import COPASI
 import sys
 import os
-_PATH = os.path.abspath("./")
+_PATH = os.path.abspath(os.path.dirname(__file__))
+_BENCHMARK_DIR = os.path.join(_PATH, '..', 'benchmarks',
+                              'hackathon_contributions_new_data_format')
 sys.path.append(_PATH)
 from copasi_petab_importer import convert_petab
 import glob
 
 try:
     import petabtests
     petab_tests_available = True
 except ImportError:
     petab_tests_available = False
 
+class TestConverter(unittest.TestCase):
+    def test_copasi_version(self):
+        self.assertGreater(int(COPASI.CVersion.VERSION.getVersionDevel()),  214,
+                           "Need newer COPASI version")
+
+    @unittest.skipIf(not os.path.exists(_BENCHMARK_DIR), 'benchmarks not available')
+    def test_petab_problem(self):
+        problem = convert_petab.PEtabProblem.from_yaml(os.path.join(_BENCHMARK_DIR,
+                                        'Bruno_JExpBio2016/'
+                                        'Bruno_JExpBio2016.yaml'))
+        self.assertTrue(os.path.exists(problem.measurement_file))
+        self.assertTrue(os.path.exists(problem.model_file))
+        self.assertTrue(os.path.exists(problem.observable_file))
+        self.assertTrue(os.path.exists(problem.condition_file))
+        self.assertTrue(os.path.exists(problem.parameter_file))
+
+    @unittest.skipIf(not os.path.exists(_BENCHMARK_DIR), 'benchmarks not available')
+    def test_import_bruno(self):
+        petab_dir = os.path.join(_BENCHMARK_DIR, 'Bruno_JExpBio2016')
+        self.assertTrue(os.path.exists(petab_dir))
+        model_name = 'Bruno_JExpBio2016'
+        out_dir = os.path.join(_PATH, 'out')
+        if not os.path.exists(out_dir):
+            os.mkdir(out_dir)
 
-def test_copasi_version():
-    assert int(COPASI.CVersion.VERSION.getVersionDevel()) >= 214, \
-        "Need newer COPASI version"
-
-
-def test_petab_problem():
-    problem = convert_petab.PEtabProblem.from_yaml(os.path.join(_PATH, 'benchmarks/'
-                                    'hackathon_contributions_new_data_format/'
-                                    'Bruno_JExpBio2016/'
-                                    'Bruno_JExpBio2016.yaml'))
-    assert os.path.exists(problem.measurement_file)
-    assert os.path.exists(problem.model_file)
-    assert os.path.exists(problem.observable_file)
-    assert os.path.exists(problem.condition_file)
-    assert os.path.exists(problem.parameter_file)
-
-
-def test_import():
-    petab_dir = os.path.join(_PATH, 'benchmarks/'
-                                    'hackathon_contributions_new_data_format/'
-                                    'Bruno_JExpBio2016')
-    assert os.path.exists(petab_dir)
-    model_name = 'Bruno_JExpBio2016'
-    out_dir = os.path.join(_PATH, 'out')
-    if not os.path.exists(out_dir):
-        os.mkdir(out_dir)
-
-    converter = convert_petab.PEtabConverter(petab_dir, model_name, out_dir)
-    converter.convert()
-
-    assert os.path.exists(converter.experimental_data_file)
-
-
-@unittest.skipUnless(petab_tests_available, 'petabtests need to be installed to run this')
-def test_petabtest_import():
-    cases = [c for c in glob.glob(petabtests.CASES_DIR + '/*/*.yaml') if '0' in c and 'solution' not in c]
-    for case in cases:
-        if '17' not in case:
-            continue
-        converter = convert_petab.PEtabConverter.from_yaml(case)
+        converter = convert_petab.PEtabConverter(petab_dir, model_name, out_dir)
         converter.convert()
+
+        self.assertTrue(os.path.exists(converter.experimental_data_file))
+    @unittest.skipIf(not os.path.exists(_BENCHMARK_DIR), 'benchmarks not available')
+    def test_import_bachmann(self):
+        petab_dir = os.path.join(_BENCHMARK_DIR, 'Bachmann_MSB2011')
+        self.assertTrue(os.path.exists(petab_dir))
+        model_name = 'Bachmann_MSB2011'
+        out_dir = os.path.join(_PATH, 'out')
+        if not os.path.exists(out_dir):
+            os.mkdir(out_dir)
+
+        converter = convert_petab.PEtabConverter(petab_dir, model_name, out_dir)
+        converter.convert()
+
+        self.assertTrue(os.path.exists(converter.experimental_data_file))
+    @unittest.skipUnless(petab_tests_available, 'petabtests need to be installed to run this')
+    def test_petabtest_import(self):
+        cases = [c for c in glob.glob(str(petabtests.CASES_DIR) + '/*/*.yaml') if '0' in c and 'solution' not in c]
+        for case in cases:
+            if '17' not in case:
+                continue
+            converter = convert_petab.PEtabConverter.from_yaml(case)
+            converter.convert()
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `copasi-petab-importer-1.0.3/versioneer.py` & `copasi-petab-importer-1.0.4/versioneer.py`

 * *Files identical despite different names*

