# Comparing `tmp/collective.taxonomy-3.0.1.tar.gz` & `tmp/collective.taxonomy-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.taxonomy-3.0.1.tar", last modified: Thu Feb  2 11:59:30 2023, max compression
+gzip compressed data, was "collective.taxonomy-3.1.tar", last modified: Fri May 26 12:19:29 2023, max compression
```

## Comparing `collective.taxonomy-3.0.1.tar` & `collective.taxonomy-3.1.tar`

### file list

```diff
@@ -1,230 +1,261 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.710899 collective.taxonomy-3.0.1/
--rw-r--r--   0 ericof     (501) staff       (20)      148 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/.coveragerc
--rw-r--r--   0 ericof     (501) staff       (20)     8454 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/CHANGES.rst
--rw-r--r--   0 ericof     (501) staff       (20)      619 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)    11517 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/Makefile
--rw-r--r--   0 ericof     (501) staff       (20)    18989 2023-02-02 11:59:30.711000 collective.taxonomy-3.0.1/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     9575 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/README.rst
--rw-r--r--   0 ericof     (501) staff       (20)       58 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/constraints.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.685838 collective.taxonomy-3.0.1/docs/
--rw-r--r--   0 ericof     (501) staff       (20)       28 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/105.bugfix
--rw-r--r--   0 ericof     (501) staff       (20)       47 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/116.bugfix
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/LICENSE.GPL
--rw-r--r--   0 ericof     (501) staff       (20)      726 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/LICENSE.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.690778 collective.taxonomy-3.0.1/docs/img/
--rw-r--r--   0 ericof     (501) staff       (20)    84621 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/add-portfolio-view-001.png
--rw-r--r--   0 ericof     (501) staff       (20)   131192 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/add-portfolio-view-002.png
--rw-r--r--   0 ericof     (501) staff       (20)   238942 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/add-portfolio-view-003.png
--rw-r--r--   0 ericof     (501) staff       (20)   410063 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/add-portfolio-view-004.png
--rw-r--r--   0 ericof     (501) staff       (20)    84604 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/add-taxonomy-001.png
--rw-r--r--   0 ericof     (501) staff       (20)    89941 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/add-taxonomy-002.png
--rw-r--r--   0 ericof     (501) staff       (20)    89267 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/add-taxonomy-003.png
--rw-r--r--   0 ericof     (501) staff       (20)    92683 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/add-taxonomy-004.png
--rw-r--r--   0 ericof     (501) staff       (20)   125750 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/create-portfolio-data-001.png
--rw-r--r--   0 ericof     (501) staff       (20)    58306 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/create-portfolio-data-002.png
--rw-r--r--   0 ericof     (501) staff       (20)    96146 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/create-portfolio-data-003.png
--rw-r--r--   0 ericof     (501) staff       (20)   100598 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/create-portfolio-data-004.png
--rw-r--r--   0 ericof     (501) staff       (20)    76273 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/create-portfolio-data-005.png
--rw-r--r--   0 ericof     (501) staff       (20)    70538 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/create-portfolio-data-006.png
--rw-r--r--   0 ericof     (501) staff       (20)   100654 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/edit-taxonomy-data-001.png
--rw-r--r--   0 ericof     (501) staff       (20)    96150 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/edit-taxonomy-data-002.png
--rw-r--r--   0 ericof     (501) staff       (20)   140964 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/edit-taxonomy-data-003.png
--rw-r--r--   0 ericof     (501) staff       (20)   103935 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/edit-taxonomy-data-004.png
--rw-r--r--   0 ericof     (501) staff       (20)    66228 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/enable-behavior-001.png
--rw-r--r--   0 ericof     (501) staff       (20)    97900 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/enable-behavior-002.png
--rw-r--r--   0 ericof     (501) staff       (20)    91223 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/enable-behavior-003.png
--rw-r--r--   0 ericof     (501) staff       (20)    95399 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/enable-behavior-004.png
--rw-r--r--   0 ericof     (501) staff       (20)    78953 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/enable-behavior-005.png
--rw-r--r--   0 ericof     (501) staff       (20)   182658 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/img/video-generated-by-test.gif
--rw-r--r--   0 ericof     (501) staff       (20)     8276 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/docs/tutorial.md
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.691021 collective.taxonomy-3.0.1/images/
--rw-r--r--   0 ericof     (501) staff       (20)   178318 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/images/edit_taxonomy_data.gif
--rw-r--r--   0 ericof     (501) staff       (20)      459 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/instance.yaml
--rw-r--r--   0 ericof     (501) staff       (20)      821 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/mx.ini
--rw-r--r--   0 ericof     (501) staff       (20)      148 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)      154 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/requirements.txt
--rw-r--r--   0 ericof     (501) staff       (20)       38 2023-02-02 11:59:30.711238 collective.taxonomy-3.0.1/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2006 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.681219 collective.taxonomy-3.0.1/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.691258 collective.taxonomy-3.0.1/src/collective/
--rw-r--r--   0 ericof     (501) staff       (20)      169 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.696133 collective.taxonomy-3.0.1/src/collective/taxonomy/
--rw-r--r--   0 ericof     (501) staff       (20)      125 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     8384 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/behavior.py
--rw-r--r--   0 ericof     (501) staff       (20)     2487 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/browser.py
--rw-r--r--   0 ericof     (501) staff       (20)     1983 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/collectionfilter.py
--rw-r--r--   0 ericof     (501) staff       (20)     2817 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/collective.taxonomy.css
--rw-r--r--   0 ericof     (501) staff       (20)     4680 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)    11736 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/controlpanel.py
--rw-r--r--   0 ericof     (501) staff       (20)     1167 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/edit_taxonomy_data.pt
--rw-r--r--   0 ericof     (501) staff       (20)     4864 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/exportimport.py
--rw-r--r--   0 ericof     (501) staff       (20)     1218 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/factory.py
--rw-r--r--   0 ericof     (501) staff       (20)     1771 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/generated.py
--rw-r--r--   0 ericof     (501) staff       (20)      152 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/i18n.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.696612 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/
--rw-r--r--   0 ericof     (501) staff       (20)      355 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/LICENSE.txt
--rw-r--r--   0 ericof     (501) staff       (20)     2877 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/README.txt
--rw-r--r--   0 ericof     (501) staff       (20)      943 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/config.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.697336 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/
--rw-r--r--   0 ericof     (501) staff       (20)     1857 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/animation.css
--rw-r--r--   0 ericof     (501) staff       (20)      373 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/taxonomy-codes.css
--rw-r--r--   0 ericof     (501) staff       (20)    14717 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/taxonomy-embedded.css
--rw-r--r--   0 ericof     (501) staff       (20)      679 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/taxonomy-ie7-codes.css
--rw-r--r--   0 ericof     (501) staff       (20)      948 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/taxonomy-ie7.css
--rw-r--r--   0 ericof     (501) staff       (20)     2122 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/taxonomy.css
--rw-r--r--   0 ericof     (501) staff       (20)     6951 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/demo.html
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.697939 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/font/
--rw-r--r--   0 ericof     (501) staff       (20)     6120 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/font/taxonomy.eot
--rw-r--r--   0 ericof     (501) staff       (20)     2284 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/font/taxonomy.svg
--rw-r--r--   0 ericof     (501) staff       (20)     5952 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/font/taxonomy.ttf
--rw-r--r--   0 ericof     (501) staff       (20)     3588 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/font/taxonomy.woff
--rw-r--r--   0 ericof     (501) staff       (20)     2976 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/icons/font/taxonomy.woff2
--rw-r--r--   0 ericof     (501) staff       (20)     3009 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/indexer.py
--rw-r--r--   0 ericof     (501) staff       (20)     4081 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/interfaces.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.699186 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/
--rw-r--r--   0 ericof     (501) staff       (20)      416 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/.babelrc
--rw-r--r--   0 ericof     (501) staff       (20)       91 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/.eslintignore
--rw-r--r--   0 ericof     (501) staff       (20)      824 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/.eslintrc
--rw-r--r--   0 ericof     (501) staff       (20)       36 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/.gitignore
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.699956 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/build/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/build/.gitkeep
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.700082 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/build/css/
--rw-r--r--   0 ericof     (501) staff       (20)      681 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/build/css/react-treeview.css
--rw-r--r--   0 ericof     (501) staff       (20)   486420 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/build/edittaxonomydata.js
--rw-r--r--   0 ericof     (501) staff       (20)      260 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/build/edittaxonomydata.js.map
--rw-r--r--   0 ericof     (501) staff       (20)      787 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/index.html
--rw-r--r--   0 ericof     (501) staff       (20)     2511 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/package.json
--rw-r--r--   0 ericof     (501) staff       (20)      596 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/server.js
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.682374 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.700794 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/
--rw-r--r--   0 ericof     (501) staff       (20)     1385 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/actions.js
--rw-r--r--   0 ericof     (501) staff       (20)     1820 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/api.js
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.703528 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/
--rw-r--r--   0 ericof     (501) staff       (20)      861 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/AddNodeButton.js
--rw-r--r--   0 ericof     (501) staff       (20)     3333 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/App.js
--rw-r--r--   0 ericof     (501) staff       (20)     1442 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/EditableId.js
--rw-r--r--   0 ericof     (501) staff       (20)      831 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/EditableIds.js
--rw-r--r--   0 ericof     (501) staff       (20)     1056 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/EditableTree.js
--rw-r--r--   0 ericof     (501) staff       (20)     1340 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/EditableValue.js
--rw-r--r--   0 ericof     (501) staff       (20)      628 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/EditableValues.js
--rw-r--r--   0 ericof     (501) staff       (20)     1686 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/FormControls.js
--rw-r--r--   0 ericof     (501) staff       (20)      674 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/HideTreeCheckbox.js
--rw-r--r--   0 ericof     (501) staff       (20)      822 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/InputText.js
--rw-r--r--   0 ericof     (501) staff       (20)      838 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/LanguageSelector.js
--rw-r--r--   0 ericof     (501) staff       (20)     1940 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/Leaf.js
--rw-r--r--   0 ericof     (501) staff       (20)      821 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/MoveDownButton.js
--rw-r--r--   0 ericof     (501) staff       (20)      797 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/MoveUpButton.js
--rw-r--r--   0 ericof     (501) staff       (20)     1838 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/Node.js
--rw-r--r--   0 ericof     (501) staff       (20)      947 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/ReadOnlySubTree.js
--rw-r--r--   0 ericof     (501) staff       (20)      846 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/RemoveNodeButton.js
--rw-r--r--   0 ericof     (501) staff       (20)      947 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/SubTree.js
--rw-r--r--   0 ericof     (501) staff       (20)     1195 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/TaxonomyTree.js
--rw-r--r--   0 ericof     (501) staff       (20)      608 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/Tree.js
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.704016 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/common/
--rw-r--r--   0 ericof     (501) staff       (20)      483 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/common/Button.js
--rw-r--r--   0 ericof     (501) staff       (20)      398 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/common/MessageBox.js
--rw-r--r--   0 ericof     (501) staff       (20)      271 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/common/Spinner.js
--rw-r--r--   0 ericof     (501) staff       (20)      531 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/constants.js
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.705997 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/
--rw-r--r--   0 ericof     (501) staff       (20)      443 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/AddNodeButton.js
--rw-r--r--   0 ericof     (501) staff       (20)      420 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/App.js
--rw-r--r--   0 ericof     (501) staff       (20)      367 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/DevTools.js
--rw-r--r--   0 ericof     (501) staff       (20)      334 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/EditableId.js
--rw-r--r--   0 ericof     (501) staff       (20)      242 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/EditableIds.js
--rw-r--r--   0 ericof     (501) staff       (20)      345 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/EditableValue.js
--rw-r--r--   0 ericof     (501) staff       (20)      251 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/EditableValues.js
--rw-r--r--   0 ericof     (501) staff       (20)      334 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/LanguageSelector.js
--rw-r--r--   0 ericof     (501) staff       (20)      222 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/MoveDownButton.js
--rw-r--r--   0 ericof     (501) staff       (20)      212 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/MoveUpButton.js
--rw-r--r--   0 ericof     (501) staff       (20)      205 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/ReadOnlySubTree.js
--rw-r--r--   0 ericof     (501) staff       (20)      209 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/RemoveNodeButton.js
--rw-r--r--   0 ericof     (501) staff       (20)      393 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/SubTree.js
--rw-r--r--   0 ericof     (501) staff       (20)      383 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/containers/Tree.js
--rw-r--r--   0 ericof     (501) staff       (20)      618 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/i18n.js
--rw-r--r--   0 ericof     (501) staff       (20)     1630 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/index.js
--rw-r--r--   0 ericof     (501) staff       (20)     4338 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/reducers.js
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.706514 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/store/
--rw-r--r--   0 ericof     (501) staff       (20)      649 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/store/configureStore.dev.js
--rw-r--r--   0 ericof     (501) staff       (20)      256 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/store/configureStore.js
--rw-r--r--   0 ericof     (501) staff       (20)      291 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/store/configureStore.prod.js
--rw-r--r--   0 ericof     (501) staff       (20)      171 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/store/middlewares.js
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.707018 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/translations/
--rw-r--r--   0 ericof     (501) staff       (20)      639 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/translations/es.js
--rw-r--r--   0 ericof     (501) staff       (20)      691 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/translations/fr.js
--rw-r--r--   0 ericof     (501) staff       (20)      143 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/translations/index.js
--rw-r--r--   0 ericof     (501) staff       (20)      617 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/translations/nl.js
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.707402 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/test/
--rw-r--r--   0 ericof     (501) staff       (20)     1305 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/test/actions.spec.js
--rw-r--r--   0 ericof     (501) staff       (20)     1739 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/test/reducers.spec.js
--rw-r--r--   0 ericof     (501) staff       (20)      326 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/test/setup.js
--rw-r--r--   0 ericof     (501) staff       (20)      893 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/webpack.config.js
--rw-r--r--   0 ericof     (501) staff       (20)      935 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/webpack.config.prod.js
--rw-r--r--   0 ericof     (501) staff       (20)   264054 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/yarn.lock
--rw-r--r--   0 ericof     (501) staff       (20)     5648 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/jsonimpl.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.707528 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/
--rw-r--r--   0 ericof     (501) staff       (20)     3858 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/collective.taxonomy.pot
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.682584 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/da/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.707653 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/da/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)     3924 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/da/LC_MESSAGES/collective.taxonomy.po
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.682720 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/de/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.707783 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/de/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)     4601 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/de/LC_MESSAGES/collective.taxonomy.po
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.682859 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/es/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.707904 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/es/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)     5434 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/es/LC_MESSAGES/collective.taxonomy.po
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.682990 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/fr/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.708032 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/fr/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)     4757 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/fr/LC_MESSAGES/collective.taxonomy.po
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.683121 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/nl/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.708153 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/nl/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)     4722 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/locales/nl/LC_MESSAGES/collective.taxonomy.po
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.683488 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.708810 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/default/
--rw-r--r--   0 ericof     (501) staff       (20)      154 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/default/browserlayer.xml
--rw-r--r--   0 ericof     (501) staff       (20)      562 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/default/controlpanel.xml
--rw-r--r--   0 ericof     (501) staff       (20)       81 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/default/metadata.xml
--rw-r--r--   0 ericof     (501) staff       (20)      150 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/default/registry.xml
--rw-r--r--   0 ericof     (501) staff       (20)      220 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/default/rolemap.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.708930 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/examples/
--rw-r--r--   0 ericof     (501) staff       (20)      185 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/examples/metadata.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.709176 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/examples/taxonomies/
--rw-r--r--   0 ericof     (501) staff       (20)      170 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/examples/taxonomies/nihms.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     1755 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/examples/taxonomies/nihms.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.709540 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/uninstall/
--rw-r--r--   0 ericof     (501) staff       (20)      151 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 ericof     (501) staff       (20)      232 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 ericof     (501) staff       (20)      134 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/uninstall/registry.xml
--rwxr-xr-x   0 ericof     (501) staff       (20)     1207 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/rebuild_i18n.sh
--rw-r--r--   0 ericof     (501) staff       (20)      609 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/setuphandlers.py
--rw-r--r--   0 ericof     (501) staff       (20)     1494 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/testing.py
--rw-r--r--   0 ericof     (501) staff       (20)      524 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/testing.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.710632 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.710776 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/robot/
--rw-r--r--   0 ericof     (501) staff       (20)     3303 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/robot/todo_test_taxonomy.robot
--rw-r--r--   0 ericof     (501) staff       (20)     2770 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_behavior.py
--rw-r--r--   0 ericof     (501) staff       (20)     2923 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_controlpanel.py
--rw-r--r--   0 ericof     (501) staff       (20)     4839 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_indexer.py
--rw-r--r--   0 ericof     (501) staff       (20)     6421 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_json.py
--rw-r--r--   0 ericof     (501) staff       (20)      757 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_robot.py
--rw-r--r--   0 ericof     (501) staff       (20)     2733 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_setup.py
--rw-r--r--   0 ericof     (501) staff       (20)      862 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_traverser.py
--rw-r--r--   0 ericof     (501) staff       (20)      582 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_utility.py
--rw-r--r--   0 ericof     (501) staff       (20)     2024 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/upgradesteps.py
--rw-r--r--   0 ericof     (501) staff       (20)     1372 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/upgradesteps.zcml
--rw-r--r--   0 ericof     (501) staff       (20)    10621 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/utility.py
--rw-r--r--   0 ericof     (501) staff       (20)     6317 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/vdex.py
--rw-r--r--   0 ericof     (501) staff       (20)     6162 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/vocabulary.py
--rw-r--r--   0 ericof     (501) staff       (20)     1703 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/widget.py
--rw-r--r--   0 ericof     (501) staff       (20)      673 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/widget.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1032 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/widget_display.pt
--rw-r--r--   0 ericof     (501) staff       (20)     8275 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective/taxonomy/widget_input.pt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-02 11:59:30.692481 collective.taxonomy-3.0.1/src/collective.taxonomy.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)    18989 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective.taxonomy.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     9130 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective.taxonomy.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective.taxonomy.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)       40 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective.taxonomy.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)       11 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective.taxonomy.egg-info/namespace_packages.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective.taxonomy.egg-info/not-zip-safe
--rw-r--r--   0 ericof     (501) staff       (20)      228 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective.taxonomy.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)       11 2023-02-02 11:59:30.000000 collective.taxonomy-3.0.1/src/collective.taxonomy.egg-info/top_level.txt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.057200 collective.taxonomy-3.1/
+-rw-r--r--   0 peterm     (501) staff       (20)      148 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/.coveragerc
+-rw-r--r--   0 peterm     (501) staff       (20)     8637 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/CHANGES.rst
+-rw-r--r--   0 peterm     (501) staff       (20)      619 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/MANIFEST.in
+-rw-r--r--   0 peterm     (501) staff       (20)    11517 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/Makefile
+-rw-r--r--   0 peterm     (501) staff       (20)    20513 2023-05-26 12:19:29.057347 collective.taxonomy-3.1/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)    10918 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/README.rst
+-rw-r--r--   0 peterm     (501) staff       (20)       58 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/constraints.txt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:28.999896 collective.taxonomy-3.1/docs/
+-rw-r--r--   0 peterm     (501) staff       (20)       28 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/105.bugfix
+-rw-r--r--   0 peterm     (501) staff       (20)       47 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/116.bugfix
+-rw-r--r--   0 peterm     (501) staff       (20)    18092 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/LICENSE.GPL
+-rw-r--r--   0 peterm     (501) staff       (20)      726 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/LICENSE.rst
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.009352 collective.taxonomy-3.1/docs/img/
+-rw-r--r--   0 peterm     (501) staff       (20)    84621 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/add-portfolio-view-001.png
+-rw-r--r--   0 peterm     (501) staff       (20)   131192 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/add-portfolio-view-002.png
+-rw-r--r--   0 peterm     (501) staff       (20)   238942 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/add-portfolio-view-003.png
+-rw-r--r--   0 peterm     (501) staff       (20)   410063 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/add-portfolio-view-004.png
+-rw-r--r--   0 peterm     (501) staff       (20)    84604 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/add-taxonomy-001.png
+-rw-r--r--   0 peterm     (501) staff       (20)    89941 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/add-taxonomy-002.png
+-rw-r--r--   0 peterm     (501) staff       (20)    89267 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/add-taxonomy-003.png
+-rw-r--r--   0 peterm     (501) staff       (20)    92683 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/add-taxonomy-004.png
+-rw-r--r--   0 peterm     (501) staff       (20)   125750 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/create-portfolio-data-001.png
+-rw-r--r--   0 peterm     (501) staff       (20)    58306 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/create-portfolio-data-002.png
+-rw-r--r--   0 peterm     (501) staff       (20)    96146 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/create-portfolio-data-003.png
+-rw-r--r--   0 peterm     (501) staff       (20)   100598 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/create-portfolio-data-004.png
+-rw-r--r--   0 peterm     (501) staff       (20)    76273 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/create-portfolio-data-005.png
+-rw-r--r--   0 peterm     (501) staff       (20)    70538 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/create-portfolio-data-006.png
+-rw-r--r--   0 peterm     (501) staff       (20)   100654 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/edit-taxonomy-data-001.png
+-rw-r--r--   0 peterm     (501) staff       (20)    96150 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/edit-taxonomy-data-002.png
+-rw-r--r--   0 peterm     (501) staff       (20)   140964 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/edit-taxonomy-data-003.png
+-rw-r--r--   0 peterm     (501) staff       (20)   103935 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/edit-taxonomy-data-004.png
+-rw-r--r--   0 peterm     (501) staff       (20)    66228 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/enable-behavior-001.png
+-rw-r--r--   0 peterm     (501) staff       (20)    97900 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/enable-behavior-002.png
+-rw-r--r--   0 peterm     (501) staff       (20)    91223 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/enable-behavior-003.png
+-rw-r--r--   0 peterm     (501) staff       (20)    95399 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/enable-behavior-004.png
+-rw-r--r--   0 peterm     (501) staff       (20)    78953 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/enable-behavior-005.png
+-rw-r--r--   0 peterm     (501) staff       (20)   182658 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/img/video-generated-by-test.gif
+-rw-r--r--   0 peterm     (501) staff       (20)     8276 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/docs/tutorial.md
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.009812 collective.taxonomy-3.1/images/
+-rw-r--r--   0 peterm     (501) staff       (20)   178318 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/images/edit_taxonomy_data.gif
+-rw-r--r--   0 peterm     (501) staff       (20)      459 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/instance.yaml
+-rw-r--r--   0 peterm     (501) staff       (20)      821 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/mx.ini
+-rw-r--r--   0 peterm     (501) staff       (20)      148 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/pyproject.toml
+-rw-r--r--   0 peterm     (501) staff       (20)      186 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/requirements.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      336 2023-05-26 12:19:29.057827 collective.taxonomy-3.1/setup.cfg
+-rw-r--r--   0 peterm     (501) staff       (20)     2119 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/setup.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:28.989897 collective.taxonomy-3.1/src/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.010251 collective.taxonomy-3.1/src/collective/
+-rw-r--r--   0 peterm     (501) staff       (20)      169 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.020120 collective.taxonomy-3.1/src/collective/taxonomy/
+-rw-r--r--   0 peterm     (501) staff       (20)      125 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     8384 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/behavior.py
+-rw-r--r--   0 peterm     (501) staff       (20)     5750 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/browser.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1983 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/collectionfilter.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2817 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/collective.taxonomy.css
+-rw-r--r--   0 peterm     (501) staff       (20)     5090 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)    11808 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/controlpanel.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1167 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/edit_taxonomy_data.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     4862 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/exportimport.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1218 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/factory.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1771 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/generated.py
+-rw-r--r--   0 peterm     (501) staff       (20)      152 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/i18n.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.021131 collective.taxonomy-3.1/src/collective/taxonomy/icons/
+-rw-r--r--   0 peterm     (501) staff       (20)      355 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/LICENSE.txt
+-rw-r--r--   0 peterm     (501) staff       (20)     2877 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/README.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      943 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/config.json
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.022669 collective.taxonomy-3.1/src/collective/taxonomy/icons/css/
+-rw-r--r--   0 peterm     (501) staff       (20)     1857 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/css/animation.css
+-rw-r--r--   0 peterm     (501) staff       (20)      373 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/css/taxonomy-codes.css
+-rw-r--r--   0 peterm     (501) staff       (20)    14717 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/css/taxonomy-embedded.css
+-rw-r--r--   0 peterm     (501) staff       (20)      679 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/css/taxonomy-ie7-codes.css
+-rw-r--r--   0 peterm     (501) staff       (20)      948 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/css/taxonomy-ie7.css
+-rw-r--r--   0 peterm     (501) staff       (20)     2122 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/css/taxonomy.css
+-rw-r--r--   0 peterm     (501) staff       (20)     6951 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/demo.html
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.023982 collective.taxonomy-3.1/src/collective/taxonomy/icons/font/
+-rw-r--r--   0 peterm     (501) staff       (20)     6120 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/font/taxonomy.eot
+-rw-r--r--   0 peterm     (501) staff       (20)     2284 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/font/taxonomy.svg
+-rw-r--r--   0 peterm     (501) staff       (20)     5952 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/font/taxonomy.ttf
+-rw-r--r--   0 peterm     (501) staff       (20)     3588 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/font/taxonomy.woff
+-rw-r--r--   0 peterm     (501) staff       (20)     2976 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/icons/font/taxonomy.woff2
+-rw-r--r--   0 peterm     (501) staff       (20)     3001 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/indexer.py
+-rw-r--r--   0 peterm     (501) staff       (20)     4223 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/interfaces.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.026502 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/
+-rw-r--r--   0 peterm     (501) staff       (20)      416 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/.babelrc
+-rw-r--r--   0 peterm     (501) staff       (20)       91 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/.eslintignore
+-rw-r--r--   0 peterm     (501) staff       (20)      824 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/.eslintrc
+-rw-r--r--   0 peterm     (501) staff       (20)       36 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/.gitignore
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.028172 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/build/
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/build/.gitkeep
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.028525 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/build/css/
+-rw-r--r--   0 peterm     (501) staff       (20)      681 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/build/css/react-treeview.css
+-rw-r--r--   0 peterm     (501) staff       (20)   486420 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/build/edittaxonomydata.js
+-rw-r--r--   0 peterm     (501) staff       (20)      260 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/build/edittaxonomydata.js.map
+-rw-r--r--   0 peterm     (501) staff       (20)      787 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/index.html
+-rw-r--r--   0 peterm     (501) staff       (20)     2511 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/package.json
+-rw-r--r--   0 peterm     (501) staff       (20)      596 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/server.js
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:28.992033 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.030090 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/
+-rw-r--r--   0 peterm     (501) staff       (20)     1385 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/actions.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1820 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/api.js
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.035530 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/
+-rw-r--r--   0 peterm     (501) staff       (20)      861 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/AddNodeButton.js
+-rw-r--r--   0 peterm     (501) staff       (20)     3333 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/App.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1442 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/EditableId.js
+-rw-r--r--   0 peterm     (501) staff       (20)      831 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/EditableIds.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1056 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/EditableTree.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1340 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/EditableValue.js
+-rw-r--r--   0 peterm     (501) staff       (20)      628 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/EditableValues.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1686 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/FormControls.js
+-rw-r--r--   0 peterm     (501) staff       (20)      674 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/HideTreeCheckbox.js
+-rw-r--r--   0 peterm     (501) staff       (20)      822 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/InputText.js
+-rw-r--r--   0 peterm     (501) staff       (20)      838 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/LanguageSelector.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1940 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/Leaf.js
+-rw-r--r--   0 peterm     (501) staff       (20)      821 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/MoveDownButton.js
+-rw-r--r--   0 peterm     (501) staff       (20)      797 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/MoveUpButton.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1838 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/Node.js
+-rw-r--r--   0 peterm     (501) staff       (20)      947 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/ReadOnlySubTree.js
+-rw-r--r--   0 peterm     (501) staff       (20)      846 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/RemoveNodeButton.js
+-rw-r--r--   0 peterm     (501) staff       (20)      947 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/SubTree.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1195 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/TaxonomyTree.js
+-rw-r--r--   0 peterm     (501) staff       (20)      608 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/Tree.js
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.036350 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/common/
+-rw-r--r--   0 peterm     (501) staff       (20)      483 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/common/Button.js
+-rw-r--r--   0 peterm     (501) staff       (20)      398 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/common/MessageBox.js
+-rw-r--r--   0 peterm     (501) staff       (20)      271 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/common/Spinner.js
+-rw-r--r--   0 peterm     (501) staff       (20)      531 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/constants.js
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.040084 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/
+-rw-r--r--   0 peterm     (501) staff       (20)      443 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/AddNodeButton.js
+-rw-r--r--   0 peterm     (501) staff       (20)      420 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/App.js
+-rw-r--r--   0 peterm     (501) staff       (20)      367 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/DevTools.js
+-rw-r--r--   0 peterm     (501) staff       (20)      334 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/EditableId.js
+-rw-r--r--   0 peterm     (501) staff       (20)      242 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/EditableIds.js
+-rw-r--r--   0 peterm     (501) staff       (20)      345 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/EditableValue.js
+-rw-r--r--   0 peterm     (501) staff       (20)      251 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/EditableValues.js
+-rw-r--r--   0 peterm     (501) staff       (20)      334 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/LanguageSelector.js
+-rw-r--r--   0 peterm     (501) staff       (20)      222 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/MoveDownButton.js
+-rw-r--r--   0 peterm     (501) staff       (20)      212 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/MoveUpButton.js
+-rw-r--r--   0 peterm     (501) staff       (20)      205 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/ReadOnlySubTree.js
+-rw-r--r--   0 peterm     (501) staff       (20)      209 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/RemoveNodeButton.js
+-rw-r--r--   0 peterm     (501) staff       (20)      393 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/SubTree.js
+-rw-r--r--   0 peterm     (501) staff       (20)      383 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/containers/Tree.js
+-rw-r--r--   0 peterm     (501) staff       (20)      618 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/i18n.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1630 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/index.js
+-rw-r--r--   0 peterm     (501) staff       (20)     4338 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/reducers.js
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.041242 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/store/
+-rw-r--r--   0 peterm     (501) staff       (20)      649 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/store/configureStore.dev.js
+-rw-r--r--   0 peterm     (501) staff       (20)      256 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/store/configureStore.js
+-rw-r--r--   0 peterm     (501) staff       (20)      291 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/store/configureStore.prod.js
+-rw-r--r--   0 peterm     (501) staff       (20)      171 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/store/middlewares.js
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.042402 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/translations/
+-rw-r--r--   0 peterm     (501) staff       (20)      639 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/translations/es.js
+-rw-r--r--   0 peterm     (501) staff       (20)      691 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/translations/fr.js
+-rw-r--r--   0 peterm     (501) staff       (20)      143 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/translations/index.js
+-rw-r--r--   0 peterm     (501) staff       (20)      617 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/translations/nl.js
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.043388 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/test/
+-rw-r--r--   0 peterm     (501) staff       (20)     1305 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/test/actions.spec.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1739 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/test/reducers.spec.js
+-rw-r--r--   0 peterm     (501) staff       (20)      326 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/test/setup.js
+-rw-r--r--   0 peterm     (501) staff       (20)      893 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/webpack.config.js
+-rw-r--r--   0 peterm     (501) staff       (20)      935 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/webpack.config.prod.js
+-rw-r--r--   0 peterm     (501) staff       (20)   264054 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/javascripts/yarn.lock
+-rw-r--r--   0 peterm     (501) staff       (20)     5648 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/jsonimpl.py
+-rw-r--r--   0 peterm     (501) staff       (20)     5520 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/listing_tabular.pt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.043654 collective.taxonomy-3.1/src/collective/taxonomy/locales/
+-rw-r--r--   0 peterm     (501) staff       (20)     3858 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/locales/collective.taxonomy.pot
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:28.992426 collective.taxonomy-3.1/src/collective/taxonomy/locales/da/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.044266 collective.taxonomy-3.1/src/collective/taxonomy/locales/da/LC_MESSAGES/
+-rw-r--r--   0 peterm     (501) staff       (20)      973 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/locales/da/LC_MESSAGES/collective.taxonomy.mo
+-rw-r--r--   0 peterm     (501) staff       (20)     3924 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/locales/da/LC_MESSAGES/collective.taxonomy.po
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:28.992668 collective.taxonomy-3.1/src/collective/taxonomy/locales/de/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.044796 collective.taxonomy-3.1/src/collective/taxonomy/locales/de/LC_MESSAGES/
+-rw-r--r--   0 peterm     (501) staff       (20)     2671 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/locales/de/LC_MESSAGES/collective.taxonomy.mo
+-rw-r--r--   0 peterm     (501) staff       (20)     4601 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/locales/de/LC_MESSAGES/collective.taxonomy.po
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:28.992919 collective.taxonomy-3.1/src/collective/taxonomy/locales/es/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.045329 collective.taxonomy-3.1/src/collective/taxonomy/locales/es/LC_MESSAGES/
+-rw-r--r--   0 peterm     (501) staff       (20)     3926 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/locales/es/LC_MESSAGES/collective.taxonomy.mo
+-rw-r--r--   0 peterm     (501) staff       (20)     5434 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/locales/es/LC_MESSAGES/collective.taxonomy.po
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:28.993285 collective.taxonomy-3.1/src/collective/taxonomy/locales/fr/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.045861 collective.taxonomy-3.1/src/collective/taxonomy/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 peterm     (501) staff       (20)     2890 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/locales/fr/LC_MESSAGES/collective.taxonomy.mo
+-rw-r--r--   0 peterm     (501) staff       (20)     4757 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/locales/fr/LC_MESSAGES/collective.taxonomy.po
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:28.993544 collective.taxonomy-3.1/src/collective/taxonomy/locales/nl/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.046377 collective.taxonomy-3.1/src/collective/taxonomy/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 peterm     (501) staff       (20)     3176 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/locales/nl/LC_MESSAGES/collective.taxonomy.mo
+-rw-r--r--   0 peterm     (501) staff       (20)     4722 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/locales/nl/LC_MESSAGES/collective.taxonomy.po
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:28.994245 collective.taxonomy-3.1/src/collective/taxonomy/profiles/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.047654 collective.taxonomy-3.1/src/collective/taxonomy/profiles/default/
+-rw-r--r--   0 peterm     (501) staff       (20)      165 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/profiles/default/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      617 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/profiles/default/controlpanel.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      121 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/profiles/default/metadata.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      170 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/profiles/default/registry.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      260 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/profiles/default/rolemap.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.047925 collective.taxonomy-3.1/src/collective/taxonomy/profiles/examples/
+-rw-r--r--   0 peterm     (501) staff       (20)      230 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/profiles/examples/metadata.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.048452 collective.taxonomy-3.1/src/collective/taxonomy/profiles/examples/taxonomies/
+-rw-r--r--   0 peterm     (501) staff       (20)      170 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/profiles/examples/taxonomies/nihms.cfg
+-rw-r--r--   0 peterm     (501) staff       (20)     1786 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/profiles/examples/taxonomies/nihms.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.049248 collective.taxonomy-3.1/src/collective/taxonomy/profiles/uninstall/
+-rw-r--r--   0 peterm     (501) staff       (20)      188 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      261 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      164 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/profiles/uninstall/registry.xml
+-rwxr-xr-x   0 peterm     (501) staff       (20)     1207 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/rebuild_i18n.sh
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.050016 collective.taxonomy-3.1/src/collective/taxonomy/restapi/
+-rw-r--r--   0 peterm     (501) staff       (20)       24 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)      286 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/configure.zcml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.050788 collective.taxonomy-3.1/src/collective/taxonomy/restapi/serializers/
+-rw-r--r--   0 peterm     (501) staff       (20)       24 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/serializers/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)      181 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/serializers/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1557 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/serializers/taxonomy.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.051282 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/
+-rw-r--r--   0 peterm     (501) staff       (20)       24 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)      200 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/configure.zcml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.052063 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/controlpanel/
+-rw-r--r--   0 peterm     (501) staff       (20)       24 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/controlpanel/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)      325 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/controlpanel/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1136 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/controlpanel/controlpanel.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.053960 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/taxonomy/
+-rw-r--r--   0 peterm     (501) staff       (20)       24 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/taxonomy/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     3562 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/taxonomy/add.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1203 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/taxonomy/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1681 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/taxonomy/delete.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2833 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/taxonomy/get.py
+-rw-r--r--   0 peterm     (501) staff       (20)      848 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/taxonomy/schema.py
+-rw-r--r--   0 peterm     (501) staff       (20)     3584 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/services/taxonomy/update.py
+-rw-r--r--   0 peterm     (501) staff       (20)      840 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/restapi/utils.py
+-rw-r--r--   0 peterm     (501) staff       (20)      609 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/setuphandlers.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1554 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/testing.py
+-rw-r--r--   0 peterm     (501) staff       (20)      526 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/testing.zcml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.056733 collective.taxonomy-3.1/src/collective/taxonomy/tests/
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.056984 collective.taxonomy-3.1/src/collective/taxonomy/tests/robot/
+-rw-r--r--   0 peterm     (501) staff       (20)     3303 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/robot/todo_test_taxonomy.robot
+-rw-r--r--   0 peterm     (501) staff       (20)     2769 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/test_behavior.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2923 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/test_controlpanel.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2048 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/test_controlpanel_restapi.py
+-rw-r--r--   0 peterm     (501) staff       (20)     6373 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/test_indexer.py
+-rw-r--r--   0 peterm     (501) staff       (20)     6421 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/test_json.py
+-rw-r--r--   0 peterm     (501) staff       (20)      757 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/test_robot.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2732 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/test_setup.py
+-rw-r--r--   0 peterm     (501) staff       (20)     6092 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/test_taxonomy_endpoint.py
+-rw-r--r--   0 peterm     (501) staff       (20)      862 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/test_traverser.py
+-rw-r--r--   0 peterm     (501) staff       (20)      582 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/tests/test_utility.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2020 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/upgradesteps.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1430 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/upgradesteps.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)    10611 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/utility.py
+-rw-r--r--   0 peterm     (501) staff       (20)     6315 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/vdex.py
+-rw-r--r--   0 peterm     (501) staff       (20)     6160 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/vocabulary.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1703 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/widget.py
+-rw-r--r--   0 peterm     (501) staff       (20)      679 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/widget.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1032 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/widget_display.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     8275 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective/taxonomy/widget_input.pt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-26 12:19:29.012435 collective.taxonomy-3.1/src/collective.taxonomy.egg-info/
+-rw-r--r--   0 peterm     (501) staff       (20)    20513 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective.taxonomy.egg-info/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)    10676 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective.taxonomy.egg-info/SOURCES.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective.taxonomy.egg-info/dependency_links.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       40 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective.taxonomy.egg-info/entry_points.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       11 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective.taxonomy.egg-info/namespace_packages.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective.taxonomy.egg-info/not-zip-safe
+-rw-r--r--   0 peterm     (501) staff       (20)      280 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective.taxonomy.egg-info/requires.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       11 2023-05-26 12:19:28.000000 collective.taxonomy-3.1/src/collective.taxonomy.egg-info/top_level.txt
```

### Comparing `collective.taxonomy-3.0.1/CHANGES.rst` & `collective.taxonomy-3.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 =======
 
+3.1 (2023-05-26)
+----------------
+
+- Integrate taxonomies into Collection tabular view, display values are now resolved
+  [MrTango]
+- Restapi endpoints support [cekk, nileshgulia1]
+
+
 3.0.1 (2023-02-02)
 ------------------
 
 - export/import of field_prefix value.
   [eikichi18]
```

### Comparing `collective.taxonomy-3.0.1/MANIFEST.in` & `collective.taxonomy-3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/Makefile` & `collective.taxonomy-3.1/Makefile`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/PKG-INFO` & `collective.taxonomy-3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.taxonomy
-Version: 3.0.1
+Version: 3.1
 Summary: Create, edit and use hierarchical taxonomies in Plone!
 Home-page: https://pypi.org/project/collective.taxonomy/
 Author: Bo Simonsen and Malthe Borch
 Author-email: bo@headnet.dk
 License: GPLv2+
 Keywords: plone taxonomy dexterity
 Classifier: Development Status :: 6 - Mature
@@ -221,14 +221,36 @@
         fr
     }
 
 You'll have to rebuild the js bundle: ``npm run build``
 
 That's it!
 
+Restapi support
+---------------
+
+This package also supports endpoints for basic CRUD operations that can be consumend by any frontend service.
+
+The API consumer can create, read, and delete taxonomies.
+
++----------+---------------------+----------------------------------------+
+| Verb     | URL                 | Action                                 |
++==========+=====================+========================================+
+| `POST`   | `/@taxonomy`        | Add taxonomy with specific data        |
++----------+---------------------+----------------------------------------+
+| `GET`    | `/@taxonomy`        | List all taxonomies                    |
++----------+---------------------+----------------------------------------+
+| `GET`    | `/@taxonomy/{name}` | Get taxonomy data                      |
++----------+---------------------+----------------------------------------+
+| `DELETE` | `/@taxonomy/{name}` | Remove one or more taxonomies          |
++----------+---------------------+----------------------------------------+
+| `PATCH`  | `/@taxonomy/{name}` | Update taxonomy data                   |
++----------+---------------------+----------------------------------------+
+| `GET`    | `/@taxonomySchema`  | Get current taxonomy schema            |
++----------+---------------------+----------------------------------------+
 
 Translations
 ------------
 
 This product has been translated into
 
 - Danish.
@@ -341,14 +363,22 @@
 
 .. _Plone: https://plone.org/
 .. _`opening a ticket`: https://github.com/collective/collective.taxonomy/issues
 
 Changes
 =======
 
+3.1 (2023-05-26)
+----------------
+
+- Integrate taxonomies into Collection tabular view, display values are now resolved
+  [MrTango]
+- Restapi endpoints support [cekk, nileshgulia1]
+
+
 3.0.1 (2023-02-02)
 ------------------
 
 - export/import of field_prefix value.
   [eikichi18]
```

### Comparing `collective.taxonomy-3.0.1/README.rst` & `collective.taxonomy-3.1/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -195,14 +195,36 @@
         fr
     }
 
 You'll have to rebuild the js bundle: ``npm run build``
 
 That's it!
 
+Restapi support
+---------------
+
+This package also supports endpoints for basic CRUD operations that can be consumend by any frontend service.
+
+The API consumer can create, read, and delete taxonomies.
+
++----------+---------------------+----------------------------------------+
+| Verb     | URL                 | Action                                 |
++==========+=====================+========================================+
+| `POST`   | `/@taxonomy`        | Add taxonomy with specific data        |
++----------+---------------------+----------------------------------------+
+| `GET`    | `/@taxonomy`        | List all taxonomies                    |
++----------+---------------------+----------------------------------------+
+| `GET`    | `/@taxonomy/{name}` | Get taxonomy data                      |
++----------+---------------------+----------------------------------------+
+| `DELETE` | `/@taxonomy/{name}` | Remove one or more taxonomies          |
++----------+---------------------+----------------------------------------+
+| `PATCH`  | `/@taxonomy/{name}` | Update taxonomy data                   |
++----------+---------------------+----------------------------------------+
+| `GET`    | `/@taxonomySchema`  | Get current taxonomy schema            |
++----------+---------------------+----------------------------------------+
 
 Translations
 ------------
 
 This product has been translated into
 
 - Danish.
```

### Comparing `collective.taxonomy-3.0.1/docs/LICENSE.GPL` & `collective.taxonomy-3.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/LICENSE.rst` & `collective.taxonomy-3.1/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/add-portfolio-view-001.png` & `collective.taxonomy-3.1/docs/img/add-portfolio-view-001.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/add-portfolio-view-002.png` & `collective.taxonomy-3.1/docs/img/add-portfolio-view-002.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/add-portfolio-view-003.png` & `collective.taxonomy-3.1/docs/img/add-portfolio-view-003.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/add-portfolio-view-004.png` & `collective.taxonomy-3.1/docs/img/add-portfolio-view-004.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/add-taxonomy-001.png` & `collective.taxonomy-3.1/docs/img/add-taxonomy-001.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/add-taxonomy-002.png` & `collective.taxonomy-3.1/docs/img/add-taxonomy-002.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/add-taxonomy-003.png` & `collective.taxonomy-3.1/docs/img/add-taxonomy-003.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/add-taxonomy-004.png` & `collective.taxonomy-3.1/docs/img/add-taxonomy-004.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/create-portfolio-data-001.png` & `collective.taxonomy-3.1/docs/img/create-portfolio-data-001.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/create-portfolio-data-002.png` & `collective.taxonomy-3.1/docs/img/create-portfolio-data-002.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/create-portfolio-data-003.png` & `collective.taxonomy-3.1/docs/img/create-portfolio-data-003.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/create-portfolio-data-004.png` & `collective.taxonomy-3.1/docs/img/create-portfolio-data-004.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/create-portfolio-data-005.png` & `collective.taxonomy-3.1/docs/img/create-portfolio-data-005.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/create-portfolio-data-006.png` & `collective.taxonomy-3.1/docs/img/create-portfolio-data-006.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/edit-taxonomy-data-001.png` & `collective.taxonomy-3.1/docs/img/edit-taxonomy-data-001.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/edit-taxonomy-data-002.png` & `collective.taxonomy-3.1/docs/img/edit-taxonomy-data-002.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/edit-taxonomy-data-003.png` & `collective.taxonomy-3.1/docs/img/edit-taxonomy-data-003.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/edit-taxonomy-data-004.png` & `collective.taxonomy-3.1/docs/img/edit-taxonomy-data-004.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/enable-behavior-001.png` & `collective.taxonomy-3.1/docs/img/enable-behavior-001.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/enable-behavior-002.png` & `collective.taxonomy-3.1/docs/img/enable-behavior-002.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/enable-behavior-003.png` & `collective.taxonomy-3.1/docs/img/enable-behavior-003.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/enable-behavior-004.png` & `collective.taxonomy-3.1/docs/img/enable-behavior-004.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/enable-behavior-005.png` & `collective.taxonomy-3.1/docs/img/enable-behavior-005.png`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/img/video-generated-by-test.gif` & `collective.taxonomy-3.1/docs/img/video-generated-by-test.gif`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/docs/tutorial.md` & `collective.taxonomy-3.1/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/images/edit_taxonomy_data.gif` & `collective.taxonomy-3.1/images/edit_taxonomy_data.gif`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/mx.ini` & `collective.taxonomy-3.1/mx.ini`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/setup.py` & `collective.taxonomy-3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import os
 
 from setuptools import find_packages
 from setuptools import setup
 
-version = '3.0.1'
+version = "3.1"
 
 
 def read(*pathnames):
     with open(os.path.join(os.path.dirname(__file__), *pathnames)) as fh:
         return fh.read()
 
 
 setup(
-    name='collective.taxonomy',
+    name="collective.taxonomy",
     version=version,
     description="Create, edit and use hierarchical taxonomies in Plone!",
-    url='https://pypi.org/project/collective.taxonomy/',
-    long_description='\n'.join([
-        read('README.rst'),
-        read('CHANGES.rst'),
-    ]),
+    url="https://pypi.org/project/collective.taxonomy/",
+    long_description="\n".join(
+        [
+            read("README.rst"),
+            read("CHANGES.rst"),
+        ]
+    ),
     classifiers=[
         "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Addon",
         "Framework :: Zope",
@@ -31,42 +33,45 @@
         "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    keywords='plone taxonomy dexterity',
-    author='Bo Simonsen and Malthe Borch',
-    author_email='bo@headnet.dk',
+    keywords="plone taxonomy dexterity",
+    author="Bo Simonsen and Malthe Borch",
+    author_email="bo@headnet.dk",
     license="GPLv2+",
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
-    namespace_packages=['collective'],
+    packages=find_packages("src"),
+    package_dir={"": "src"},
+    namespace_packages=["collective"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
-        'setuptools',
-        'plone.supermodel',
-        'plone.api >= 1.5',
-        'plone.app.registry',
-        'lxml',
-        'six >= 1.12',
+        "setuptools",
+        "plone.supermodel",
+        "plone.api >= 1.5",
+        "plone.app.registry",
+        "plone.app.dexterity",
+        "plone.synchronize",
+        "lxml",
+        "six >= 1.12",
     ],
     extras_require={
-        'dev': [
-            'zest.releaser[recommended]',
+        "dev": [
+            "zest.releaser[recommended]",
+        ],
+        "test": [
+            "plone.testing",
+            "plone.app.testing",
+            "plone.app.contenttypes",
+            "plone.app.querystring",
+            "plone.app.robotframework[debug]",
+            "plone.restapi"
         ],
-        'test': [
-            'plone.testing',
-            'plone.app.testing',
-            'plone.app.contenttypes',
-            'plone.app.querystring',
-            'plone.app.robotframework[debug]',
-        ]
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     """,
 )
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/behavior.py` & `collective.taxonomy-3.1/src/collective/taxonomy/behavior.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/collectionfilter.py` & `collective.taxonomy-3.1/src/collective/taxonomy/collectionfilter.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/collective.taxonomy.css` & `collective.taxonomy-3.1/src/collective/taxonomy/collective.taxonomy.css`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/configure.zcml` & `collective.taxonomy-3.1/src/collective/taxonomy/configure.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
+    xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:five="http://namespaces.zope.org/five"
-    xmlns:i18n="http://namespaces.zope.org/i18n"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    xmlns:i18n="http://namespaces.zope.org/i18n"
     xmlns:plone="http://namespaces.plone.org/plone"
-    xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:z3c="http://namespaces.zope.org/z3c"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    i18n_domain="collective.taxonomy">
+    i18n_domain="collective.taxonomy"
+    >
 
   <i18n:registerTranslations directory="locales" />
 
   <include package="plone.app.registry" />
+  <include package=".restapi" />
+ 
+
   <include package="plone.supermodel" />
 
-  <permission id="collective.taxonomy.ManageTaxonomies"
-              title="Manage taxonomies" />
+  <permission
+      id="collective.taxonomy.ManageTaxonomies"
+      title="Manage taxonomies"
+      />
 
   <genericsetup:registerProfile
       name="default"
       title="collective.taxonomy"
-      directory="profiles/default"
       description="Registers control panel and default settings."
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/default"
       />
 
   <genericsetup:registerProfile
       name="uninstall"
       title="collective.taxonomy uninstall"
-      directory="profiles/uninstall"
       description="Uninstall profile for collective.taxonomy."
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/uninstall"
       post_handler=".setuphandlers.uninstall"
       />
 
   <genericsetup:importStep
       name="collective.taxonomy"
       title="Manage the taxonomy tool"
       description="Import taxonomies from VDEX-format."
-      handler=".exportimport.importTaxonomy">
-  </genericsetup:importStep>
+      handler=".exportimport.importTaxonomy"
+      >
+</genericsetup:importStep>
 
   <genericsetup:exportStep
       name="collective.taxonomy"
       title="Export the taxonomies into VDEX-format."
       description="Exports records and settings"
       handler=".exportimport.exportTaxonomy"
       />
@@ -80,22 +87,34 @@
       layer=".interfaces.IBrowserLayer"
       />
 
   <browser:page
       name="taxonomy"
       for="*"
       class=".browser.TaxonomyView"
-      permission="zope.Public"
       allowed_interface=".interfaces.ITaxonomyView"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="tabular_view"
+      template="listing_tabular.pt"
+      menu="plone_displayviews"
+      title="Tabular view"
+      for="plone.app.contenttypes.behaviors.collection.ISyndicatableCollection"
+      class=".browser.TaxonomyCollectionView"
+      permission="zope2.View"
+      layer=".interfaces.IBrowserLayer"
       />
 
   <adapter
-      name="taxonomy"
-      for="* *"
       factory=".browser.TaxonomyTraverser"
+      for="*
+           *"
+      name="taxonomy"
       />
 
   <browser:resourceDirectory
       name="taxonomy"
       directory="javascripts/build"
       layer=".interfaces.IBrowserLayer"
       />
@@ -126,33 +145,34 @@
       for="Products.CMFCore.interfaces.ISiteRoot"
       class=".jsonimpl.ImportJson"
       permission="collective.taxonomy.ManageTaxonomies"
       layer=".interfaces.IBrowserLayer"
       />
 
   <adapter
-      zcml:condition="installed collective.collectionfilter"
       factory=".collectionfilter.groupby_modifier"
-      name="modifier_1" />
+      name="modifier_1"
+      zcml:condition="installed collective.collectionfilter"
+      />
 
   <utility
       factory=".vocabulary.TaxonomyVocabulary"
-      name="collective.taxonomy.taxonomies"
       provides="zope.schema.interfaces.IVocabularyFactory"
+      name="collective.taxonomy.taxonomies"
       />
 
   <utility
       factory=".vocabulary.PermissionsVocabulary"
-      name="collective.taxonomy.permissions"
       provides="zope.schema.interfaces.IVocabularyFactory"
+      name="collective.taxonomy.permissions"
       />
 
   <utility
       factory=".vocabulary.LanguagesVocabulary"
-      name="collective.taxonomy.languages"
       provides="zope.schema.interfaces.IVocabularyFactory"
+      name="collective.taxonomy.languages"
       />
 
   <include file="widget.zcml" />
   <include file="upgradesteps.zcml" />
 
 </configure>
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/controlpanel.py` & `collective.taxonomy-3.1/src/collective/taxonomy/controlpanel.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,47 +156,46 @@
         self.request.RESPONSE.setHeader(
             "Content-disposition", 'attachment; filename="taxonomy_export.zip"'
         )
         return stream.getvalue()
 
 
 class TaxonomyAddForm(form.AddForm):
-
     fields = field.Fields(ITaxonomyForm)
 
     def updateWidgets(self):
         form.AddForm.updateWidgets(self)
         self.widgets["import_file_purge"].mode = HIDDEN_MODE
 
     def create(self, data):
         return data
 
     def add(self, data):
-        if "import_file" not in data:
-            raise ValueError("Import file is not in form")
-
+        # if "import_file" not in data:
+        #     raise ValueError("Import file is not in form")
         taxonomy = registerTaxonomy(
             self.context,
             name=data["taxonomy"],
             title=data["field_title"],
-            description=data["field_description"],
+            description=data.get("field_description", ""),
             default_language=data["default_language"],
         )
 
         # Import
         adapter = TaxonomyImportExportAdapter(self.context)
 
         if "import_file" in data:
             if data["import_file"]:
                 import_file = data["import_file"].data
                 adapter.importDocument(taxonomy, import_file)
             del data["import_file"]
 
         del data["taxonomy"]
-        del data["import_file_purge"]
+        if "import_file_purge" in data:
+            del data["import_file_purge"]
 
         taxonomy.registerBehavior(**data)
         api.portal.show_message(_("Taxonomy imported."), request=self.request)
 
         return self.request.RESPONSE.redirect(
             self.context.portal_url() + "/@@taxonomy-settings"
         )
@@ -267,19 +266,18 @@
             "{0}/@@taxonomy-settings".format(self.context.absolute_url())
         )
 
 
 @adapter(IPloneSiteRoot)
 @implementer(ITaxonomyForm)
 class TaxonomyEditFormAdapter(object):
-
     purge = False
 
-    def __init__(self, context):
-        taxonomy = context.REQUEST.get("form.widgets.taxonomy")
+    def __init__(self, context, name=None):
+        taxonomy = context.REQUEST.get("form.widgets.taxonomy") or name
         if taxonomy is None:
             return
 
         sm = context.getSiteManager()
         utility = sm.getUtility(ITaxonomy, name=taxonomy)
         generated_name = utility.getGeneratedName()
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/edit_taxonomy_data.pt` & `collective.taxonomy-3.1/src/collective/taxonomy/edit_taxonomy_data.pt`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/exportimport.py` & `collective.taxonomy-3.1/src/collective/taxonomy/exportimport.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
                 taxonomy.registerBehavior(**result)
 
 
 def exportTaxonomy(context):
     site = context.getSite()
     sm = site.getSiteManager()
-    for (name, taxonomy) in sm.getUtilitiesFor(ITaxonomy):
+    for name, taxonomy in sm.getUtilitiesFor(ITaxonomy):
         behavior = sm.queryUtility(IBehavior, name=taxonomy.getGeneratedName())
 
         short_name = name.split(".")[-1]
         exporter = TaxonomyImportExportAdapter(context)
         body = exporter.exportDocument(taxonomy)
 
         if body is not None:
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/factory.py` & `collective.taxonomy-3.1/src/collective/taxonomy/factory.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/generated.py` & `collective.taxonomy-3.1/src/collective/taxonomy/generated.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/README.txt` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/README.txt`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/config.json` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/config.json`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/animation.css` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/css/animation.css`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/taxonomy-embedded.css` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/css/taxonomy-embedded.css`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/taxonomy-ie7-codes.css` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/css/taxonomy-ie7-codes.css`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/taxonomy-ie7.css` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/css/taxonomy-ie7.css`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/css/taxonomy.css` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/css/taxonomy.css`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/demo.html` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/demo.html`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/font/taxonomy.eot` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/font/taxonomy.eot`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/font/taxonomy.svg` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/font/taxonomy.svg`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/font/taxonomy.ttf` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/font/taxonomy.ttf`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/font/taxonomy.woff` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/font/taxonomy.woff`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/icons/font/taxonomy.woff2` & `collective.taxonomy-3.1/src/collective/taxonomy/icons/font/taxonomy.woff2`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/indexer.py` & `collective.taxonomy-3.1/src/collective/taxonomy/indexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,32 +44,32 @@
         found = []
         stored_element = getattr(self.context, self.field_name)
         if not isinstance(stored_element, Iterable) or isinstance(
             stored_element, six.string_types
         ):
             stored_element = [stored_element]
 
-        for (language, data) in utility.data.items():
-            for (identifier, path) in utility.inverted_data[language].items():
+        for language, data in utility.data.items():
+            for identifier, path in utility.inverted_data[language].items():
                 if identifier in stored_element:
                     found.append(
                         (
                             identifier,
                             language,
                             path,
                         )
                     )
 
         lang = get_language(self.context)
         if lang not in utility.inverted_data:
             lang = utility.default_language
 
         result = []
-        for (key, value) in utility.inverted_data[lang].items():
-            for (found_identifier, found_language, found_path) in found:
+        for key, value in utility.inverted_data[lang].items():
+            for found_identifier, found_language, found_path in found:
                 if found_path.startswith(value) and key not in result:
                     result.append(key)
 
         return result
 
 
 @adapter(IDexterityContent, IZCatalog)
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/interfaces.py` & `collective.taxonomy-3.1/src/collective/taxonomy/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
-
 from .i18n import CollectiveTaxonomyMessageFactory as _
 from plone import api
 from plone.namedfile.field import NamedBlobFile
+from plone.restapi.controlpanels.interfaces import IControlpanel
 from zope import schema
 from zope.i18n.interfaces import ITranslationDomain
 from zope.interface import Interface
 from zope.schema.interfaces import IVocabularyFactory
 
 
 class ITaxonomySelectWidget(Interface):
@@ -64,15 +64,14 @@
     taxonomy = api.portal.get().REQUEST.get("form.widgets.taxonomy")
     if not taxonomy:
         return ""
     return taxonomy
 
 
 class ITaxonomyForm(Interface):
-
     taxonomy = schema.TextLine(
         title=_("Taxonomy"),
         description=_("The taxonomy identifier"),
         required=True,
         defaultFactory=taxonomyDefaultValue,
     )
 
@@ -147,7 +146,11 @@
 
 class ITaxonomyView(Interface):
     def taxonomiesForContext(self):
         """ """
 
     def translate(self, msgid, domain, target_language):
         """ """
+
+
+class ITaxonomyControlPanel(IControlpanel):
+    """Taxonomy Control panel"""
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/.eslintrc` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/.eslintrc`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/build/css/react-treeview.css` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/build/css/react-treeview.css`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/build/edittaxonomydata.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/build/edittaxonomydata.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/index.html` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/index.html`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/package.json` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/package.json`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/server.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/server.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/actions.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/actions.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/api.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/api.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/AddNodeButton.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/AddNodeButton.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/App.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/App.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/EditableId.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/EditableId.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/EditableIds.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/EditableIds.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/EditableTree.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/EditableTree.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/EditableValue.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/EditableValue.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/EditableValues.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/EditableValues.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/FormControls.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/FormControls.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/HideTreeCheckbox.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/HideTreeCheckbox.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/InputText.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/InputText.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/LanguageSelector.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/LanguageSelector.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/Leaf.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/Leaf.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/MoveDownButton.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/MoveDownButton.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/MoveUpButton.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/MoveUpButton.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/Node.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/Node.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/ReadOnlySubTree.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/ReadOnlySubTree.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/RemoveNodeButton.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/RemoveNodeButton.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/SubTree.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/SubTree.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/TaxonomyTree.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/TaxonomyTree.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/components/Tree.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/components/Tree.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/constants.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/constants.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/i18n.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/i18n.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/index.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/index.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/reducers.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/reducers.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/store/configureStore.dev.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/store/configureStore.dev.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/translations/es.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/translations/es.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/translations/fr.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/translations/fr.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/js/translations/nl.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/js/translations/nl.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/test/actions.spec.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/test/actions.spec.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/src/test/reducers.spec.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/src/test/reducers.spec.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/webpack.config.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/webpack.config.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/webpack.config.prod.js` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/webpack.config.prod.js`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/javascripts/yarn.lock` & `collective.taxonomy-3.1/src/collective/taxonomy/javascripts/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -5453,17 +5453,17 @@
 
 typedarray@^0.0.6:
   version "0.0.6"
   resolved "https://registry.yarnpkg.com/typedarray/-/typedarray-0.0.6.tgz#867ac74e3864187b1d3d47d996a78ec5c8830777"
   integrity sha512-/aCDEGatGvZ2BIk+HmLf4ifCJFwvKFNb9/JeZPMulfgFracn9QFcAf5GO8B/mweUjSoblS5In0cWhqpfs/5PQA==
 
 ua-parser-js@^0.7.30:
-  version "0.7.32"
-  resolved "https://registry.yarnpkg.com/ua-parser-js/-/ua-parser-js-0.7.32.tgz#cd8c639cdca949e30fa68c44b7813ef13e36d211"
-  integrity sha512-f9BESNVhzlhEFf2CHMSj40NWOjYPl1YKYbrvIr/hFTDEmLq7SRbWvm7FcdcpCYT95zrOhC7gZSxjdnnTpBcwVw==
+  version "0.7.33"
+  resolved "https://registry.yarnpkg.com/ua-parser-js/-/ua-parser-js-0.7.33.tgz#1d04acb4ccef9293df6f70f2c3d22f3030d8b532"
+  integrity sha512-s8ax/CeZdK9R/56Sui0WM6y9OFREJarMRHqLB2EwkovemBxNQ+Bqu8GAsUnVcXKgphb++ghr/B2BZx4mahujPw==
 
 uglify-js@^3.1.4:
   version "3.17.4"
   resolved "https://registry.yarnpkg.com/uglify-js/-/uglify-js-3.17.4.tgz#61678cf5fa3f5b7eb789bb345df29afb8257c22c"
   integrity sha512-T9q82TJI9e/C1TAxYvfb16xO120tMVFZrGA3f9/P4424DNu6ypK103y0GPFVa17yotwSyZW5iYXgjYHkGrJW/g==
 
 uglify-js@~2.7.3:
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/jsonimpl.py` & `collective.taxonomy-3.1/src/collective/taxonomy/jsonimpl.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/locales/collective.taxonomy.pot` & `collective.taxonomy-3.1/src/collective/taxonomy/locales/collective.taxonomy.pot`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/locales/da/LC_MESSAGES/collective.taxonomy.po` & `collective.taxonomy-3.1/src/collective/taxonomy/locales/da/LC_MESSAGES/collective.taxonomy.po`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/locales/de/LC_MESSAGES/collective.taxonomy.po` & `collective.taxonomy-3.1/src/collective/taxonomy/locales/de/LC_MESSAGES/collective.taxonomy.po`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/locales/es/LC_MESSAGES/collective.taxonomy.po` & `collective.taxonomy-3.1/src/collective/taxonomy/locales/es/LC_MESSAGES/collective.taxonomy.po`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/locales/fr/LC_MESSAGES/collective.taxonomy.po` & `collective.taxonomy-3.1/src/collective/taxonomy/locales/fr/LC_MESSAGES/collective.taxonomy.po`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/locales/nl/LC_MESSAGES/collective.taxonomy.po` & `collective.taxonomy-3.1/src/collective/taxonomy/locales/nl/LC_MESSAGES/collective.taxonomy.po`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/profiles/examples/taxonomies/nihms.xml` & `collective.taxonomy-3.1/src/collective/taxonomy/profiles/examples/taxonomies/nihms.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 text, with very long lines (333)*

 * *Files 5% similar despite different names*

```diff
@@ -1,110 +1,112 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
-00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0a3c 7664 6578 206c 616e  F-8"?>.<vdex lan
-00000030: 6775 6167 653d 2265 6e22 206f 7264 6572  guage="en" order
-00000040: 5369 676e 6966 6963 616e 743d 2266 616c  Significant="fal
-00000050: 7365 2220 7072 6f66 696c 6554 7970 653d  se" profileType=
-00000060: 2268 6965 7261 7263 6869 6361 6c54 6f6b  "hierarchicalTok
-00000070: 656e 5465 726d 7322 2078 6d6c 6e73 3d22  enTerms" xmlns="
-00000080: 6874 7470 3a2f 2f77 7777 2e69 6d73 676c  http://www.imsgl
-00000090: 6f62 616c 2e6f 7267 2f78 7364 2f69 6d73  obal.org/xsd/ims
-000000a0: 7664 6578 5f76 3170 3022 2078 6d6c 6e73  vdex_v1p0" xmlns
-000000b0: 3a78 7369 3d22 6874 7470 3a2f 2f77 7777  :xsi="http://www
-000000c0: 2e77 332e 6f72 672f 3230 3031 2f58 4d4c  .w3.org/2001/XML
-000000d0: 5363 6865 6d61 2d69 6e73 7461 6e63 6522  Schema-instance"
-000000e0: 2078 7369 3a73 6368 656d 614c 6f63 6174   xsi:schemaLocat
-000000f0: 696f 6e3d 2268 7474 703a 2f2f 7777 772e  ion="http://www.
-00000100: 696d 7367 6c6f 6261 6c2e 6f72 672f 7873  imsglobal.org/xs
-00000110: 642f 696d 7376 6465 785f 7631 7030 2069  d/imsvdex_v1p0 i
-00000120: 6d73 7664 6578 5f76 3170 302e 7873 6420  msvdex_v1p0.xsd 
-00000130: 6874 7470 3a2f 2f77 7777 2e69 6d73 676c  http://www.imsgl
-00000140: 6f62 616c 2e6f 7267 2f78 7364 2f69 6d73  obal.org/xsd/ims
-00000150: 6d64 5f72 6f6f 7476 3170 3270 3120 696d  md_rootv1p2p1 im
-00000160: 736d 645f 726f 6f74 7631 7032 7031 2e78  smd_rootv1p2p1.x
-00000170: 7364 223e 0a20 203c 766f 6361 624e 616d  sd">.  <vocabNam
-00000180: 653e 0a20 2020 203c 6c61 6e67 7374 7269  e>.    <langstri
-00000190: 6e67 206c 616e 6775 6167 653d 2265 6e22  ng language="en"
-000001a0: 3e54 6573 7420 766f 6361 6275 6c61 7279  >Test vocabulary
-000001b0: 3c2f 6c61 6e67 7374 7269 6e67 3e0a 2020  </langstring>.  
-000001c0: 3c2f 766f 6361 624e 616d 653e 0a20 203c  </vocabName>.  <
-000001d0: 766f 6361 6249 6465 6e74 6966 6965 723e  vocabIdentifier>
-000001e0: 7465 7374 566f 6361 6275 6c61 7279 3c2f  testVocabulary</
-000001f0: 766f 6361 6249 6465 6e74 6966 6965 723e  vocabIdentifier>
-00000200: 0a20 203c 7465 726d 3e0a 2020 2020 3c74  .  <term>.    <t
-00000210: 6572 6d49 6465 6e74 6966 6965 723e 313c  ermIdentifier>1<
-00000220: 2f74 6572 6d49 6465 6e74 6966 6965 723e  /termIdentifier>
-00000230: 0a20 2020 203c 6361 7074 696f 6e3e 0a20  .    <caption>. 
-00000240: 2020 2020 203c 6c61 6e67 7374 7269 6e67       <langstring
-00000250: 206c 616e 6775 6167 653d 2264 6122 3e49   language="da">I
-00000260: 6e66 6f72 6d61 7469 6f6e 7376 6964 656e  nformationsviden
-00000270: 736b 6162 3c2f 6c61 6e67 7374 7269 6e67  skab</langstring
-00000280: 3e0a 2020 2020 2020 3c6c 616e 6773 7472  >.      <langstr
-00000290: 696e 6720 6c61 6e67 7561 6765 3d22 6465  ing language="de
-000002a0: 223e 496e 666f 726d 6174 696b 3c2f 6c61  ">Informatik</la
-000002b0: 6e67 7374 7269 6e67 3e0a 2020 2020 2020  ngstring>.      
-000002c0: 3c6c 616e 6773 7472 696e 6720 6c61 6e67  <langstring lang
-000002d0: 7561 6765 3d22 656e 223e 496e 666f 726d  uage="en">Inform
-000002e0: 6174 696f 6e20 5363 6965 6e63 653c 2f6c  ation Science</l
-000002f0: 616e 6773 7472 696e 673e 0a20 2020 2020  angstring>.     
-00000300: 203c 6c61 6e67 7374 7269 6e67 206c 616e   <langstring lan
-00000310: 6775 6167 653d 2272 7522 3ed0 98d0 bdd1  guage="ru">.....
-00000320: 84d0 bed1 80d0 bcd0 b0d1 82d0 b8d0 bad1  ................
-00000330: 833c 2f6c 616e 6773 7472 696e 673e 0a20  .</langstring>. 
-00000340: 2020 203c 2f63 6170 7469 6f6e 3e0a 2020     </caption>.  
-00000350: 2020 3c74 6572 6d3e 0a20 2020 2020 203c    <term>.      <
-00000360: 7465 726d 4964 656e 7469 6669 6572 3e32  termIdentifier>2
-00000370: 3c2f 7465 726d 4964 656e 7469 6669 6572  </termIdentifier
-00000380: 3e0a 2020 2020 2020 3c63 6170 7469 6f6e  >.      <caption
-00000390: 3e0a 2020 2020 2020 2020 3c6c 616e 6773  >.        <langs
-000003a0: 7472 696e 6720 6c61 6e67 7561 6765 3d22  tring language="
-000003b0: 6461 223e 426f 6773 616d 6c69 6e67 3c2f  da">Bogsamling</
-000003c0: 6c61 6e67 7374 7269 6e67 3e0a 2020 2020  langstring>.    
-000003d0: 2020 2020 3c6c 616e 6773 7472 696e 6720      <langstring 
-000003e0: 6c61 6e67 7561 6765 3d22 656e 223e 426f  language="en">Bo
-000003f0: 6f6b 2043 6f6c 6c65 6374 696e 673c 2f6c  ok Collecting</l
-00000400: 616e 6773 7472 696e 673e 0a20 2020 2020  angstring>.     
-00000410: 203c 2f63 6170 7469 6f6e 3e0a 2020 2020   </caption>.    
-00000420: 2020 3c74 6572 6d3e 0a20 2020 2020 2020    <term>.       
-00000430: 203c 7465 726d 4964 656e 7469 6669 6572   <termIdentifier
-00000440: 3e34 3c2f 7465 726d 4964 656e 7469 6669  >4</termIdentifi
-00000450: 6572 3e0a 2020 2020 2020 2020 3c63 6170  er>.        <cap
-00000460: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-00000470: 3c6c 616e 6773 7472 696e 6720 6c61 6e67  <langstring lang
-00000480: 7561 6765 3d22 6461 223e 4865 7374 3c2f  uage="da">Hest</
-00000490: 6c61 6e67 7374 7269 6e67 3e0a 2020 2020  langstring>.    
-000004a0: 2020 2020 3c2f 6361 7074 696f 6e3e 0a20      </caption>. 
-000004b0: 2020 2020 203c 2f74 6572 6d3e 0a20 2020       </term>.   
-000004c0: 203c 2f74 6572 6d3e 0a20 2020 203c 7465   </term>.    <te
-000004d0: 726d 3e0a 2020 2020 2020 3c74 6572 6d49  rm>.      <termI
-000004e0: 6465 6e74 6966 6965 723e 333c 2f74 6572  dentifier>3</ter
-000004f0: 6d49 6465 6e74 6966 6965 723e 0a20 2020  mIdentifier>.   
-00000500: 2020 203c 6361 7074 696f 6e3e 0a20 2020     <caption>.   
-00000510: 2020 2020 203c 6c61 6e67 7374 7269 6e67       <langstring
-00000520: 206c 616e 6775 6167 653d 2264 6122 3e4b   language="da">K
-00000530: 726f 6e6f 6c6f 6769 3c2f 6c61 6e67 7374  ronologi</langst
-00000540: 7269 6e67 3e0a 2020 2020 2020 2020 3c6c  ring>.        <l
-00000550: 616e 6773 7472 696e 6720 6c61 6e67 7561  angstring langua
-00000560: 6765 3d22 656e 223e 4368 726f 6e6f 6c6f  ge="en">Chronolo
-00000570: 6779 3c2f 6c61 6e67 7374 7269 6e67 3e0a  gy</langstring>.
-00000580: 2020 2020 2020 3c2f 6361 7074 696f 6e3e        </caption>
-00000590: 0a20 2020 203c 2f74 6572 6d3e 0a20 2020  .    </term>.   
-000005a0: 203c 7465 726d 3e0a 2020 2020 2020 3c74   <term>.      <t
-000005b0: 6572 6d49 6465 6e74 6966 6965 723e 353c  ermIdentifier>5<
-000005c0: 2f74 6572 6d49 6465 6e74 6966 6965 723e  /termIdentifier>
-000005d0: 0a20 2020 2020 203c 6361 7074 696f 6e3e  .      <caption>
-000005e0: 0a20 2020 2020 2020 203c 6c61 6e67 7374  .        <langst
-000005f0: 7269 6e67 206c 616e 6775 6167 653d 2265  ring language="e
-00000600: 6e22 3e53 706f 7274 3c2f 6c61 6e67 7374  n">Sport</langst
-00000610: 7269 6e67 3e0a 2020 2020 2020 3c2f 6361  ring>.      </ca
-00000620: 7074 696f 6e3e 0a20 2020 203c 2f74 6572  ption>.    </ter
-00000630: 6d3e 0a20 2020 203c 7465 726d 3e0a 2020  m>.    <term>.  
-00000640: 2020 2020 3c74 6572 6d49 6465 6e74 6966      <termIdentif
-00000650: 6965 723e 3535 3c2f 7465 726d 4964 656e  ier>55</termIden
-00000660: 7469 6669 6572 3e0a 2020 2020 2020 3c63  tifier>.      <c
-00000670: 6170 7469 6f6e 3e0a 2020 2020 2020 2020  aption>.        
-00000680: 3c6c 616e 6773 7472 696e 6720 6c61 6e67  <langstring lang
-00000690: 7561 6765 3d22 656e 223e 4361 7273 3c2f  uage="en">Cars</
-000006a0: 6c61 6e67 7374 7269 6e67 3e0a 2020 2020  langstring>.    
-000006b0: 2020 3c2f 6361 7074 696f 6e3e 0a20 2020    </caption>.   
-000006c0: 203c 2f74 6572 6d3e 0a20 203c 2f74 6572   </term>.  </ter
-000006d0: 6d3e 0a3c 2f76 6465 783e 0a              m>.</vdex>.
+00000010: 2e30 2220 656e 636f 6469 6e67 3d22 7574  .0" encoding="ut
+00000020: 662d 3822 3f3e 0a3c 7664 6578 2078 6d6c  f-8"?>.<vdex xml
+00000030: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e69  ns="http://www.i
+00000040: 6d73 676c 6f62 616c 2e6f 7267 2f78 7364  msglobal.org/xsd
+00000050: 2f69 6d73 7664 6578 5f76 3170 3022 0a20  /imsvdex_v1p0". 
+00000060: 2020 2020 2078 6d6c 6e73 3a78 7369 3d22       xmlns:xsi="
+00000070: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+00000080: 672f 3230 3031 2f58 4d4c 5363 6865 6d61  g/2001/XMLSchema
+00000090: 2d69 6e73 7461 6e63 6522 0a20 2020 2020  -instance".     
+000000a0: 206c 616e 6775 6167 653d 2265 6e22 0a20   language="en". 
+000000b0: 2020 2020 206f 7264 6572 5369 676e 6966       orderSignif
+000000c0: 6963 616e 743d 2266 616c 7365 220a 2020  icant="false".  
+000000d0: 2020 2020 7072 6f66 696c 6554 7970 653d      profileType=
+000000e0: 2268 6965 7261 7263 6869 6361 6c54 6f6b  "hierarchicalTok
+000000f0: 656e 5465 726d 7322 0a20 2020 2020 2078  enTerms".      x
+00000100: 7369 3a73 6368 656d 614c 6f63 6174 696f  si:schemaLocatio
+00000110: 6e3d 2268 7474 703a 2f2f 7777 772e 696d  n="http://www.im
+00000120: 7367 6c6f 6261 6c2e 6f72 672f 7873 642f  sglobal.org/xsd/
+00000130: 696d 7376 6465 785f 7631 7030 2069 6d73  imsvdex_v1p0 ims
+00000140: 7664 6578 5f76 3170 302e 7873 6420 6874  vdex_v1p0.xsd ht
+00000150: 7470 3a2f 2f77 7777 2e69 6d73 676c 6f62  tp://www.imsglob
+00000160: 616c 2e6f 7267 2f78 7364 2f69 6d73 6d64  al.org/xsd/imsmd
+00000170: 5f72 6f6f 7476 3170 3270 3120 696d 736d  _rootv1p2p1 imsm
+00000180: 645f 726f 6f74 7631 7032 7031 2e78 7364  d_rootv1p2p1.xsd
+00000190: 220a 3e0a 2020 3c76 6f63 6162 4e61 6d65  ".>.  <vocabName
+000001a0: 3e0a 2020 2020 3c6c 616e 6773 7472 696e  >.    <langstrin
+000001b0: 6720 6c61 6e67 7561 6765 3d22 656e 223e  g language="en">
+000001c0: 5465 7374 2076 6f63 6162 756c 6172 793c  Test vocabulary<
+000001d0: 2f6c 616e 6773 7472 696e 673e 0a20 203c  /langstring>.  <
+000001e0: 2f76 6f63 6162 4e61 6d65 3e0a 2020 3c76  /vocabName>.  <v
+000001f0: 6f63 6162 4964 656e 7469 6669 6572 3e74  ocabIdentifier>t
+00000200: 6573 7456 6f63 6162 756c 6172 793c 2f76  estVocabulary</v
+00000210: 6f63 6162 4964 656e 7469 6669 6572 3e0a  ocabIdentifier>.
+00000220: 2020 3c74 6572 6d3e 0a20 2020 203c 7465    <term>.    <te
+00000230: 726d 4964 656e 7469 6669 6572 3e31 3c2f  rmIdentifier>1</
+00000240: 7465 726d 4964 656e 7469 6669 6572 3e0a  termIdentifier>.
+00000250: 2020 2020 3c63 6170 7469 6f6e 3e0a 2020      <caption>.  
+00000260: 2020 2020 3c6c 616e 6773 7472 696e 6720      <langstring 
+00000270: 6c61 6e67 7561 6765 3d22 6461 223e 496e  language="da">In
+00000280: 666f 726d 6174 696f 6e73 7669 6465 6e73  formationsvidens
+00000290: 6b61 623c 2f6c 616e 6773 7472 696e 673e  kab</langstring>
+000002a0: 0a20 2020 2020 203c 6c61 6e67 7374 7269  .      <langstri
+000002b0: 6e67 206c 616e 6775 6167 653d 2264 6522  ng language="de"
+000002c0: 3e49 6e66 6f72 6d61 7469 6b3c 2f6c 616e  >Informatik</lan
+000002d0: 6773 7472 696e 673e 0a20 2020 2020 203c  gstring>.      <
+000002e0: 6c61 6e67 7374 7269 6e67 206c 616e 6775  langstring langu
+000002f0: 6167 653d 2265 6e22 3e49 6e66 6f72 6d61  age="en">Informa
+00000300: 7469 6f6e 2053 6369 656e 6365 3c2f 6c61  tion Science</la
+00000310: 6e67 7374 7269 6e67 3e0a 2020 2020 2020  ngstring>.      
+00000320: 3c6c 616e 6773 7472 696e 6720 6c61 6e67  <langstring lang
+00000330: 7561 6765 3d22 7275 223e d098 d0bd d184  uage="ru">......
+00000340: d0be d180 d0bc d0b0 d182 d0b8 d0ba d183  ................
+00000350: 3c2f 6c61 6e67 7374 7269 6e67 3e0a 2020  </langstring>.  
+00000360: 2020 3c2f 6361 7074 696f 6e3e 0a20 2020    </caption>.   
+00000370: 203c 7465 726d 3e0a 2020 2020 2020 3c74   <term>.      <t
+00000380: 6572 6d49 6465 6e74 6966 6965 723e 323c  ermIdentifier>2<
+00000390: 2f74 6572 6d49 6465 6e74 6966 6965 723e  /termIdentifier>
+000003a0: 0a20 2020 2020 203c 6361 7074 696f 6e3e  .      <caption>
+000003b0: 0a20 2020 2020 2020 203c 6c61 6e67 7374  .        <langst
+000003c0: 7269 6e67 206c 616e 6775 6167 653d 2264  ring language="d
+000003d0: 6122 3e42 6f67 7361 6d6c 696e 673c 2f6c  a">Bogsamling</l
+000003e0: 616e 6773 7472 696e 673e 0a20 2020 2020  angstring>.     
+000003f0: 2020 203c 6c61 6e67 7374 7269 6e67 206c     <langstring l
+00000400: 616e 6775 6167 653d 2265 6e22 3e42 6f6f  anguage="en">Boo
+00000410: 6b20 436f 6c6c 6563 7469 6e67 3c2f 6c61  k Collecting</la
+00000420: 6e67 7374 7269 6e67 3e0a 2020 2020 2020  ngstring>.      
+00000430: 3c2f 6361 7074 696f 6e3e 0a20 2020 2020  </caption>.     
+00000440: 203c 7465 726d 3e0a 2020 2020 2020 2020   <term>.        
+00000450: 3c74 6572 6d49 6465 6e74 6966 6965 723e  <termIdentifier>
+00000460: 343c 2f74 6572 6d49 6465 6e74 6966 6965  4</termIdentifie
+00000470: 723e 0a20 2020 2020 2020 203c 6361 7074  r>.        <capt
+00000480: 696f 6e3e 0a20 2020 2020 2020 2020 203c  ion>.          <
+00000490: 6c61 6e67 7374 7269 6e67 206c 616e 6775  langstring langu
+000004a0: 6167 653d 2264 6122 3e48 6573 743c 2f6c  age="da">Hest</l
+000004b0: 616e 6773 7472 696e 673e 0a20 2020 2020  angstring>.     
+000004c0: 2020 203c 2f63 6170 7469 6f6e 3e0a 2020     </caption>.  
+000004d0: 2020 2020 3c2f 7465 726d 3e0a 2020 2020      </term>.    
+000004e0: 3c2f 7465 726d 3e0a 2020 2020 3c74 6572  </term>.    <ter
+000004f0: 6d3e 0a20 2020 2020 203c 7465 726d 4964  m>.      <termId
+00000500: 656e 7469 6669 6572 3e33 3c2f 7465 726d  entifier>3</term
+00000510: 4964 656e 7469 6669 6572 3e0a 2020 2020  Identifier>.    
+00000520: 2020 3c63 6170 7469 6f6e 3e0a 2020 2020    <caption>.    
+00000530: 2020 2020 3c6c 616e 6773 7472 696e 6720      <langstring 
+00000540: 6c61 6e67 7561 6765 3d22 6461 223e 4b72  language="da">Kr
+00000550: 6f6e 6f6c 6f67 693c 2f6c 616e 6773 7472  onologi</langstr
+00000560: 696e 673e 0a20 2020 2020 2020 203c 6c61  ing>.        <la
+00000570: 6e67 7374 7269 6e67 206c 616e 6775 6167  ngstring languag
+00000580: 653d 2265 6e22 3e43 6872 6f6e 6f6c 6f67  e="en">Chronolog
+00000590: 793c 2f6c 616e 6773 7472 696e 673e 0a20  y</langstring>. 
+000005a0: 2020 2020 203c 2f63 6170 7469 6f6e 3e0a       </caption>.
+000005b0: 2020 2020 3c2f 7465 726d 3e0a 2020 2020      </term>.    
+000005c0: 3c74 6572 6d3e 0a20 2020 2020 203c 7465  <term>.      <te
+000005d0: 726d 4964 656e 7469 6669 6572 3e35 3c2f  rmIdentifier>5</
+000005e0: 7465 726d 4964 656e 7469 6669 6572 3e0a  termIdentifier>.
+000005f0: 2020 2020 2020 3c63 6170 7469 6f6e 3e0a        <caption>.
+00000600: 2020 2020 2020 2020 3c6c 616e 6773 7472          <langstr
+00000610: 696e 6720 6c61 6e67 7561 6765 3d22 656e  ing language="en
+00000620: 223e 5370 6f72 743c 2f6c 616e 6773 7472  ">Sport</langstr
+00000630: 696e 673e 0a20 2020 2020 203c 2f63 6170  ing>.      </cap
+00000640: 7469 6f6e 3e0a 2020 2020 3c2f 7465 726d  tion>.    </term
+00000650: 3e0a 2020 2020 3c74 6572 6d3e 0a20 2020  >.    <term>.   
+00000660: 2020 203c 7465 726d 4964 656e 7469 6669     <termIdentifi
+00000670: 6572 3e35 353c 2f74 6572 6d49 6465 6e74  er>55</termIdent
+00000680: 6966 6965 723e 0a20 2020 2020 203c 6361  ifier>.      <ca
+00000690: 7074 696f 6e3e 0a20 2020 2020 2020 203c  ption>.        <
+000006a0: 6c61 6e67 7374 7269 6e67 206c 616e 6775  langstring langu
+000006b0: 6167 653d 2265 6e22 3e43 6172 733c 2f6c  age="en">Cars</l
+000006c0: 616e 6773 7472 696e 673e 0a20 2020 2020  angstring>.     
+000006d0: 203c 2f63 6170 7469 6f6e 3e0a 2020 2020   </caption>.    
+000006e0: 3c2f 7465 726d 3e0a 2020 3c2f 7465 726d  </term>.  </term
+000006f0: 3e0a 3c2f 7664 6578 3e0a                 >.</vdex>.
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/rebuild_i18n.sh` & `collective.taxonomy-3.1/src/collective/taxonomy/rebuild_i18n.sh`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/setuphandlers.py` & `collective.taxonomy-3.1/src/collective/taxonomy/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/testing.py` & `collective.taxonomy-3.1/src/collective/taxonomy/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from plone.app.robotframework.testing import REMOTE_LIBRARY_BUNDLE_FIXTURE
 from plone.app.testing import applyProfile
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from plone.testing import z2
+from plone.testing import zope
 
 import collective.taxonomy
 
 
 class CollectiveTaxonomyLayer(PloneSandboxLayer):
-
     defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load any other ZCML that is required for your tests.
         # The z3c.autoinclude feature is disabled in the Plone fixture base
         # layer.
         import plone.app.dexterity
@@ -32,15 +32,16 @@
 COLLECTIVE_TAXONOMY_FIXTURE = CollectiveTaxonomyLayer()
 
 INTEGRATION_TESTING = IntegrationTesting(
     bases=(COLLECTIVE_TAXONOMY_FIXTURE,), name="TaxonomyFixture:Integration"
 )
 
 FUNCTIONAL_TESTING = FunctionalTesting(
-    bases=(COLLECTIVE_TAXONOMY_FIXTURE,), name="TaxonomyFixture:Functional"
+    bases=(COLLECTIVE_TAXONOMY_FIXTURE, zope.WSGI_SERVER_FIXTURE),
+    name="TaxonomyFixture:Functional",
 )
 
 ROBOT_TESTING = FunctionalTesting(
     bases=(
         COLLECTIVE_TAXONOMY_FIXTURE,
         REMOTE_LIBRARY_BUNDLE_FIXTURE,
         z2.ZSERVER_FIXTURE,
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/testing.zcml` & `collective.taxonomy-3.1/src/collective/taxonomy/testing.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-<configure xmlns="http://namespaces.zope.org/zope"
-           xmlns:genericsetup="http://namespaces.zope.org/genericsetup">
+<configure
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    >
 
   <include file="configure.zcml" />
   <include package="plone.app.contenttypes" />
   <include package="plone.app.querystring" />
 
   <genericsetup:registerProfile
       name="examples"
       title="collective.taxonomy"
-      directory="profiles/examples"
       description="Registers example taxonomy used in tests."
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/examples"
       />
 
 </configure>
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/tests/robot/todo_test_taxonomy.robot` & `collective.taxonomy-3.1/src/collective/taxonomy/tests/robot/todo_test_taxonomy.robot`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_behavior.py` & `collective.taxonomy-3.1/src/collective/taxonomy/tests/test_behavior.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from zope.component import queryUtility
 from zope.component.hooks import getSiteManager
 
 import unittest
 
 
 class TestBehaviorRegistration(unittest.TestCase):
-
     layer = INTEGRATION_TESTING
 
     def test_register_behavior(self):
         # Test taxonomy registration
         taxonomy = queryUtility(ITaxonomy, name="collective.taxonomy.test")
         self.assertIsNotNone(taxonomy)
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_controlpanel.py` & `collective.taxonomy-3.1/src/collective/taxonomy/tests/test_controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_indexer.py` & `collective.taxonomy-3.1/src/collective/taxonomy/tests/test_indexer.py`

 * *Files 21% similar despite different names*

```diff
@@ -57,14 +57,26 @@
         notify(ObjectRemovedEvent(self.taxonomy_test, self.document_schema))
         notify(FieldRemovedEvent(self.fti, self.taxonomy_test))
 
     def test_indexer_with_field(self):
         portal_catalog = api.portal.get_tool("portal_catalog")
         utility = queryUtility(ITaxonomy, name="collective.taxonomy.test")
         taxonomy = utility.data
+        taxonomy_test = schema.Set(
+            title="taxonomy_test",
+            description="taxonomy description schema",
+            required=False,
+            value_type=schema.Choice(vocabulary="collective.taxonomy.taxonomies"),
+        )
+        portal_types = api.portal.get_tool("portal_types")
+        fti = portal_types.get("Document")
+        document_schema = fti.lookupSchema()
+        notify(ObjectAddedEvent(taxonomy_test, document_schema))
+        notify(FieldAddedEvent(fti, taxonomy_test))
+
         index = portal_catalog.Indexes["taxonomy_test"]
         self.assertEqual(index.numObjects(), 0)
 
         self.document.taxonomy_test = []
         self.document.reindexObject()
         query = {}
         query["taxonomy_test"] = "1"
@@ -82,14 +94,25 @@
         index = portal_catalog.Indexes["taxonomy_test"]
         self.assertEqual(index.numObjects(), 1)
 
     def test_multilanguage_indexer(self):
         portal_catalog = api.portal.get_tool("portal_catalog")
         utility = queryUtility(ITaxonomy, name="collective.taxonomy.test")
         taxonomy = utility.data
+        taxonomy_test = schema.Set(
+            title="taxonomy_test",
+            description="taxonomy description schema",
+            required=False,
+            value_type=schema.Choice(vocabulary="collective.taxonomy.taxonomies"),
+        )
+        portal_types = api.portal.get_tool("portal_types")
+        fti = portal_types.get("Document")
+        document_schema = fti.lookupSchema()
+        notify(ObjectAddedEvent(taxonomy_test, document_schema))
+        notify(FieldAddedEvent(fti, taxonomy_test))
         query = {}
         query["taxonomy_test"] = "5"
         taxo_val = taxonomy["en"]["\u241fInformation Science\u241fSport"]
         self.document.taxonomy_test = [taxo_val]
         self.document.reindexObject()
         self.assertEqual(len(portal_catalog(query)), 1)
 
@@ -107,12 +130,23 @@
             ],
         )
 
     def test_index_single_select(self):
         portal_catalog = api.portal.get_tool("portal_catalog")
         utility = queryUtility(ITaxonomy, name="collective.taxonomy.test")
         taxonomy = utility.data
+        taxonomy_test = schema.Set(
+            title="taxonomy_test",
+            description="taxonomy description schema",
+            required=False,
+            value_type=schema.Choice(vocabulary="collective.taxonomy.taxonomies"),
+        )
+        portal_types = api.portal.get_tool("portal_types")
+        fti = portal_types.get("Document")
+        document_schema = fti.lookupSchema()
+        notify(ObjectAddedEvent(taxonomy_test, document_schema))
+        notify(FieldAddedEvent(fti, taxonomy_test))
         taxo_val = taxonomy["en"]["\u241fInformation Science\u241fCars"]
         self.document.taxonomy_test = taxo_val
         self.document.reindexObject()
         self.assertEqual(len(portal_catalog({"taxonomy_test": "5"})), 0)
         self.assertEqual(len(portal_catalog({"taxonomy_test": "55"})), 1)
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_json.py` & `collective.taxonomy-3.1/src/collective/taxonomy/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_robot.py` & `collective.taxonomy-3.1/src/collective/taxonomy/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_setup.py` & `collective.taxonomy-3.1/src/collective/taxonomy/tests/test_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         from collective.taxonomy.interfaces import IBrowserLayer
         from plone.browserlayer import utils
 
         self.assertIn(IBrowserLayer, utils.registered_layers())
 
 
 class TestUninstall(unittest.TestCase):
-
     layer = INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.installer = get_installer(self.portal, self.layer["request"])
         roles_before = api.user.get_roles(TEST_USER_ID)
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_traverser.py` & `collective.taxonomy-3.1/src/collective/taxonomy/tests/test_traverser.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/tests/test_utility.py` & `collective.taxonomy-3.1/src/collective/taxonomy/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/upgradesteps.py` & `collective.taxonomy-3.1/src/collective/taxonomy/upgradesteps.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def reactivateSearchable(tool):
     """ """
     tool = tool.aq_parent
     sm = tool.getSiteManager()
     utilities = sm.getUtilitiesFor(IBehavior)
-    for (utility_name, utility) in utilities:
+    for utility_name, utility in utilities:
         if utility_name.startswith("collective.taxonomy.generated."):
             utility.deactivateSearchable()
             utility.activateSearchable()
             log.info("Reactivated searchable for " + utility_name)
 
 
 def import_registry(tool):
@@ -29,15 +29,15 @@
     )
 
 
 def fix_metadata(tool):
     tool = tool.aq_parent
     sm = tool.getSiteManager()
     utilities = sm.getUtilitiesFor(ITaxonomy)
-    for (utility_name, utility) in utilities:
+    for utility_name, utility in utilities:
         utility._fixup()
         for lang, data in utility.data.items():
             version = data.pop("#VERSION", None)
             if version is not None:
                 utility.version[lang] = version
 
             count = data.pop("#COUNT", None)
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/upgradesteps.zcml` & `collective.taxonomy-3.1/src/collective/taxonomy/upgradesteps.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,51 @@
-<configure xmlns="http://namespaces.zope.org/zope"
-           xmlns:genericsetup="http://namespaces.zope.org/genericsetup">
+<configure
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    >
 
   <genericsetup:upgradeSteps
-     profile="collective.taxonomy:default"
-     source="0.2"
-     destination="0.3">
+      profile="collective.taxonomy:default"
+      source="0.2"
+      destination="0.3"
+      >
     <genericsetup:upgradeStep
-       handler=".upgradesteps.reactivateSearchable"
-       title="Reactivate searchable for every taxonomy"
-       description=""
-       />
+        title="Reactivate searchable for every taxonomy"
+        description=""
+        handler=".upgradesteps.reactivateSearchable"
+        />
   </genericsetup:upgradeSteps>
   <genericsetup:upgradeSteps
-     profile="collective.taxonomy:default"
-     source="1004"
-     destination="1005">
+      profile="collective.taxonomy:default"
+      source="1004"
+      destination="1005"
+      >
     <genericsetup:upgradeStep
-       handler=".upgradesteps.fix_metadata"
-       title="Fixes taxonomy metadata"
-       description=""
-       />
+        title="Fixes taxonomy metadata"
+        description=""
+        handler=".upgradesteps.fix_metadata"
+        />
   </genericsetup:upgradeSteps>
   <genericsetup:upgradeSteps
-     profile="collective.taxonomy:default"
-     source="1005"
-     destination="1006">
+      profile="collective.taxonomy:default"
+      source="1005"
+      destination="1006"
+      >
     <genericsetup:upgradeStep
-       handler=".upgradesteps.update_configlet_properties"
-       title="Use new 'Manage taxonomies' permission"
-       description=""
-       />
+        title="Use new 'Manage taxonomies' permission"
+        description=""
+        handler=".upgradesteps.update_configlet_properties"
+        />
   </genericsetup:upgradeSteps>
   <genericsetup:upgradeSteps
-     profile="collective.taxonomy:default"
-     source="1006"
-     destination="2000">
+      profile="collective.taxonomy:default"
+      source="1006"
+      destination="2000"
+      >
     <genericsetup:upgradeStep
-       handler=".upgradesteps.update_configlet_icon"
-       title="Use new icon for configlet"
-       description=""
-       />
+        title="Use new icon for configlet"
+        description=""
+        handler=".upgradesteps.update_configlet_icon"
+        />
   </genericsetup:upgradeSteps>
 
 </configure>
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/utility.py` & `collective.taxonomy-3.1/src/collective/taxonomy/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-
 from BTrees.IOBTree import IOBTree
 from BTrees.OOBTree import OOBTree
 from collective.taxonomy import generated
 from collective.taxonomy import LEGACY_PATH_SEPARATOR
 from collective.taxonomy import NODE
 from collective.taxonomy import PATH_SEPARATOR
 from collective.taxonomy import PRETTY_PATH_SEPARATOR
@@ -74,17 +73,17 @@
         language = self.getCurrentLanguage(request)
         return self.makeVocabulary(language)
 
     @property
     @ram.cache(lambda method, self: (self.name, self.data._p_mtime))
     def inverted_data(self):
         inv_data = {}
-        for (language, elements) in self.data.items():
+        for language, elements in self.data.items():
             inv_data[language] = {}
-            for (path, identifier) in elements.items():
+            for path, identifier in elements.items():
                 inv_data[language][identifier] = path
         return inv_data
 
     def getShortName(self):
         return self.name.split(".")[-1]
 
     def getGeneratedName(self):
@@ -142,15 +141,15 @@
         behavior.addIndex()
         behavior.addMetadata()
         behavior.activateSearchable()
 
     def cleanupFTI(self):
         """Cleanup the FTIs"""
         generated_name = self.getGeneratedName()
-        for (name, fti) in self.sm.getUtilitiesFor(IDexterityFTI):
+        for name, fti in self.sm.getUtilitiesFor(IDexterityFTI):
             if generated_name in fti.behaviors:
                 fti.behaviors = [
                     behavior for behavior in fti.behaviors if behavior != generated_name
                 ]
             modified(fti, DexterityFTIModificationDescription("behaviors", ""))
 
     def updateBehavior(self, **kwargs):
@@ -165,15 +164,15 @@
                 utility.title = kwargs.pop("field_title")
 
             for k, v in kwargs.items():
                 setattr(utility, k, v)
 
         delattr(generated, short_name)
 
-        for (name, fti) in self.sm.getUtilitiesFor(IDexterityFTI):
+        for name, fti in self.sm.getUtilitiesFor(IDexterityFTI):
             if behavior_name in fti.behaviors:
                 modified(fti, DexterityFTIModificationDescription("behaviors", ""))
 
     def unregisterBehavior(self):
         behavior_name = self.getGeneratedName()
         utility = self.sm.queryUtility(IBehavior, name=behavior_name)
 
@@ -292,15 +291,14 @@
         context=None,
         target_language=None,
         default=None,
         msgid_plural=None,
         default_plural=None,
         number=None,
     ):
-
         if target_language is None or target_language not in self.inverted_data:
             target_language = str(api.portal.get_current_language())
 
             if target_language not in self.inverted_data:
                 # might be a non standard language or the portal has
                 # switched standard language after creating the taxonomy
                 lngs = list(self.inverted_data.keys())
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/vdex.py` & `collective.taxonomy-3.1/src/collective/taxonomy/vdex.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         for identifier in index.keys():
             termnode = etree.Element("term")
             identifiernode = etree.Element("termIdentifier")
             identifiernode.text = str(identifier)
             captionnode = etree.Element("caption")
             translations = sorted(table[identifier].items())
 
-            for (language, langstring) in translations:
+            for language, langstring in translations:
                 langstringnode = etree.Element("langstring")
                 langstringnode.text = langstring
                 langstringnode.attrib["language"] = (
                     language or self.taxonomy.default_language or ""
                 )  # noqa: E501
                 captionnode.append(langstringnode)
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/vocabulary.py` & `collective.taxonomy-3.1/src/collective/taxonomy/vocabulary.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
 @implementer(IVocabularyFactory)
 class PermissionsVocabulary(object):
     def __call__(self, context):
         result = []
         sm = getSite().getSiteManager()
 
-        for (permission, permission_object) in sm.getUtilitiesFor(IPermission):
+        for permission, permission_object in sm.getUtilitiesFor(IPermission):
             result.append(
                 SimpleTerm(
                     value=permission_object.id, title=_pmf(permission_object.title)
                 )
             )
 
         result.sort(key=lambda permission: permission.title)
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/widget.py` & `collective.taxonomy-3.1/src/collective/taxonomy/widget.py`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/widget.zcml` & `collective.taxonomy-3.1/src/collective/taxonomy/widget.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:z3c="http://namespaces.zope.org/z3c"
-    i18n_domain="z3c.form">
+    i18n_domain="z3c.form"
+    >
 
   <class class=".widget.TaxonomySelectWidget">
     <require
         permission="zope.Public"
         interface=".interfaces.ITaxonomySelectWidget"
         />
   </class>
 
   <z3c:widgetTemplate
-      mode="display"
       widget=".interfaces.ITaxonomySelectWidget"
-      layer="z3c.form.interfaces.IFormLayer"
       template="widget_display.pt"
+      layer="z3c.form.interfaces.IFormLayer"
+      mode="display"
       />
 
   <z3c:widgetTemplate
-      mode="input"
       widget=".interfaces.ITaxonomySelectWidget"
-      layer="z3c.form.interfaces.IFormLayer"
       template="widget_input.pt"
+      layer="z3c.form.interfaces.IFormLayer"
+      mode="input"
       />
 
-</configure>
+</configure>
```

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/widget_display.pt` & `collective.taxonomy-3.1/src/collective/taxonomy/widget_display.pt`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective/taxonomy/widget_input.pt` & `collective.taxonomy-3.1/src/collective/taxonomy/widget_input.pt`

 * *Files identical despite different names*

### Comparing `collective.taxonomy-3.0.1/src/collective.taxonomy.egg-info/PKG-INFO` & `collective.taxonomy-3.1/src/collective.taxonomy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.taxonomy
-Version: 3.0.1
+Version: 3.1
 Summary: Create, edit and use hierarchical taxonomies in Plone!
 Home-page: https://pypi.org/project/collective.taxonomy/
 Author: Bo Simonsen and Malthe Borch
 Author-email: bo@headnet.dk
 License: GPLv2+
 Keywords: plone taxonomy dexterity
 Classifier: Development Status :: 6 - Mature
@@ -221,14 +221,36 @@
         fr
     }
 
 You'll have to rebuild the js bundle: ``npm run build``
 
 That's it!
 
+Restapi support
+---------------
+
+This package also supports endpoints for basic CRUD operations that can be consumend by any frontend service.
+
+The API consumer can create, read, and delete taxonomies.
+
++----------+---------------------+----------------------------------------+
+| Verb     | URL                 | Action                                 |
++==========+=====================+========================================+
+| `POST`   | `/@taxonomy`        | Add taxonomy with specific data        |
++----------+---------------------+----------------------------------------+
+| `GET`    | `/@taxonomy`        | List all taxonomies                    |
++----------+---------------------+----------------------------------------+
+| `GET`    | `/@taxonomy/{name}` | Get taxonomy data                      |
++----------+---------------------+----------------------------------------+
+| `DELETE` | `/@taxonomy/{name}` | Remove one or more taxonomies          |
++----------+---------------------+----------------------------------------+
+| `PATCH`  | `/@taxonomy/{name}` | Update taxonomy data                   |
++----------+---------------------+----------------------------------------+
+| `GET`    | `/@taxonomySchema`  | Get current taxonomy schema            |
++----------+---------------------+----------------------------------------+
 
 Translations
 ------------
 
 This product has been translated into
 
 - Danish.
@@ -341,14 +363,22 @@
 
 .. _Plone: https://plone.org/
 .. _`opening a ticket`: https://github.com/collective/collective.taxonomy/issues
 
 Changes
 =======
 
+3.1 (2023-05-26)
+----------------
+
+- Integrate taxonomies into Collection tabular view, display values are now resolved
+  [MrTango]
+- Restapi endpoints support [cekk, nileshgulia1]
+
+
 3.0.1 (2023-02-02)
 ------------------
 
 - export/import of field_prefix value.
   [eikichi18]
```

### Comparing `collective.taxonomy-3.0.1/src/collective.taxonomy.egg-info/SOURCES.txt` & `collective.taxonomy-3.1/src/collective.taxonomy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 src/collective/taxonomy/exportimport.py
 src/collective/taxonomy/factory.py
 src/collective/taxonomy/generated.py
 src/collective/taxonomy/i18n.py
 src/collective/taxonomy/indexer.py
 src/collective/taxonomy/interfaces.py
 src/collective/taxonomy/jsonimpl.py
+src/collective/taxonomy/listing_tabular.pt
 src/collective/taxonomy/rebuild_i18n.sh
 src/collective/taxonomy/setuphandlers.py
 src/collective/taxonomy/testing.py
 src/collective/taxonomy/testing.zcml
 src/collective/taxonomy/upgradesteps.py
 src/collective/taxonomy/upgradesteps.zcml
 src/collective/taxonomy/utility.py
@@ -157,33 +158,58 @@
 src/collective/taxonomy/javascripts/src/js/translations/fr.js
 src/collective/taxonomy/javascripts/src/js/translations/index.js
 src/collective/taxonomy/javascripts/src/js/translations/nl.js
 src/collective/taxonomy/javascripts/src/test/actions.spec.js
 src/collective/taxonomy/javascripts/src/test/reducers.spec.js
 src/collective/taxonomy/javascripts/src/test/setup.js
 src/collective/taxonomy/locales/collective.taxonomy.pot
+src/collective/taxonomy/locales/da/LC_MESSAGES/collective.taxonomy.mo
 src/collective/taxonomy/locales/da/LC_MESSAGES/collective.taxonomy.po
+src/collective/taxonomy/locales/de/LC_MESSAGES/collective.taxonomy.mo
 src/collective/taxonomy/locales/de/LC_MESSAGES/collective.taxonomy.po
+src/collective/taxonomy/locales/es/LC_MESSAGES/collective.taxonomy.mo
 src/collective/taxonomy/locales/es/LC_MESSAGES/collective.taxonomy.po
+src/collective/taxonomy/locales/fr/LC_MESSAGES/collective.taxonomy.mo
 src/collective/taxonomy/locales/fr/LC_MESSAGES/collective.taxonomy.po
+src/collective/taxonomy/locales/nl/LC_MESSAGES/collective.taxonomy.mo
 src/collective/taxonomy/locales/nl/LC_MESSAGES/collective.taxonomy.po
 src/collective/taxonomy/profiles/default/browserlayer.xml
 src/collective/taxonomy/profiles/default/controlpanel.xml
 src/collective/taxonomy/profiles/default/metadata.xml
 src/collective/taxonomy/profiles/default/registry.xml
 src/collective/taxonomy/profiles/default/rolemap.xml
 src/collective/taxonomy/profiles/examples/metadata.xml
 src/collective/taxonomy/profiles/examples/taxonomies/nihms.cfg
 src/collective/taxonomy/profiles/examples/taxonomies/nihms.xml
 src/collective/taxonomy/profiles/uninstall/browserlayer.xml
 src/collective/taxonomy/profiles/uninstall/controlpanel.xml
 src/collective/taxonomy/profiles/uninstall/registry.xml
+src/collective/taxonomy/restapi/__init__.py
+src/collective/taxonomy/restapi/configure.zcml
+src/collective/taxonomy/restapi/utils.py
+src/collective/taxonomy/restapi/serializers/__init__.py
+src/collective/taxonomy/restapi/serializers/configure.zcml
+src/collective/taxonomy/restapi/serializers/taxonomy.py
+src/collective/taxonomy/restapi/services/__init__.py
+src/collective/taxonomy/restapi/services/configure.zcml
+src/collective/taxonomy/restapi/services/controlpanel/__init__.py
+src/collective/taxonomy/restapi/services/controlpanel/configure.zcml
+src/collective/taxonomy/restapi/services/controlpanel/controlpanel.py
+src/collective/taxonomy/restapi/services/taxonomy/__init__.py
+src/collective/taxonomy/restapi/services/taxonomy/add.py
+src/collective/taxonomy/restapi/services/taxonomy/configure.zcml
+src/collective/taxonomy/restapi/services/taxonomy/delete.py
+src/collective/taxonomy/restapi/services/taxonomy/get.py
+src/collective/taxonomy/restapi/services/taxonomy/schema.py
+src/collective/taxonomy/restapi/services/taxonomy/update.py
 src/collective/taxonomy/tests/__init__.py
 src/collective/taxonomy/tests/test_behavior.py
 src/collective/taxonomy/tests/test_controlpanel.py
+src/collective/taxonomy/tests/test_controlpanel_restapi.py
 src/collective/taxonomy/tests/test_indexer.py
 src/collective/taxonomy/tests/test_json.py
 src/collective/taxonomy/tests/test_robot.py
 src/collective/taxonomy/tests/test_setup.py
+src/collective/taxonomy/tests/test_taxonomy_endpoint.py
 src/collective/taxonomy/tests/test_traverser.py
 src/collective/taxonomy/tests/test_utility.py
 src/collective/taxonomy/tests/robot/todo_test_taxonomy.robot
```

