# Comparing `tmp/dprox-0.1.2.tar.gz` & `tmp/dprox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/hyper-pnp/submit/Delta-Prox/dist/.tmp-tnkyh1ex/dprox-0.1.2.tar", last modified: Fri May 26 06:24:32 2023, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/hyper-pnp/submit/Delta-Prox/dist/.tmp-otob2k3v/dprox-0.1.3.tar", last modified: Fri May 26 06:26:21 2023, max compression
```

## Comparing `dprox-0.1.2.tar` & `dprox-0.1.3.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      304 2023-05-26 06:24:32.000000 dprox-0.1.2/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3141 2023-05-22 07:49:24.000000 dprox-0.1.2/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      126 2023-05-26 05:55:22.000000 dprox-0.1.2/dprox/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/algo/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      276 2023-05-20 03:14:24.000000 dprox-0.1.2/dprox/algo/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3676 2023-05-24 07:18:47.000000 dprox-0.1.2/dprox/algo/admm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7654 2023-05-24 04:36:39.000000 dprox-0.1.2/dprox/algo/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      515 2023-05-20 03:14:24.000000 dprox-0.1.2/dprox/algo/hqs.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      685 2023-05-24 07:17:40.000000 dprox-0.1.2/dprox/algo/invert.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/algo/lp/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       63 2023-05-20 03:14:24.000000 dprox-0.1.2/dprox/algo/lp/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13337 2023-05-22 14:14:30.000000 dprox-0.1.2/dprox/algo/lp/solvers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6017 2023-05-20 03:14:24.000000 dprox-0.1.2/dprox/algo/lp/utils.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/algo/opt/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       41 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/opt/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1289 2023-05-13 14:56:20.000000 dprox-0.1.2/dprox/algo/opt/absorb.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2713 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/opt/equil.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2241 2023-05-22 07:49:41.000000 dprox-0.1.2/dprox/algo/opt/merge.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1074 2023-05-20 03:14:24.000000 dprox-0.1.2/dprox/algo/pc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1370 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/pgd.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4625 2023-05-24 07:18:27.000000 dprox-0.1.2/dprox/algo/problem.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/algo/special/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       72 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/special/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6866 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/special/deq.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/algo/special/deq_utils/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/special/deq_utils/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1863 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/special/deq_utils/jacobian.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1332 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/special/deq_utils/layer_utils.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11133 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/special/deq_utils/optimizations.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8090 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/special/deq_utils/radam.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13962 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/special/deq_utils/solvers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1688 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/special/unroll.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/algo/tune/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       23 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/tune/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12895 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/tune/autotune.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1850 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/tune/dpir.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      511 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/algo/tune/learnable.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/linalg/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-05-22 11:53:09.000000 dprox-0.1.2/dprox/linalg/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1785 2023-05-22 12:39:40.000000 dprox-0.1.2/dprox/linalg/custom.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/linalg/solve/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      410 2023-05-22 11:53:09.000000 dprox-0.1.2/dprox/linalg/solve/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6498 2023-05-22 14:14:30.000000 dprox-0.1.2/dprox/linalg/solve/cg.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9704 2023-05-22 14:14:30.000000 dprox-0.1.2/dprox/linalg/solve/minres.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3448 2023-05-22 14:14:30.000000 dprox-0.1.2/dprox/linalg/solve/plss.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/linop/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-10 14:07:17.000000 dprox-0.1.2/dprox/linop/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7440 2023-05-20 03:13:06.000000 dprox-0.1.2/dprox/linop/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2365 2023-05-24 07:38:28.000000 dprox-0.1.2/dprox/linop/blackbox.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    15084 2023-05-20 09:13:41.000000 dprox-0.1.2/dprox/linop/comp_graph.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      445 2023-05-20 03:13:06.000000 dprox-0.1.2/dprox/linop/constaints.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2882 2023-05-24 07:43:37.000000 dprox-0.1.2/dprox/linop/constant.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5480 2023-05-24 07:43:49.000000 dprox-0.1.2/dprox/linop/conv.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      464 2023-05-20 03:12:27.000000 dprox-0.1.2/dprox/linop/edge.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1219 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/linop/grad.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      489 2023-05-24 06:31:56.000000 dprox-0.1.2/dprox/linop/placeholder.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2580 2023-05-24 07:43:58.000000 dprox-0.1.2/dprox/linop/scale.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3459 2023-05-24 07:38:58.000000 dprox-0.1.2/dprox/linop/subsample.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3051 2023-05-24 07:44:13.000000 dprox-0.1.2/dprox/linop/sum.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2988 2023-05-24 07:44:22.000000 dprox-0.1.2/dprox/linop/variable.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3717 2023-05-24 07:44:41.000000 dprox-0.1.2/dprox/linop/vstack.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      285 2023-05-22 11:53:09.000000 dprox-0.1.2/dprox/proxfn/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2693 2023-05-20 01:26:10.000000 dprox-0.1.2/dprox/proxfn/base.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/fast/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/fast/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      711 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/fast/cs.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      884 2023-05-20 03:23:29.000000 dprox-0.1.2/dprox/proxfn/fast/csmri.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1721 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/fast/pr.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2328 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/fast/spi.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3925 2023-05-13 14:56:20.000000 dprox-0.1.2/dprox/proxfn/fast/sr.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/linalg/
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/linalg/solve/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5069 2023-05-20 03:14:24.000000 dprox-0.1.2/dprox/proxfn/linalg/solve/bicgstab.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1134 2023-05-20 03:14:24.000000 dprox-0.1.2/dprox/proxfn/linalg/solve/broyden.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6501 2023-05-20 03:14:24.000000 dprox-0.1.2/dprox/proxfn/linalg/solve/gmres.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1631 2023-05-20 03:14:24.000000 dprox-0.1.2/dprox/proxfn/linalg/solve/plss.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/nlm/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       32 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/nlm/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4758 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/nlm/nlm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      301 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/nlm/patch_nlm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      210 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/nonneg.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      606 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/norm.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/pnp/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       29 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      321 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      763 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3315 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/composite.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1694 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/TV_denoising.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/basicblock.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6167 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/network_dncnn.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4157 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    16619 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/network_unet.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      870 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3258 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3916 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5264 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5741 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      449 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12973 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4278 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3226 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      835 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/unet/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       22 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/unet/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12412 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/unet/unet.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7588 2023-05-20 02:09:19.000000 dprox-0.1.2/dprox/proxfn/pnp/denoisers/wrapper.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2902 2023-05-20 03:14:24.000000 dprox-0.1.2/dprox/proxfn/pnp/prior.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5751 2023-05-24 07:40:18.000000 dprox-0.1.2/dprox/proxfn/sum_square.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/proxfn/unrolling/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       33 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/unrolling/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13120 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/unrolling/dgu.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      482 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/proxfn/unrolling/prior.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/utils/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      173 2023-05-24 04:36:39.000000 dprox-0.1.2/dprox/utils/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1504 2023-05-24 04:36:39.000000 dprox-0.1.2/dprox/utils/containar.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/utils/examples/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-05-13 14:43:30.000000 dprox-0.1.2/dprox/utils/examples/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/utils/examples/csmri/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       82 2023-05-13 14:45:34.000000 dprox-0.1.2/dprox/utils/examples/csmri/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3011 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/utils/examples/csmri/common.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4146 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/utils/examples/csmri/dataset.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2083 2023-05-22 15:23:16.000000 dprox-0.1.2/dprox/utils/examples/csmri/misc.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/utils/examples/derain/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       40 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/utils/examples/derain/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2564 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/utils/examples/derain/custom_linop.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/utils/examples/energy_system/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      947 2023-05-20 03:14:24.000000 dprox-0.1.2/dprox/utils/examples/energy_system/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/utils/examples/optic/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       46 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/utils/examples/optic/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9960 2023-05-26 05:40:51.000000 dprox-0.1.2/dprox/utils/examples/optic/common.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    18268 2023-05-26 05:40:51.000000 dprox-0.1.2/dprox/utils/examples/optic/doe_model.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3063 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/utils/examples/optic/unet.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2488 2023-05-14 13:57:57.000000 dprox-0.1.2/dprox/utils/examples/restoration.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox/utils/init/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.2/dprox/utils/init/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4705 2023-05-24 04:36:39.000000 dprox-0.1.2/dprox/utils/init/mosaic.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      756 2023-05-24 04:36:39.000000 dprox-0.1.2/dprox/utils/init/sr.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5788 2023-05-26 05:40:51.000000 dprox-0.1.2/dprox/utils/io.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4630 2023-05-24 04:36:39.000000 dprox-0.1.2/dprox/utils/metrics.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4958 2023-05-24 06:20:38.000000 dprox-0.1.2/dprox/utils/misc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3978 2023-05-24 04:36:39.000000 dprox-0.1.2/dprox/utils/psf2otf.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      304 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4287 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      108 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        6 2023-05-26 06:24:32.000000 dprox-0.1.2/dprox.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-26 06:24:32.000000 dprox-0.1.2/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      656 2023-05-26 06:24:18.000000 dprox-0.1.2/setup.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:24:32.000000 dprox-0.1.2/tests/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2715 2023-05-20 03:13:06.000000 dprox-0.1.2/tests/test_algorithms.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1043 2023-05-24 07:09:33.000000 dprox-0.1.2/tests/test_derain.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      318 2023-05-22 14:14:30.000000 dprox-0.1.2/tests/test_energy_system.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1688 2023-05-23 08:23:24.000000 dprox-0.1.2/tests/test_inverse_problems.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      790 2023-05-24 07:49:26.000000 dprox-0.1.2/tests/test_jd23.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2586 2023-05-24 04:36:39.000000 dprox-0.1.2/tests/test_linear_solver.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3280 2023-05-22 11:53:09.000000 dprox-0.1.2/tests/test_linear_solver_grad.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6231 2023-05-24 08:13:09.000000 dprox-0.1.2/tests/test_linear_solver_torch.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2692 2023-05-20 03:13:06.000000 dprox-0.1.2/tests/test_linop.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      180 2023-05-20 03:13:06.000000 dprox-0.1.2/tests/test_linop_primitive.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1198 2023-05-24 04:36:39.000000 dprox-0.1.2/tests/test_ml_problems.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      304 2023-05-26 06:26:21.000000 dprox-0.1.3/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3141 2023-05-22 07:49:24.000000 dprox-0.1.3/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      126 2023-05-26 05:55:22.000000 dprox-0.1.3/dprox/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      276 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/algo/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3676 2023-05-24 07:18:47.000000 dprox-0.1.3/dprox/algo/admm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7654 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/algo/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      515 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/algo/hqs.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      685 2023-05-24 07:17:40.000000 dprox-0.1.3/dprox/algo/invert.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/lp/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       63 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/algo/lp/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13337 2023-05-22 14:14:30.000000 dprox-0.1.3/dprox/algo/lp/solvers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6017 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/algo/lp/utils.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/opt/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       41 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/opt/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1289 2023-05-13 14:56:20.000000 dprox-0.1.3/dprox/algo/opt/absorb.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2713 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/opt/equil.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2241 2023-05-22 07:49:41.000000 dprox-0.1.3/dprox/algo/opt/merge.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1074 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/algo/pc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1370 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/pgd.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4625 2023-05-24 07:18:27.000000 dprox-0.1.3/dprox/algo/problem.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/special/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       72 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6866 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/special/deq_utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1863 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/jacobian.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1332 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/layer_utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11133 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/optimizations.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8090 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/radam.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13962 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/solvers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1688 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/unroll.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/tune/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       23 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/tune/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12895 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/tune/autotune.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1850 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/tune/dpir.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      511 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/tune/learnable.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/linalg/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-05-22 11:53:09.000000 dprox-0.1.3/dprox/linalg/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1785 2023-05-22 12:39:40.000000 dprox-0.1.3/dprox/linalg/custom.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/linalg/solve/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      410 2023-05-22 11:53:09.000000 dprox-0.1.3/dprox/linalg/solve/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6498 2023-05-22 14:14:30.000000 dprox-0.1.3/dprox/linalg/solve/cg.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9704 2023-05-22 14:14:30.000000 dprox-0.1.3/dprox/linalg/solve/minres.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3448 2023-05-22 14:14:30.000000 dprox-0.1.3/dprox/linalg/solve/plss.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/linop/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-10 14:07:17.000000 dprox-0.1.3/dprox/linop/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7440 2023-05-20 03:13:06.000000 dprox-0.1.3/dprox/linop/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2365 2023-05-24 07:38:28.000000 dprox-0.1.3/dprox/linop/blackbox.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    15084 2023-05-20 09:13:41.000000 dprox-0.1.3/dprox/linop/comp_graph.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      445 2023-05-20 03:13:06.000000 dprox-0.1.3/dprox/linop/constaints.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2882 2023-05-24 07:43:37.000000 dprox-0.1.3/dprox/linop/constant.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5480 2023-05-24 07:43:49.000000 dprox-0.1.3/dprox/linop/conv.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      464 2023-05-20 03:12:27.000000 dprox-0.1.3/dprox/linop/edge.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1219 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/linop/grad.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      489 2023-05-24 06:31:56.000000 dprox-0.1.3/dprox/linop/placeholder.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2580 2023-05-24 07:43:58.000000 dprox-0.1.3/dprox/linop/scale.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3459 2023-05-24 07:38:58.000000 dprox-0.1.3/dprox/linop/subsample.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3051 2023-05-24 07:44:13.000000 dprox-0.1.3/dprox/linop/sum.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2988 2023-05-24 07:44:22.000000 dprox-0.1.3/dprox/linop/variable.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3717 2023-05-24 07:44:41.000000 dprox-0.1.3/dprox/linop/vstack.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      285 2023-05-22 11:53:09.000000 dprox-0.1.3/dprox/proxfn/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2693 2023-05-20 01:26:10.000000 dprox-0.1.3/dprox/proxfn/base.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/fast/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/fast/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      711 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/fast/cs.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      884 2023-05-20 03:23:29.000000 dprox-0.1.3/dprox/proxfn/fast/csmri.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1721 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/fast/pr.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2328 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/fast/spi.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3925 2023-05-13 14:56:20.000000 dprox-0.1.3/dprox/proxfn/fast/sr.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/linalg/
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/linalg/solve/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5069 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/proxfn/linalg/solve/bicgstab.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1134 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/proxfn/linalg/solve/broyden.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6501 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/proxfn/linalg/solve/gmres.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1631 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/proxfn/linalg/solve/plss.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/nlm/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       32 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/nlm/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4758 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/nlm/nlm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      301 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/nlm/patch_nlm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      210 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/nonneg.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      606 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/norm.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       29 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      321 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      763 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3315 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/composite.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1694 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/TV_denoising.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/basicblock.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6167 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_dncnn.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4157 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    16619 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_unet.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      870 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3258 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3916 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5264 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5741 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      449 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12973 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4278 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3226 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      835 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       22 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12412 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/unet.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7588 2023-05-20 02:09:19.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/wrapper.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2902 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/proxfn/pnp/prior.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5751 2023-05-24 07:40:18.000000 dprox-0.1.3/dprox/proxfn/sum_square.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/unrolling/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       33 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/unrolling/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13120 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/unrolling/dgu.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      482 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/unrolling/prior.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      173 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1504 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/containar.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/examples/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-05-13 14:43:30.000000 dprox-0.1.3/dprox/utils/examples/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/examples/csmri/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       82 2023-05-13 14:45:34.000000 dprox-0.1.3/dprox/utils/examples/csmri/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3011 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/csmri/common.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4146 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/csmri/dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2083 2023-05-22 15:23:16.000000 dprox-0.1.3/dprox/utils/examples/csmri/misc.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/examples/derain/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       40 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/derain/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2564 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/derain/custom_linop.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/examples/energy_system/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      947 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/utils/examples/energy_system/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/examples/optic/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       46 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/optic/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9960 2023-05-26 05:40:51.000000 dprox-0.1.3/dprox/utils/examples/optic/common.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    18268 2023-05-26 05:40:51.000000 dprox-0.1.3/dprox/utils/examples/optic/doe_model.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3063 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/optic/unet.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2488 2023-05-14 13:57:57.000000 dprox-0.1.3/dprox/utils/examples/restoration.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/init/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/init/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4705 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/init/mosaic.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      756 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/init/sr.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5788 2023-05-26 05:40:51.000000 dprox-0.1.3/dprox/utils/io.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4630 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/metrics.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4958 2023-05-24 06:20:38.000000 dprox-0.1.3/dprox/utils/misc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3978 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/psf2otf.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      304 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4287 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      108 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        6 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-26 06:26:21.000000 dprox-0.1.3/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      656 2023-05-26 06:25:51.000000 dprox-0.1.3/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/tests/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2715 2023-05-20 03:13:06.000000 dprox-0.1.3/tests/test_algorithms.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1043 2023-05-24 07:09:33.000000 dprox-0.1.3/tests/test_derain.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      318 2023-05-22 14:14:30.000000 dprox-0.1.3/tests/test_energy_system.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1688 2023-05-23 08:23:24.000000 dprox-0.1.3/tests/test_inverse_problems.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      790 2023-05-24 07:49:26.000000 dprox-0.1.3/tests/test_jd23.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2586 2023-05-24 04:36:39.000000 dprox-0.1.3/tests/test_linear_solver.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3280 2023-05-22 11:53:09.000000 dprox-0.1.3/tests/test_linear_solver_grad.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6231 2023-05-24 08:13:09.000000 dprox-0.1.3/tests/test_linear_solver_torch.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2692 2023-05-20 03:13:06.000000 dprox-0.1.3/tests/test_linop.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      180 2023-05-20 03:13:06.000000 dprox-0.1.3/tests/test_linop_primitive.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1198 2023-05-24 04:36:39.000000 dprox-0.1.3/tests/test_ml_problems.py
```

### Comparing `dprox-0.1.2/README.md` & `dprox-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/admm.py` & `dprox-0.1.3/dprox/algo/admm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/base.py` & `dprox-0.1.3/dprox/algo/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/hqs.py` & `dprox-0.1.3/dprox/algo/hqs.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/invert.py` & `dprox-0.1.3/dprox/algo/invert.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/lp/solvers.py` & `dprox-0.1.3/dprox/algo/lp/solvers.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/lp/utils.py` & `dprox-0.1.3/dprox/algo/lp/utils.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/opt/absorb.py` & `dprox-0.1.3/dprox/algo/opt/absorb.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/opt/equil.py` & `dprox-0.1.3/dprox/algo/opt/equil.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/opt/merge.py` & `dprox-0.1.3/dprox/algo/opt/merge.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/pc.py` & `dprox-0.1.3/dprox/algo/pc.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/pgd.py` & `dprox-0.1.3/dprox/algo/pgd.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/problem.py` & `dprox-0.1.3/dprox/algo/problem.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/special/deq.py` & `dprox-0.1.3/dprox/algo/special/deq.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/special/deq_utils/jacobian.py` & `dprox-0.1.3/dprox/algo/special/deq_utils/jacobian.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/special/deq_utils/layer_utils.py` & `dprox-0.1.3/dprox/algo/special/deq_utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/special/deq_utils/optimizations.py` & `dprox-0.1.3/dprox/algo/special/deq_utils/optimizations.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/special/deq_utils/radam.py` & `dprox-0.1.3/dprox/algo/special/deq_utils/radam.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/special/deq_utils/solvers.py` & `dprox-0.1.3/dprox/algo/special/deq_utils/solvers.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/special/unroll.py` & `dprox-0.1.3/dprox/algo/special/unroll.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/tune/autotune.py` & `dprox-0.1.3/dprox/algo/tune/autotune.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/algo/tune/dpir.py` & `dprox-0.1.3/dprox/algo/tune/dpir.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linalg/custom.py` & `dprox-0.1.3/dprox/linalg/custom.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linalg/solve/cg.py` & `dprox-0.1.3/dprox/linalg/solve/cg.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linalg/solve/minres.py` & `dprox-0.1.3/dprox/linalg/solve/minres.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linalg/solve/plss.py` & `dprox-0.1.3/dprox/linalg/solve/plss.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/__init__.py` & `dprox-0.1.3/dprox/linop/__init__.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/base.py` & `dprox-0.1.3/dprox/linop/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/blackbox.py` & `dprox-0.1.3/dprox/linop/blackbox.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/comp_graph.py` & `dprox-0.1.3/dprox/linop/comp_graph.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/constant.py` & `dprox-0.1.3/dprox/linop/constant.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/conv.py` & `dprox-0.1.3/dprox/linop/conv.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/grad.py` & `dprox-0.1.3/dprox/linop/grad.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/scale.py` & `dprox-0.1.3/dprox/linop/scale.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/subsample.py` & `dprox-0.1.3/dprox/linop/subsample.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/sum.py` & `dprox-0.1.3/dprox/linop/sum.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/variable.py` & `dprox-0.1.3/dprox/linop/variable.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/linop/vstack.py` & `dprox-0.1.3/dprox/linop/vstack.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/base.py` & `dprox-0.1.3/dprox/proxfn/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/fast/cs.py` & `dprox-0.1.3/dprox/proxfn/fast/cs.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/fast/csmri.py` & `dprox-0.1.3/dprox/proxfn/fast/csmri.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/fast/pr.py` & `dprox-0.1.3/dprox/proxfn/fast/pr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/fast/spi.py` & `dprox-0.1.3/dprox/proxfn/fast/spi.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/fast/sr.py` & `dprox-0.1.3/dprox/proxfn/fast/sr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/linalg/solve/bicgstab.py` & `dprox-0.1.3/dprox/proxfn/linalg/solve/bicgstab.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/linalg/solve/broyden.py` & `dprox-0.1.3/dprox/proxfn/linalg/solve/broyden.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/linalg/solve/gmres.py` & `dprox-0.1.3/dprox/proxfn/linalg/solve/gmres.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/linalg/solve/plss.py` & `dprox-0.1.3/dprox/proxfn/linalg/solve/plss.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/nlm/nlm.py` & `dprox-0.1.3/dprox/proxfn/nlm/nlm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/norm.py` & `dprox-0.1.3/dprox/proxfn/norm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/base.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/composite.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/composite.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/TV_denoising.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/TV_denoising.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/basicblock.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/basicblock.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/network_dncnn.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_dncnn.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/network_unet.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/models/unet/unet.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/denoisers/wrapper.py` & `dprox-0.1.3/dprox/proxfn/pnp/denoisers/wrapper.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/pnp/prior.py` & `dprox-0.1.3/dprox/proxfn/pnp/prior.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/sum_square.py` & `dprox-0.1.3/dprox/proxfn/sum_square.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/proxfn/unrolling/dgu.py` & `dprox-0.1.3/dprox/proxfn/unrolling/dgu.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/containar.py` & `dprox-0.1.3/dprox/utils/containar.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/examples/csmri/common.py` & `dprox-0.1.3/dprox/utils/examples/csmri/common.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/examples/csmri/dataset.py` & `dprox-0.1.3/dprox/utils/examples/csmri/dataset.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/examples/csmri/misc.py` & `dprox-0.1.3/dprox/utils/examples/csmri/misc.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/examples/derain/custom_linop.py` & `dprox-0.1.3/dprox/utils/examples/derain/custom_linop.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/examples/energy_system/__init__.py` & `dprox-0.1.3/dprox/utils/examples/energy_system/__init__.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/examples/optic/common.py` & `dprox-0.1.3/dprox/utils/examples/optic/common.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/examples/optic/doe_model.py` & `dprox-0.1.3/dprox/utils/examples/optic/doe_model.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/examples/optic/unet.py` & `dprox-0.1.3/dprox/utils/examples/optic/unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/examples/restoration.py` & `dprox-0.1.3/dprox/utils/examples/restoration.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/init/mosaic.py` & `dprox-0.1.3/dprox/utils/init/mosaic.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/init/sr.py` & `dprox-0.1.3/dprox/utils/init/sr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/io.py` & `dprox-0.1.3/dprox/utils/io.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/metrics.py` & `dprox-0.1.3/dprox/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/misc.py` & `dprox-0.1.3/dprox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox/utils/psf2otf.py` & `dprox-0.1.3/dprox/utils/psf2otf.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/dprox.egg-info/SOURCES.txt` & `dprox-0.1.3/dprox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/setup.py` & `dprox-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 setup(
     name='dprox',
     description='A domain-specific language and compiler that transforms optimization problems into differentiable proximal solvers.',
     url='https://github.com/princeton-computational-imaging/Delta-Prox',
     author='Zeqiang Lai',
     author_email='laizeqiang@outlook.com',
     packages=find_packages(),
-    version='0.1.2',
+    version='0.1.3',
     include_package_data=True,
     install_requires=deps,
 )
```

### Comparing `dprox-0.1.2/tests/test_algorithms.py` & `dprox-0.1.3/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/tests/test_derain.py` & `dprox-0.1.3/tests/test_derain.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/tests/test_inverse_problems.py` & `dprox-0.1.3/tests/test_inverse_problems.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/tests/test_jd23.py` & `dprox-0.1.3/tests/test_jd23.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/tests/test_linear_solver.py` & `dprox-0.1.3/tests/test_linear_solver.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/tests/test_linear_solver_grad.py` & `dprox-0.1.3/tests/test_linear_solver_grad.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/tests/test_linear_solver_torch.py` & `dprox-0.1.3/tests/test_linear_solver_torch.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/tests/test_linop.py` & `dprox-0.1.3/tests/test_linop.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.2/tests/test_ml_problems.py` & `dprox-0.1.3/tests/test_ml_problems.py`

 * *Files identical despite different names*

