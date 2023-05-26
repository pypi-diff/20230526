# Comparing `tmp/time_series_test-0.7.2.tar.gz` & `tmp/time_series_test-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series_test-0.7.2.tar", last modified: Thu Nov 24 15:36:54 2022, max compression
+gzip compressed data, was "time_series_test-0.9.2.tar", last modified: Mon Jan 23 08:47:47 2023, max compression
```

## Comparing `time_series_test-0.7.2.tar` & `time_series_test-0.9.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35147 2022-11-24 15:36:38.661288 time_series_test-0.7.2/COPYING
--rw-r--r--   0        0        0      629 2022-11-24 15:36:38.773290 time_series_test-0.7.2/pyproject.toml
--rw-r--r--   0        0        0    14789 2022-11-24 15:36:38.773290 time_series_test-0.7.2/readme.md
--rw-r--r--   0        0        0    18326 2022-11-24 15:36:38.773290 time_series_test-0.7.2/time_series_test.py
--rw-r--r--   0        0        0    15476 1970-01-01 00:00:00.000000 time_series_test-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-01-23 08:47:32.899334 time_series_test-0.9.2/COPYING
+-rw-r--r--   0        0        0      629 2023-01-23 08:47:33.027343 time_series_test-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    17700 2023-01-23 08:47:33.027343 time_series_test-0.9.2/readme.md
+-rw-r--r--   0        0        0    25507 2023-01-23 08:47:33.027343 time_series_test-0.9.2/time_series_test.py
+-rw-r--r--   0        0        0    18387 1970-01-01 00:00:00.000000 time_series_test-0.9.2/PKG-INFO
```

### Comparing `time_series_test-0.7.2/COPYING` & `time_series_test-0.9.2/COPYING`

 * *Files identical despite different names*

### Comparing `time_series_test-0.7.2/pyproject.toml` & `time_series_test-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `time_series_test-0.7.2/readme.md` & `time_series_test-0.9.2/readme.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Time Series Test
 
-*A statistical test and plotting function for time-series data in general, and data from cognitive-pupillometry experiments in particular. Based on linear mixed effects modeling and crossvalidation.*
+*Statistical testing and plotting functions for time-series data in general, and data from cognitive-pupillometry experiments in particular. Based on linear mixed effects modeling, crossvalidation, and cluster-based permutation testing.*
 
 Sebastiaan Mathôt (@smathot) <br />
-Copyright 2021 - 2022
+Copyright 2021 - 2023
 
 [![Publish to PyPi](https://github.com/smathot/time_series_test/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/smathot/time_series_test/actions/workflows/publish-package.yaml)
 [![Tests](https://github.com/smathot/time_series_test/actions/workflows/run-unittests.yaml/badge.svg)](https://github.com/smathot/time_series_test/actions/workflows/run-unittests.yaml)
 
 
 ## Contents
 
@@ -22,33 +22,41 @@
 ## Citation
 
 Mathôt, S., & Vilotijević, A. (2022). Methods in cognitive pupillometry: design, preprocessing, and analysis. *Behavior Research Methods*. <https://doi.org/10.1101/2022.02.23.481628>
 
 
 ## About
 
-In general terms, this package implements a statistical test for a specific-yet-common question when analyzing time-series data:
+This library provides two main functions for statistical testing of time-series data: `lmer_crossvalidation_test()` and `lmer_permutation_test()`. For a detailed description, see the manuscript above, but below a short introduction to both functions with their respective advantages and disadavantages.
+
+
+### When to use crossvalidation?
+
+In general terms, `lmer_crossvalidation_test()` implements a statistical test for a specific-yet-common question when analyzing time-series data:
 
 > Do one or more independent variables affect a continuously recorded dependent variable (a 'time series') at any point in time?
 
 When to use this test:
 
 - For time series consisting of only a single component, that is, when each independent variable has only a single effect on the time series. An example of this is the effect of stimulus intensity on pupil size, when presenting light flashes of different intensities.
 - When you do not know a priori which time points to test.
 
 When *not* to use this test:
 
 - For time series that contain multiple components, that is, when each independent variable affects the time series in multiple ways that change over time. An example of this is the effect of visual attention on lateralized EEG recordings, where different EEG components emerge at different points in time.
 - When you know a priori which time points to test.
 
-More specifically, this package provides a function (`find()`) that locates and statistically tests effects in time-series data. It does so by using crossvalidation to identify time points to test, and then using a linear mixed effects model to actually perform the statistical test. More specifically, the data is subdivided in a number of subsets (by default 4). It takes one of the subsets (the *test* set) out of the full dataset, and conducts a linear mixed effects model on each sample of the remaining data (the *training* set). The sample with the highest absolute z value in the training set is used as the sample-to-be-tested for the test set. This procedure is repeated for all subsets of the data, and for all fixed effects in the model. Finally, a single linear mixed effects model is conducted for each fixed effects on the samples that were thus identified.
+More specifically, `lmer_crossvalidation_test()` locates and statistically tests effects in time-series data. It does so by using crossvalidation to identify time points to test, and then using a linear mixed effects model to actually perform the statistical test. More specifically, the data is subdivided in a number of subsets (by default 4). It takes one of the subsets (the *test* set) out of the full dataset, and conducts a linear mixed effects model on each sample of the remaining data (the *training* set). The sample with the highest absolute z value in the training set is used as the sample-to-be-tested for the test set. This procedure is repeated for all subsets of the data, and for all fixed effects in the model. Finally, a single linear mixed effects model is conducted for each fixed effects on the samples that were thus identified.
+
+This packages also provides a function (`plot()`) to visualize time-series data to visually annotate the results of `lmer_crossvalidation_test()`.
+
 
-This packages also provides a function (`plot()`) to visualize time-series data to visually annotate the results of `find()`.
+### When to use `lmer_permutation_test()`?
 
-For a more detailed description, see the manuscript above.
+`lmer_permutation_test()` implements a fairly standard cluster-based permutation test, which differs from most other implementations in that it relies on linear mixed-effects modeling to calculate the test statistics. Therefore, this function tends to be extremely computationally intensive, but should also be more sensitive than cluster-based permutation tests that are based on average data. Its main advantage as compared to `lmer_crossvalidation_test()` is that it is also valid for data with multiple components, such as event-related potentials (ERPs).
 
 
 ## Installation
 
 ```
 pip install time_series_test
 ```
@@ -190,15 +198,15 @@
 
 
 ![](https://github.com/smathot/time_series_test/raw/master/img/signal-plot-2.png)
 
 
 ## Function reference
 
-## <span style="color:purple">time\_series\_test.find</span>_(dm, formula, groups, re\_formula=None, winlen=1, split=4, split\_method='interleaved', samples\_fe=True, samples\_re=True, localizer\_re=False, fit\_method=None, suppress\_convergence\_warnings=False, fit\_kwargs=None, \*\*kwargs)_
+## <span style="color:purple">time\_series\_test.lmer\_crossvalidation\_test</span>_(dm, formula, groups, re\_formula=None, winlen=1, split=4, split\_method='interleaved', samples\_fe=True, samples\_re=True, localizer\_re=False, fit\_method=None, suppress\_convergence\_warnings=False, fit\_kwargs=None, \*\*kwargs)_
 
 Conducts a single linear mixed effects model to a time series, where the
 to-be-tested samples are determined through crossvalidation.
 
 This function uses `mixedlm()` from the `statsmodels` package. See the
 statsmodels documentation for a more detailed explanation of the
 parameters.
@@ -283,17 +291,68 @@
 ### Returns
 
 * **_dict_**
 
   A dict where keys are effect labels, and values are named tuples
   of `model`, `samples`, `p`, and `z`.
 
+## <span style="color:purple">time\_series\_test.lmer\_permutation\_test</span>_(dm, formula, groups, re\_formula=None, winlen=1, suppress\_convergence\_warnings=False, fit\_kwargs={}, iterations=1000, cluster\_p\_threshold=0.05, \*\*kwargs)_
+
+Performs a cluster-based permutation test based on sample-by-sample
+linear-mixed-effects analyses. The permutation test identifies clusters
+based on p-value threshold and uses the absolute of the summed z-values of
+the clusters as test statistic.
+
+If no clusters reach the threshold, the test is skipped right away. The
+Intercept is ignored for this criterion, because the intercept usually has
+significant clusters that we're not interested in.
+
+*Warning:* This is generally an extremely time-consuming analysis because
+it requires thousands of lmers to be run.
+
+See `lmer_crossvalidation()` for an explanation of the arguments.
+
+### Parameters
+
+* **dm: DataMatrix**
+
+* **formula: str**
+
+* **groups: str**
+
+* **re\_formula: str or None, optional**
+
+* **winlen: int, optional**
+
+* **suppress\_convergence\_warnings: bool, optional**
+
+* **fit\_kwargs: dict, optional**
+
+* **iterations: int, optional**
+
+  The number of permutations to run.
+
+* **cluster\_p\_threshold: float or None, optional**
+
+  The maximum p-value for a sample to be considered part of a cluster.
+
+* **\*\*kwargs: dict, optional**
+
+### Returns
+
+* **_dict_**
+
+  A dict with effects as keys and lists of clusters defined by
+  (start, end, z-sum, hit proportion) tuples. The p-value is
+  1 - hit proportion.
+
 ## <span style="color:purple">time\_series\_test.lmer\_series</span>_(dm, formula, winlen=1, fit\_kwargs={}, \*\*kwargs)_
 
-Performs a sample-by-sample linear-mixed-effects analysis.
+Performs a sample-by-sample linear-mixed-effects analysis. See `lmer_crossvalidation()`
+for an explanation of the arguments.
 
 ### Parameters
 
 * **dm: DataMatrix**
 
 * **formula: str**
 
@@ -312,15 +371,15 @@
   specified in the formula:
 
   - `est`: the slope
   - `p`: the p value
   - `z`: the z value
   - `se`: the standard error
 
-## <span style="color:purple">time\_series\_test.plot</span>_(dm, dv, hue\_factor, results=None, linestyle\_factor=None, hues=None, linestyles=None, alpha\_level=0.05, annotate\_intercept=False, annotation\_hues=None, annotation\_linestyle=':')_
+## <span style="color:purple">time\_series\_test.plot</span>_(dm, dv, hue\_factor, results=None, linestyle\_factor=None, hues=None, linestyles=None, alpha\_level=0.05, annotate\_intercept=False, annotation\_hues=None, annotation\_linestyle=':', legend\_kwargs=None, annotation\_legend\_kwargs=None)_
 
 Visualizes a time series, where the signal is plotted as a function of
 sample number on the x-axis. One fixed effect is indicated by the hue
 (color) of the lines. An optional second fixed effect is indicated by the
 linestyle. If the `results` parameter is used, significant effects are
 annotated in the figure.
 
@@ -338,15 +397,15 @@
 * **hue\_factor: str**
 
   The name of a regular (non-series) column in `dm` that specifies the
   hue (color) of the lines.
 
 * **results: dict, optional**
 
-  A `results` dict as returned by `find()`.
+  A `results` dict as returned by `lmer_crossvalidation()`.
 
 * **linestyle\_factor: str, optional**
 
   The name of a regular (non-series) column in `dm` that specifies the
   linestyle of the lines for a two-factor plot.
 
 * **hues: str, list, or None, optional**
@@ -373,24 +432,33 @@
   The name of a matplotlib colormap or a list of hues to be used for the
   annotations if `results` is provided.
 
 * **annotation\_linestyle: str, optional**
 
   The linestyle for the annotations.
 
+* **legend\_kwargs: None or dict, optional**
+
+  Optional keywords to be passed to `plt.legend()` for the factor legend.
+
+* **annotation\_legend\_kwargs: None or dict, optional**
+
+  Optional keywords to be passed to `plt.legend()` for the annotation
+  legend.
+
 ## <span style="color:purple">time\_series\_test.summarize</span>_(results, detailed=False)_
 
 Generates a string with a human-readable summary of a results `dict` as
-returned by `find()`.
+returned by `lmer_crossvalidation()`.
 
 ### Parameters
 
 * **results: dict**
 
-  A `results` dict as returned by `find()`.
+  A `results` dict as returned by `lmer_crossvalidation()`.
 
 * **detailed: bool, optional**
 
   Indicates whether model details should be included in the summary.
 
 ### Returns
```

### Comparing `time_series_test-0.7.2/time_series_test.py` & `time_series_test-0.9.2/time_series_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 from matplotlib.lines import Line2D
 import statsmodels.formula.api as smf
 import warnings
 import logging
 import re
 from collections import namedtuple
 
-__version__ = '0.7.2'
+__version__ = '0.9.2'
 DEFAULT_HUE_COLORMAP = 'Dark2'
 DEFAULT_ANNOTATION_COLORMAP = 'brg'
 DEEP_ORANGE = ['#bf360c', '#e64a19', '#ff5722', '#ff8a65', '#ffccbc']
 LINESTYLES = ['-', '--', ':']
 logger = logging.getLogger('time_series_test')
 
 
-def find(dm, formula, groups, re_formula=None, winlen=1, split=4,
-         split_method='interleaved', samples_fe=True, samples_re=True,
-         localizer_re=False, fit_method=None,
-         suppress_convergence_warnings=False, fit_kwargs=None, **kwargs):
+def lmer_crossvalidation_test(dm, formula, groups, re_formula=None, winlen=1,
+        split=4, split_method='interleaved', samples_fe=True, samples_re=True,
+        localizer_re=False, fit_method=None,
+        suppress_convergence_warnings=False, fit_kwargs=None, **kwargs):
     """Conducts a single linear mixed effects model to a time series, where the
     to-be-tested samples are determined through crossvalidation.
     
     This function uses `mixedlm()` from the `statsmodels` package. See the
     statsmodels documentation for a more detailed explanation of the
     parameters.
     
@@ -109,15 +109,16 @@
         return _lmer_test_localizer(dm, formula, groups, re_formula=re_formula,
                                     winlen=winlen, samples_fe=samples_fe,
                                     fit_kwargs=fit_kwargs, samples_re=samples_re,
                                     **kwargs)
 
 
 def lmer_series(dm, formula, winlen=1, fit_kwargs={}, **kwargs):
-    """Performs a sample-by-sample linear-mixed-effects analysis.
+    """Performs a sample-by-sample linear-mixed-effects analysis. See `lmer_crossvalidation()`
+    for an explanation of the arguments.
     
     Parameters
     ----------
     dm: DataMatrix
     formula: str
     winlen: int, optional
     fit_kwargs: dict, optional
@@ -170,17 +171,127 @@
             rm.p[:, sample] = list(lm.pvalues[:length])
             rm.z[:, sample] = list(lm.tvalues[:length])
             rm.est[:, sample] = list(lm.params[:length])
             rm.se[:, sample] = list(lm.bse[:length])
     return rm
 
 
+def lmer_permutation_test(dm, formula, groups, re_formula=None, winlen=1,
+                          suppress_convergence_warnings=False, fit_kwargs={},
+                          iterations=1000, cluster_p_threshold=.05, **kwargs):
+    """Performs a cluster-based permutation test based on sample-by-sample
+    linear-mixed-effects analyses. The permutation test identifies clusters
+    based on p-value threshold and uses the absolute of the summed z-values of
+    the clusters as test statistic.
+    
+    If no clusters reach the threshold, the test is skipped right away. The
+    Intercept is ignored for this criterion, because the intercept usually has
+    significant clusters that we're not interested in.
+    
+    *Warning:* This is generally an extremely time-consuming analysis because
+    it requires thousands of lmers to be run.
+    
+    See `lmer_crossvalidation()` for an explanation of the arguments.
+    
+    Parameters
+    ----------
+    dm: DataMatrix
+    formula: str
+    groups: str
+    re_formula: str or None, optional
+    winlen: int, optional
+    suppress_convergence_warnings: bool, optional
+    fit_kwargs: dict, optional
+    iterations: int, optional
+        The number of permutations to run.
+    cluster_p_threshold: float or None, optional
+        The maximum p-value for a sample to be considered part of a cluster.
+    **kwargs: dict, optional
+    
+    Returns
+    -------
+    dict
+        A dict with effects as keys and lists of clusters defined by
+        (start, end, z-sum, hit proportion) tuples. The p-value is
+        1 - hit proportion.
+    """
+    dm = _trim_dm(dm, formula, groups, re_formula)
+    terms = _terms(formula, **kwargs)
+    dv = terms[0]
+    # First conduct a regular sample-by-sample lme, and get the size of the
+    # largest clusters for each effect
+    with warnings.catch_warnings():
+        if suppress_convergence_warnings:
+            from statsmodels.tools.sm_exceptions import ConvergenceWarning
+            warnings.simplefilter(action='ignore', category=ConvergenceWarning)
+        rm_obs = lmer_series(dm, formula=formula, groups=groups,
+                             re_formula=re_formula, winlen=winlen,
+                             fit_kwargs=fit_kwargs, **kwargs)
+    cluster_obs = _clusters(rm_obs, cluster_p_threshold)
+    # This is where we will store the hits for each of the observed clusters
+    cluster_hits = {effect: [0] * len(clusters)
+                    for effect, clusters in cluster_obs.items()}
+    logger.info(f'observed clusters: {cluster_obs}')
+    # Now run through all iterations
+    for i in range(iterations):
+        # If there are no significant clusters, we'll skip the test altogether
+        # to save time. The Intercept doesn't count here, because the intercept
+        # generally does have significant clusters but we're not interested in
+        # those.
+        if not any(clusters for effect, clusters in cluster_obs.items()
+                   if effect != 'Intercept'):
+            logger.info(f'no clusters reach threshold, skipping test')
+            break
+        logger.info(f'start of iteration {i}')
+        # Permute the order of the terms while keeping groups intact
+        for group, gdm in ops.split(dm[groups]):
+            for term in terms:
+                dm[term][gdm] = ops.shuffle(gdm[term])
+        # Conduct a sample-by-sample lme on the permuted data, and get the
+        # largest (spurious) clusters
+        with warnings.catch_warnings():
+            if suppress_convergence_warnings:
+                from statsmodels.tools.sm_exceptions import ConvergenceWarning
+                warnings.simplefilter(action='ignore', category=ConvergenceWarning)
+            rm_it = lmer_series(dm, formula=formula, groups=groups,
+                                re_formula=re_formula, winlen=winlen,
+                                fit_kwargs=fit_kwargs, **kwargs)
+        cluster_it = _clusters(rm_it, cluster_p_threshold)
+        logger.info(f'observed clusters: {cluster_obs}')
+        logger.info(f'permuted clusters: {cluster_it}')
+        # For each effect, when the observed cluster size exceeds the spurious
+        # cluster size, consider this a hit
+        for effect in cluster_hits:
+            if not cluster_it[effect]:
+                zsum_it = 0
+            else:
+                # Get the biggers spurious cluster
+                _, _, zsum_it = cluster_it[effect][0]
+            logger.info(f'permutation zsum for {effect} = {zsum_it:.2f}')
+            for j, (_, _, zsum_obs) in enumerate(cluster_obs[effect]):
+                if zsum_obs > zsum_it:
+                    logger.info(f'hit for {effect} cluster {j} ({zsum_obs:.2f} > {zsum_it:.2f})')
+                    cluster_hits[effect][j] += 1
+                else:
+                    logger.info(f'miss for {effect} cluster {j} ({zsum_obs:.2f} <= {zsum_it:.2f})')
+        logger.info(f'hits after iteration {i}: {cluster_hits}')
+    # Return a dict with a list of (start, end, zsum, pvalue) tuples
+    cluster_pvalues = {}
+    for effect, hitlist in cluster_hits.items():
+        cluster_pvalues[effect] = []
+        for hits, (start, end, zsum) in zip(hitlist, cluster_obs[effect]):
+            cluster_pvalues[effect].append(
+                (start, end, zsum, hits / iterations))
+    return cluster_pvalues
+
+
 def plot(dm, dv, hue_factor, results=None, linestyle_factor=None, hues=None,
          linestyles=None, alpha_level=.05, annotate_intercept=False,
-         annotation_hues=None, annotation_linestyle=':'):
+         annotation_hues=None, annotation_linestyle=':', legend_kwargs=None,
+         annotation_legend_kwargs=None):
     """Visualizes a time series, where the signal is plotted as a function of
     sample number on the x-axis. One fixed effect is indicated by the hue
     (color) of the lines. An optional second fixed effect is indicated by the
     linestyle. If the `results` parameter is used, significant effects are
     annotated in the figure.
     
     Parameters
@@ -190,15 +301,15 @@
     dv: str
         The name of the dependent variable, which should be a series column
         in `dm`.
     hue_factor: str
         The name of a regular (non-series) column in `dm` that specifies the
         hue (color) of the lines.
     results: dict, optional
-        A `results` dict as returned by `find()`.
+        A `results` dict as returned by `lmer_crossvalidation()`.
     linestyle_factor: str, optional
         The name of a regular (non-series) column in `dm` that specifies the
         linestyle of the lines for a two-factor plot.
     hues: str, list, or None, optional
         The name of a matplotlib colormap or a list of hues to be used as line
         colors for the hue factor.
     linestyles: list or None, optional
@@ -210,14 +321,19 @@
         Specifies whether the intercept should also be annotated along with
         the fixed effects.
     annotation_hues: str, list, or None, optional
         The name of a matplotlib colormap or a list of hues to be used for the
         annotations if `results` is provided.
     annotation_linestyle: str, optional
         The linestyle for the annotations.
+    legend_kwargs: None or dict, optional
+        Optional keywords to be passed to `plt.legend()` for the factor legend.
+    annotation_legend_kwargs: None or dict, optional
+        Optional keywords to be passed to `plt.legend()` for the annotation
+        legend.
     """
     cols = [dv]
     if hue_factor is not None:
         cols.append(hue_factor)
     if linestyle_factor is not None:
         cols.append(linestyle_factor)
     dm = dm[cols]
@@ -269,42 +385,49 @@
                 yerr = dm2[dv].std / np.sqrt(n)
                 ymin = y - yerr
                 ymax = y + yerr
                 plt.fill_between(x, ymin, ymax, color=hue, alpha=.2)
                 plt.plot(y, color=hue, linestyle=linestyle)
     # Implement legend
     if annotation_elements:
-        plt.gca().add_artist(plt.legend(loc='lower right'))
+        if annotation_legend_kwargs is not None:
+            annotation_legend = plt.legend(**annotation_legend_kwargs)
+        else:
+            annotation_legend = plt.legend(loc='lower right')
+        plt.gca().add_artist(annotation_legend)
     hue_legend = [
         Line2D([0], [0], color=hues[i1 % len(hues)], label=f1)
         for i1, f1 in enumerate(dm[hue_factor].unique)
     ]
-    legend = plt.gca().legend(
-        handles=hue_legend,
-        title=hue_factor,
-        loc='upper left')
+    if legend_kwargs is not None:
+        legend = plt.gca().legend(handles=hue_legend, **legend_kwargs)
+    else:
+        legend = plt.gca().legend(
+            handles=hue_legend,
+            title=hue_factor,
+            loc='upper left')
     if linestyle_factor is not None:
         plt.gca().add_artist(legend)
         linestyle_legend = [
             Line2D([0], [0], color='black',
                    linestyle=linestyles[i2 % len(linestyles)], label=f2)
             for i2, f2 in enumerate(dm[linestyle_factor].unique)
         ]
         plt.gca().legend(handles=linestyle_legend, title=linestyle_factor,
                          loc='upper right')
 
 
 def summarize(results, detailed=False):
     """Generates a string with a human-readable summary of a results `dict` as
-    returned by `find()`.
+    returned by `lmer_crossvalidation()`.
 
     Parameters
     ----------
     results: dict
-        A `results` dict as returned by `find()`.
+        A `results` dict as returned by `lmer_crossvalidation()`.
     detailed: bool, optional
         Indicates whether model details should be included in the summary.
 
     Returns
     -------
     str
     """
@@ -442,7 +565,39 @@
         terms += _split_terms(kwargs['re_formula'])
     return terms
 
 
 def _colors(colormap, n):
     cm = plt.colormaps[colormap]
     return [cm(int(hue)) for hue in np.linspace(0, cm.N, n)]
+
+
+def _clusters(rm, cluster_p_threshold):
+    """Extracts the largest clusters based on a p-threshold of .05 based on a
+    datamatrix as returned by lmer_series(). Returns a dict with effects as
+    keys and a list of (start, end, zsum) tuples as values. The list is sorted
+    by the zsum.
+    """
+    clusters = {}
+    for row in rm:
+        pi = None
+        clusters[row.effect] = []
+        # Loop through all indices that are part of clusters
+        for i in np.where(row.p < cluster_p_threshold)[0]:
+            # We're entering a new cluster
+            if i - 1 != pi:
+                # Store previous cluster
+                if pi is not None:
+                    clusters[row.effect].append((start, i, abs(z_sum)))
+                start = i
+                z_sum = 0
+            z_sum += row.z[i]
+            pi = i
+        if pi is not None:
+            # Store last cluster
+            clusters[row.effect].append((start, i, abs(z_sum)))
+        clusters[row.effect].sort(key=lambda i: -i[2])
+    return clusters
+
+
+# alias for backwards compatibility
+find = lmer_crossvalidation_test
```

### Comparing `time_series_test-0.7.2/PKG-INFO` & `time_series_test-0.9.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: time_series_test
-Version: 0.7.2
+Version: 0.9.2
 Summary: A statistical test and plotting function for time-series data in general, and data from cognitive-pupillometry experiments in particular. Based on linear mixed effects modeling and crossvalidation.
 Keywords: signal processing,statistics,plotting,data analysis,crossvalidation
 Author-email: Sebastiaan Mathôt <s.mathot@cogsci.nl>
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Requires-Dist: python-datamatrix
 Requires-Dist: statsmodels
 Requires-Dist: matplotlib
 Project-URL: Documentation, https://github.com/smathot/time_series_test
 Project-URL: Source, https://github.com/smathot/time_series_test
 
 # Time Series Test
 
-*A statistical test and plotting function for time-series data in general, and data from cognitive-pupillometry experiments in particular. Based on linear mixed effects modeling and crossvalidation.*
+*Statistical testing and plotting functions for time-series data in general, and data from cognitive-pupillometry experiments in particular. Based on linear mixed effects modeling, crossvalidation, and cluster-based permutation testing.*
 
 Sebastiaan Mathôt (@smathot) <br />
-Copyright 2021 - 2022
+Copyright 2021 - 2023
 
 [![Publish to PyPi](https://github.com/smathot/time_series_test/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/smathot/time_series_test/actions/workflows/publish-package.yaml)
 [![Tests](https://github.com/smathot/time_series_test/actions/workflows/run-unittests.yaml/badge.svg)](https://github.com/smathot/time_series_test/actions/workflows/run-unittests.yaml)
 
 
 ## Contents
 
@@ -36,33 +36,41 @@
 ## Citation
 
 Mathôt, S., & Vilotijević, A. (2022). Methods in cognitive pupillometry: design, preprocessing, and analysis. *Behavior Research Methods*. <https://doi.org/10.1101/2022.02.23.481628>
 
 
 ## About
 
-In general terms, this package implements a statistical test for a specific-yet-common question when analyzing time-series data:
+This library provides two main functions for statistical testing of time-series data: `lmer_crossvalidation_test()` and `lmer_permutation_test()`. For a detailed description, see the manuscript above, but below a short introduction to both functions with their respective advantages and disadavantages.
+
+
+### When to use crossvalidation?
+
+In general terms, `lmer_crossvalidation_test()` implements a statistical test for a specific-yet-common question when analyzing time-series data:
 
 > Do one or more independent variables affect a continuously recorded dependent variable (a 'time series') at any point in time?
 
 When to use this test:
 
 - For time series consisting of only a single component, that is, when each independent variable has only a single effect on the time series. An example of this is the effect of stimulus intensity on pupil size, when presenting light flashes of different intensities.
 - When you do not know a priori which time points to test.
 
 When *not* to use this test:
 
 - For time series that contain multiple components, that is, when each independent variable affects the time series in multiple ways that change over time. An example of this is the effect of visual attention on lateralized EEG recordings, where different EEG components emerge at different points in time.
 - When you know a priori which time points to test.
 
-More specifically, this package provides a function (`find()`) that locates and statistically tests effects in time-series data. It does so by using crossvalidation to identify time points to test, and then using a linear mixed effects model to actually perform the statistical test. More specifically, the data is subdivided in a number of subsets (by default 4). It takes one of the subsets (the *test* set) out of the full dataset, and conducts a linear mixed effects model on each sample of the remaining data (the *training* set). The sample with the highest absolute z value in the training set is used as the sample-to-be-tested for the test set. This procedure is repeated for all subsets of the data, and for all fixed effects in the model. Finally, a single linear mixed effects model is conducted for each fixed effects on the samples that were thus identified.
+More specifically, `lmer_crossvalidation_test()` locates and statistically tests effects in time-series data. It does so by using crossvalidation to identify time points to test, and then using a linear mixed effects model to actually perform the statistical test. More specifically, the data is subdivided in a number of subsets (by default 4). It takes one of the subsets (the *test* set) out of the full dataset, and conducts a linear mixed effects model on each sample of the remaining data (the *training* set). The sample with the highest absolute z value in the training set is used as the sample-to-be-tested for the test set. This procedure is repeated for all subsets of the data, and for all fixed effects in the model. Finally, a single linear mixed effects model is conducted for each fixed effects on the samples that were thus identified.
+
+This packages also provides a function (`plot()`) to visualize time-series data to visually annotate the results of `lmer_crossvalidation_test()`.
+
 
-This packages also provides a function (`plot()`) to visualize time-series data to visually annotate the results of `find()`.
+### When to use `lmer_permutation_test()`?
 
-For a more detailed description, see the manuscript above.
+`lmer_permutation_test()` implements a fairly standard cluster-based permutation test, which differs from most other implementations in that it relies on linear mixed-effects modeling to calculate the test statistics. Therefore, this function tends to be extremely computationally intensive, but should also be more sensitive than cluster-based permutation tests that are based on average data. Its main advantage as compared to `lmer_crossvalidation_test()` is that it is also valid for data with multiple components, such as event-related potentials (ERPs).
 
 
 ## Installation
 
 ```
 pip install time_series_test
 ```
@@ -204,15 +212,15 @@
 
 
 ![](https://github.com/smathot/time_series_test/raw/master/img/signal-plot-2.png)
 
 
 ## Function reference
 
-## <span style="color:purple">time\_series\_test.find</span>_(dm, formula, groups, re\_formula=None, winlen=1, split=4, split\_method='interleaved', samples\_fe=True, samples\_re=True, localizer\_re=False, fit\_method=None, suppress\_convergence\_warnings=False, fit\_kwargs=None, \*\*kwargs)_
+## <span style="color:purple">time\_series\_test.lmer\_crossvalidation\_test</span>_(dm, formula, groups, re\_formula=None, winlen=1, split=4, split\_method='interleaved', samples\_fe=True, samples\_re=True, localizer\_re=False, fit\_method=None, suppress\_convergence\_warnings=False, fit\_kwargs=None, \*\*kwargs)_
 
 Conducts a single linear mixed effects model to a time series, where the
 to-be-tested samples are determined through crossvalidation.
 
 This function uses `mixedlm()` from the `statsmodels` package. See the
 statsmodels documentation for a more detailed explanation of the
 parameters.
@@ -297,17 +305,68 @@
 ### Returns
 
 * **_dict_**
 
   A dict where keys are effect labels, and values are named tuples
   of `model`, `samples`, `p`, and `z`.
 
+## <span style="color:purple">time\_series\_test.lmer\_permutation\_test</span>_(dm, formula, groups, re\_formula=None, winlen=1, suppress\_convergence\_warnings=False, fit\_kwargs={}, iterations=1000, cluster\_p\_threshold=0.05, \*\*kwargs)_
+
+Performs a cluster-based permutation test based on sample-by-sample
+linear-mixed-effects analyses. The permutation test identifies clusters
+based on p-value threshold and uses the absolute of the summed z-values of
+the clusters as test statistic.
+
+If no clusters reach the threshold, the test is skipped right away. The
+Intercept is ignored for this criterion, because the intercept usually has
+significant clusters that we're not interested in.
+
+*Warning:* This is generally an extremely time-consuming analysis because
+it requires thousands of lmers to be run.
+
+See `lmer_crossvalidation()` for an explanation of the arguments.
+
+### Parameters
+
+* **dm: DataMatrix**
+
+* **formula: str**
+
+* **groups: str**
+
+* **re\_formula: str or None, optional**
+
+* **winlen: int, optional**
+
+* **suppress\_convergence\_warnings: bool, optional**
+
+* **fit\_kwargs: dict, optional**
+
+* **iterations: int, optional**
+
+  The number of permutations to run.
+
+* **cluster\_p\_threshold: float or None, optional**
+
+  The maximum p-value for a sample to be considered part of a cluster.
+
+* **\*\*kwargs: dict, optional**
+
+### Returns
+
+* **_dict_**
+
+  A dict with effects as keys and lists of clusters defined by
+  (start, end, z-sum, hit proportion) tuples. The p-value is
+  1 - hit proportion.
+
 ## <span style="color:purple">time\_series\_test.lmer\_series</span>_(dm, formula, winlen=1, fit\_kwargs={}, \*\*kwargs)_
 
-Performs a sample-by-sample linear-mixed-effects analysis.
+Performs a sample-by-sample linear-mixed-effects analysis. See `lmer_crossvalidation()`
+for an explanation of the arguments.
 
 ### Parameters
 
 * **dm: DataMatrix**
 
 * **formula: str**
 
@@ -326,15 +385,15 @@
   specified in the formula:
 
   - `est`: the slope
   - `p`: the p value
   - `z`: the z value
   - `se`: the standard error
 
-## <span style="color:purple">time\_series\_test.plot</span>_(dm, dv, hue\_factor, results=None, linestyle\_factor=None, hues=None, linestyles=None, alpha\_level=0.05, annotate\_intercept=False, annotation\_hues=None, annotation\_linestyle=':')_
+## <span style="color:purple">time\_series\_test.plot</span>_(dm, dv, hue\_factor, results=None, linestyle\_factor=None, hues=None, linestyles=None, alpha\_level=0.05, annotate\_intercept=False, annotation\_hues=None, annotation\_linestyle=':', legend\_kwargs=None, annotation\_legend\_kwargs=None)_
 
 Visualizes a time series, where the signal is plotted as a function of
 sample number on the x-axis. One fixed effect is indicated by the hue
 (color) of the lines. An optional second fixed effect is indicated by the
 linestyle. If the `results` parameter is used, significant effects are
 annotated in the figure.
 
@@ -352,15 +411,15 @@
 * **hue\_factor: str**
 
   The name of a regular (non-series) column in `dm` that specifies the
   hue (color) of the lines.
 
 * **results: dict, optional**
 
-  A `results` dict as returned by `find()`.
+  A `results` dict as returned by `lmer_crossvalidation()`.
 
 * **linestyle\_factor: str, optional**
 
   The name of a regular (non-series) column in `dm` that specifies the
   linestyle of the lines for a two-factor plot.
 
 * **hues: str, list, or None, optional**
@@ -387,24 +446,33 @@
   The name of a matplotlib colormap or a list of hues to be used for the
   annotations if `results` is provided.
 
 * **annotation\_linestyle: str, optional**
 
   The linestyle for the annotations.
 
+* **legend\_kwargs: None or dict, optional**
+
+  Optional keywords to be passed to `plt.legend()` for the factor legend.
+
+* **annotation\_legend\_kwargs: None or dict, optional**
+
+  Optional keywords to be passed to `plt.legend()` for the annotation
+  legend.
+
 ## <span style="color:purple">time\_series\_test.summarize</span>_(results, detailed=False)_
 
 Generates a string with a human-readable summary of a results `dict` as
-returned by `find()`.
+returned by `lmer_crossvalidation()`.
 
 ### Parameters
 
 * **results: dict**
 
-  A `results` dict as returned by `find()`.
+  A `results` dict as returned by `lmer_crossvalidation()`.
 
 * **detailed: bool, optional**
 
   Indicates whether model details should be included in the summary.
 
 ### Returns
```

