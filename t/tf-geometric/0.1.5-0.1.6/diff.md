# Comparing `tmp/tf_geometric-0.1.5.tar.gz` & `tmp/tf_geometric-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tf_geometric-0.1.5.tar", last modified: Tue Dec 27 08:17:13 2022, max compression
+gzip compressed data, was "dist/tf_geometric-0.1.6.tar", last modified: Fri May 26 09:14:13 2023, max compression
```

## Comparing `tf_geometric-0.1.5.tar` & `tf_geometric-0.1.6.tar`

### file list

```diff
@@ -1,113 +1,103 @@
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)    35149 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/LICENSE
--rw-rw-r--   0 hujun     (1002) hujun     (1003)    14922 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/PKG-INFO
--rw-rw-r--   0 hujun     (1002) hujun     (1003)    14449 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/README.rst
--rw-rw-r--   0 hujun     (1002) hujun     (1003)       38 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/setup.cfg
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1186 2022-12-27 08:16:12.000000 tf_geometric-0.1.5/setup.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/test/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1144 2021-04-24 16:46:15.000000 tf_geometric-0.1.5/test/test.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1777 2022-04-27 03:34:18.000000 tf_geometric-0.1.5/test/test_batch_graph.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)      891 2021-08-18 01:59:16.000000 tf_geometric-0.1.5/test/test_blog_catalog.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     3797 2021-11-16 12:13:48.000000 tf_geometric-0.1.5/test/test_gcn.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1458 2022-04-26 06:30:22.000000 tf_geometric-0.1.5/test/test_gcn_norm_edge.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)      754 2021-10-03 03:32:59.000000 tf_geometric-0.1.5/test/test_num_edges.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     6585 2021-12-01 00:17:06.000000 tf_geometric-0.1.5/test/test_ogb_speed.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)    12089 2021-12-01 05:48:40.000000 tf_geometric-0.1.5/test/test_ogb_speed2.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1417 2021-11-15 05:34:39.000000 tf_geometric-0.1.5/test/test_sparse_adj.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     3824 2021-11-16 12:17:40.000000 tf_geometric-0.1.5/test/test_sparse_gat.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1777 2022-04-27 01:45:39.000000 tf_geometric-0.1.5/test/test_sparse_node_features.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)      323 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/__init__.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/data/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)        0 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/data/__init__.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     3388 2021-11-11 04:26:16.000000 tf_geometric-0.1.5/tf_geometric/data/dataset.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)    27020 2022-12-27 08:16:12.000000 tf_geometric-0.1.5/tf_geometric/data/graph.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/datasets/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1150 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/datasets/__init__.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1804 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/datasets/abnormal.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1226 2021-11-11 04:48:44.000000 tf_geometric-0.1.5/tf_geometric/datasets/amazon_electronics.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1136 2021-08-18 07:29:22.000000 tf_geometric-0.1.5/tf_geometric/datasets/blog_catalog.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1187 2021-11-11 04:48:44.000000 tf_geometric-0.1.5/tf_geometric/datasets/coauthor.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1312 2021-11-11 04:48:44.000000 tf_geometric-0.1.5/tf_geometric/datasets/csr_npz.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     9564 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/datasets/hgb.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     5437 2021-08-18 07:29:22.000000 tf_geometric-0.1.5/tf_geometric/datasets/model_net.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     4518 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/datasets/nars_academic.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1777 2021-04-27 19:13:57.000000 tf_geometric-0.1.5/tf_geometric/datasets/ogb.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     5286 2021-04-24 18:37:23.000000 tf_geometric-0.1.5/tf_geometric/datasets/planetoid.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     2487 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/datasets/ppi.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     2344 2021-04-24 18:37:23.000000 tf_geometric-0.1.5/tf_geometric/datasets/reddit.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     6999 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/datasets/tu.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/layers/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)      767 2021-11-21 17:50:48.000000 tf_geometric-0.1.5/tf_geometric/layers/__init__.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)        0 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/__init__.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     5809 2022-06-25 07:57:36.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/appnp.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     4982 2022-06-25 07:57:36.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/chebynet.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     4372 2022-01-10 13:10:13.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/gat.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     7213 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/gcn.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1249 2021-07-30 19:32:57.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/gin.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)    16888 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/graph_sage.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     3692 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/le_conv.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     4787 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/sgc.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     6064 2022-06-25 07:57:36.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/ssgc.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     4913 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/layers/conv/tagcn.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/layers/kernel/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)        0 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/kernel/__init__.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1152 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/kernel/map_reduce.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/layers/pool/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)        0 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/pool/__init__.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     5274 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/pool/asap.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1081 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/pool/common_pool.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     2488 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/pool/diff_pool.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     3655 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/pool/min_cut_pool.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1519 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/pool/sag_pool.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1118 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/pool/set2set.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1316 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/pool/sort_pool.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/layers/sampling/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)        0 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/sampling/__init__.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)      994 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/layers/sampling/drop_edge.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/nn/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1242 2022-06-24 10:09:02.000000 tf_geometric-0.1.5/tf_geometric/nn/__init__.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)        0 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/__init__.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     3826 2022-04-25 08:51:36.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/appnp.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     5330 2022-04-25 08:51:36.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/chebynet.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     4654 2022-07-04 06:29:06.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/gat.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)    12223 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/gcn.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1138 2022-04-25 08:51:36.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/gin.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)    12713 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/graph_sage.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1835 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/le_conv.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     2235 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/sgc.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     3915 2022-04-25 08:51:36.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/ssgc.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1825 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/nn/conv/tagcn.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/nn/kernel/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)        0 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/kernel/__init__.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     2366 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/kernel/map_reduce.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1355 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/kernel/segment.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/nn/pool/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)        0 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/pool/__init__.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     6082 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/pool/asap.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     7635 2022-04-25 08:51:36.000000 tf_geometric-0.1.5/tf_geometric/nn/pool/cluster_pool.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     2058 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/pool/common_pool.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     5244 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/pool/diff_pool.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)    11576 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/pool/min_cut_pool.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     2067 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/pool/sag_pool.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1648 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/pool/set2set.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     1584 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/pool/sort_pool.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     3241 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/pool/topk_pool.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/nn/sampling/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)        0 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/sampling/__init__.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     2070 2021-04-23 12:34:58.000000 tf_geometric-0.1.5/tf_geometric/nn/sampling/drop_edge.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric/utils/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)       16 2021-11-14 20:21:41.000000 tf_geometric-0.1.5/tf_geometric/utils/__init__.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)      668 2021-08-18 07:29:22.000000 tf_geometric-0.1.5/tf_geometric/utils/data_utils.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)    37303 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/utils/graph_utils.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     3039 2022-12-27 07:45:01.000000 tf_geometric-0.1.5/tf_geometric/utils/tf_sparse_utils.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)      703 2021-07-31 07:17:00.000000 tf_geometric-0.1.5/tf_geometric/utils/tf_utils.py
--rw-rw-r--   0 hujun     (1002) hujun     (1003)      533 2021-11-16 16:45:07.000000 tf_geometric-0.1.5/tf_geometric/utils/union_utils.py
-drwxrwxr-x   0 hujun     (1002) hujun     (1003)        0 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric.egg-info/
--rw-rw-r--   0 hujun     (1002) hujun     (1003)    14922 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric.egg-info/PKG-INFO
--rw-rw-r--   0 hujun     (1002) hujun     (1003)     3006 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric.egg-info/SOURCES.txt
--rw-rw-r--   0 hujun     (1002) hujun     (1003)        1 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric.egg-info/dependency_links.txt
--rw-rw-r--   0 hujun     (1002) hujun     (1003)      235 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric.egg-info/requires.txt
--rw-rw-r--   0 hujun     (1002) hujun     (1003)       13 2022-12-27 08:17:13.000000 tf_geometric-0.1.5/tf_geometric.egg-info/top_level.txt
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/
+-rw-rw-r--   0 tf        (1000) tf        (1000)    35149 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/LICENSE
+-rw-rw-r--   0 tf        (1000) tf        (1000)    14902 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/PKG-INFO
+-rw-rw-r--   0 tf        (1000) tf        (1000)    14449 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/README.rst
+-rw-rw-r--   0 tf        (1000) tf        (1000)       38 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/setup.cfg
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1186 2023-05-26 09:13:12.000000 tf_geometric-0.1.6/setup.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/test/
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1131 2023-05-26 09:12:52.000000 tf_geometric-0.1.6/test/test_hetero_batch_graph.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/
+-rw-rw-r--   0 tf        (1000) tf        (1000)      337 2023-05-26 08:43:00.000000 tf_geometric-0.1.6/tf_geometric/__init__.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/data/
+-rw-rw-r--   0 tf        (1000) tf        (1000)        0 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/data/__init__.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     3388 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/data/dataset.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)    39375 2023-05-26 09:12:22.000000 tf_geometric-0.1.6/tf_geometric/data/graph.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/datasets/
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1150 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/__init__.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1804 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/abnormal.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1226 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/amazon_electronics.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1136 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/blog_catalog.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1187 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/coauthor.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1312 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/csr_npz.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     9556 2023-05-26 08:42:27.000000 tf_geometric-0.1.6/tf_geometric/datasets/hgb.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     5437 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/model_net.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     4510 2023-05-26 08:42:27.000000 tf_geometric-0.1.6/tf_geometric/datasets/nars_academic.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1777 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/ogb.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     5286 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/planetoid.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     2487 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/ppi.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     2344 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/reddit.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     6999 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/datasets/tu.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/layers/
+-rw-rw-r--   0 tf        (1000) tf        (1000)      767 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/__init__.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/
+-rw-rw-r--   0 tf        (1000) tf        (1000)        0 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/__init__.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     5809 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/appnp.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     4982 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/chebynet.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     4372 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/gat.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     7213 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/gcn.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1249 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/gin.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)    16888 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/graph_sage.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     3692 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/le_conv.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     4787 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/sgc.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     6064 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/ssgc.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     4913 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/conv/tagcn.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/layers/kernel/
+-rw-rw-r--   0 tf        (1000) tf        (1000)        0 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/kernel/__init__.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1152 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/kernel/map_reduce.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/layers/pool/
+-rw-rw-r--   0 tf        (1000) tf        (1000)        0 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/pool/__init__.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     5274 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/pool/asap.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1081 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/pool/common_pool.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     2488 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/pool/diff_pool.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     3655 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/pool/min_cut_pool.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1519 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/pool/sag_pool.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1118 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/pool/set2set.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1316 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/pool/sort_pool.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/layers/sampling/
+-rw-rw-r--   0 tf        (1000) tf        (1000)        0 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/sampling/__init__.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)      994 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/layers/sampling/drop_edge.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/nn/
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1242 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/__init__.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/
+-rw-rw-r--   0 tf        (1000) tf        (1000)        0 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/__init__.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     3826 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/appnp.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     5330 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/chebynet.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     4654 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/gat.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)    12223 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/gcn.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1138 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/gin.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)    12761 2023-05-26 06:00:09.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/graph_sage.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1835 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/le_conv.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     2235 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/sgc.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     3915 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/ssgc.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1825 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/conv/tagcn.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/nn/kernel/
+-rw-rw-r--   0 tf        (1000) tf        (1000)        0 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/kernel/__init__.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     2366 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/kernel/map_reduce.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1355 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/kernel/segment.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/nn/pool/
+-rw-rw-r--   0 tf        (1000) tf        (1000)        0 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/pool/__init__.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     6082 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/pool/asap.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     7635 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/pool/cluster_pool.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     2058 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/pool/common_pool.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     5244 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/pool/diff_pool.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)    11576 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/pool/min_cut_pool.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     2067 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/pool/sag_pool.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1648 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/pool/set2set.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     1584 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/pool/sort_pool.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     3241 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/pool/topk_pool.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/nn/sampling/
+-rw-rw-r--   0 tf        (1000) tf        (1000)        0 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/sampling/__init__.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     2070 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/nn/sampling/drop_edge.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric/utils/
+-rw-rw-r--   0 tf        (1000) tf        (1000)       16 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/utils/__init__.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)      668 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/utils/data_utils.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)    37303 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/utils/graph_utils.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)     3039 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/utils/tf_sparse_utils.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)      703 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/utils/tf_utils.py
+-rw-rw-r--   0 tf        (1000) tf        (1000)      533 2023-05-26 05:40:40.000000 tf_geometric-0.1.6/tf_geometric/utils/union_utils.py
+drwxrwxr-x   0 tf        (1000) tf        (1000)        0 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric.egg-info/
+-rw-rw-r--   0 tf        (1000) tf        (1000)    14902 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric.egg-info/PKG-INFO
+-rw-rw-r--   0 tf        (1000) tf        (1000)     2778 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric.egg-info/SOURCES.txt
+-rw-rw-r--   0 tf        (1000) tf        (1000)        1 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric.egg-info/dependency_links.txt
+-rw-rw-r--   0 tf        (1000) tf        (1000)      235 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric.egg-info/requires.txt
+-rw-rw-r--   0 tf        (1000) tf        (1000)       13 2023-05-26 09:14:13.000000 tf_geometric-0.1.6/tf_geometric.egg-info/top_level.txt
```

### Comparing `tf_geometric-0.1.5/LICENSE` & `tf_geometric-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/PKG-INFO` & `tf_geometric-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tf_geometric
-Version: 0.1.5
+Version: 0.1.6
 Summary: Efficient and Friendly Graph Neural Network Library for TensorFlow 1.x and 2.x.
 Home-page: https://github.com/CrawlScript/tf_geometric
 Author: Jun Hu
 Author-email: hujunxianligong@gmail.com
 License: GNU General Public License v3.0 (See LICENSE)
-Platform: UNKNOWN
 Requires-Python: >3.5.0
 Provides-Extra: tf1-cpu
 Provides-Extra: tf1-gpu
 Provides-Extra: tf2-cpu
 Provides-Extra: tf2-gpu
 License-File: LICENSE
 
@@ -382,9 +381,7 @@
 Related Projects
 ----------------
 
 
 * **tf_sparse:** We develop `TensorFlow Sparse (tf_sparse) <https://github.com/CrawlScript/tf_sparse>`_ to implement efficient and elegant 
   sparse TensorFlow operations for tf_geometric. URL: `https://github.com/CrawlScript/tf_sparse <https://github.com/CrawlScript/tf_sparse>`_.
 * **GRecX:** `GRecX <https://github.com/maenzhier/GRecX>`_ is an efficient and unified benchmark for GNN-based recommendation. URL: `https://github.com/maenzhier/GRecX <https://github.com/maenzhier/GRecX>`_.
-
-
```

### Comparing `tf_geometric-0.1.5/README.rst` & `tf_geometric-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/setup.py` & `tf_geometric-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name="tf_geometric",
     python_requires='>3.5.0',
-    version="0.1.5",
+    version="0.1.6",
     author="Jun Hu",
     author_email="hujunxianligong@gmail.com",
     packages=find_packages(
         exclude=[
             'benchmarks',
             'data',
             'demo',
```

### Comparing `tf_geometric-0.1.5/tf_geometric/data/dataset.py` & `tf_geometric-0.1.6/tf_geometric/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/data/graph.py` & `tf_geometric-0.1.6/tf_geometric/data/graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # coding=utf-8
+from itertools import chain
 import types
+from typing import List
 import warnings
 
 import tensorflow as tf
 import numpy as np
 import tf_sparse as tfs
 
 from tf_geometric.utils.graph_utils import convert_edge_to_directed, compute_edge_mask_by_node_index
@@ -614,58 +616,69 @@
         warnings.warn(
             "'BatchGraph.convert_edge_to_directed(self, merge_mode)' is deprecated, use 'BatchGraph.to_directed(inplace=True)' instead",
             DeprecationWarning)
 
         return self.to_directed(merge_mode, inplace=True)
 
 
-class HeteroDictGraph(object):
+class HeteroGraph(object):
 
     def __init__(self, x_dict=None, edge_index_dict=None, y_dict=None, edge_weight_dict=None):
         if x_dict is None:
             x_dict = {}
 
         if edge_index_dict is None:
             edge_index_dict = {}
 
         if y_dict is None:
             y_dict = {}
 
         if edge_weight_dict is None:
             edge_weight_dict = {}
 
-        self.x_dict = {node_type: Graph.cast_x(x) for node_type, x in x_dict.items()}
-        self.edge_index_dict = {edge_type: Graph.cast_edge_index(edge_index)
-                                for edge_type, edge_index in edge_index_dict.items()}
+        self.x_dict = {ntype: Graph.cast_x(x) for ntype, x in x_dict.items()}
+        self.edge_index_dict = {etype: Graph.cast_edge_index(edge_index)
+                                for etype, edge_index in edge_index_dict.items()}
         self.y_dict = {y_type: Graph.cast_y(y) for y_type, y in y_dict.items()}
-        self.edge_weight_dict = {edge_type: Graph.cast_edge_weight(edge_weight)
-                                 for edge_type, edge_weight in edge_weight_dict}
+        self.edge_weight_dict = {etype: Graph.cast_edge_weight(edge_weight)
+                                 for etype, edge_weight in edge_weight_dict}
 
         self.cache = {}
 
-    def num_nodes(self, node_type=None):
-        if node_type is not None:
-            return tfs.shape(self.x_dict[node_type])[0]
+    
+    @property
+    def ntypes(self):
+        return sorted(list(self.x_dict.keys()))
+
+
+    @property
+    def etypes(self):
+        return sorted(list(self.edge_index_dict.keys()))
+
+
+    def num_nodes(self, ntype=None):
+        if ntype is not None:
+            return tfs.shape(self.x_dict[ntype])[0]
         else:
-            return {node_type: self.num_nodes(node_type=node_type) for node_type in self.x_dict}
+            return {ntype: self.num_nodes(ntype=ntype) for ntype in self.x_dict}
 
-    def num_edges(self, edge_type=None):
-        if edge_type is not None:
-            return tf.shape(self.edge_index_dict[edge_type])[1]
+    def num_edges(self, etype=None):
+        if etype is not None:
+            return tf.shape(self.edge_index_dict[etype])[1]
         else:
-            return {edge_type: self.num_edges(edge_type) for edge_type in self.edge_index_dict}
+            return {etype: self.num_edges(etype) for etype in self.edge_index_dict}
 
     def get_shape_desc(self):
 
         x_shape_desc_dict = {
-            node_type: _get_shape(x) for node_type, x in self.x_dict.items()
+            ntype: _get_shape(x) for ntype, x in self.x_dict.items()
         }
 
         edge_index_shape_desc_dict = {
-            edge_type: _get_shape(edge_index) for edge_type, edge_index in self.edge_index_dict.items()
+            etype: _get_shape(edge_index) for etype, edge_index in self.edge_index_dict.items()
         }
 
         y_shape_desc_dict = {
             y_type: _get_shape(y) for y_type, y in self.y_dict.items()
         }
 
         return "HeteroGraph Shape: \n\tx => {}\n\tedge_index => {}\n\ty => {}".format(
@@ -674,32 +687,367 @@
 
     def add_reversed_edges(self, reverse_prefix="r.", inplace=False):
         """
         """
         new_edge_index_dict = {**self.edge_index_dict}
         new_edge_weight_dict = {**self.edge_weight_dict}
 
-        for edge_type, edge_index in self.edge_index_dict.items():
-            edge_weight = self.edge_weight_dict[edge_type] if edge_type in self.edge_weight_dict else None
-            reversed_edge_type = (edge_type[2], "{}{}".format(reverse_prefix, edge_type[1]), edge_type[0])
+        for etype, edge_index in self.edge_index_dict.items():
+            edge_weight = self.edge_weight_dict[etype] if etype in self.edge_weight_dict else None
+            reversed_etype = (etype[2], "{}{}".format(reverse_prefix, etype[1]), etype[0])
 
             if tf.is_tensor(edge_index):
                 reversed_edge_index = tf.stack([edge_index[1], edge_index[0]], axis=0)
             else:
                 reversed_edge_index = np.stack([edge_index[1], edge_index[0]], axis=0)
 
-            new_edge_index_dict[reversed_edge_type] = reversed_edge_index
+            new_edge_index_dict[reversed_etype] = reversed_edge_index
             if edge_weight is not None:
-                new_edge_weight_dict[reversed_edge_type] = edge_weight
+                new_edge_weight_dict[reversed_etype] = edge_weight
 
         if inplace:
             self.edge_index_dict, self.edge_weight_dict = new_edge_index_dict, new_edge_weight_dict
             return self
         else:
-            return HeteroDictGraph(self.x_dict, new_edge_index_dict, y_dict=self.y_dict,
+            return HeteroGraph(self.x_dict, new_edge_index_dict, y_dict=self.y_dict,
                                    edge_weight_dict=new_edge_weight_dict)
 
+    
+    def _inplace_convert_data_to_tensor(self, keys):
+        for key in keys:
+            data = getattr(self, key)
+
+            if isinstance(data, dict):
+                data = {k: tf.convert_to_tensor(v) if (v is not None and not tf.is_tensor(v) and not isinstance(v, types.FunctionType)) else v 
+                        for k, v in data.items()}
+                setattr(self, key, data)
+            else:
+                if data is not None and not tf.is_tensor(data) and not isinstance(data, types.FunctionType):
+                    setattr(self, key, tf.convert_to_tensor(data))
+
+        return self
+
+    
     def __str__(self):
         return self.get_shape_desc()
 
     def __repr__(self):
         return self.__str__()
+
+
+
+
+
+
+class HeteroBatchGraph(HeteroGraph):
+
+    def __init__(self, x_dict=None, edge_index_dict=None, node_graph_index_dict=None, edge_graph_index_dict=None,
+                 y_dict=None, edge_weight_dict=None, graphs=None):
+
+        super().__init__(x_dict, edge_index_dict, y_dict=y_dict, edge_weight_dict=edge_weight_dict)
+        self.node_graph_index_dict = node_graph_index_dict
+        self.edge_graph_index_dict = edge_graph_index_dict
+        self.graphs = graphs
+
+    @property
+    def num_graphs(self):
+
+        is_tensor = tf.is_tensor(list(self.node_graph_index_dict.values())[0])
+
+        num_graphs_list = [
+            tf.reduce_max(node_graph_index) + 1
+            for node_graph_index in self.node_graph_index_dict.values()
+        ]
+
+        num_graphs = tf.reduce_max(tf.stack(num_graphs_list))
+
+        if tf.executing_eagerly() and not is_tensor:
+            return num_graphs.numpy()
+        else:
+            return num_graphs
+            
+            
+
+    # def reorder(self):
+    #     node_sort_index = tf.argsort(self.node_graph_index)
+    #     node_graph_index = tf.gather(self.node_graph_index, node_sort_index)
+    #     x = tf.gather(self.x, node_sort_index)
+    #     if self.y is None:
+    #         y = None
+    #     else:
+    #         y = tf.gather(self.y, node_sort_index)
+
+    #     edge_sort_index = tf.argsort(self.edge_graph_index)
+    #     edge_graph_index = tf.gather(self.edge_graph_index, edge_sort_index)
+    #     edge_index = tf.gather(self.edge_index, edge_sort_index, axis=1)
+
+    #     if self.edge_weight is None:
+    #         edge_weight = None
+    #     else:
+    #         edge_weight = tf.gather(self.edge_weight, edge_sort_index)
+
+    #     return BatchGraph(x, edge_index, node_graph_index, edge_graph_index, y=y, edge_weight=edge_weight)
+
+
+    # def to_graphs(self):
+    #     batch_graph = self.reorder()
+    #     # num_nodes_list = tf.math.segment_sum(tf.ones([self.num_nodes]), self.node_graph_index)
+    #     num_graphs = batch_graph.num_graphs
+    #     num_nodes_list = tf.math.unsorted_segment_sum(tf.ones([batch_graph.num_nodes]), batch_graph.node_graph_index, num_graphs)
+
+    #     num_nodes_before_graph = tf.concat([
+    #         tf.zeros([1]),
+    #         tf.math.cumsum(num_nodes_list)
+    #     ], axis=0).numpy().astype(np.int32).tolist()
+
+    #     # num_edges_list = tf.math.segment_sum(tf.ones([self.num_edges]), self.edge_graph_index)
+    #     num_edges_list = tf.math.unsorted_segment_sum(tf.ones([batch_graph.num_edges]), batch_graph.edge_graph_index, num_graphs)
+    #     num_edges_before_graph = tf.concat([
+    #         tf.zeros([1]),
+    #         tf.math.cumsum(num_edges_list)
+    #     ], axis=0).numpy().astype(np.int32).tolist()
+
+    #     graphs = []
+    #     for i in range(batch_graph.num_graphs):
+    #         if isinstance(batch_graph.x, tf.sparse.SparseTensor):
+    #             x = tf.sparse.slice(
+    #                 batch_graph.x,
+    #                 [num_nodes_before_graph[i], 0],
+    #                 [num_nodes_before_graph[i + 1] - num_nodes_before_graph[i], tf.shape(batch_graph.x)[-1]]
+    #             )
+    #         else:
+    #             x = batch_graph.x[num_nodes_before_graph[i]: num_nodes_before_graph[i + 1]]
+
+    #         if batch_graph.y is None:
+    #             y = None
+    #         else:
+    #             y = batch_graph.y[num_nodes_before_graph[i]: num_nodes_before_graph[i + 1]]
+
+    #         edge_index = batch_graph.edge_index[:, num_edges_before_graph[i]:num_edges_before_graph[i + 1]] - \
+    #                      num_nodes_before_graph[i]
+
+    #         if batch_graph.edge_weight is None:
+    #             edge_weight = None
+    #         else:
+    #             edge_weight = batch_graph.edge_weight[num_edges_before_graph[i]:num_edges_before_graph[i + 1]]
+
+    #         graph = Graph(x=x, edge_index=edge_index, y=y, edge_weight=edge_weight)
+    #         graphs.append(graph)
+    #     return graphs
+
+    @classmethod
+    def from_graphs(cls, graphs):
+
+        node_graph_index_dict = HeteroBatchGraph.build_node_graph_index_dict(graphs)
+        edge_graph_index_dict = HeteroBatchGraph.build_edge_graph_index_dict(graphs)
+
+        x_dict = HeteroBatchGraph.build_x_dict(graphs)
+        edge_index_dict = HeteroBatchGraph.build_edge_index_dict(graphs)
+        y_dict = HeteroBatchGraph.build_y_dict(graphs)
+        edge_weight_dict = HeteroBatchGraph.build_edge_weight_dict(graphs)
+
+        return HeteroBatchGraph(x_dict=x_dict, edge_index_dict=edge_index_dict,
+                          node_graph_index_dict=node_graph_index_dict, edge_graph_index_dict=edge_graph_index_dict,
+                          graphs=graphs, y_dict=y_dict, edge_weight_dict=edge_weight_dict)
+
+    @classmethod
+    def build_node_graph_index_dict(cls, graphs: List[HeteroGraph]):
+        is_tensor = tf.is_tensor(list(graphs[0].edge_index_dict.values())[0])
+
+        ntypes = list(set(chain(*[graph.ntypes for graph in graphs])))
+        node_graph_index_list_dict = {
+            ntype: [] for ntype in ntypes
+        }
+
+        for i, graph in enumerate(graphs):
+            for ntype in graph.ntypes:
+                node_graph_index_list_dict[ntype].append(tf.fill([graph.num_nodes(ntype=ntype)], i))
+
+
+        node_graph_index_dict = {
+            ntype: tf.cast(tf.concat(node_graph_index_list, axis=0), tf.int32)
+            for ntype, node_graph_index_list in node_graph_index_list_dict.items()
+        }
+
+        if tf.executing_eagerly() and not is_tensor:
+            node_graph_index_dict = {
+                ntype: node_graph_index.numpy()
+                for ntype, node_graph_index in node_graph_index_dict.items()
+            }
+
+        return node_graph_index_dict
+    
+
+    @classmethod
+    def build_edge_graph_index_dict(cls, graphs):
+
+        is_tensor = tf.is_tensor(list(graphs[0].edge_index_dict.values())[0])
+        etypes = list(set(chain(*[graph.etypes for graph in graphs])))
+
+        edge_graph_index_list_dict = {etype: [] for etype in etypes}
+
+        for i, graph in enumerate(graphs):
+            for etype in graph.etypes:
+                edge_graph_index_list_dict[etype].append(tf.fill([graph.num_edges(etype=etype)], i))
+
+
+        edge_graph_index_dict = {
+            etype: tf.cast(tf.concat(edge_graph_index_list, axis=0), tf.int32)
+            for etype, edge_graph_index_list in edge_graph_index_list_dict.items()
+        }
+
+        if tf.executing_eagerly() and not is_tensor:
+            edge_graph_index_dict = {
+                etype: edge_graph_index.numpy()
+                for etype, edge_graph_index in edge_graph_index_dict.items()
+            }
+
+        return edge_graph_index_dict
+
+
+    @classmethod
+    def build_x_dict(cls, graphs: List[HeteroGraph]):
+        ntypes = list(set(chain(*[graph.ntypes for graph in graphs])))
+
+        x_dict = {}
+
+        for ntype in ntypes:
+            x_list = [
+                graph.x_dict[ntype] if ntype in graph.x_dict else None
+                for graph in graphs 
+            ]
+
+            first_x = x_list[0]
+            if tf.is_tensor(first_x):
+                if isinstance(first_x, tfs.SparseMatrix):
+                    x = tfs.concat(x_list, axis=0)
+                elif isinstance(first_x, tf.sparse.SparseTensor):
+                    x = tf.sparse.concat(0, x_list)
+                else:
+                    x = tf.concat(x_list, axis=0)
+            else:
+                x = np.concatenate(x_list, axis=0)
+
+            x_dict[ntype] = x
+
+        return x_dict
+
+
+
+
+    @classmethod
+    def build_edge_index_dict(cls, graphs):
+        ntypes = list(set(chain(*[graph.ntypes for graph in graphs])))
+        num_history_nodes_dict = {ntype: 0 for ntype in ntypes}
+
+        etypes = list(set(chain(*[graph.etypes for graph in graphs])))
+        edge_index_list_dict = {etype: [] for etype in etypes}
+
+        is_tensor = tf.is_tensor(list(graphs[0].edge_index_dict.values())[0])
+        
+        for _, graph in enumerate(graphs):
+            for etype, edge_index in graph.edge_index_dict.items():
+                row, col = edge_index[0], edge_index[1]
+            
+                new_edge_index = tf.stack([
+                    row + num_history_nodes_dict[etype[0]],
+                    col + num_history_nodes_dict[etype[-1]]
+                ], axis=0)
+
+                edge_index_list_dict[etype].append(new_edge_index)
+
+            for ntype in graph.ntypes:
+                num_history_nodes_dict[ntype] += graph.num_nodes(ntype=ntype)
+
+        edge_index_dict = {
+            etype: tf.concat(edge_index_list, axis=1)
+            for etype, edge_index_list in edge_index_list_dict.items()
+        }
+
+        if tf.executing_eagerly() and not is_tensor:
+            edge_index_dict = {
+                etype: edge_index.numpy()
+                for etype, edge_index in edge_index_dict.items()
+            }
+
+        return edge_index_dict
+
+
+    @classmethod
+    def build_edge_weight_dict(cls, graphs: List[HeteroGraph]):
+        if graphs[0].edge_weight_dict is None:
+            return None
+        
+        if len(graphs[0].edge_weight_dict) == 0:
+            return {}
+        
+        is_tensor = tf.is_tensor(list(graphs[0].edge_weight_dict.values())[0])
+
+        etypes = list(set(chain(*[graph.etypes for graph in graphs])))
+        edge_weight_list_dict = {etype: [] for etype in etypes}
+
+        for graph in graphs:
+            for etype, edge_weight in graph.edge_weight_dict.items():
+                edge_weight_list_dict[etype].append(edge_weight)
+
+        edge_weight_dict = {
+            etype: tf.concat(edge_weight_list, axis=0)
+            for etype, edge_weight_list in edge_weight_list_dict.items()
+        }
+
+        if tf.executing_eagerly() and not is_tensor:
+            edge_weight_dict = {
+                etype: edge_weight.numpy()
+                for etype, edge_weight in edge_weight_dict.items()
+            }
+
+        return edge_weight_dict
+
+
+    @classmethod
+    def build_y_dict(cls, graphs):
+
+        if graphs[0].y_dict is None:
+            return None
+        
+        if len(graphs[0].y_dict) == 0:
+            return {}
+        
+        y_types = list(set(chain(*[graph.y_dict.keys() for graph in graphs])))
+
+        is_tensor = tf.is_tensor(list(graphs[0].y_dict.values())[0])
+
+        y_list_dict = {y_type: [] for y_type in y_types}
+        
+        for graph in graphs:
+            for y_type, y in graph.y_dict.items():
+                y_list_dict[y_type].append(y)
+
+        y_dict = {
+            y_type: tf.concat(y_list, axis=0)
+            for y_type, y_list in y_list_dict.items()
+        }
+
+        if tf.executing_eagerly() and not is_tensor:
+            y_dict = {
+                y_type: y.numpy()
+                for y_type, y in y_dict.items()
+            }
+
+        return y_dict
+
+
+    def convert_data_to_tensor(self, inplace=False):
+        """
+        Convert all graph data into Tensors. All corresponding properties will be replaces by their Tensor versions.
+
+        :return: The Graph object itself.
+        """
+        if inplace:
+            graph = self
+        else:
+            graph = HeteroBatchGraph(x_dict=self.x_dict, edge_index_dict=self.edge_index_dict,
+                          node_graph_index_dict=self.node_graph_index_dict, edge_graph_index_dict=self.edge_graph_index_dict,
+                          graphs=self.graphs, y_dict=self.y_dict, edge_weight_dict=self.edge_weight_dict)
+        return graph._inplace_convert_data_to_tensor(["x_dict", "edge_index_dict", "edge_weight_dict", "y_dict",
+                                                    "node_graph_index_dict", "edge_graph_index_dict"])
+
```

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/__init__.py` & `tf_geometric-0.1.6/tf_geometric/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/abnormal.py` & `tf_geometric-0.1.6/tf_geometric/datasets/abnormal.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/amazon_electronics.py` & `tf_geometric-0.1.6/tf_geometric/datasets/amazon_electronics.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/blog_catalog.py` & `tf_geometric-0.1.6/tf_geometric/datasets/blog_catalog.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/coauthor.py` & `tf_geometric-0.1.6/tf_geometric/datasets/coauthor.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/csr_npz.py` & `tf_geometric-0.1.6/tf_geometric/datasets/csr_npz.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/hgb.py` & `tf_geometric-0.1.6/tf_geometric/datasets/hgb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding=utf-8
 import os.path
 import json
 from collections import defaultdict
 import numpy as np
-from tf_geometric.data.graph import HeteroDictGraph
+from tf_geometric.data.graph import HeteroGraph
 from tf_geometric.data.dataset import DownloadableDataset
 
 
 class HGBDataset(DownloadableDataset):
 
     def __init__(self, dataset_name, dataset_root_path=None):
         """
@@ -193,15 +193,15 @@
         #         for v in y[3].split(','):
         #             data[n_type].y[n_id, int(v)] = 1
         #     else:
         #         data[n_type].y[n_id] = int(y[3])
         #     data[n_type].test_mask[n_id] = True
 
 
-        hetero_graph = HeteroDictGraph(x_dict=x_dict,
+        hetero_graph = HeteroGraph(x_dict=x_dict,
                                        edge_index_dict=edge_index_dict,
                                        y_dict=y_dict,
                                        edge_weight_dict=edge_weight_dict)
 
         return hetero_graph, train_mask_dict, test_mask_dict
```

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/model_net.py` & `tf_geometric-0.1.6/tf_geometric/datasets/model_net.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/nars_academic.py` & `tf_geometric-0.1.6/tf_geometric/datasets/nars_academic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
 import os.path
 import json
 from collections import defaultdict
 import numpy as np
 from scipy.io import loadmat
 
-from tf_geometric.data.graph import HeteroDictGraph
+from tf_geometric.data.graph import HeteroGraph
 from tf_geometric.data.dataset import DownloadableDataset
 
 
 class _NARSAcademicDataset(DownloadableDataset):
 
     def __init__(self, dataset_name, dataset_root_path=None):
         """
@@ -105,15 +105,15 @@
             float_mask[pc_c_mask] = np.random.permutation(np.linspace(0, 1, pc_c_mask.sum()))
         train_index = np.where(float_mask <= 0.2)[0]
         valid_index = np.where((float_mask > 0.2) & (float_mask <= 0.3))[0]
         test_index = np.where(float_mask > 0.3)[0]
 
         # hg.nodes["paper"].data["feat"] = features
 
-        hetero_graph = HeteroDictGraph(x_dict=x_dict, edge_index_dict=edge_index_dict, y_dict=y_dict)
+        hetero_graph = HeteroGraph(x_dict=x_dict, edge_index_dict=edge_index_dict, y_dict=y_dict)
 
         target_node_type = "paper"
 
         return hetero_graph, target_node_type, (train_index, valid_index, test_index)
 
         # return hg, labels, num_classes, train_idx, val_idx, test_idx
```

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/ogb.py` & `tf_geometric-0.1.6/tf_geometric/datasets/ogb.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/planetoid.py` & `tf_geometric-0.1.6/tf_geometric/datasets/planetoid.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/ppi.py` & `tf_geometric-0.1.6/tf_geometric/datasets/ppi.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/reddit.py` & `tf_geometric-0.1.6/tf_geometric/datasets/reddit.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/datasets/tu.py` & `tf_geometric-0.1.6/tf_geometric/datasets/tu.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/__init__.py` & `tf_geometric-0.1.6/tf_geometric/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/conv/appnp.py` & `tf_geometric-0.1.6/tf_geometric/layers/conv/appnp.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/conv/chebynet.py` & `tf_geometric-0.1.6/tf_geometric/layers/conv/chebynet.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/conv/gat.py` & `tf_geometric-0.1.6/tf_geometric/layers/conv/gat.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/conv/gcn.py` & `tf_geometric-0.1.6/tf_geometric/layers/conv/gcn.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/conv/gin.py` & `tf_geometric-0.1.6/tf_geometric/layers/conv/gin.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/conv/graph_sage.py` & `tf_geometric-0.1.6/tf_geometric/layers/conv/graph_sage.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/conv/le_conv.py` & `tf_geometric-0.1.6/tf_geometric/layers/conv/le_conv.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/conv/sgc.py` & `tf_geometric-0.1.6/tf_geometric/layers/conv/sgc.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/conv/ssgc.py` & `tf_geometric-0.1.6/tf_geometric/layers/conv/ssgc.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/conv/tagcn.py` & `tf_geometric-0.1.6/tf_geometric/layers/conv/tagcn.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/kernel/map_reduce.py` & `tf_geometric-0.1.6/tf_geometric/layers/kernel/map_reduce.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/pool/asap.py` & `tf_geometric-0.1.6/tf_geometric/layers/pool/asap.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/pool/common_pool.py` & `tf_geometric-0.1.6/tf_geometric/layers/pool/common_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/pool/diff_pool.py` & `tf_geometric-0.1.6/tf_geometric/layers/pool/diff_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/pool/min_cut_pool.py` & `tf_geometric-0.1.6/tf_geometric/layers/pool/min_cut_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/pool/sag_pool.py` & `tf_geometric-0.1.6/tf_geometric/layers/pool/sag_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/pool/set2set.py` & `tf_geometric-0.1.6/tf_geometric/layers/pool/set2set.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/pool/sort_pool.py` & `tf_geometric-0.1.6/tf_geometric/layers/pool/sort_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/layers/sampling/drop_edge.py` & `tf_geometric-0.1.6/tf_geometric/layers/sampling/drop_edge.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/__init__.py` & `tf_geometric-0.1.6/tf_geometric/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/conv/appnp.py` & `tf_geometric-0.1.6/tf_geometric/nn/conv/appnp.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/conv/chebynet.py` & `tf_geometric-0.1.6/tf_geometric/nn/conv/chebynet.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/conv/gat.py` & `tf_geometric-0.1.6/tf_geometric/nn/conv/gat.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/conv/gcn.py` & `tf_geometric-0.1.6/tf_geometric/nn/conv/gcn.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/conv/gin.py` & `tf_geometric-0.1.6/tf_geometric/nn/conv/gin.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/conv/graph_sage.py` & `tf_geometric-0.1.6/tf_geometric/nn/conv/graph_sage.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     :param edge_index: Tensor, shape: [2, num_edges], edge information
     :param edge_weight: Tensor or None, shape: [num_edges]
     :param self_kernel: Tensor, shape: [num_features, num_hidden_units], weight
     :param neighbor_kernel: Tensor, shape: [num_features, num_hidden_units], weight.
     :param bias: Tensor, shape: [num_output_features], bias
     :param activation: Activation function to use.
     :param normalize: If set to :obj:`True`, output features
-                will be :math:`\ell_2`-normalized, *i.e.*,
-                :math:`\frac{\mathbf{x}^{\prime}_i}
-                {\| \mathbf{x}^{\prime}_i \|_2}`.
+                will be :math:`\\ell_2`-normalized, *i.e.*,
+                :math:`\\frac{\\mathbf{x}^{\\prime}_i}
+                {\\| \\mathbf{x}^{\\prime}_i \\|_2}`.
                 (default: :obj:`False`)
     :return: Updated node features (x), shape: [num_nodes, num_output_features]
     """
     num_nodes = tf.shape(x)[0]
     # num_edges = tf.shape(edge_index)[1]
 
     row, col = edge_index[0], edge_index[1]
@@ -73,17 +73,17 @@
     :param edge_index: Tensor, shape: [2, num_edges], edge information
     :param edge_weight: Tensor or None, shape: [num_edges]
     :param self_kernel: Tensor, shape: [num_features, num_hidden_units], weight
     :param neighbor_kernel: Tensor, shape: [num_features, num_hidden_units], weight.
     :param bias: Tensor, shape: [num_output_features], bias
     :param activation: Activation function to use.
     :param normalize: If set to :obj:`True`, output features
-                will be :math:`\ell_2`-normalized, *i.e.*,
-                :math:`\frac{\mathbf{x}^{\prime}_i}
-                {\| \mathbf{x}^{\prime}_i \|_2}`.
+                will be :math:`\\ell_2`-normalized, *i.e.*,
+                :math:`\\frac{\\mathbf{x}^{\\prime}_i}
+                {\\| \\mathbf{x}^{\\prime}_i \\|_2}`.
                 (default: :obj:`False`)
     :return: Updated node features (x), shape: [num_nodes, num_output_features]
     """
     num_nodes = tf.shape(x)[0]
     # num_edges = tf.shape(edge_index)[1]
 
     row, col = edge_index[0], edge_index[1]
@@ -122,17 +122,17 @@
         :param x: Tensor, shape: [num_nodes, num_features], node features
         :param edge_index: Tensor, shape: [2, num_edges], edge information
         :param edge_weight: Tensor or None, shape: [num_edges]
         :param kernel: Tensor, shape: [num_features, num_output_features], weight
         :param bias: Tensor, shape: [num_output_features], bias
         :param activation: Activation function to use.
         :param normalize: If set to :obj:`True`, output features
-                will be :math:`\ell_2`-normalized, *i.e.*,
-                :math:`\frac{\mathbf{x}^{\prime}_i}
-                {\| \mathbf{x}^{\prime}_i \|_2}`.
+                will be :math:`\\ell_2`-normalized, *i.e.*,
+                :math:`\\frac{\\mathbf{x}^{\\prime}_i}
+                {\\| \\mathbf{x}^{\\prime}_i \\|_2}`.
                 (default: :obj:`False`)
         :param cache: A dict for caching A' for GCN. Different graph should not share the same cache dict.
         :return: Updated node features (x), shape: [num_nodes, num_output_features]
     """
     num_nodes = tf.shape(x)[0]
     num_edges = tf.shape(edge_index)[1]
 
@@ -173,17 +173,17 @@
     :param self_kernel: Tensor, shape: [num_features, num_hidden_units], weight.
     :param neighbor_mlp_kernel: Tensor, shape: [num_features, num_hidden_units]. weight.
     :param neighbor_kernel: Tensor, shape: [num_hidden_units, num_hidden_units], weight.
     :param neighbor_mlp_bias: Tensor, shape: [num_hidden_units * 2], bias
     :param bias: Tensor, shape: [num_output_features], bias.
     :param activation: Activation function to use.
     :param normalize: If set to :obj:`True`, output features
-                will be :math:`\ell_2`-normalized, *i.e.*,
-                :math:`\frac{\mathbf{x}^{\prime}_i}
-                {\| \mathbf{x}^{\prime}_i \|_2}`.
+                will be :math:`\\ell_2`-normalized, *i.e.*,
+                :math:`\\frac{\\mathbf{x}^{\\prime}_i}
+                {\\| \\mathbf{x}^{\\prime}_i \\|_2}`.
                 (default: :obj:`False`)
     :return: Updated node features (x), shape: [num_nodes, num_output_features]
     """
 
     num_nodes = tf.shape(x)[0]
     num_edges = tf.shape(edge_index)[1]
 
@@ -237,17 +237,17 @@
             :param self_kernel: Tensor, shape: [num_features, num_hidden_units], weight.
             :param neighbor_mlp_kernel: Tensor, shape: [num_features, num_hidden_units]. weight.
             :param neighbor_kernel: Tensor, shape: [num_hidden_units, num_hidden_units], weight.
             :param neighbor_mlp_bias: Tensor, shape: [num_hidden_units * 2], bias
             :param bias: Tensor, shape: [num_output_features], bias.
             :param activation: Activation function to use.
             :param normalize: If set to :obj:`True`, output features
-                        will be :math:`\ell_2`-normalized, *i.e.*,
-                        :math:`\frac{\mathbf{x}^{\prime}_i}
-                        {\| \mathbf{x}^{\prime}_i \|_2}`.
+                        will be :math:`\\ell_2`-normalized, *i.e.*,
+                        :math:`\\frac{\\mathbf{x}^{\\prime}_i}
+                        {\\| \\mathbf{x}^{\\prime}_i \\|_2}`.
                         (default: :obj:`False`)
             :return: Updated node features (x), shape: [num_nodes, num_output_features]
             """
     num_nodes = tf.shape(x)[0]
     num_edges = tf.shape(edge_index)[1]
 
     if edge_weight is not None:
@@ -297,17 +297,17 @@
     :param edge_index: Tensor, shape: [2, num_edges], edge information.
     :param lstm: Long Short-Term Merory.
     :param self_kernel: Tensor, shape: [num_features, num_hidden_units], weight.
     :param neighbor_kernel: Tensor, shape: [num_hidden_units, num_hidden_units], weight.
     :param bias: Tensor, shape: [num_output_features], bias.
     :param activation: Activation function to use.
     :param normalize: If set to :obj:`True`, output features
-                will be :math:`\ell_2`-normalized, *i.e.*,
-                :math:`\frac{\mathbf{x}^{\prime}_i}
-                {\| \mathbf{x}^{\prime}_i \|_2}`.
+                will be :math:`\\ell_2`-normalized, *i.e.*,
+                :math:`\\frac{\\mathbf{x}^{\\prime}_i}
+                {\\| \\mathbf{x}^{\\prime}_i \\|_2}`.
                 (default: :obj:`False`)
     :return: Updated node features (x), shape: [num_nodes, num_output_features]
     """
     num_nodes = tf.shape(x)[0]
     num_edges = tf.shape(edge_index)[1]
 
     row, col = edge_index[0], edge_index[1]
```

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/conv/le_conv.py` & `tf_geometric-0.1.6/tf_geometric/nn/conv/le_conv.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/conv/sgc.py` & `tf_geometric-0.1.6/tf_geometric/nn/conv/sgc.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/conv/ssgc.py` & `tf_geometric-0.1.6/tf_geometric/nn/conv/ssgc.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/conv/tagcn.py` & `tf_geometric-0.1.6/tf_geometric/nn/conv/tagcn.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/kernel/map_reduce.py` & `tf_geometric-0.1.6/tf_geometric/nn/kernel/map_reduce.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/kernel/segment.py` & `tf_geometric-0.1.6/tf_geometric/nn/kernel/segment.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/pool/asap.py` & `tf_geometric-0.1.6/tf_geometric/nn/pool/asap.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/pool/cluster_pool.py` & `tf_geometric-0.1.6/tf_geometric/nn/pool/cluster_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/pool/common_pool.py` & `tf_geometric-0.1.6/tf_geometric/nn/pool/common_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/pool/diff_pool.py` & `tf_geometric-0.1.6/tf_geometric/nn/pool/diff_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/pool/min_cut_pool.py` & `tf_geometric-0.1.6/tf_geometric/nn/pool/min_cut_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/pool/sag_pool.py` & `tf_geometric-0.1.6/tf_geometric/nn/pool/sag_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/pool/set2set.py` & `tf_geometric-0.1.6/tf_geometric/nn/pool/set2set.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/pool/sort_pool.py` & `tf_geometric-0.1.6/tf_geometric/nn/pool/sort_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/pool/topk_pool.py` & `tf_geometric-0.1.6/tf_geometric/nn/pool/topk_pool.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/nn/sampling/drop_edge.py` & `tf_geometric-0.1.6/tf_geometric/nn/sampling/drop_edge.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/utils/data_utils.py` & `tf_geometric-0.1.6/tf_geometric/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/utils/graph_utils.py` & `tf_geometric-0.1.6/tf_geometric/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/utils/tf_sparse_utils.py` & `tf_geometric-0.1.6/tf_geometric/utils/tf_sparse_utils.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/utils/tf_utils.py` & `tf_geometric-0.1.6/tf_geometric/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric/utils/union_utils.py` & `tf_geometric-0.1.6/tf_geometric/utils/union_utils.py`

 * *Files identical despite different names*

### Comparing `tf_geometric-0.1.5/tf_geometric.egg-info/PKG-INFO` & `tf_geometric-0.1.6/tf_geometric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tf-geometric
-Version: 0.1.5
+Version: 0.1.6
 Summary: Efficient and Friendly Graph Neural Network Library for TensorFlow 1.x and 2.x.
 Home-page: https://github.com/CrawlScript/tf_geometric
 Author: Jun Hu
 Author-email: hujunxianligong@gmail.com
 License: GNU General Public License v3.0 (See LICENSE)
-Platform: UNKNOWN
 Requires-Python: >3.5.0
 Provides-Extra: tf1-cpu
 Provides-Extra: tf1-gpu
 Provides-Extra: tf2-cpu
 Provides-Extra: tf2-gpu
 License-File: LICENSE
 
@@ -382,9 +381,7 @@
 Related Projects
 ----------------
 
 
 * **tf_sparse:** We develop `TensorFlow Sparse (tf_sparse) <https://github.com/CrawlScript/tf_sparse>`_ to implement efficient and elegant 
   sparse TensorFlow operations for tf_geometric. URL: `https://github.com/CrawlScript/tf_sparse <https://github.com/CrawlScript/tf_sparse>`_.
 * **GRecX:** `GRecX <https://github.com/maenzhier/GRecX>`_ is an efficient and unified benchmark for GNN-based recommendation. URL: `https://github.com/maenzhier/GRecX <https://github.com/maenzhier/GRecX>`_.
-
-
```

### Comparing `tf_geometric-0.1.5/tf_geometric.egg-info/SOURCES.txt` & `tf_geometric-0.1.6/tf_geometric.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,11 @@
 LICENSE
 README.rst
 setup.py
-test/test.py
-test/test_batch_graph.py
-test/test_blog_catalog.py
-test/test_gcn.py
-test/test_gcn_norm_edge.py
-test/test_num_edges.py
-test/test_ogb_speed.py
-test/test_ogb_speed2.py
-test/test_sparse_adj.py
-test/test_sparse_gat.py
-test/test_sparse_node_features.py
+test/test_hetero_batch_graph.py
 tf_geometric/__init__.py
 tf_geometric.egg-info/PKG-INFO
 tf_geometric.egg-info/SOURCES.txt
 tf_geometric.egg-info/dependency_links.txt
 tf_geometric.egg-info/requires.txt
 tf_geometric.egg-info/top_level.txt
 tf_geometric/data/__init__.py
```

