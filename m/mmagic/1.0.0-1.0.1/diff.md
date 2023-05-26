# Comparing `tmp/mmagic-1.0.0.tar.gz` & `tmp/mmagic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmagic-1.0.0.tar", last modified: Tue Apr 25 09:46:46 2023, max compression
+gzip compressed data, was "dist/mmagic-1.0.1.tar", last modified: Fri May 26 08:38:56 2023, max compression
```

## Comparing `mmagic-1.0.0.tar` & `mmagic-1.0.1.tar`

### file list

```diff
@@ -1,973 +1,975 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 09:46:23.000000 mmagic-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    26353 2023-04-25 09:46:46.000000 mmagic-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21471 2023-04-25 09:46:23.000000 mmagic-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/basicvsr_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/cifar10_noaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/cifar10_nopad.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/comp1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/deblurring-defocus_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/deblurring-motion_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/decompression_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/denoising-gaussian_color_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/denoising-gaussian_gray_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/denoising-real_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/deraining_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/ffhq_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/grow_scale_imgs_ffhq_styleganv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/imagenet_128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/imagenet_256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/imagenet_512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/imagenet_64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/imagenet_noaug_128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/liif_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/lsun_stylegan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/paired_imgs_256x256_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/places.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/sisr_x2_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/sisr_x3_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/sisr_x4_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/tdan_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_flip_512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_flip_lanczos_resize_256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/unpaired_imgs_256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/default_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/gen_default_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/inpaint_default_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/matting_default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_cyclegan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_deepfillv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_deepfillv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_edvr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_glean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_liif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_pconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_pix2pix.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_styleganv1.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_styleganv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_styleganv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_tof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/biggan/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/biggan/base_biggan_128x128.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/dcgan/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/dcgan/base_dcgan_128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/dcgan/base_dcgan_64x64.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/sagan/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/sagan/base_sagan_128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/sagan/base_sagan_32x32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/sngan_proj/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/sngan_proj/base_sngan_proj_128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/_base_/models/sngan_proj/base_sngan_proj_32x32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/aot_gan/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/aot_gan/aot-gan_smpgan_4xb4_places-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/aot_gan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr/
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr/basicvsr_2xb4_reds4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr/basicvsr_2xb4_vimeo90k-bd.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr/basicvsr_2xb4_vimeo90k-bi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-decompress-track1.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-decompress-track2.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-decompress-track3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-vsr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_4xb2-300k_vimeo90k-bd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_4xb2-300k_vimeo90k-bi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_8xb1-600k_reds4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/biggan/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face-rgb_imagenet1k-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face_rgb_imagenet1k-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face_rgb_imagenet1k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan_2xb25-500kiters_cifar10-32x32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan_ajbrock-sn_8xb32-1500kiters_imagenet1k-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan_cvt-BigGAN-PyTorch-rgb_imagenet1k-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/biggan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/cain/
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/cain/cain_g1b32_1xb5_vimeo90k-triplet.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/cain/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/controlnet/controlnet-1xb1-fill50k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/controlnet/controlnet-canny.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/controlnet/controlnet-pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/controlnet/controlnet-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/controlnet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/controlnet_animation/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/controlnet_animation/anythingv3_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/controlnet_animation/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/cyclegan/
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-250kiters_summer2winter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-270kiters_horse2zebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-80kiters_facades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-250kiters_summer2winter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-270kiters_horse2zebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-80kiters_facades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/cyclegan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/dcgan/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dcgan/dcgan_1xb128-300kiters_celeba-cropped-64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dcgan/dcgan_1xb128-5epoches_lsun-bedroom-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dcgan/dcgan_Glr4e-4_Dlr1e-4_1xb128-5kiters_mnist-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dcgan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/deepfillv1/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/deepfillv1/deepfillv1_4xb4_celeba-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/deepfillv1/deepfillv1_8xb2_places-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/deepfillv1/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/deepfillv2/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/deepfillv2/deepfillv2_8xb2_celeba-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/deepfillv2/deepfillv2_8xb2_places-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/deepfillv2/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/dic/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dic/dic_gan-x8c48b6_4xb2-500k_celeba-hq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dic/dic_x8c48b6_4xb2-150k_celeba-hq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dic/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/dim/
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dim/dim_stage1-v16_1xb1-1000k_comp1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dim/dim_stage1-v16_1xb1-1000k_comp1k_online-merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dim/dim_stage2-v16-pln_1xb1-1000k_comp1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dim/dim_stage3-v16-pln_1xb1-1000k_comp1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dim/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/disco_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/disco_diffusion/disco-diffusion_adm-u-finetuned_imagenet-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/disco_diffusion/disco-diffusion_adm-u-finetuned_imagenet-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/disco_diffusion/disco-diffusion_portrait-generator-v001.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/disco_diffusion/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/dreambooth/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dreambooth/dreambooth-finetune_text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dreambooth/dreambooth-lora-prior_pre.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dreambooth/dreambooth-lora.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dreambooth/dreambooth-prior_pre.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dreambooth/dreambooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/dreambooth/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/edsr/
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/edsr/edsr_x2c64b16_1xb16-300k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/edsr/edsr_x3c64b16_1xb16-300k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/edsr/edsr_x4c64b16_1xb16-300k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/edsr/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/edvr/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/edvr/edvrl_c128b40_8xb8-lr2e-4-600k_reds4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/edvr/edvrl_wotsa-c128b40_8xb8-lr2e-4-600k_reds4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/edvr/edvrm_8xb4-600k_reds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/edvr/edvrm_wotsa_8xb4-600k_reds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/edvr/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/eg3d/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_afhq-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_ffhq-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_shapenet-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/eg3d/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/esrgan/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/esrgan/esrgan_psnr-x4c64b23g32_1xb16-1000k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/esrgan/esrgan_x4c64b23g32_1xb16-400k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/esrgan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/flavr/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/flavr/flavr_in4out1_8xb4_vimeo90k-septuplet.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/flavr/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/gca/
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/gca/baseline_r34_4xb10-200k_comp1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/gca/baseline_r34_4xb10-dimaug-200k_comp1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/gca/gca_r34_4xb10-200k_comp1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/gca/gca_r34_4xb10-dimaug-200k_comp1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/gca/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/ggan/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/ggan/ggan_dcgan-archi_lr1e-3-1xb128-12Mimgs_celeba-cropped-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/ggan/ggan_dcgan-archi_lr1e-4-1xb64-10Mimgs_celeba-cropped-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/ggan/ggan_lsgan-archi_lr1e-4-1xb128-20Mimgs_lsun-bedroom-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/ggan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/glean/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/glean/glean_in128out1024-fp16_4xb2-300k_ffhq-celeba-hq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/glean/glean_in128out1024_4xb2-300k_ffhq-celeba-hq.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/glean/glean_x16-fp16_2xb8_ffhq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/glean/glean_x16_2xb8_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/glean/glean_x16_2xb8_ffhq.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/glean/glean_x8-fp16_2xb8_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/glean/glean_x8_2xb8_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/glean/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/global_local/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/global_local/gl_8xb12_celeba-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/global_local/gl_8xb12_places-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/global_local/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/iconvsr/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_reds4.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_vimeo90k-bd.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_vimeo90k-bi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/iconvsr/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/indexnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/indexnet/indexnet_mobv2-dimaug_1xb16-78k_comp1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/indexnet/indexnet_mobv2_1xb16-78k_comp1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/indexnet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/inst_colorization/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/inst_colorization/inst-colorizatioon_full_official_cocostuff-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/inst_colorization/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/liif/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/liif/liif-edsr-norm_c64b16_1xb16-1000k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/liif/liif-rdn-norm_c64b16_1xb16-1000k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/liif/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/lsgan/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-3-1xb128-12Mimgs_celeba-cropped-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-4-1xb128-12Mimgs_lsun-bedroom-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-4-1xb64-10Mimgs_celeba-cropped-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/lsgan/lsgan_lsgan-archi_lr1e-4-1xb64-10Mimgs_lsun-bedroom-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/lsgan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/nafnet/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/nafnet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/nafnet/nafnet_c64eb11128mb1db1111_8xb8-lr1e-3-400k_gopro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/nafnet/nafnet_c64eb2248mb12db2222_8xb8-lr1e-3-400k_sidd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/partial_conv/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/partial_conv/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/partial_conv/pconv_stage1_8xb12_places-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/partial_conv/pconv_stage1_8xb1_celeba-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/partial_conv/pconv_stage2_4xb2_celeba-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/partial_conv/pconv_stage2_4xb2_places-256x256.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/pggan/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/pggan/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/pggan/pggan_8xb4-12Mimg_celeba-hq-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/pggan/pggan_8xb4-12Mimgs_celeba-cropped-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/pggan/pggan_8xb4-12Mimgs_lsun-bedroom-128x128.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/pix2pix/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-220kiters_aerial2maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-220kiters_maps2aerial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-80kiters_facades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_wo-jitter-flip-1xb4-190kiters_edges2shoes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-c_c2_8xb3-1100kiters_ffhq-256-512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-d_c2_8xb3-1100kiters_ffhq-256-512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-e_c2_8xb3-1100kiters_ffhq-256-512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c1_8xb2-1600kiters_ffhq-256-1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c2_8xb3-1100kiters_ffhq-256-512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c2_8xb3-1100kiters_ffhq-256-896.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-g_c1_8xb3-1100kiters_ffhq-256-512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-h_c2_8xb3-1100kiters_ffhq-256-512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-i_c2_8xb3-1100kiters_ffhq-256-512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-j_c2_8xb3-1100kiters_ffhq-256-512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-k_c2_8xb3-1100kiters_ffhq-256-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan-csg_bohemian.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan-csg_fish.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan_interp-pad_balloons.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan_interp-pad_disc-nobn_balloons.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan_interp-pad_disc-nobn_fish.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim4_bohemian.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim4_fish.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim8_bohemian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/stylegan2_c2_8xb3-1100kiters_ffhq-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/stylegan2_c2_8xb3-1100kiters_ffhq-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/rdn/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/rdn/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/rdn/rdn_x2c64b16_1xb16-1000k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/rdn/rdn_x3c64b16_1xb16-1000k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/rdn/rdn_x4c64b16_1xb16-1000k_div2k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/real_basicvsr/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/real_basicvsr/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/real_basicvsr/realbasicvsr_c64b20-1x30x8_8xb1-lr5e-5-150k_reds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/real_basicvsr/realbasicvsr_wogan-c64b20-2x30x8_8xb2-lr1e-4-300k_reds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/real_esrgan/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/real_esrgan/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/real_esrgan/realesrgan_c64b23g32_4xb12-lr1e-4-400k_df2k-ost.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/real_esrgan/realesrnet_c64b23g32_4xb12-lr2e-4-1000k_df2k-ost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/
--rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma15.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma25.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma15.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma25.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma50.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dpdd-dual.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dpdd-single.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_gopro.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_rain13k.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_sidd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/sagan/
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sagan/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_128_cvt_studioGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_cvt-studioGAN_cifar10-32x32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_wReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_woReLUinplace-Glr1e-4_Dlr4e-4_noaug-ndisc1-8xb32-bigGAN-sch_imagenet1k-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_woReLUinplace_Glr1e-4_Dlr4e-4_ndisc1-4xb64_imagenet1k-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_woReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/singan/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/singan/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/singan/singan_balloons.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/singan/singan_bohemian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/singan/singan_fish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj-cvt-studioGAN_cifar10-32x32.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj-cvt-studioGAN_imagenet1k-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj_wReLUinplace_Glr2e-4_Dlr5e-5_ndisc5-2xb128_imagenet1k-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj_wReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj_woReLUinplace_Glr2e-4_Dlr5e-5_ndisc5-2xb128_imagenet1k-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj_woReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/srcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/srcnn/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/srcnn/srcnn_x4k915_1xb16-1000k_div2k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/srgan_resnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/srgan_resnet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/srgan_resnet/msrresnet_x4c64b16_1xb16-1000k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/srgan_resnet/srgan_x4c64b16_1xb16-1000k_div2k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/stable_diffusion/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/stable_diffusion/stable-diffusion_ddim_denoisingunet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv1/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv1/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv1/styleganv1_ffhq-1024x1024_8xb4-25Mimgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv1/styleganv1_ffhq-256x256_8xb4-25Mimgs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv2/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv2/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2-PL-R1_8xb4-apex-fp16-no-scaler-800kiters_ffhq-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2-PL-R1_8xb4-fp16-globalG-partialD-no-scaler-800kiters_ffhq-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2-PL_8xb4-fp16-partial-GD-no-scaler-800kiters_ffhq-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_ffhq-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-cat-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-church-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-horse-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4_ffhq-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4_lsun-car-384x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-r_ada-gamma3.3_8xb4-fp16_metfaces-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4_ffhq-1024x1024.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4_ffhqu-256x256.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4x8_afhqv2-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_ada-gamma6.6_8xb4-fp16_metfaces-1024x1024.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_afhqv2-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_ffhq-1024x1024.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1383 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_ffhqu-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_gamma2.0_8xb4-fp16-noaug_ffhq-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_gamma32.8_8xb4-fp16-noaug_ffhq-1024x1024.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/
--rw-r--r--   0 runner    (1001) docker     (123)    19414 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_gan-x2s64w8d6e180_8xb4-lr1e-4-600k_df2k-ost.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_gan-x4s64w8d6e180_8xb4-lr1e-4-600k_df2k-ost.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_gan-x4s64w8d9e240_8xb4-lr1e-4-600k_df2k-ost.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_psnr-x2s64w8d6e180_8xb4-lr1e-4-600k_df2k-ost.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_psnr-x4s64w8d6e180_8xb4-lr1e-4-600k_df2k-ost.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_psnr-x4s64w8d9e240_8xb4-lr1e-4-600k_df2k-ost.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR10.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR20.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR30.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR40.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR10.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR20.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR30.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR40.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN15.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN25.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN50.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN15.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN25.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN50.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x2s48w8d6e180_8xb4-lr2e-4-500k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x2s64w8d4e60_8xb4-lr2e-4-500k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x2s64w8d6e180_8xb4-lr2e-4-500k_df2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x3s48w8d6e180_8xb4-lr2e-4-500k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x3s64w8d4e60_8xb4-lr2e-4-500k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x3s64w8d6e180_8xb4-lr2e-4-500k_df2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x4s48w8d6e180_8xb4-lr2e-4-500k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x4s64w8d4e60_8xb4-lr2e-4-500k_div2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x4s64w8d6e180_8xb4-lr2e-4-500k_df2k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/tdan/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tdan/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tdan/tdan_x4_8xb16-lr1e-4-400k_vimeo90k-bd.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tdan/tdan_x4_8xb16-lr1e-4-400k_vimeo90k-bi.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tdan/tdan_x4ft_8xb16-lr5e-5-400k_vimeo90k-bi.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tdan/tdan_x4ft_8xb16-lr5e-5-800k_vimeo90k-bd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/tof/
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tof/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tof/tof_spynet-chair-wobn_1xb1_vimeo90k-triplet.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tof/tof_spynet-kitti-wobn_1xb1_vimeo90k-triplet.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tof/tof_spynet-pytoflow-wobn_1xb1_vimeo90k-triplet.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tof/tof_spynet-sintel-wobn-clean_1xb1_vimeo90k-triplet.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tof/tof_spynet-sintel-wobn-final_1xb1_vimeo90k-triplet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/tof/tof_x4_official_vimeo90k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/ttsr/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/ttsr/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/ttsr/ttsr-gan_x4c64b16_1xb9-500k_CUFED.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/ttsr/ttsr-rec_x4c64b16_1xb9-200k_CUFED.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/configs/wgan-gp/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/wgan-gp/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/wgan-gp/wgangp_GN-GP-50_1xb64-160kiters_lsun-bedroom-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/configs/wgan-gp/wgangp_GN_1xb64-160kiters_celeba-cropped-128x128.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/demo/download_inference_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/demo/gradio_controlnet_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/demo/gradio_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/demo/mmagic_inference_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/demo/singan_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-25 09:46:45.000000 mmagic-1.0.0/mmagic/.mim/model-index.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/analysis_tools/get_flops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/analysis_tools/print_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      265 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/cpu_train.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/bgm/
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/bgm/preprocess_bgm_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/comp1k/
--rwxr-xr-x   0 runner    (1001) docker     (123)      939 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/comp1k/check_extended_fg.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/comp1k/evaluate_comp1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/comp1k/extend_fg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/comp1k/filter_comp1k_anno.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/comp1k/preprocess_comp1k_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/df2k_ost/
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/df2k_ost/preprocess_df2k_ost_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/div2k/
--rw-r--r--   0 runner    (1001) docker     (123)    14978 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/div2k/preprocess_div2k_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/glean/
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/glean/preprocess_cat_test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/glean/preprocess_cat_train_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/glean/preprocess_ffhq_celebahq_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/reds/
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/reds/crop_sub_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/reds/preprocess_reds_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/sidd/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/sidd/preprocess_sidd_test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/vid4/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/vid4/preprocess_vid4_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/vimeo90k/
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/vimeo90k/preprocess_vimeo90k_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dist_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/dist_train.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/gui/
--rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/gui/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/gui/page_general.py
--rw-r--r--   0 runner    (1001) docker     (123)    34328 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/gui/page_sr.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/gui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/.mim/tools/model_converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/model_converters/publish_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/model_converters/pytorch2onnx.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/slurm_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      622 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/slurm_train.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/.mim/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/apis/inferencers/
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/base_mmagic_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/colorization_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/conditional_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/controlnet_animation_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/eg3d_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/image_super_resolution_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/inference_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/inpainting_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/matting_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/text2image_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/translation_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/unconditional_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/video_interpolation_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/inferencers/video_restoration_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/apis/mmagic_inferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/basic_conditional_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/basic_frames_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/basic_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    29271 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/cifar10_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/comp1k_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/controlnet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/dreambooth_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/grow_scale_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/imagenet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/mscoco_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/paired_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/singan_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/datasets/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/aug_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/aug_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/aug_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/blur_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    37682 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/fgbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/generate_assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/generate_frame_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/get_masked_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/matlab_like_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/random_degradations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/random_down_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/trimap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/transforms/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/datasets/unpaired_image_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/hooks/iter_time_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/hooks/pggan_fetch_data_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/hooks/pickle_data_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/hooks/reduce_lr_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/hooks/visualization_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/engine/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/optimizers/multi_optimizer_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/optimizers/pggan_optimizer_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/optimizers/singan_optimizer_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/engine/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/runner/log_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/runner/loop_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/runner/multi_loops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/engine/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/schedulers/linear_lr_scheduler_with_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/engine/schedulers/reduce_lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/evaluation/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/functional/fid_inception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/functional/gaussian_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/functional/inception_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/base_gen_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/base_sample_wise_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/connectivity_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/equivariance.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/fid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/gradient_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/inception_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/matting_mse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/ms_ssim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/mse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/niqe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/niqe_pris_params.npz
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/ppl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/precision_and_recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/psnr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/sad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/ssim.py
--rw-r--r--   0 runner    (1001) docker     (123)    14289 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/evaluation/metrics/swd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/archs/
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/all_gather_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/gated_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/img_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/linear_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/multi_layer_disc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/patch_disc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/simple_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/smpatch_disc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/sr_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/archs/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/base_models/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/base_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/base_models/average_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/base_models/base_conditional_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/base_models/base_edit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    25496 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/base_models/base_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/base_models/base_mattor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/base_models/base_translation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/base_models/basic_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17954 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/base_models/one_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/base_models/two_stage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/data_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/data_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37022 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/data_preprocessors/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/data_preprocessors/mattor_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/diffusion_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/diffusion_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/diffusion_schedulers/ddim_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/diffusion_schedulers/ddpm_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/aotgan/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/aotgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/aotgan/aot_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/aotgan/aot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/aotgan/aot_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/aotgan/aot_inpaintor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/aotgan/aot_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/arcface/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/arcface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/arcface/arcface_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/arcface/id_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/arcface/model_irse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/basicvsr/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/basicvsr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/basicvsr/basicvsr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/basicvsr/basicvsr_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/basicvsr_plusplus_net/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/basicvsr_plusplus_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16236 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/basicvsr_plusplus_net/basicvsr_plusplus_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/biggan/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/biggan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/biggan/biggan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/biggan/biggan_deep_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/biggan/biggan_deep_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/biggan/biggan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19952 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/biggan/biggan_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    30009 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/biggan/biggan_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/biggan/biggan_snmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/cain/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/cain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/cain/cain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/cain/cain_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/controlnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35750 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/controlnet/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/controlnet/controlnet_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/cyclegan/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/cyclegan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/cyclegan/cyclegan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/cyclegan/cyclegan_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/cyclegan/cyclegan_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/dcgan/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dcgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dcgan/dcgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dcgan/dcgan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dcgan/dcgan_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/ddpm/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ddpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21369 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ddpm/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    52979 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ddpm/denoising_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ddpm/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ddpm/res_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    20328 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ddpm/unet_blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv1/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv1/contextual_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv1/contextual_attention_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv1/deepfill_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv1/deepfill_disc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv1/deepfill_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv1/deepfill_refiner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15868 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv1/deepfillv1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv2/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/deepfillv2/two_stage_encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/dic/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dic/dic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dic/dic_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dic/feedback_hour_glass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dic/light_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/dim/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dim/dim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/disco_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/disco_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/disco_diffusion/clip_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/disco_diffusion/disco.py
--rw-r--r--   0 runner    (1001) docker     (123)    19913 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/disco_diffusion/guider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/disco_diffusion/secondary_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/dreambooth/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dreambooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/dreambooth/dreambooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/duf/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/duf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/duf/duf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/edsr/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/edsr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/edsr/edsr_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/edvr/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/edvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/edvr/edvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    18568 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/edvr/edvr_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/eg3d/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/eg3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20954 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/eg3d/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/eg3d/dual_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/eg3d/eg3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/eg3d/eg3d_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/eg3d/eg3d_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/eg3d/eg3d_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/eg3d/ray_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    24027 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/eg3d/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/esrgan/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/esrgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/esrgan/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/esrgan/rrdb_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/fba/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/fba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/fba/fba_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/fba/fba_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/flavr/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/flavr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/flavr/flavr.py
--rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/flavr/flavr_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/gca/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/gca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/gca/gca.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/gca/gca_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/gca/resgca_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/gca/resgca_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/ggan/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ggan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ggan/ggan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/glean/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/glean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/glean/glean_styleganv2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/global_local/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/global_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/global_local/gl_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/global_local/gl_dilation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/global_local/gl_disc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/global_local/gl_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/global_local/gl_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/global_local/gl_inpaintor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/guided_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/guided_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/guided_diffusion/adm.py
--rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/guided_diffusion/classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/iconvsr/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/iconvsr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/iconvsr/iconvsr_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/indexnet/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/indexnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/indexnet/indexnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/indexnet/indexnet_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19088 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/indexnet/indexnet_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/inst_colorization/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/inst_colorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/inst_colorization/color_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/inst_colorization/colorization_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/inst_colorization/fusion_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/inst_colorization/inst_colorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/inst_colorization/weight_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/liif/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/liif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/liif/liif.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/liif/liif_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/liif/mlp_refiner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/lsgan/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/lsgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/lsgan/lsgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/lsgan/lsgan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/lsgan/lsgan_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/mspie/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/mspie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/mspie/mspie_stylegan2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/mspie/mspie_stylegan2_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/mspie/mspie_stylegan2_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/mspie/mspie_stylegan2_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/mspie/pe_singan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/mspie/pe_singan_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/mspie/positional_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/nafnet/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/nafnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/nafnet/naf_avgpool2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/nafnet/naf_layerNorm2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/nafnet/nafbaseline_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/nafnet/nafnet_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/pconv/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pconv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pconv/mask_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pconv/partial_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pconv/pconv_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pconv/pconv_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pconv/pconv_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pconv/pconv_inpaintor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/pggan/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pggan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20643 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pggan/pggan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pggan/pggan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pggan/pggan_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19717 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pggan/pggan_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pix2pix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pix2pix/pix2pix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pix2pix/pix2pix_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/pix2pix/pix2pix_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/plain/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/plain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/plain/plain_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/plain/plain_refiner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/rdn/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/rdn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/rdn/rdn_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/real_basicvsr/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/real_basicvsr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/real_basicvsr/real_basicvsr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/real_basicvsr/real_basicvsr_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/real_esrgan/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/real_esrgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/real_esrgan/real_esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/real_esrgan/unet_disc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/restormer/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/restormer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17236 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/restormer/restormer_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/sagan/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/sagan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/sagan/sagan.py
--rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/sagan/sagan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20851 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/sagan/sagan_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25894 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/sagan/sagan_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/singan/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/singan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/singan/singan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/singan/singan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/singan/singan_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/singan/singan_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/srcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/srcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/srcnn/srcnn_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/srgan/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/srgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/srgan/modified_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/srgan/sr_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/srgan/srgan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stable_diffusion/clip_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    25994 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stable_diffusion/stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    34487 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/stylegan1/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan1/stylegan1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan1/stylegan1_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan1/stylegan1_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan1/stylegan1_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan1/stylegan_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/ada/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/ada/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32653 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/ada/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/ada/grid_sample_gradfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/ada/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/ada/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/stylegan2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/stylegan2_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23415 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/stylegan2_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan2/stylegan2_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/stylegan3/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan3/stylegan3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan3/stylegan3_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28215 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan3/stylegan3_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/stylegan3/stylegan3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/swinir/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/swinir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/swinir/swinir_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/swinir/swinir_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/swinir/swinir_rstb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/swinir/swinir_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/tdan/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/tdan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/tdan/tdan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/tdan/tdan_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/tof/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/tof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/tof/tof_vfi_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/tof/tof_vsr_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/ttsr/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ttsr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ttsr/lte.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ttsr/search_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ttsr/ttsr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ttsr/ttsr_disc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13923 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/ttsr/ttsr_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/editors/wgan_gp/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/wgan_gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/wgan_gp/wgan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/wgan_gp/wgan_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/wgan_gp/wgan_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/editors/wgan_gp/wgan_gp_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/clip_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/composition_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/face_id_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/feature_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    21058 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/gan_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/gradient_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/losses/loss_comps/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/loss_comps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/loss_comps/clip_loss_comps.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/loss_comps/disc_auxiliary_loss_comps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/loss_comps/face_id_loss_comps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/loss_comps/gan_loss_comps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/loss_comps/gen_auxiliary_loss_comps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/loss_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/perceptual_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/losses/pixelwise_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/utils/bbox_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/utils/diffusion_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/utils/flow_warp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/utils/sampling_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/models/utils/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/structures/data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/utils/img_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/utils/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/utils/trans_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/visualization/concat_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/visualization/vis_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-04-25 09:46:23.000000 mmagic-1.0.0/mmagic/visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26353 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 09:46:46.000000 mmagic-1.0.0/mmagic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:46:46.000000 mmagic-1.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 09:46:23.000000 mmagic-1.0.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-25 09:46:23.000000 mmagic-1.0.0/requirements/mminstall.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-25 09:46:23.000000 mmagic-1.0.0/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-25 09:46:23.000000 mmagic-1.0.0/requirements/readthedocs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-25 09:46:23.000000 mmagic-1.0.0/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-25 09:46:23.000000 mmagic-1.0.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-25 09:46:46.000000 mmagic-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-04-25 09:46:23.000000 mmagic-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 08:38:18.000000 mmagic-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-05-26 08:38:56.000000 mmagic-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21816 2023-05-26 08:38:18.000000 mmagic-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/basicvsr_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/cifar10_noaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/cifar10_nopad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/comp1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/deblurring-defocus_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/deblurring-motion_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/decompression_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/denoising-gaussian_color_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/denoising-gaussian_gray_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/denoising-real_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/deraining_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/ffhq_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/grow_scale_imgs_ffhq_styleganv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/imagenet_128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/imagenet_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/imagenet_512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/imagenet_64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/imagenet_noaug_128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/liif_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/lsun_stylegan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/paired_imgs_256x256_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/places.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/sisr_x2_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/sisr_x3_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/sisr_x4_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/tdan_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_flip_512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_flip_lanczos_resize_256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/unpaired_imgs_256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/default_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/gen_default_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/inpaint_default_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/matting_default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_cyclegan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_deepfillv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_deepfillv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_edvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_glean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_liif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_pconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_pix2pix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_styleganv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_styleganv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_styleganv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_tof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/biggan/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/biggan/base_biggan_128x128.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/dcgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/dcgan/base_dcgan_128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/dcgan/base_dcgan_64x64.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/sagan/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/sagan/base_sagan_128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/sagan/base_sagan_32x32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/sngan_proj/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/sngan_proj/base_sngan_proj_128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/_base_/models/sngan_proj/base_sngan_proj_32x32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/aot_gan/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/aot_gan/aot-gan_smpgan_4xb4_places-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/aot_gan/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr/basicvsr_2xb4_reds4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr/basicvsr_2xb4_vimeo90k-bd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr/basicvsr_2xb4_vimeo90k-bi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-decompress-track1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-decompress-track2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-decompress-track3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-vsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_4xb2-300k_vimeo90k-bd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_4xb2-300k_vimeo90k-bi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_8xb1-600k_reds4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/biggan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face-rgb_imagenet1k-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face_rgb_imagenet1k-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face_rgb_imagenet1k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan_2xb25-500kiters_cifar10-32x32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan_ajbrock-sn_8xb32-1500kiters_imagenet1k-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan_cvt-BigGAN-PyTorch-rgb_imagenet1k-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/biggan/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/cain/
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/cain/cain_g1b32_1xb5_vimeo90k-triplet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/cain/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/controlnet/controlnet-1xb1-fill50k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/controlnet/controlnet-canny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/controlnet/controlnet-pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/controlnet/controlnet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/controlnet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/controlnet_animation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/controlnet_animation/anythingv3_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/controlnet_animation/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/cyclegan/
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-250kiters_summer2winter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-270kiters_horse2zebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-80kiters_facades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-250kiters_summer2winter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-270kiters_horse2zebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-80kiters_facades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/cyclegan/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/dcgan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dcgan/dcgan_1xb128-300kiters_celeba-cropped-64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dcgan/dcgan_1xb128-5epoches_lsun-bedroom-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dcgan/dcgan_Glr4e-4_Dlr1e-4_1xb128-5kiters_mnist-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dcgan/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/deepfillv1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/deepfillv1/deepfillv1_4xb4_celeba-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/deepfillv1/deepfillv1_8xb2_places-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/deepfillv1/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/deepfillv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/deepfillv2/deepfillv2_8xb2_celeba-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/deepfillv2/deepfillv2_8xb2_places-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/deepfillv2/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/dic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dic/dic_gan-x8c48b6_4xb2-500k_celeba-hq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dic/dic_x8c48b6_4xb2-150k_celeba-hq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dic/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/dim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dim/dim_stage1-v16_1xb1-1000k_comp1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dim/dim_stage1-v16_1xb1-1000k_comp1k_online-merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dim/dim_stage2-v16-pln_1xb1-1000k_comp1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dim/dim_stage3-v16-pln_1xb1-1000k_comp1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dim/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/disco_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/disco_diffusion/disco-diffusion_adm-u-finetuned_imagenet-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/disco_diffusion/disco-diffusion_adm-u-finetuned_imagenet-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/disco_diffusion/disco-diffusion_portrait-generator-v001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/disco_diffusion/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/dreambooth/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dreambooth/dreambooth-finetune_text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dreambooth/dreambooth-lora-prior_pre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dreambooth/dreambooth-lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dreambooth/dreambooth-prior_pre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dreambooth/dreambooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/dreambooth/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/edsr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/edsr/edsr_x2c64b16_1xb16-300k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/edsr/edsr_x3c64b16_1xb16-300k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/edsr/edsr_x4c64b16_1xb16-300k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/edsr/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/edvr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/edvr/edvrl_c128b40_8xb8-lr2e-4-600k_reds4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/edvr/edvrl_wotsa-c128b40_8xb8-lr2e-4-600k_reds4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/edvr/edvrm_8xb4-600k_reds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/edvr/edvrm_wotsa_8xb4-600k_reds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/edvr/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/eg3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_afhq-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_ffhq-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_shapenet-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/eg3d/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/esrgan/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/esrgan/esrgan_psnr-x4c64b23g32_1xb16-1000k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/esrgan/esrgan_x4c64b23g32_1xb16-400k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/esrgan/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/flavr/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/flavr/flavr_in4out1_8xb4_vimeo90k-septuplet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/flavr/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/gca/
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/gca/baseline_r34_4xb10-200k_comp1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/gca/baseline_r34_4xb10-dimaug-200k_comp1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/gca/gca_r34_4xb10-200k_comp1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/gca/gca_r34_4xb10-dimaug-200k_comp1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/gca/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/ggan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/ggan/ggan_dcgan-archi_lr1e-3-1xb128-12Mimgs_celeba-cropped-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/ggan/ggan_dcgan-archi_lr1e-4-1xb64-10Mimgs_celeba-cropped-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/ggan/ggan_lsgan-archi_lr1e-4-1xb128-20Mimgs_lsun-bedroom-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/ggan/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/glean/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/glean/glean_in128out1024-fp16_4xb2-300k_ffhq-celeba-hq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/glean/glean_in128out1024_4xb2-300k_ffhq-celeba-hq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/glean/glean_x16-fp16_2xb8_ffhq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/glean/glean_x16_2xb8_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/glean/glean_x16_2xb8_ffhq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/glean/glean_x8-fp16_2xb8_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/glean/glean_x8_2xb8_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/glean/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/global_local/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/global_local/gl_8xb12_celeba-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/global_local/gl_8xb12_places-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/global_local/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/iconvsr/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_reds4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_vimeo90k-bd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_vimeo90k-bi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/iconvsr/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/indexnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/indexnet/indexnet_mobv2-dimaug_1xb16-78k_comp1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/indexnet/indexnet_mobv2_1xb16-78k_comp1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/indexnet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/inst_colorization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/inst_colorization/inst-colorizatioon_full_official_cocostuff-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/inst_colorization/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/liif/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/liif/liif-edsr-norm_c64b16_1xb16-1000k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/liif/liif-rdn-norm_c64b16_1xb16-1000k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/liif/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/lsgan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-3-1xb128-12Mimgs_celeba-cropped-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-4-1xb128-12Mimgs_lsun-bedroom-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-4-1xb64-10Mimgs_celeba-cropped-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/lsgan/lsgan_lsgan-archi_lr1e-4-1xb64-10Mimgs_lsun-bedroom-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/lsgan/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/nafnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/nafnet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/nafnet/nafnet_c64eb11128mb1db1111_8xb8-lr1e-3-400k_gopro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/nafnet/nafnet_c64eb2248mb12db2222_8xb8-lr1e-3-400k_sidd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/partial_conv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/partial_conv/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/partial_conv/pconv_stage1_8xb12_places-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/partial_conv/pconv_stage1_8xb1_celeba-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/partial_conv/pconv_stage2_4xb2_celeba-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/partial_conv/pconv_stage2_4xb2_places-256x256.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/pggan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/pggan/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/pggan/pggan_8xb4-12Mimg_celeba-hq-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/pggan/pggan_8xb4-12Mimgs_celeba-cropped-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/pggan/pggan_8xb4-12Mimgs_lsun-bedroom-128x128.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/pix2pix/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-220kiters_aerial2maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-220kiters_maps2aerial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-80kiters_facades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_wo-jitter-flip-1xb4-190kiters_edges2shoes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-c_c2_8xb3-1100kiters_ffhq-256-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-d_c2_8xb3-1100kiters_ffhq-256-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-e_c2_8xb3-1100kiters_ffhq-256-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c1_8xb2-1600kiters_ffhq-256-1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c2_8xb3-1100kiters_ffhq-256-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c2_8xb3-1100kiters_ffhq-256-896.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-g_c1_8xb3-1100kiters_ffhq-256-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-h_c2_8xb3-1100kiters_ffhq-256-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-i_c2_8xb3-1100kiters_ffhq-256-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-j_c2_8xb3-1100kiters_ffhq-256-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-k_c2_8xb3-1100kiters_ffhq-256-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan-csg_bohemian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan-csg_fish.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan_interp-pad_balloons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan_interp-pad_disc-nobn_balloons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan_interp-pad_disc-nobn_fish.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim4_bohemian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim4_fish.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim8_bohemian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/stylegan2_c2_8xb3-1100kiters_ffhq-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/stylegan2_c2_8xb3-1100kiters_ffhq-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/rdn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/rdn/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/rdn/rdn_x2c64b16_1xb16-1000k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/rdn/rdn_x3c64b16_1xb16-1000k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/rdn/rdn_x4c64b16_1xb16-1000k_div2k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/real_basicvsr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/real_basicvsr/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/real_basicvsr/realbasicvsr_c64b20-1x30x8_8xb1-lr5e-5-150k_reds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/real_basicvsr/realbasicvsr_wogan-c64b20-2x30x8_8xb2-lr1e-4-300k_reds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/real_esrgan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/real_esrgan/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/real_esrgan/realesrgan_c64b23g32_4xb12-lr1e-4-400k_df2k-ost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/real_esrgan/realesrnet_c64b23g32_4xb12-lr2e-4-1000k_df2k-ost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma15.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma25.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma15.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma25.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dpdd-dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dpdd-single.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_gopro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_rain13k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_sidd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/sagan/
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sagan/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_128_cvt_studioGAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_cvt-studioGAN_cifar10-32x32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_wReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_woReLUinplace-Glr1e-4_Dlr4e-4_noaug-ndisc1-8xb32-bigGAN-sch_imagenet1k-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_woReLUinplace_Glr1e-4_Dlr4e-4_ndisc1-4xb64_imagenet1k-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_woReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/singan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/singan/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/singan/singan_balloons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/singan/singan_bohemian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/singan/singan_fish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj-cvt-studioGAN_cifar10-32x32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj-cvt-studioGAN_imagenet1k-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj_wReLUinplace_Glr2e-4_Dlr5e-5_ndisc5-2xb128_imagenet1k-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj_wReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj_woReLUinplace_Glr2e-4_Dlr5e-5_ndisc5-2xb128_imagenet1k-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj_woReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/srcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/srcnn/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/srcnn/srcnn_x4k915_1xb16-1000k_div2k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/srgan_resnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/srgan_resnet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/srgan_resnet/msrresnet_x4c64b16_1xb16-1000k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/srgan_resnet/srgan_x4c64b16_1xb16-1000k_div2k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/stable_diffusion/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/stable_diffusion/stable-diffusion_ddim_denoisingunet-tomesd_5e-1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/stable_diffusion/stable-diffusion_ddim_denoisingunet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv1/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv1/styleganv1_ffhq-1024x1024_8xb4-25Mimgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv1/styleganv1_ffhq-256x256_8xb4-25Mimgs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv2/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2-PL-R1_8xb4-apex-fp16-no-scaler-800kiters_ffhq-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2-PL-R1_8xb4-fp16-globalG-partialD-no-scaler-800kiters_ffhq-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2-PL_8xb4-fp16-partial-GD-no-scaler-800kiters_ffhq-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_ffhq-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-cat-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-church-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-horse-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4_ffhq-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4_lsun-car-384x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-r_ada-gamma3.3_8xb4-fp16_metfaces-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4_ffhq-1024x1024.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4_ffhqu-256x256.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4x8_afhqv2-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_ada-gamma6.6_8xb4-fp16_metfaces-1024x1024.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_afhqv2-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_ffhq-1024x1024.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1383 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_ffhqu-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_gamma2.0_8xb4-fp16-noaug_ffhq-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_gamma32.8_8xb4-fp16-noaug_ffhq-1024x1024.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/
+-rw-r--r--   0 runner    (1001) docker     (123)    19414 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_gan-x2s64w8d6e180_8xb4-lr1e-4-600k_df2k-ost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_gan-x4s64w8d6e180_8xb4-lr1e-4-600k_df2k-ost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_gan-x4s64w8d9e240_8xb4-lr1e-4-600k_df2k-ost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_psnr-x2s64w8d6e180_8xb4-lr1e-4-600k_df2k-ost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_psnr-x4s64w8d6e180_8xb4-lr1e-4-600k_df2k-ost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_psnr-x4s64w8d9e240_8xb4-lr1e-4-600k_df2k-ost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR20.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR30.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR40.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR20.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR30.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR40.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN15.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN25.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN15.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN25.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x2s48w8d6e180_8xb4-lr2e-4-500k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x2s64w8d4e60_8xb4-lr2e-4-500k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x2s64w8d6e180_8xb4-lr2e-4-500k_df2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x3s48w8d6e180_8xb4-lr2e-4-500k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x3s64w8d4e60_8xb4-lr2e-4-500k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x3s64w8d6e180_8xb4-lr2e-4-500k_df2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x4s48w8d6e180_8xb4-lr2e-4-500k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x4s64w8d4e60_8xb4-lr2e-4-500k_div2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x4s64w8d6e180_8xb4-lr2e-4-500k_df2k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/tdan/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tdan/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tdan/tdan_x4_8xb16-lr1e-4-400k_vimeo90k-bd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tdan/tdan_x4_8xb16-lr1e-4-400k_vimeo90k-bi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tdan/tdan_x4ft_8xb16-lr5e-5-400k_vimeo90k-bi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tdan/tdan_x4ft_8xb16-lr5e-5-800k_vimeo90k-bd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/tof/
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tof/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tof/tof_spynet-chair-wobn_1xb1_vimeo90k-triplet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tof/tof_spynet-kitti-wobn_1xb1_vimeo90k-triplet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tof/tof_spynet-pytoflow-wobn_1xb1_vimeo90k-triplet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tof/tof_spynet-sintel-wobn-clean_1xb1_vimeo90k-triplet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tof/tof_spynet-sintel-wobn-final_1xb1_vimeo90k-triplet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/tof/tof_x4_official_vimeo90k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/ttsr/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/ttsr/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/ttsr/ttsr-gan_x4c64b16_1xb9-500k_CUFED.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/ttsr/ttsr-rec_x4c64b16_1xb9-200k_CUFED.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/configs/wgan-gp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/wgan-gp/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/wgan-gp/wgangp_GN-GP-50_1xb64-160kiters_lsun-bedroom-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/configs/wgan-gp/wgangp_GN_1xb64-160kiters_celeba-cropped-128x128.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/demo/download_inference_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/demo/gradio_controlnet_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/demo/gradio_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/demo/mmagic_inference_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/.mim/demo/singan_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-26 08:38:55.000000 mmagic-1.0.1/mmagic/.mim/model-index.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/analysis_tools/get_flops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/analysis_tools/print_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      265 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/cpu_train.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/bgm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/bgm/preprocess_bgm_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/comp1k/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      939 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/comp1k/check_extended_fg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/comp1k/evaluate_comp1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/comp1k/extend_fg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/comp1k/filter_comp1k_anno.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/comp1k/preprocess_comp1k_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/df2k_ost/
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/df2k_ost/preprocess_df2k_ost_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/div2k/
+-rw-r--r--   0 runner    (1001) docker     (123)    14978 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/div2k/preprocess_div2k_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/glean/
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/glean/preprocess_cat_test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/glean/preprocess_cat_train_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/glean/preprocess_ffhq_celebahq_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/reds/
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/reds/crop_sub_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/reds/preprocess_reds_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/sidd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/sidd/preprocess_sidd_test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/vid4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/vid4/preprocess_vid4_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/vimeo90k/
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/vimeo90k/preprocess_vimeo90k_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dist_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/dist_train.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/gui/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/gui/page_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34328 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/gui/page_sr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/gui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/.mim/tools/model_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/model_converters/publish_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/slurm_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      622 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/slurm_train.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-26 08:38:19.000000 mmagic-1.0.1/mmagic/.mim/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/apis/inferencers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/base_mmagic_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/colorization_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/conditional_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/controlnet_animation_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/eg3d_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/image_super_resolution_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/inference_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/inpainting_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/matting_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/text2image_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/translation_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/unconditional_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/video_interpolation_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/inferencers/video_restoration_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/apis/mmagic_inferencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/basic_conditional_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/basic_frames_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/basic_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29271 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/cifar10_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/comp1k_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/controlnet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/dreambooth_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/grow_scale_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/imagenet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/mscoco_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/paired_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/singan_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/datasets/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/aug_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/aug_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/aug_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/blur_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37682 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/fgbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/generate_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/generate_frame_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/get_masked_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/matlab_like_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/random_degradations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/random_down_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/trimap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/transforms/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/datasets/unpaired_image_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/hooks/iter_time_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/hooks/pggan_fetch_data_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/hooks/pickle_data_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/hooks/reduce_lr_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/hooks/visualization_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/engine/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/optimizers/multi_optimizer_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/optimizers/pggan_optimizer_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/optimizers/singan_optimizer_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/engine/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/runner/log_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/runner/loop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/runner/multi_loops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/engine/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/schedulers/linear_lr_scheduler_with_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/engine/schedulers/reduce_lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/evaluation/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/functional/fid_inception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/functional/gaussian_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/functional/inception_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/base_gen_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/base_sample_wise_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/connectivity_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/equivariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/fid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/gradient_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/inception_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/matting_mse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/ms_ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/mse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/niqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/niqe_pris_params.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/ppl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/precision_and_recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/sad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/evaluation/metrics/swd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/archs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/all_gather_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/gated_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/img_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/linear_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/multi_layer_disc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/patch_disc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18814 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/simple_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/smpatch_disc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/sr_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/archs/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/base_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/base_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/base_models/average_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/base_models/base_conditional_gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/base_models/base_edit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/base_models/base_gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/base_models/base_mattor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/base_models/base_translation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/base_models/basic_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17956 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/base_models/one_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14495 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/base_models/two_stage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/data_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/data_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37022 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/data_preprocessors/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/data_preprocessors/mattor_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/diffusion_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/diffusion_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/diffusion_schedulers/ddim_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/diffusion_schedulers/ddpm_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/aotgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/aotgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/aotgan/aot_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/aotgan/aot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/aotgan/aot_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/aotgan/aot_inpaintor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/aotgan/aot_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/arcface/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/arcface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/arcface/arcface_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/arcface/id_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/arcface/model_irse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/basicvsr/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/basicvsr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/basicvsr/basicvsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/basicvsr/basicvsr_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/basicvsr_plusplus_net/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/basicvsr_plusplus_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16236 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/basicvsr_plusplus_net/basicvsr_plusplus_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/biggan/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/biggan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/biggan/biggan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/biggan/biggan_deep_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/biggan/biggan_deep_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/biggan/biggan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/biggan/biggan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30009 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/biggan/biggan_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/biggan/biggan_snmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/cain/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/cain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/cain/cain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/cain/cain_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/controlnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36120 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/controlnet/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/controlnet/controlnet_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/cyclegan/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/cyclegan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/cyclegan/cyclegan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/cyclegan/cyclegan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/cyclegan/cyclegan_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/dcgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dcgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dcgan/dcgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dcgan/dcgan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dcgan/dcgan_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/ddpm/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ddpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21369 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ddpm/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52981 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ddpm/denoising_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ddpm/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ddpm/res_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20328 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ddpm/unet_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv1/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv1/contextual_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv1/contextual_attention_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv1/deepfill_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv1/deepfill_disc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv1/deepfill_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv1/deepfill_refiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv1/deepfillv1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/deepfillv2/two_stage_encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/dic/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dic/dic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dic/dic_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dic/feedback_hour_glass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dic/light_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/dim/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dim/dim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/disco_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/disco_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/disco_diffusion/clip_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/disco_diffusion/disco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19913 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/disco_diffusion/guider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/disco_diffusion/secondary_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/dreambooth/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dreambooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/dreambooth/dreambooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/duf/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/duf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/duf/duf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/edsr/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/edsr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/edsr/edsr_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/edvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/edvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/edvr/edvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18568 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/edvr/edvr_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/eg3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/eg3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20954 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/eg3d/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/eg3d/dual_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/eg3d/eg3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/eg3d/eg3d_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/eg3d/eg3d_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/eg3d/eg3d_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/eg3d/ray_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24026 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/eg3d/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/esrgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/esrgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/esrgan/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/esrgan/rrdb_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/fba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/fba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/fba/fba_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/fba/fba_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/flavr/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/flavr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/flavr/flavr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18189 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/flavr/flavr_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/gca/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/gca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/gca/gca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/gca/gca_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/gca/resgca_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/gca/resgca_enc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/ggan/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ggan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ggan/ggan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/glean/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/glean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/glean/glean_styleganv2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/global_local/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/global_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/global_local/gl_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/global_local/gl_dilation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/global_local/gl_disc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/global_local/gl_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/global_local/gl_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/global_local/gl_inpaintor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/guided_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/guided_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/guided_diffusion/adm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/guided_diffusion/classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/iconvsr/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/iconvsr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/iconvsr/iconvsr_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/indexnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/indexnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/indexnet/indexnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/indexnet/indexnet_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/indexnet/indexnet_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/inst_colorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/inst_colorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/inst_colorization/color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/inst_colorization/colorization_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/inst_colorization/fusion_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/inst_colorization/inst_colorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/inst_colorization/weight_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/liif/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/liif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/liif/liif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/liif/liif_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/liif/mlp_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/lsgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/lsgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/lsgan/lsgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/lsgan/lsgan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/lsgan/lsgan_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/mspie/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/mspie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/mspie/mspie_stylegan2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/mspie/mspie_stylegan2_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/mspie/mspie_stylegan2_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/mspie/mspie_stylegan2_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/mspie/pe_singan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/mspie/pe_singan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/mspie/positional_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/nafnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/nafnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/nafnet/naf_avgpool2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/nafnet/naf_layerNorm2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/nafnet/nafbaseline_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/nafnet/nafnet_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/pconv/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pconv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pconv/mask_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pconv/partial_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pconv/pconv_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pconv/pconv_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pconv/pconv_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pconv/pconv_inpaintor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/pggan/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pggan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20644 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pggan/pggan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pggan/pggan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pggan/pggan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19717 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pggan/pggan_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pix2pix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pix2pix/pix2pix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pix2pix/pix2pix_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/pix2pix/pix2pix_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/plain/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/plain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/plain/plain_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/plain/plain_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/rdn/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/rdn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/rdn/rdn_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/real_basicvsr/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/real_basicvsr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/real_basicvsr/real_basicvsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/real_basicvsr/real_basicvsr_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/real_esrgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/real_esrgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/real_esrgan/real_esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/real_esrgan/unet_disc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/restormer/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/restormer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17236 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/restormer/restormer_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/sagan/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/sagan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/sagan/sagan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17474 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/sagan/sagan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/sagan/sagan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25894 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/sagan/sagan_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/singan/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/singan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28077 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/singan/singan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/singan/singan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/singan/singan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/singan/singan_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/srcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/srcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/srcnn/srcnn_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/srgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/srgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/srgan/modified_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/srgan/sr_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/srgan/srgan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stable_diffusion/clip_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26832 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stable_diffusion/stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34487 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/stylegan1/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan1/stylegan1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan1/stylegan1_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan1/stylegan1_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan1/stylegan1_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan1/stylegan_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/ada/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/ada/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32653 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/ada/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/ada/grid_sample_gradfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/ada/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/ada/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/stylegan2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/stylegan2_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23414 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/stylegan2_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan2/stylegan2_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/stylegan3/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan3/stylegan3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan3/stylegan3_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28215 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan3/stylegan3_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/stylegan3/stylegan3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/swinir/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/swinir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/swinir/swinir_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/swinir/swinir_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/swinir/swinir_rstb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/swinir/swinir_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/tdan/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/tdan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/tdan/tdan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/tdan/tdan_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/tof/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/tof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/tof/tof_vfi_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/tof/tof_vsr_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/ttsr/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ttsr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ttsr/lte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ttsr/search_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ttsr/ttsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ttsr/ttsr_disc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13923 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/ttsr/ttsr_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/editors/wgan_gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/wgan_gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/wgan_gp/wgan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/wgan_gp/wgan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/wgan_gp/wgan_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/editors/wgan_gp/wgan_gp_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/clip_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/composition_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/face_id_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/feature_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21057 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/gan_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/gradient_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/losses/loss_comps/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/loss_comps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/loss_comps/clip_loss_comps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/loss_comps/disc_auxiliary_loss_comps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/loss_comps/face_id_loss_comps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/loss_comps/gan_loss_comps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/loss_comps/gen_auxiliary_loss_comps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/loss_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/perceptual_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/losses/pixelwise_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/utils/bbox_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/utils/diffusion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/utils/flow_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/utils/sampling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/utils/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/models/utils/tome_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/structures/data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/utils/img_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/utils/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/utils/trans_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/visualization/concat_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/visualization/vis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-26 08:38:18.000000 mmagic-1.0.1/mmagic/visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43009 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 08:38:56.000000 mmagic-1.0.1/mmagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:38:56.000000 mmagic-1.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-26 08:38:19.000000 mmagic-1.0.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 08:38:19.000000 mmagic-1.0.1/requirements/mminstall.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 08:38:19.000000 mmagic-1.0.1/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-26 08:38:19.000000 mmagic-1.0.1/requirements/readthedocs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-26 08:38:19.000000 mmagic-1.0.1/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-26 08:38:19.000000 mmagic-1.0.1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-26 08:38:56.000000 mmagic-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-05-26 08:38:19.000000 mmagic-1.0.1/setup.py
```

### Comparing `mmagic-1.0.0/PKG-INFO` & `mmagic-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmagic
-Version: 1.0.0
+Version: 1.0.1
 Summary: OpenMMLab Multimodal Advanced, Generative, and Intelligent Creation Toolbox
 Home-page: https://github.com/open-mmlab/mmagic
 Maintainer: MMagic Contributors
 Maintainer-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div id="top" align="center">
           <img src="docs/en/_static/image/mmagic-logo.png" width="500px"/>
@@ -61,15 +61,21 @@
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
         </div>
         
         ## 🚀 What's New <a><img width="35" height="20" src="https://user-images.githubusercontent.com/12782558/212848161-5e783dd6-11e8-4fe0-bbba-39ffb77730be.png"></a>
         
-        ### New release [**MMagic v1.0.0**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.0) \[25/04/2023\]:
+        ### New release [**MMagic v1.0.1**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.1) \[26/05/2023\]:
+        
+        - Support tomesd for StableDiffusion speed-up.
+        - Support all inpainting/matting/image restoration models inferencer.
+        - Support animated drawings.
+        - Support Style-Based Global Appearance Flow for Virtual Try-On.
+        - Fix inferencer in pip-install.
         
         We are excited to announce the release of MMagic v1.0.0 that inherits from [MMEditing](https://github.com/open-mmlab/mmediting) and [MMGeneration](https://github.com/open-mmlab/mmgeneration).
         
         After iterative updates with OpenMMLab 2.0 framework and merged with MMGeneration, MMEditing has become a powerful tool that supports low-level algorithms based on both GAN and CNN. Today, MMEditing embraces Generative AI and transforms into a more advanced and comprehensive AIGC toolkit: **MMagic** (**M**ultimodal **A**dvanced, **G**enerative, and **I**ntelligent **C**reation). MMagic will provide more agile and flexible experimental support for researchers and AIGC enthusiasts, and help you on your AIGC exploration journey.
         
         We highlight the following new features.
         
@@ -380,14 +386,15 @@
                 <ul>
                   <li><a href="projects/glide/configs/README.md">GLIDE (NeurIPS'2021)</a></li>
                   <li><a href="configs/guided_diffusion/README.md">Guided Diffusion (NeurIPS'2021)</a></li>
                   <li><a href="configs/disco_diffusion/README.md">Disco-Diffusion (2022)</a></li>
                   <li><a href="configs/stable_diffusion/README.md">Stable-Diffusion (2022)</a></li>
                   <li><a href="configs/dreambooth/README.md">DreamBooth (2022)</a></li>
                   <li><a href="configs/controlnet/README.md">ControlNet (2023)</a></li>
+                  <li><a href="configs/controlnet_animation/README.md">ControlNet Animation (2023)</a></li>
                 </ul>
               </td>
               <td>
                 <ul>
                   <li><a href="configs/eg3d/README.md">EG3D (CVPR'2022)</a></li>
                 </ul>
               </td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmagic Version: 1.0.0 Summary: OpenMMLab Multimodal
+Metadata-Version: 2.1 Name: mmagic Version: 1.0.1 Summary: OpenMMLab Multimodal
 Advanced, Generative, and Intelligent Creation Toolbox Home-page: https://
 github.com/open-mmlab/mmagic Maintainer: MMagic Contributors Maintainer-email:
 openmmlab@gmail.com License: Apache License 2.0 Description:
                     [docs/en/_static/image/mmagic-logo.png]
                                         
       Multimodal Advanced, Generative, and Intelligent Creation (MMagic
                                 [em'mÃ¦dÊÉªk])
@@ -26,28 +26,31 @@
  News](https://mmagic.readthedocs.io/en/latest/changelog.html) | [ðOngoing
    Projects](https://github.com/open-mmlab/mmagic/projects) | [ð¤Reporting
  Issues](https://github.com/open-mmlab/mmagic/issues) English | [ç®ä½ä¸­æ]
                                (README_zh-CN.md)
 
 ## ð What's New [https://user-images.githubusercontent.com/12782558/
 212848161-5e783dd6-11e8-4fe0-bbba-39ffb77730be.png] ### New release [**MMagic
-v1.0.0**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.0) \[25/04/
-2023\]: We are excited to announce the release of MMagic v1.0.0 that inherits
-from [MMEditing](https://github.com/open-mmlab/mmediting) and [MMGeneration]
-(https://github.com/open-mmlab/mmgeneration). After iterative updates with
-OpenMMLab 2.0 framework and merged with MMGeneration, MMEditing has become a
-powerful tool that supports low-level algorithms based on both GAN and CNN.
-Today, MMEditing embraces Generative AI and transforms into a more advanced and
-comprehensive AIGC toolkit: **MMagic** (**M**ultimodal **A**dvanced,
-**G**enerative, and **I**ntelligent **C**reation). MMagic will provide more
-agile and flexible experimental support for researchers and AIGC enthusiasts,
-and help you on your AIGC exploration journey. We highlight the following new
-features. **1. New Models** We support 11 new models in 4 new tasks. -
-Text2Image / Diffusion - ControlNet - DreamBooth - Stable Diffusion - Disco
-Diffusion - GLIDE - Guided Diffusion - 3D-aware Generation - EG3D - Image
+v1.0.1**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.1) \[26/05/
+2023\]: - Support tomesd for StableDiffusion speed-up. - Support all
+inpainting/matting/image restoration models inferencer. - Support animated
+drawings. - Support Style-Based Global Appearance Flow for Virtual Try-On. -
+Fix inferencer in pip-install. We are excited to announce the release of MMagic
+v1.0.0 that inherits from [MMEditing](https://github.com/open-mmlab/mmediting)
+and [MMGeneration](https://github.com/open-mmlab/mmgeneration). After iterative
+updates with OpenMMLab 2.0 framework and merged with MMGeneration, MMEditing
+has become a powerful tool that supports low-level algorithms based on both GAN
+and CNN. Today, MMEditing embraces Generative AI and transforms into a more
+advanced and comprehensive AIGC toolkit: **MMagic** (**M**ultimodal
+**A**dvanced, **G**enerative, and **I**ntelligent **C**reation). MMagic will
+provide more agile and flexible experimental support for researchers and AIGC
+enthusiasts, and help you on your AIGC exploration journey. We highlight the
+following new features. **1. New Models** We support 11 new models in 4 new
+tasks. - Text2Image / Diffusion - ControlNet - DreamBooth - Stable Diffusion -
+Disco Diffusion - GLIDE - Guided Diffusion - 3D-aware Generation - EG3D - Image
 Restoration - NAFNet - Restormer - SwinIR - Image Colorization -
 InstColorization **2. Magic Diffusion Model** For the Diffusion Model, we
 provide the following "magic" : - Support image generation based on Stable
 Diffusion and Disco Diffusion. - Support Finetune methods such as Dreambooth
 and DreamBooth LoRA. - Support controllability in text-to-image generation
 using ControlNet. - Support acceleration and optimization strategies based on
 xFormers to improve training and inference efficiency. - Support video
@@ -187,14 +190,16 @@
       (ECCV'2018)        (AAAI'2020)          (2022)
     * DeepFillv2_                           * Stable-Diffusion
       (CVPR'2019)                             (2022)
     * AOT-GAN_                              * DreamBooth_
       (TVCG'2019)                             (2022)
                                             * ControlNet_
                                               (2023)
+                                            * ControlNet
+                                              Animation_(2023)
 Please refer to [model_zoo](https://mmagic.readthedocs.io/en/latest/model_zoo/
 overview.html) for more details.
                                                                 ðBack_to_top
 ## ð¤ Acknowledgement MMagic is an open source project that is contributed by
 researchers and engineers from various colleges and companies. We wish that the
 toolbox and benchmark could serve the growing research community by providing a
 flexible toolkit to reimplement existing methods and develop their own new
```

### Comparing `mmagic-1.0.0/README.md` & `mmagic-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,21 @@
   <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
   <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
     <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
 </div>
 
 ## 🚀 What's New <a><img width="35" height="20" src="https://user-images.githubusercontent.com/12782558/212848161-5e783dd6-11e8-4fe0-bbba-39ffb77730be.png"></a>
 
-### New release [**MMagic v1.0.0**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.0) \[25/04/2023\]:
+### New release [**MMagic v1.0.1**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.1) \[26/05/2023\]:
+
+- Support tomesd for StableDiffusion speed-up.
+- Support all inpainting/matting/image restoration models inferencer.
+- Support animated drawings.
+- Support Style-Based Global Appearance Flow for Virtual Try-On.
+- Fix inferencer in pip-install.
 
 We are excited to announce the release of MMagic v1.0.0 that inherits from [MMEditing](https://github.com/open-mmlab/mmediting) and [MMGeneration](https://github.com/open-mmlab/mmgeneration).
 
 After iterative updates with OpenMMLab 2.0 framework and merged with MMGeneration, MMEditing has become a powerful tool that supports low-level algorithms based on both GAN and CNN. Today, MMEditing embraces Generative AI and transforms into a more advanced and comprehensive AIGC toolkit: **MMagic** (**M**ultimodal **A**dvanced, **G**enerative, and **I**ntelligent **C**reation). MMagic will provide more agile and flexible experimental support for researchers and AIGC enthusiasts, and help you on your AIGC exploration journey.
 
 We highlight the following new features.
 
@@ -372,14 +378,15 @@
         <ul>
           <li><a href="projects/glide/configs/README.md">GLIDE (NeurIPS'2021)</a></li>
           <li><a href="configs/guided_diffusion/README.md">Guided Diffusion (NeurIPS'2021)</a></li>
           <li><a href="configs/disco_diffusion/README.md">Disco-Diffusion (2022)</a></li>
           <li><a href="configs/stable_diffusion/README.md">Stable-Diffusion (2022)</a></li>
           <li><a href="configs/dreambooth/README.md">DreamBooth (2022)</a></li>
           <li><a href="configs/controlnet/README.md">ControlNet (2023)</a></li>
+          <li><a href="configs/controlnet_animation/README.md">ControlNet Animation (2023)</a></li>
         </ul>
       </td>
       <td>
         <ul>
           <li><a href="configs/eg3d/README.md">EG3D (CVPR'2022)</a></li>
         </ul>
       </td>
```

#### html2text {}

```diff
@@ -22,28 +22,31 @@
  News](https://mmagic.readthedocs.io/en/latest/changelog.html) | [ðOngoing
    Projects](https://github.com/open-mmlab/mmagic/projects) | [ð¤Reporting
  Issues](https://github.com/open-mmlab/mmagic/issues) English | [ç®ä½ä¸­æ]
                                (README_zh-CN.md)
 
 ## ð What's New [https://user-images.githubusercontent.com/12782558/
 212848161-5e783dd6-11e8-4fe0-bbba-39ffb77730be.png] ### New release [**MMagic
-v1.0.0**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.0) \[25/04/
-2023\]: We are excited to announce the release of MMagic v1.0.0 that inherits
-from [MMEditing](https://github.com/open-mmlab/mmediting) and [MMGeneration]
-(https://github.com/open-mmlab/mmgeneration). After iterative updates with
-OpenMMLab 2.0 framework and merged with MMGeneration, MMEditing has become a
-powerful tool that supports low-level algorithms based on both GAN and CNN.
-Today, MMEditing embraces Generative AI and transforms into a more advanced and
-comprehensive AIGC toolkit: **MMagic** (**M**ultimodal **A**dvanced,
-**G**enerative, and **I**ntelligent **C**reation). MMagic will provide more
-agile and flexible experimental support for researchers and AIGC enthusiasts,
-and help you on your AIGC exploration journey. We highlight the following new
-features. **1. New Models** We support 11 new models in 4 new tasks. -
-Text2Image / Diffusion - ControlNet - DreamBooth - Stable Diffusion - Disco
-Diffusion - GLIDE - Guided Diffusion - 3D-aware Generation - EG3D - Image
+v1.0.1**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.1) \[26/05/
+2023\]: - Support tomesd for StableDiffusion speed-up. - Support all
+inpainting/matting/image restoration models inferencer. - Support animated
+drawings. - Support Style-Based Global Appearance Flow for Virtual Try-On. -
+Fix inferencer in pip-install. We are excited to announce the release of MMagic
+v1.0.0 that inherits from [MMEditing](https://github.com/open-mmlab/mmediting)
+and [MMGeneration](https://github.com/open-mmlab/mmgeneration). After iterative
+updates with OpenMMLab 2.0 framework and merged with MMGeneration, MMEditing
+has become a powerful tool that supports low-level algorithms based on both GAN
+and CNN. Today, MMEditing embraces Generative AI and transforms into a more
+advanced and comprehensive AIGC toolkit: **MMagic** (**M**ultimodal
+**A**dvanced, **G**enerative, and **I**ntelligent **C**reation). MMagic will
+provide more agile and flexible experimental support for researchers and AIGC
+enthusiasts, and help you on your AIGC exploration journey. We highlight the
+following new features. **1. New Models** We support 11 new models in 4 new
+tasks. - Text2Image / Diffusion - ControlNet - DreamBooth - Stable Diffusion -
+Disco Diffusion - GLIDE - Guided Diffusion - 3D-aware Generation - EG3D - Image
 Restoration - NAFNet - Restormer - SwinIR - Image Colorization -
 InstColorization **2. Magic Diffusion Model** For the Diffusion Model, we
 provide the following "magic" : - Support image generation based on Stable
 Diffusion and Disco Diffusion. - Support Finetune methods such as Dreambooth
 and DreamBooth LoRA. - Support controllability in text-to-image generation
 using ControlNet. - Support acceleration and optimization strategies based on
 xFormers to improve training and inference efficiency. - Support video
@@ -183,14 +186,16 @@
       (ECCV'2018)        (AAAI'2020)          (2022)
     * DeepFillv2_                           * Stable-Diffusion
       (CVPR'2019)                             (2022)
     * AOT-GAN_                              * DreamBooth_
       (TVCG'2019)                             (2022)
                                             * ControlNet_
                                               (2023)
+                                            * ControlNet
+                                              Animation_(2023)
 Please refer to [model_zoo](https://mmagic.readthedocs.io/en/latest/model_zoo/
 overview.html) for more details.
                                                                 ðBack_to_top
 ## ð¤ Acknowledgement MMagic is an open source project that is contributed by
 researchers and engineers from various colleges and companies. We wish that the
 toolbox and benchmark could serve the growing research community by providing a
 flexible toolkit to reimplement existing methods and develop their own new
```

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/basicvsr_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/basicvsr_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/celeba.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/celeba.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/cifar10_noaug.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/cifar10_noaug.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/cifar10_nopad.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/cifar10_nopad.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/comp1k.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/comp1k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/deblurring-defocus_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/deblurring-defocus_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/deblurring-motion_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/deblurring-motion_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/decompression_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/decompression_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/denoising-gaussian_color_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/denoising-gaussian_color_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/denoising-gaussian_gray_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/denoising-gaussian_gray_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/denoising-real_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/denoising-real_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/deraining_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/deraining_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/ffhq_flip.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/ffhq_flip.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/grow_scale_imgs_ffhq_styleganv1.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/grow_scale_imgs_ffhq_styleganv1.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/imagenet_128.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/imagenet_128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/imagenet_256.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/imagenet_256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/imagenet_512.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/imagenet_512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/imagenet_64.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/imagenet_64.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/imagenet_noaug_128.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/imagenet_noaug_128.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # dataset settings
 dataset_type = 'ImageNet'
 
 # different from mmcls, we adopt the setting used in BigGAN.
 # Remove `RandomFlip` augmentation and change `RandomCropLongEdge` to
-# `CenterCropLongEdge` to elminiate randomness.
+# `CenterCropLongEdge` to eliminate randomness.
 # dataset settings
 train_pipeline = [
     dict(type='LoadImageFromFile', key='img'),
     dict(type='CenterCropLongEdge'),
     dict(type='Resize', scale=(128, 128), backend='pillow'),
     dict(type='PackInputs')
 ]
```

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/liif_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/liif_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/lsun_stylegan.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/lsun_stylegan.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/paired_imgs_256x256_crop.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/paired_imgs_256x256_crop.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/places.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/places.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/sisr_x2_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/sisr_x2_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/sisr_x3_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/sisr_x3_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/sisr_x4_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/sisr_x4_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/tdan_test_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/tdan_test_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_64x64.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_64x64.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_flip_512x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_flip_512x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_flip_lanczos_resize_256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/unconditional_imgs_flip_lanczos_resize_256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/datasets/unpaired_imgs_256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/datasets/unpaired_imgs_256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/default_runtime.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/gen_default_runtime.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/gen_default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/inpaint_default_runtime.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/inpaint_default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/matting_default_runtime.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/matting_default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_cyclegan.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_cyclegan.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_deepfillv1.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_deepfillv1.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_deepfillv2.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_deepfillv2.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_edvr.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_edvr.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_gl.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_gl.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_glean.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_glean.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_liif.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_liif.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_pconv.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_pconv.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_pix2pix.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_pix2pix.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_styleganv2.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_styleganv2.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_styleganv3.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_styleganv3.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/base_tof.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/base_tof.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/biggan/base_biggan_128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/biggan/base_biggan_128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/sagan/base_sagan_128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/sagan/base_sagan_128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/_base_/models/sagan/base_sagan_32x32.py` & `mmagic-1.0.1/mmagic/.mim/configs/_base_/models/sagan/base_sagan_32x32.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/aot_gan/aot-gan_smpgan_4xb4_places-512x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/aot_gan/aot-gan_smpgan_4xb4_places-512x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/aot_gan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/aot_gan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/basicvsr/basicvsr_2xb4_reds4.py` & `mmagic-1.0.1/mmagic/.mim/configs/basicvsr/basicvsr_2xb4_reds4.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/basicvsr/basicvsr_2xb4_vimeo90k-bd.py` & `mmagic-1.0.1/mmagic/.mim/configs/basicvsr/basicvsr_2xb4_vimeo90k-bd.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/basicvsr/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/basicvsr/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-decompress-track1.py` & `mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-decompress-track1.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-vsr.py` & `mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c128n25_600k_ntire-vsr.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_4xb2-300k_vimeo90k-bd.py` & `mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_4xb2-300k_vimeo90k-bd.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_4xb2-300k_vimeo90k-bi.py` & `mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_4xb2-300k_vimeo90k-bi.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_8xb1-600k_reds4.py` & `mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/basicvsr-pp_c64n7_8xb1-600k_reds4.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/basicvsr_pp/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/basicvsr_pp/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face-rgb_imagenet1k-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face-rgb_imagenet1k-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face_rgb_imagenet1k-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face_rgb_imagenet1k-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face_rgb_imagenet1k-512x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan-deep_cvt-hugging-face_rgb_imagenet1k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan_2xb25-500kiters_cifar10-32x32.py` & `mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan_2xb25-500kiters_cifar10-32x32.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan_ajbrock-sn_8xb32-1500kiters_imagenet1k-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan_ajbrock-sn_8xb32-1500kiters_imagenet1k-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/biggan/biggan_cvt-BigGAN-PyTorch-rgb_imagenet1k-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/biggan/biggan_cvt-BigGAN-PyTorch-rgb_imagenet1k-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/biggan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/biggan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/cain/cain_g1b32_1xb5_vimeo90k-triplet.py` & `mmagic-1.0.1/mmagic/.mim/configs/cain/cain_g1b32_1xb5_vimeo90k-triplet.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/cain/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/cain/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/controlnet/controlnet-1xb1-fill50k.py` & `mmagic-1.0.1/mmagic/.mim/configs/controlnet/controlnet-1xb1-fill50k.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         data_keys='prompt',
         meta_keys=[
             'source_channel_order', 'source_color_type',
             'target_channel_order', 'target_color_type'
         ])
 ]
 dataset = dict(
-    type='ControlDataset',
+    type='ControlNetDataset',
     data_root='./data/fill50k',
     ann_file='prompt.json',
     pipeline=pipeline)
 train_dataloader = dict(
     dataset=dataset,
     num_workers=16,
     sampler=dict(type='InfiniteSampler', shuffle=True),
```

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/controlnet/controlnet-canny.py` & `mmagic-1.0.1/mmagic/.mim/configs/controlnet/controlnet-canny.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/controlnet/controlnet-pose.py` & `mmagic-1.0.1/mmagic/.mim/configs/controlnet/controlnet-pose.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/controlnet/controlnet-seg.py` & `mmagic-1.0.1/mmagic/.mim/configs/controlnet/controlnet-seg.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/controlnet/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/controlnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/controlnet_animation/anythingv3_config.py` & `mmagic-1.0.1/mmagic/.mim/configs/controlnet_animation/anythingv3_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-250kiters_summer2winter.py` & `mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-250kiters_summer2winter.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-270kiters_horse2zebra.py` & `mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-270kiters_horse2zebra.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-80kiters_facades.py` & `mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-id0-resnet-in_1xb1-80kiters_facades.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-250kiters_summer2winter.py` & `mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-250kiters_summer2winter.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-270kiters_horse2zebra.py` & `mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-270kiters_horse2zebra.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-80kiters_facades.py` & `mmagic-1.0.1/mmagic/.mim/configs/cyclegan/cyclegan_lsgan-resnet-in_1xb1-80kiters_facades.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/cyclegan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/cyclegan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dcgan/dcgan_1xb128-300kiters_celeba-cropped-64.py` & `mmagic-1.0.1/mmagic/.mim/configs/dcgan/dcgan_1xb128-300kiters_celeba-cropped-64.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dcgan/dcgan_1xb128-5epoches_lsun-bedroom-64x64.py` & `mmagic-1.0.1/mmagic/.mim/configs/dcgan/dcgan_1xb128-5epoches_lsun-bedroom-64x64.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dcgan/dcgan_Glr4e-4_Dlr1e-4_1xb128-5kiters_mnist-64x64.py` & `mmagic-1.0.1/mmagic/.mim/configs/dcgan/dcgan_Glr4e-4_Dlr1e-4_1xb128-5kiters_mnist-64x64.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dcgan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/dcgan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/deepfillv1/deepfillv1_4xb4_celeba-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/deepfillv1/deepfillv1_4xb4_celeba-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/deepfillv1/deepfillv1_8xb2_places-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/deepfillv1/deepfillv1_8xb2_places-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/deepfillv1/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/deepfillv1/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/deepfillv2/deepfillv2_8xb2_celeba-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/deepfillv2/deepfillv2_8xb2_celeba-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/deepfillv2/deepfillv2_8xb2_places-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/deepfillv2/deepfillv2_8xb2_places-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/deepfillv2/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/deepfillv2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dic/dic_gan-x8c48b6_4xb2-500k_celeba-hq.py` & `mmagic-1.0.1/mmagic/.mim/configs/dic/dic_gan-x8c48b6_4xb2-500k_celeba-hq.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dic/dic_x8c48b6_4xb2-150k_celeba-hq.py` & `mmagic-1.0.1/mmagic/.mim/configs/dic/dic_x8c48b6_4xb2-150k_celeba-hq.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dic/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/dic/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dim/dim_stage1-v16_1xb1-1000k_comp1k.py` & `mmagic-1.0.1/mmagic/.mim/configs/dim/dim_stage1-v16_1xb1-1000k_comp1k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dim/dim_stage1-v16_1xb1-1000k_comp1k_online-merge.py` & `mmagic-1.0.1/mmagic/.mim/configs/dim/dim_stage1-v16_1xb1-1000k_comp1k_online-merge.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dim/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/dim/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/disco_diffusion/disco-diffusion_adm-u-finetuned_imagenet-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/disco_diffusion/disco-diffusion_adm-u-finetuned_imagenet-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/disco_diffusion/disco-diffusion_adm-u-finetuned_imagenet-512x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/disco_diffusion/disco-diffusion_adm-u-finetuned_imagenet-512x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/disco_diffusion/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/disco_diffusion/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dreambooth/dreambooth-finetune_text_encoder.py` & `mmagic-1.0.1/mmagic/.mim/configs/dreambooth/dreambooth-finetune_text_encoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dreambooth/dreambooth-lora.py` & `mmagic-1.0.1/mmagic/.mim/configs/dreambooth/dreambooth-lora.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dreambooth/dreambooth.py` & `mmagic-1.0.1/mmagic/.mim/configs/dreambooth/dreambooth.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/dreambooth/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/dreambooth/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/edsr/edsr_x2c64b16_1xb16-300k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/edsr/edsr_x2c64b16_1xb16-300k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/edsr/edsr_x3c64b16_1xb16-300k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/edsr/edsr_x3c64b16_1xb16-300k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/edsr/edsr_x4c64b16_1xb16-300k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/edsr/edsr_x4c64b16_1xb16-300k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/edsr/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/edsr/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/edvr/edvrl_c128b40_8xb8-lr2e-4-600k_reds4.py` & `mmagic-1.0.1/mmagic/.mim/configs/edvr/edvrl_c128b40_8xb8-lr2e-4-600k_reds4.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/edvr/edvrl_wotsa-c128b40_8xb8-lr2e-4-600k_reds4.py` & `mmagic-1.0.1/mmagic/.mim/configs/edvr/edvrl_wotsa-c128b40_8xb8-lr2e-4-600k_reds4.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/edvr/edvrm_8xb4-600k_reds.py` & `mmagic-1.0.1/mmagic/.mim/configs/edvr/edvrm_8xb4-600k_reds.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/edvr/edvrm_wotsa_8xb4-600k_reds.py` & `mmagic-1.0.1/mmagic/.mim/configs/edvr/edvrm_wotsa_8xb4-600k_reds.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/edvr/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/edvr/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_afhq-512x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_afhq-512x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_ffhq-512x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_ffhq-512x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_shapenet-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/eg3d/eg3d_cvt-official-rgb_shapenet-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/eg3d/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/eg3d/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/esrgan/esrgan_psnr-x4c64b23g32_1xb16-1000k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/esrgan/esrgan_psnr-x4c64b23g32_1xb16-1000k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/esrgan/esrgan_x4c64b23g32_1xb16-400k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/esrgan/esrgan_x4c64b23g32_1xb16-400k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/esrgan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/esrgan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/flavr/flavr_in4out1_8xb4_vimeo90k-septuplet.py` & `mmagic-1.0.1/mmagic/.mim/configs/flavr/flavr_in4out1_8xb4_vimeo90k-septuplet.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/flavr/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/flavr/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/gca/baseline_r34_4xb10-200k_comp1k.py` & `mmagic-1.0.1/mmagic/.mim/configs/gca/baseline_r34_4xb10-200k_comp1k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/gca/baseline_r34_4xb10-dimaug-200k_comp1k.py` & `mmagic-1.0.1/mmagic/.mim/configs/gca/baseline_r34_4xb10-dimaug-200k_comp1k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/gca/gca_r34_4xb10-200k_comp1k.py` & `mmagic-1.0.1/mmagic/.mim/configs/gca/gca_r34_4xb10-200k_comp1k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/gca/gca_r34_4xb10-dimaug-200k_comp1k.py` & `mmagic-1.0.1/mmagic/.mim/configs/gca/gca_r34_4xb10-dimaug-200k_comp1k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/gca/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/gca/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/ggan/ggan_dcgan-archi_lr1e-3-1xb128-12Mimgs_celeba-cropped-64x64.py` & `mmagic-1.0.1/mmagic/.mim/configs/ggan/ggan_dcgan-archi_lr1e-3-1xb128-12Mimgs_celeba-cropped-64x64.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/ggan/ggan_dcgan-archi_lr1e-4-1xb64-10Mimgs_celeba-cropped-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/ggan/ggan_dcgan-archi_lr1e-4-1xb64-10Mimgs_celeba-cropped-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/ggan/ggan_lsgan-archi_lr1e-4-1xb128-20Mimgs_lsun-bedroom-64x64.py` & `mmagic-1.0.1/mmagic/.mim/configs/ggan/ggan_lsgan-archi_lr1e-4-1xb128-20Mimgs_lsun-bedroom-64x64.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/ggan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/ggan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/glean/glean_in128out1024_4xb2-300k_ffhq-celeba-hq.py` & `mmagic-1.0.1/mmagic/.mim/configs/glean/glean_in128out1024_4xb2-300k_ffhq-celeba-hq.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/glean/glean_x16_2xb8_cat.py` & `mmagic-1.0.1/mmagic/.mim/configs/glean/glean_x16_2xb8_cat.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/glean/glean_x16_2xb8_ffhq.py` & `mmagic-1.0.1/mmagic/.mim/configs/glean/glean_x16_2xb8_ffhq.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/glean/glean_x8_2xb8_cat.py` & `mmagic-1.0.1/mmagic/.mim/configs/glean/glean_x8_2xb8_cat.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/glean/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/glean/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/global_local/gl_8xb12_celeba-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/global_local/gl_8xb12_celeba-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/global_local/gl_8xb12_places-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/global_local/gl_8xb12_places-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/global_local/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/global_local/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-512x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-512x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-64x64.py` & `mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm-g_ddim25_8xb32_imagenet-64x64.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-512x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-512x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-64x64.py` & `mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/adm_ddim250_8xb32_imagenet-64x64.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/guided_diffusion/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/guided_diffusion/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_reds4.py` & `mmagic-1.0.1/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_reds4.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_vimeo90k-bd.py` & `mmagic-1.0.1/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_vimeo90k-bd.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_vimeo90k-bi.py` & `mmagic-1.0.1/mmagic/.mim/configs/iconvsr/iconvsr_2xb4_vimeo90k-bi.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/iconvsr/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/iconvsr/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/indexnet/indexnet_mobv2-dimaug_1xb16-78k_comp1k.py` & `mmagic-1.0.1/mmagic/.mim/configs/indexnet/indexnet_mobv2-dimaug_1xb16-78k_comp1k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/indexnet/indexnet_mobv2_1xb16-78k_comp1k.py` & `mmagic-1.0.1/mmagic/.mim/configs/indexnet/indexnet_mobv2_1xb16-78k_comp1k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/indexnet/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/indexnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/inst_colorization/inst-colorizatioon_full_official_cocostuff-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/inst_colorization/inst-colorizatioon_full_official_cocostuff-256x256.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,9 +51,11 @@
         finesize=256,
         box_num_upbound=5),
     dict(
         type='Resize',
         keys=['img', 'cropped_img'],
         scale=(256, 256),
         keep_ratio=False),
-    dict(type='PackInputs'),
+    dict(
+        type='PackInputs',
+        data_keys=['box_info', 'box_info_2x', 'box_info_4x', 'box_info_8x']),
 ]
```

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/inst_colorization/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/inst_colorization/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/liif/liif-edsr-norm_c64b16_1xb16-1000k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/liif/liif-edsr-norm_c64b16_1xb16-1000k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/liif/liif-rdn-norm_c64b16_1xb16-1000k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/liif/liif-rdn-norm_c64b16_1xb16-1000k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/liif/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/liif/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-3-1xb128-12Mimgs_celeba-cropped-64x64.py` & `mmagic-1.0.1/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-3-1xb128-12Mimgs_celeba-cropped-64x64.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-4-1xb128-12Mimgs_lsun-bedroom-64x64.py` & `mmagic-1.0.1/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-4-1xb128-12Mimgs_lsun-bedroom-64x64.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-4-1xb64-10Mimgs_celeba-cropped-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/lsgan/lsgan_dcgan-archi_lr1e-4-1xb64-10Mimgs_celeba-cropped-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/lsgan/lsgan_lsgan-archi_lr1e-4-1xb64-10Mimgs_lsun-bedroom-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/lsgan/lsgan_lsgan-archi_lr1e-4-1xb64-10Mimgs_lsun-bedroom-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/lsgan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/lsgan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/nafnet/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/nafnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/nafnet/nafnet_c64eb11128mb1db1111_8xb8-lr1e-3-400k_gopro.py` & `mmagic-1.0.1/mmagic/.mim/configs/nafnet/nafnet_c64eb11128mb1db1111_8xb8-lr1e-3-400k_gopro.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/nafnet/nafnet_c64eb2248mb12db2222_8xb8-lr1e-3-400k_sidd.py` & `mmagic-1.0.1/mmagic/.mim/configs/nafnet/nafnet_c64eb2248mb12db2222_8xb8-lr1e-3-400k_sidd.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/partial_conv/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/partial_conv/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/partial_conv/pconv_stage1_8xb12_places-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/partial_conv/pconv_stage1_8xb12_places-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/partial_conv/pconv_stage1_8xb1_celeba-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/partial_conv/pconv_stage1_8xb1_celeba-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/partial_conv/pconv_stage2_4xb2_celeba-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/partial_conv/pconv_stage2_4xb2_celeba-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/partial_conv/pconv_stage2_4xb2_places-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/partial_conv/pconv_stage2_4xb2_places-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/pggan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/pggan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/pggan/pggan_8xb4-12Mimg_celeba-hq-1024x1024.py` & `mmagic-1.0.1/mmagic/.mim/configs/pggan/pggan_8xb4-12Mimg_celeba-hq-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/pggan/pggan_8xb4-12Mimgs_celeba-cropped-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/pggan/pggan_8xb4-12Mimgs_celeba-cropped-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/pix2pix/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/pix2pix/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-220kiters_aerial2maps.py` & `mmagic-1.0.1/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-220kiters_aerial2maps.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-220kiters_maps2aerial.py` & `mmagic-1.0.1/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-220kiters_maps2aerial.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-80kiters_facades.py` & `mmagic-1.0.1/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_1xb1-80kiters_facades.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_wo-jitter-flip-1xb4-190kiters_edges2shoes.py` & `mmagic-1.0.1/mmagic/.mim/configs/pix2pix/pix2pix_vanilla-unet-bn_wo-jitter-flip-1xb4-190kiters_edges2shoes.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-c_c2_8xb3-1100kiters_ffhq-256-512.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-c_c2_8xb3-1100kiters_ffhq-256-512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-d_c2_8xb3-1100kiters_ffhq-256-512.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-d_c2_8xb3-1100kiters_ffhq-256-512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-e_c2_8xb3-1100kiters_ffhq-256-512.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-e_c2_8xb3-1100kiters_ffhq-256-512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c1_8xb2-1600kiters_ffhq-256-1024.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c1_8xb2-1600kiters_ffhq-256-1024.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c2_8xb3-1100kiters_ffhq-256-512.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c2_8xb3-1100kiters_ffhq-256-512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c2_8xb3-1100kiters_ffhq-256-896.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-f_c2_8xb3-1100kiters_ffhq-256-896.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-g_c1_8xb3-1100kiters_ffhq-256-512.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-g_c1_8xb3-1100kiters_ffhq-256-512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-h_c2_8xb3-1100kiters_ffhq-256-512.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-h_c2_8xb3-1100kiters_ffhq-256-512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-i_c2_8xb3-1100kiters_ffhq-256-512.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-i_c2_8xb3-1100kiters_ffhq-256-512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-j_c2_8xb3-1100kiters_ffhq-256-512.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-j_c2_8xb3-1100kiters_ffhq-256-512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-k_c2_8xb3-1100kiters_ffhq-256-512.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/mspie-stylegan2-config-k_c2_8xb3-1100kiters_ffhq-256-512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan-csg_bohemian.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan-csg_bohemian.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan-csg_fish.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan-csg_fish.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim4_bohemian.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim4_bohemian.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim4_fish.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim4_fish.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim8_bohemian.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/singan_spe-dim8_bohemian.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/stylegan2_c2_8xb3-1100kiters_ffhq-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/stylegan2_c2_8xb3-1100kiters_ffhq-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/positional_encoding_in_gans/stylegan2_c2_8xb3-1100kiters_ffhq-512x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/positional_encoding_in_gans/stylegan2_c2_8xb3-1100kiters_ffhq-512x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/rdn/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/rdn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/rdn/rdn_x2c64b16_1xb16-1000k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/rdn/rdn_x2c64b16_1xb16-1000k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/rdn/rdn_x3c64b16_1xb16-1000k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/rdn/rdn_x3c64b16_1xb16-1000k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/rdn/rdn_x4c64b16_1xb16-1000k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/rdn/rdn_x4c64b16_1xb16-1000k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/real_basicvsr/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/real_basicvsr/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/real_basicvsr/realbasicvsr_c64b20-1x30x8_8xb1-lr5e-5-150k_reds.py` & `mmagic-1.0.1/mmagic/.mim/configs/real_basicvsr/realbasicvsr_c64b20-1x30x8_8xb1-lr5e-5-150k_reds.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/real_basicvsr/realbasicvsr_wogan-c64b20-2x30x8_8xb2-lr1e-4-300k_reds.py` & `mmagic-1.0.1/mmagic/.mim/configs/real_basicvsr/realbasicvsr_wogan-c64b20-2x30x8_8xb2-lr1e-4-300k_reds.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/real_esrgan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/real_esrgan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/real_esrgan/realesrgan_c64b23g32_4xb12-lr1e-4-400k_df2k-ost.py` & `mmagic-1.0.1/mmagic/.mim/configs/real_esrgan/realesrgan_c64b23g32_4xb12-lr1e-4-400k_df2k-ost.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/real_esrgan/realesrnet_c64b23g32_4xb12-lr2e-4-1000k_df2k-ost.py` & `mmagic-1.0.1/mmagic/.mim/configs/real_esrgan/realesrnet_c64b23g32_4xb12-lr2e-4-1000k_df2k-ost.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma15.py` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma15.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma25.py` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma25.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma50.py` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-color-sigma50.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma15.py` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma15.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma25.py` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma25.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma50.py` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dfwb-gray-sigma50.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dpdd-dual.py` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dpdd-dual.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_dpdd-single.py` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_dpdd-single.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_gopro.py` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_gopro.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_rain13k.py` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_rain13k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/restormer/restormer_official_sidd.py` & `mmagic-1.0.1/mmagic/.mim/configs/restormer/restormer_official_sidd.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sagan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/sagan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_128_cvt_studioGAN.py` & `mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_128_cvt_studioGAN.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_cvt-studioGAN_cifar10-32x32.py` & `mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_cvt-studioGAN_cifar10-32x32.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_wReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py` & `mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_wReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_woReLUinplace-Glr1e-4_Dlr4e-4_noaug-ndisc1-8xb32-bigGAN-sch_imagenet1k-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_woReLUinplace-Glr1e-4_Dlr4e-4_noaug-ndisc1-8xb32-bigGAN-sch_imagenet1k-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_woReLUinplace_Glr1e-4_Dlr4e-4_ndisc1-4xb64_imagenet1k-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_woReLUinplace_Glr1e-4_Dlr4e-4_ndisc1-4xb64_imagenet1k-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sagan/sagan_woReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py` & `mmagic-1.0.1/mmagic/.mim/configs/sagan/sagan_woReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/singan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/singan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/singan/singan_balloons.py` & `mmagic-1.0.1/mmagic/.mim/configs/singan/singan_balloons.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/singan/singan_bohemian.py` & `mmagic-1.0.1/mmagic/.mim/configs/singan/singan_bohemian.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/singan/singan_fish.py` & `mmagic-1.0.1/mmagic/.mim/configs/singan/singan_fish.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj-cvt-studioGAN_cifar10-32x32.py` & `mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj-cvt-studioGAN_cifar10-32x32.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj-cvt-studioGAN_imagenet1k-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj-cvt-studioGAN_imagenet1k-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj_wReLUinplace_Glr2e-4_Dlr5e-5_ndisc5-2xb128_imagenet1k-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj_wReLUinplace_Glr2e-4_Dlr5e-5_ndisc5-2xb128_imagenet1k-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj_wReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py` & `mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj_wReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj_woReLUinplace_Glr2e-4_Dlr5e-5_ndisc5-2xb128_imagenet1k-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj_woReLUinplace_Glr2e-4_Dlr5e-5_ndisc5-2xb128_imagenet1k-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/sngan_proj/sngan-proj_woReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py` & `mmagic-1.0.1/mmagic/.mim/configs/sngan_proj/sngan-proj_woReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/srcnn/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/srcnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/srcnn/srcnn_x4k915_1xb16-1000k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/srcnn/srcnn_x4k915_1xb16-1000k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/srgan_resnet/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/srgan_resnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/srgan_resnet/msrresnet_x4c64b16_1xb16-1000k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/srgan_resnet/msrresnet_x4c64b16_1xb16-1000k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/srgan_resnet/srgan_x4c64b16_1xb16-1000k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/srgan_resnet/srgan_x4c64b16_1xb16-1000k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/stable_diffusion/stable-diffusion_ddim_denoisingunet.py` & `mmagic-1.0.1/mmagic/.mim/configs/stable_diffusion/stable-diffusion_ddim_denoisingunet.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv1/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv1/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv1/styleganv1_ffhq-1024x1024_8xb4-25Mimgs.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv1/styleganv1_ffhq-1024x1024_8xb4-25Mimgs.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv1/styleganv1_ffhq-256x256_8xb4-25Mimgs.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv1/styleganv1_ffhq-256x256_8xb4-25Mimgs.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv2/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_ffhq-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_ffhq-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-cat-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-cat-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-church-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-church-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-horse-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4-800kiters_lsun-horse-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4_ffhq-1024x1024.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4_ffhq-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4_lsun-car-384x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv2/stylegan2_c2_8xb4_lsun-car-384x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv3/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv3/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-r_ada-gamma3.3_8xb4-fp16_metfaces-1024x1024.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-r_ada-gamma3.3_8xb4-fp16_metfaces-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4_ffhq-1024x1024.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4_ffhq-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4_ffhqu-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4_ffhqu-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4x8_afhqv2-512x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-r_cvt-official-rgb_8xb4x8_afhqv2-512x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_ada-gamma6.6_8xb4-fp16_metfaces-1024x1024.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_ada-gamma6.6_8xb4-fp16_metfaces-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_afhqv2-512x512.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_afhqv2-512x512.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_ffhq-1024x1024.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_ffhq-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_ffhqu-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_cvt-official-rgb_8xb4_ffhqu-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_gamma2.0_8xb4-fp16-noaug_ffhq-256x256.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_gamma2.0_8xb4-fp16-noaug_ffhq-256x256.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/styleganv3/stylegan3-t_gamma32.8_8xb4-fp16-noaug_ffhq-1024x1024.py` & `mmagic-1.0.1/mmagic/.mim/configs/styleganv3/stylegan3-t_gamma32.8_8xb4-fp16-noaug_ffhq-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_psnr-x2s64w8d6e180_8xb4-lr1e-4-600k_df2k-ost.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_psnr-x2s64w8d6e180_8xb4-lr1e-4-600k_df2k-ost.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR10.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR10.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR20.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR20.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR30.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR30.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR40.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-colorCAR40.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR10.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR10.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR20.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR20.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR30.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR30.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR40.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s126w7d6e180_8xb1-lr2e-4-1600k_dfwb-grayCAR40.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN15.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN15.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN25.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN25.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN50.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-colorDN50.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN15.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN15.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN25.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN25.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN50.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_s128w8d6e180_8xb1-lr2e-4-1600k_dfwb-grayDN50.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x2s48w8d6e180_8xb4-lr2e-4-500k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x2s48w8d6e180_8xb4-lr2e-4-500k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x2s64w8d4e60_8xb4-lr2e-4-500k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x2s64w8d4e60_8xb4-lr2e-4-500k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x2s64w8d6e180_8xb4-lr2e-4-500k_df2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x2s64w8d6e180_8xb4-lr2e-4-500k_df2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x3s48w8d6e180_8xb4-lr2e-4-500k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x3s48w8d6e180_8xb4-lr2e-4-500k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x3s64w8d4e60_8xb4-lr2e-4-500k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x3s64w8d4e60_8xb4-lr2e-4-500k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x3s64w8d6e180_8xb4-lr2e-4-500k_df2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x3s64w8d6e180_8xb4-lr2e-4-500k_df2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x4s48w8d6e180_8xb4-lr2e-4-500k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x4s48w8d6e180_8xb4-lr2e-4-500k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x4s64w8d4e60_8xb4-lr2e-4-500k_div2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x4s64w8d4e60_8xb4-lr2e-4-500k_div2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/swinir/swinir_x4s64w8d6e180_8xb4-lr2e-4-500k_df2k.py` & `mmagic-1.0.1/mmagic/.mim/configs/swinir/swinir_x4s64w8d6e180_8xb4-lr2e-4-500k_df2k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/tdan/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/tdan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/tdan/tdan_x4_8xb16-lr1e-4-400k_vimeo90k-bd.py` & `mmagic-1.0.1/mmagic/.mim/configs/tdan/tdan_x4_8xb16-lr1e-4-400k_vimeo90k-bd.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/tdan/tdan_x4ft_8xb16-lr5e-5-800k_vimeo90k-bd.py` & `mmagic-1.0.1/mmagic/.mim/configs/tdan/tdan_x4ft_8xb16-lr5e-5-800k_vimeo90k-bd.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/tof/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/tof/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/tof/tof_spynet-chair-wobn_1xb1_vimeo90k-triplet.py` & `mmagic-1.0.1/mmagic/.mim/configs/tof/tof_spynet-chair-wobn_1xb1_vimeo90k-triplet.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/tof/tof_spynet-kitti-wobn_1xb1_vimeo90k-triplet.py` & `mmagic-1.0.1/mmagic/.mim/configs/tof/tof_spynet-kitti-wobn_1xb1_vimeo90k-triplet.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/tof/tof_spynet-pytoflow-wobn_1xb1_vimeo90k-triplet.py` & `mmagic-1.0.1/mmagic/.mim/configs/tof/tof_spynet-pytoflow-wobn_1xb1_vimeo90k-triplet.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/tof/tof_spynet-sintel-wobn-clean_1xb1_vimeo90k-triplet.py` & `mmagic-1.0.1/mmagic/.mim/configs/tof/tof_spynet-sintel-wobn-clean_1xb1_vimeo90k-triplet.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/tof/tof_spynet-sintel-wobn-final_1xb1_vimeo90k-triplet.py` & `mmagic-1.0.1/mmagic/.mim/configs/tof/tof_spynet-sintel-wobn-final_1xb1_vimeo90k-triplet.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/tof/tof_x4_official_vimeo90k.py` & `mmagic-1.0.1/mmagic/.mim/configs/tof/tof_x4_official_vimeo90k.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/ttsr/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/ttsr/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/ttsr/ttsr-gan_x4c64b16_1xb9-500k_CUFED.py` & `mmagic-1.0.1/mmagic/.mim/configs/ttsr/ttsr-gan_x4c64b16_1xb9-500k_CUFED.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/ttsr/ttsr-rec_x4c64b16_1xb9-200k_CUFED.py` & `mmagic-1.0.1/mmagic/.mim/configs/ttsr/ttsr-rec_x4c64b16_1xb9-200k_CUFED.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/wgan-gp/metafile.yml` & `mmagic-1.0.1/mmagic/.mim/configs/wgan-gp/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/configs/wgan-gp/wgangp_GN_1xb64-160kiters_celeba-cropped-128x128.py` & `mmagic-1.0.1/mmagic/.mim/configs/wgan-gp/wgangp_GN_1xb64-160kiters_celeba-cropped-128x128.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/demo/download_inference_resources.py` & `mmagic-1.0.1/mmagic/.mim/demo/download_inference_resources.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/demo/gradio_controlnet_animation.py` & `mmagic-1.0.1/mmagic/.mim/demo/gradio_controlnet_animation.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/demo/gradio_inpainting.py` & `mmagic-1.0.1/mmagic/.mim/demo/gradio_inpainting.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/demo/mmagic_inference_demo.py` & `mmagic-1.0.1/mmagic/.mim/demo/mmagic_inference_demo.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/demo/singan_demo.py` & `mmagic-1.0.1/mmagic/.mim/demo/singan_demo.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/model-index.yml` & `mmagic-1.0.1/mmagic/.mim/model-index.yml`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/analysis_tools/get_flops.py` & `mmagic-1.0.1/mmagic/.mim/tools/analysis_tools/get_flops.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/analysis_tools/print_config.py` & `mmagic-1.0.1/mmagic/.mim/tools/analysis_tools/print_config.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/bgm/preprocess_bgm_dataset.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/bgm/preprocess_bgm_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/comp1k/check_extended_fg.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/comp1k/check_extended_fg.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/comp1k/evaluate_comp1k.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/comp1k/evaluate_comp1k.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     ```
 
     Args:
         pred_root (str): Path to the predicted alpha matte folder.
         gt_root (str): Path to the ground truth alpha matte folder.
         trimap_root (str): Path to the predicted alpha matte folder.
         verbose (bool): Whether print result for each predicted alpha matte.
-        nproc (int): number of processers.
+        nproc (int): number of processes.
     """
 
     images = sorted(mmengine.scandir(pred_root))
     gt_files_num = len(list(mmengine.scandir(gt_root)))
     # If ground truth alpha mattes are not copied (number of files is 50), we
     # use the below pattern to recover the name of the original alpha matte.
     if gt_files_num == 50:
@@ -239,15 +239,15 @@
         'results are calculated on the full image.')
     parser.add_argument(
         '-v',
         '--verbose',
         action='store_true',
         help='Whether print result for each predicted alpha matte')
     parser.add_argument(
-        '--nproc', type=int, default=4, help='number of processers')
+        '--nproc', type=int, default=4, help='number of processes')
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
 
     if not osp.exists(args.pred_root):
```

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/comp1k/extend_fg.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/comp1k/extend_fg.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/comp1k/filter_comp1k_anno.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/comp1k/filter_comp1k_anno.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/comp1k/preprocess_comp1k_dataset.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/comp1k/preprocess_comp1k_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     relative path. When using these strings to read from or write to disk, a
     data_root is added to form a complete relative path.
 
     Args:
         data_root (str): path to Adobe composition-1k directory.
         source_bg_dir (str): source background directory.
         composite (bool): whether composite fg with bg and write to file.
-        nproc (int): number of processers.
+        nproc (int): number of processes.
         mode (str): training or test mode.
     """
 
     if mode == 'training':
         dir_prefix = 'Training_set'
         fname_prefix = 'training'
         num_bg = 100  # each training fg is composited with 100 bg
@@ -233,15 +233,15 @@
     parser.add_argument('coco_root', help='COCO2014 or COCO2017 dataset root')
     parser.add_argument('voc_root', help='VOCdevkit directory root')
     parser.add_argument(
         '--composite',
         action='store_true',
         help='whether to composite training foreground and background offline')
     parser.add_argument(
-        '--nproc', type=int, default=4, help='number of processer')
+        '--nproc', type=int, default=4, help='number of processes')
     parser.add_argument(
         '--skip-train',
         action='store_true',
         help='whether to skip the training data')
     args = parser.parse_args()
     return args
```

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/df2k_ost/preprocess_df2k_ost_dataset.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/df2k_ost/preprocess_df2k_ost_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/div2k/preprocess_div2k_dataset.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/div2k/preprocess_div2k_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/glean/preprocess_cat_test_dataset.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/glean/preprocess_cat_test_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/glean/preprocess_cat_train_dataset.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/glean/preprocess_cat_train_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/glean/preprocess_ffhq_celebahq_dataset.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/glean/preprocess_ffhq_celebahq_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/reds/crop_sub_images.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/reds/crop_sub_images.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/reds/preprocess_reds_dataset.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/reds/preprocess_reds_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/sidd/preprocess_sidd_test_dataset.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/sidd/preprocess_sidd_test_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/vid4/preprocess_vid4_dataset.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/vid4/preprocess_vid4_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/dataset_converters/vimeo90k/preprocess_vimeo90k_dataset.py` & `mmagic-1.0.1/mmagic/.mim/tools/dataset_converters/vimeo90k/preprocess_vimeo90k_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/gui/component.py` & `mmagic-1.0.1/mmagic/.mim/tools/gui/component.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/gui/gui.py` & `mmagic-1.0.1/mmagic/.mim/tools/gui/gui.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/gui/page_general.py` & `mmagic-1.0.1/mmagic/.mim/tools/gui/page_general.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/gui/page_sr.py` & `mmagic-1.0.1/mmagic/.mim/tools/gui/page_sr.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/gui/utils.py` & `mmagic-1.0.1/mmagic/.mim/tools/gui/utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/model_converters/publish_model.py` & `mmagic-1.0.1/mmagic/.mim/tools/model_converters/publish_model.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/slurm_test.sh` & `mmagic-1.0.1/mmagic/.mim/tools/slurm_test.sh`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/slurm_train.sh` & `mmagic-1.0.1/mmagic/.mim/tools/slurm_train.sh`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/test.py` & `mmagic-1.0.1/mmagic/.mim/tools/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     cfg.load_from = args.checkpoint
 
     # build the runner from config
     runner = Runner.from_cfg(cfg)
 
     print_colored_log(f'Working directory: {cfg.work_dir}')
-    print_colored_log(f'Log directiry: {runner._log_dir}')
+    print_colored_log(f'Log directory: {runner._log_dir}')
 
     if args.out:
 
         class SaveMetricHook(Hook):
 
             def after_test_epoch(self, _, metrics=None):
                 if metrics is not None:
```

### Comparing `mmagic-1.0.0/mmagic/.mim/tools/train.py` & `mmagic-1.0.1/mmagic/.mim/tools/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     if args.resume:
         cfg.resume = True
 
     # build the runner from config
     runner = Runner.from_cfg(cfg)
 
     print_colored_log(f'Working directory: {cfg.work_dir}')
-    print_colored_log(f'Log directiry: {runner._log_dir}')
+    print_colored_log(f'Log directory: {runner._log_dir}')
 
     # start training
     runner.train()
 
     print_colored_log(f'Log saved under {runner._log_dir}')
     print_colored_log(f'Checkpoint saved under {cfg.work_dir}')
```

### Comparing `mmagic-1.0.0/mmagic/__init__.py` & `mmagic-1.0.1/mmagic/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/__init__.py` & `mmagic-1.0.1/mmagic/apis/inferencers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,21 @@
             self.inferencer = Text2ImageInferencer(
                 config, ckpt, device, extra_parameters, seed=seed)
         elif self.task in ['3D_aware_generation', '3D-aware Generation']:
             self.inferencer = EG3DInferencer(
                 config, ckpt, device, extra_parameters, seed=seed)
         elif self.task in ['controlnet_animation']:
             self.inferencer = ControlnetAnimationInferencer(config)
+        elif self.task in [
+                'Image Restoration', 'Denoising, Deblurring, Deraining',
+                'Image Super-Resolution, Image denoising, JPEG compression '
+                'artifact reduction'
+        ]:
+            self.inferencer = ImageSuperResolutionInferencer(
+                config, ckpt, device, extra_parameters, seed=seed)
         else:
             raise ValueError(f'Unknown inferencer task: {self.task}')
 
     def __call__(self, **kwargs) -> Union[Dict, List[Dict]]:
         """Call the inferencer.
 
         Args:
```

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/base_mmagic_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/base_mmagic_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/colorization_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/colorization_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/conditional_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/conditional_inferencer.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
         Returns:
             List[np.ndarray]: Result of visualize
         """
         res_list = []
         res_list.extend([item.fake_img.data.cpu() for item in preds])
         results = torch.stack(res_list, dim=0)
-        results = (results[:, [2, 1, 0]] + 1.) / 2.
+        results = results[:, [2, 1, 0]] / 255.
 
         # save images
         if result_out_dir:
             mkdir_or_exist(os.path.dirname(result_out_dir))
             utils.save_image(results, result_out_dir)
 
         return results
```

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/controlnet_animation_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/controlnet_animation_inferencer.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,15 @@
                  controlnet_conditioning_scale=0.7,
                  image_width=512,
                  image_height=512,
                  save_path=None,
                  strength=0.75,
                  num_inference_steps=20,
                  seed=1,
+                 output_fps=None,
                  **kwargs) -> Union[Dict, List[Dict]]:
         """Call the inferencer.
 
         Args:
             kwargs: Keyword arguments for the inferencer.
 
         Returns:
@@ -133,17 +134,23 @@
 
         # load the images
         input_file_extension = os.path.splitext(video)[1]
         from_video = True
         all_images = []
         if input_file_extension in VIDEO_EXTENSIONS:
             video_reader = mmcv.VideoReader(video)
+            input_fps = int(video_reader.fps)
+            if output_fps is None:
+                output_fps = input_fps
+            if output_fps > input_fps:
+                output_fps = input_fps
+            sample_rate = int(input_fps / output_fps)
 
             fourcc = cv2.VideoWriter_fourcc(*'mp4v')
-            video_writer = cv2.VideoWriter(save_path, fourcc, video_reader.fps,
+            video_writer = cv2.VideoWriter(save_path, fourcc, output_fps,
                                            (image_width, image_height))
             for frame in video_reader:
                 all_images.append(np.flip(frame, axis=2))
         else:
             frame_files = os.listdir(video)
             frame_files = [os.path.join(video, f) for f in frame_files]
             frame_files.sort()
@@ -184,17 +191,21 @@
         first_result = result
         first_hed = hed_image
         last_result = result
         last_hed = hed_image
 
         for ind in range(len(all_images)):
             if from_video:
+                if ind % sample_rate > 0:
+                    continue
                 image = PIL.Image.fromarray(all_images[ind])
             else:
                 image = load_image(all_images[ind])
+            print('processing frame ind ' + str(ind))
+
             image = image.resize((image_width, image_height))
             hed_image = self.hed(image, image_resolution=image_width)
 
             concat_img = PIL.Image.new('RGB', (image_width * 3, image_height))
             concat_img.paste(last_result, (0, 0))
             concat_img.paste(image, (image_width, 0))
             concat_img.paste(first_result, (image_width * 2, 0))
```

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/eg3d_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/eg3d_inferencer.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 num_images: int = 100) -> Union[dict, List[dict]]:
         """Forward the inputs to the model.
 
         Args:
             inputs (ForwardInputs): Model inputs. If data sample (the second
                 element of `inputs`) is not passed, will generate a sequence
                 of images corresponding to passed `interpolation` mode.
-            interpolation (str): The interplolation mode. Supported choices
+            interpolation (str): The interpolation mode. Supported choices
                 are 'both', 'conditioning', and 'camera'. Defaults to 'both'.
             num_images (int): The number of frames of interpolation.
                 Defaults to 500.
 
         Returns:
             Union[dict, List[dict]]: Output dict corresponds to the input
                 condition or the list of output dict of each frame during the
```

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/image_super_resolution_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/matting_inferencer.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,96 +3,67 @@
 from typing import Dict, List
 
 import mmcv
 import numpy as np
 import torch
 from mmengine import mkdir_or_exist
 from mmengine.dataset import Compose
-from mmengine.dataset.utils import default_collate as collate
 
-from mmagic.utils import tensor2img
+from mmagic.structures import DataSample
 from .base_mmagic_inferencer import BaseMMagicInferencer, InputsType, PredType
 
 
-class ImageSuperResolutionInferencer(BaseMMagicInferencer):
-    """inferencer that predicts with restoration models."""
+class MattingInferencer(BaseMMagicInferencer):
+    """inferencer that predicts with matting models."""
 
     func_kwargs = dict(
-        preprocess=['img', 'ref'],
+        preprocess=['img', 'trimap'],
         forward=[],
         visualize=['result_out_dir'],
         postprocess=[])
 
-    def preprocess(self, img: InputsType, ref: InputsType = None) -> Dict:
+    def preprocess(self, img: InputsType, trimap: InputsType) -> Dict:
         """Process the inputs into a model-feedable format.
 
         Args:
-            img(InputsType): Image to be restored by models.
-            ref(InputsType): Reference image for resoration models.
-                Defaults to None.
+            img(InputsType): Image to be processed by models.
+            mask(InputsType): Mask corresponding to the input image.
 
         Returns:
-            data(Dict): Results of preprocess.
+            results(Dict): Results of preprocess.
         """
-        cfg = self.model.cfg
-        device = next(self.model.parameters()).device  # model device
-
-        # select the data pipeline
-        if cfg.get('inference_pipeline', None):
-            test_pipeline = cfg.inference_pipeline
-        elif cfg.get('demo_pipeline', None):
-            test_pipeline = cfg.demo_pipeline
-        elif cfg.get('test_pipeline', None):
-            test_pipeline = cfg.test_pipeline
-        else:
-            test_pipeline = cfg.val_pipeline
-
-        keys_to_remove = ['gt', 'gt_path']
+        # remove alpha from test_pipeline
+        keys_to_remove = ['alpha', 'ori_alpha']
         for key in keys_to_remove:
-            for pipeline in list(test_pipeline):
+            for pipeline in list(self.cfg.test_pipeline):
                 if 'key' in pipeline and key == pipeline['key']:
-                    test_pipeline.remove(pipeline)
+                    self.cfg.test_pipeline.remove(pipeline)
                 if 'keys' in pipeline and key in pipeline['keys']:
                     pipeline['keys'].remove(key)
                     if len(pipeline['keys']) == 0:
-                        test_pipeline.remove(pipeline)
+                        self.cfg.test_pipeline.remove(pipeline)
                 if 'meta_keys' in pipeline and key in pipeline['meta_keys']:
                     pipeline['meta_keys'].remove(key)
 
         # build the data pipeline
-        test_pipeline = Compose(test_pipeline)
-
+        test_pipeline = Compose(self.cfg.test_pipeline)
         # prepare data
-        if ref:  # Ref-SR
-            data = dict(img_path=img, gt_path=ref)
-        else:  # SISR
-            data = dict(img_path=img)
+        data = dict(merged_path=img, trimap_path=trimap)
         _data = test_pipeline(data)
-
-        data = dict()
-        data_preprocessor = cfg['model']['data_preprocessor']
-        mean = torch.Tensor(data_preprocessor['mean']).view([3, 1, 1])
-        std = torch.Tensor(data_preprocessor['std']).view([3, 1, 1])
-        data['inputs'] = (_data['inputs'] - mean) / std
-        data = collate([data])
-
-        if ref:
-            data['data_samples'] = [_data['data_samples']]
-        if 'cuda' in str(device):
-            data['inputs'] = data['inputs'].cuda()
-            if ref:
-                data['data_samples'][0] = data['data_samples'][0].cuda()
-
-        return data
+        trimap = _data['data_samples'].trimap.data
+        preprocess_res = dict()
+        preprocess_res['inputs'] = [_data['inputs']]
+        preprocess_res['data_samples'] = [_data['data_samples']]
+        return preprocess_res
 
     def forward(self, inputs: InputsType) -> PredType:
         """Forward the inputs to the model."""
+        inputs = self.model.data_preprocessor(inputs)
         with torch.no_grad():
-            result = self.model(mode='tensor', **inputs)
-        return result
+            return self.model(mode='predict', **inputs)
 
     def visualize(self,
                   preds: PredType,
                   result_out_dir: str = None) -> List[np.ndarray]:
         """Visualize predictions.
 
         Args:
@@ -101,13 +72,31 @@
             data (List[Dict]): Not needed by this kind of inferencer.
             result_out_dir (str): Output directory of image.
                 Defaults to ''.
 
         Returns:
             List[np.ndarray]: Result of visualize
         """
-        results = tensor2img(preds[0])
+        result = preds[0].output
+        result = result.pred_alpha.data.cpu()
+
+        # save images
         if result_out_dir:
             mkdir_or_exist(os.path.dirname(result_out_dir))
-            mmcv.imwrite(results, result_out_dir)
+            mmcv.imwrite(result.numpy(), result_out_dir)
 
-        return results
+        return result
+
+    def _pred2dict(self, data_sample: DataSample) -> Dict:
+        """Extract elements necessary to represent a prediction into a
+        dictionary. It's better to contain only basic data elements such as
+        strings and numbers in order to guarantee it's json-serializable.
+
+        Args:
+            data_sample (DataSample): The data sample to be converted.
+
+        Returns:
+            dict: The output dictionary.
+        """
+        result = {}
+        result['pred_alpha'] = data_sample.output.pred_alpha.data.cpu()
+        return result
```

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/inference_functions.py` & `mmagic-1.0.1/mmagic/apis/inferencers/inference_functions.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/inpainting_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/inpainting_inferencer.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 from typing import Dict, List
 
 import mmcv
 import numpy as np
 import torch
 from mmengine import mkdir_or_exist
 from mmengine.dataset import Compose
-from mmengine.dataset.utils import default_collate as collate
-from torch.nn.parallel import scatter
 
-from mmagic.structures import DataSample
 from mmagic.utils import tensor2img
 from .base_mmagic_inferencer import BaseMMagicInferencer, InputsType, PredType
 
 
 class InpaintingInferencer(BaseMMagicInferencer):
     """inferencer that predicts with inpainting models."""
 
@@ -49,33 +46,23 @@
         ]
 
         infer_pipeline = Compose(infer_pipeline_cfg)
 
         # prepare data
         _data = infer_pipeline(dict(gt_path=img, mask_path=mask))
         data = dict()
-        data['inputs'] = _data['inputs'] / 255.0
-        data = collate([data])
+        data['inputs'] = [_data['inputs']]
         data['data_samples'] = [_data['data_samples']]
-        if 'cuda' in str(self.device):
-            data = scatter(data, [self.device])[0]
-            data['data_samples'][0].mask.data = scatter(
-                data['data_samples'][0].mask.data, [self.device])[0] / 255.0
-
-        # save masks and masked_imgs to visualize
-        self.masks = data['data_samples'][0].mask.data * 255
-        self.masked_imgs = data['inputs'][0]
-
-        data['data_samples'] = DataSample.stack(data['data_samples'])
         return data
 
     def forward(self, inputs: InputsType) -> PredType:
         """Forward the inputs to the model."""
+        inputs = self.model.data_preprocessor(inputs)
         with torch.no_grad():
-            result, x = self.model(mode='tensor', **inputs)
+            result = self.model(mode='predict', **inputs)
         return result
 
     def visualize(self,
                   preds: PredType,
                   result_out_dir: str = None) -> List[np.ndarray]:
         """Visualize predictions.
 
@@ -85,16 +72,15 @@
             data (List[Dict]): Mask of input image.
             result_out_dir (str): Output directory of image.
                 Defaults to ''.
 
         Returns:
             List[np.ndarray]: Result of visualize
         """
-        result = preds[0]
-        result = result * self.masks + self.masked_imgs * (1. - self.masks)
+        result = preds[0].output.pred_img / 255.
 
         result = tensor2img(result)[..., ::-1]
         if result_out_dir:
             mkdir_or_exist(os.path.dirname(result_out_dir))
             mmcv.imwrite(result, result_out_dir)
 
         return result
```

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/text2image_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/text2image_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/translation_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/translation_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/unconditional_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/unconditional_inferencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,17 @@
         Returns:
             List[np.ndarray]: Result of visualize
         """
         res_list = []
         res_list.extend([item.fake_img.data.cpu() for item in preds])
         results = torch.stack(res_list, dim=0)
         if results.shape[1] == 3:
-            results = (results[:, [2, 1, 0]] + 1.) / 2.
+            results = results[:, [2, 1, 0]] / 255.
         else:
-            results = (results + 1.) / 2.
+            results = results / 255.
 
         # save images
         if result_out_dir:
             mkdir_or_exist(os.path.dirname(result_out_dir))
             utils.save_image(results, result_out_dir)
 
         return results
```

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/video_interpolation_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/video_interpolation_inferencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import math
 import os
 import os.path as osp
 from typing import Dict, List, Optional, Tuple, Union
 
 import cv2
 import mmcv
+import mmengine
 import numpy as np
 import torch
 from mmengine.dataset import Compose
 from mmengine.dataset.utils import default_collate as collate
 from mmengine.logging import MMLogger
 from mmengine.utils import ProgressBar
 
@@ -105,14 +106,15 @@
             example_frame = read_image(files[0])
             h, w = example_frame.shape[:2]
             fps = self.extra_parameters['fps']
             output_fps = fps if fps > 0 else 60
 
         # check if the output is a video
         output_file_extension = os.path.splitext(result_out_dir)[1]
+        mmengine.utils.mkdir_or_exist(osp.dirname(result_out_dir))
         if output_file_extension in VIDEO_EXTENSIONS:
             fourcc = cv2.VideoWriter_fourcc(*'mp4v')
             target = cv2.VideoWriter(result_out_dir, fourcc, output_fps,
                                      (w, h))
             to_video = True
         else:
             to_video = False
@@ -175,19 +177,20 @@
                     mmcv.imwrite(frame, save_path)
                     output_index += 1
 
             if start_index + lenth_per_step >= \
                self.extra_parameters['end_idx']:
                 break
 
-        logger: MMLogger = MMLogger.get_current_instance()
-        logger.info(f'Output video is save at {result_out_dir}.')
         if to_video:
             target.release()
 
+        logger: MMLogger = MMLogger.get_current_instance()
+        logger.info(f'Output video is save at {result_out_dir}.')
+
         return {}
 
     def visualize(self,
                   preds: PredType,
                   result_out_dir: str = '') -> List[np.ndarray]:
         """Visualize is not needed in this inferencer."""
         logger: MMLogger = MMLogger.get_current_instance()
```

### Comparing `mmagic-1.0.0/mmagic/apis/inferencers/video_restoration_inferencer.py` & `mmagic-1.0.1/mmagic/apis/inferencers/video_restoration_inferencer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 import glob
 import os
 import os.path as osp
 from typing import Dict, List, Optional, Tuple, Union
 
 import cv2
 import mmcv
+import mmengine
 import numpy as np
 import torch
 from mmengine.dataset import Compose
 from mmengine.logging import MMLogger
+from mmengine.utils import ProgressBar
 
 from mmagic.utils import tensor2img
 from .base_mmagic_inferencer import (BaseMMagicInferencer, InputsType,
                                      PredType, ResType)
 from .inference_functions import VIDEO_EXTENSIONS, pad_sequence
 
 
@@ -149,33 +151,36 @@
             result_out_dir (str): Output directory of image.
                 Defaults to ''.
 
         Returns:
             List[np.ndarray]: Result of visualize
         """
         file_extension = os.path.splitext(result_out_dir)[1]
+        mmengine.utils.mkdir_or_exist(osp.dirname(result_out_dir))
+        prog_bar = ProgressBar(preds.size(1))
         if file_extension in VIDEO_EXTENSIONS:  # save as video
             h, w = preds.shape[-2:]
             fourcc = cv2.VideoWriter_fourcc(*'mp4v')
             video_writer = cv2.VideoWriter(result_out_dir, fourcc, 25, (w, h))
             for i in range(0, preds.size(1)):
                 img = tensor2img(preds[:, i, :, :, :])
                 video_writer.write(img.astype(np.uint8))
+                prog_bar.update()
             cv2.destroyAllWindows()
             video_writer.release()
         else:
             for i in range(self.extra_parameters['start_idx'],
                            self.extra_parameters['start_idx'] + preds.size(1)):
                 output_i = \
                     preds[:, i - self.extra_parameters['start_idx'], :, :, :]
                 output_i = tensor2img(output_i)
                 filename_tmpl = self.extra_parameters['filename_tmpl']
                 save_path_i = f'{result_out_dir}/{filename_tmpl.format(i)}'
-
                 mmcv.imwrite(output_i, save_path_i)
+                prog_bar.update()
 
         logger: MMLogger = MMLogger.get_current_instance()
         logger.info(f'Output video is save at {result_out_dir}.')
 
         return []
 
     def postprocess(
```

### Comparing `mmagic-1.0.0/mmagic/apis/mmagic_inferencer.py` & `mmagic-1.0.1/mmagic/apis/mmagic_inferencer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import os
 import os.path as osp
 import warnings
 from typing import Dict, List, Optional, Union
 
 import torch
 import yaml
 from mmengine.registry import init_default_scope
@@ -59,19 +58,24 @@
         'ggan',
         'pggan',
         'styleganv1',
         'styleganv2',
         'styleganv3',
 
         # matting models
+        'dim',
+        'indexnet',
         'gca',
 
         # inpainting models
-        'global_local',
         'aot_gan',
+        'deepfillv1',
+        'deepfillv2',
+        'global_local',
+        'partial_conv',
 
         # translation models
         'pix2pix',
         'cyclegan',
 
         # image super-resolution models
         'srcnn',
@@ -92,14 +96,19 @@
         'edvr',
         'tdan',
         'basicvsr',
         'iconvsr',
         'basicvsr_pp',
         'real_basicvsr',
 
+        # image_restoration models
+        'nafnet',
+        'swinir',
+        'restormer',
+
         # text2image models
         'disco_diffusion',
         'stable_diffusion',
 
         # 3D-aware generation
         'eg3d',
 
@@ -141,16 +150,21 @@
             cfgs = self.get_model_config(model_name)
             kwargs['task'] = cfgs['task']
             setting_to_use = 0
             if model_setting:
                 setting_to_use = model_setting
             config_dir = cfgs['settings'][setting_to_use]['Config']
             config_dir = config_dir[config_dir.find('configs'):]
-            kwargs['config'] = os.path.join(
-                osp.dirname(__file__), '..', '..', config_dir)
+            if osp.exists(
+                    osp.join(osp.dirname(__file__), '..', '..', config_dir)):
+                kwargs['config'] = osp.join(
+                    osp.dirname(__file__), '..', '..', config_dir)
+            else:
+                kwargs['config'] = osp.join(
+                    osp.dirname(__file__), '..', '.mim', config_dir)
             if 'Weights' in cfgs['settings'][setting_to_use].keys():
                 kwargs['ckpt'] = cfgs['settings'][setting_to_use]['Weights']
 
         if model_config is not None:
             if kwargs.get('config', None) is not None:
                 warnings.warn(
                     f'{model_name}\'s default config '
@@ -219,17 +233,21 @@
             raise ValueError(f'Model {model_name} is not supported.')
         else:
             return self.inference_supported_models_cfg[model_name]
 
     @staticmethod
     def init_inference_supported_models_cfg() -> None:
         if not MMagicInferencer.inference_supported_models_cfg_inited:
-            all_cfgs_dir = osp.join(
-                osp.dirname(__file__), '..', '..', 'configs')
-
+            if osp.exists(
+                    osp.join(osp.dirname(__file__), '..', '..', 'configs')):
+                all_cfgs_dir = osp.join(
+                    osp.dirname(__file__), '..', '..', 'configs')
+            else:
+                all_cfgs_dir = osp.join(
+                    osp.dirname(__file__), '..', '.mim', 'configs')
             for model_name in MMagicInferencer.inference_supported_models:
                 meta_file_dir = osp.join(all_cfgs_dir, model_name,
                                          'metafile.yml')
                 with open(meta_file_dir, 'r') as stream:
                     parsed_yaml = yaml.safe_load(stream)
                 task = parsed_yaml['Models'][0]['Results'][0]['Task']
                 MMagicInferencer.inference_supported_models_cfg[
```

### Comparing `mmagic-1.0.0/mmagic/datasets/__init__.py` & `mmagic-1.0.1/mmagic/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/basic_conditional_dataset.py` & `mmagic-1.0.1/mmagic/datasets/basic_conditional_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/basic_frames_dataset.py` & `mmagic-1.0.1/mmagic/datasets/basic_frames_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         pipeline (list, optional): Processing pipeline. Defaults to [].
         test_mode (bool, optional): ``test_mode=True`` means in test phase.
             Defaults to False.
         filename_tmpl (str): Template for each filename. Note that the
             template excludes the file extension. Default: '{}'.
         search_key (str): The key used for searching the folder to get
             data_list. Default: 'gt'.
-        backend_args (dict, optional): Arguments to instantiate the preifx of
+        backend_args (dict, optional): Arguments to instantiate the prefix of
             uri corresponding backend. Defaults to None.
         depth (int): The depth of path. Default: 1
         num_input_frames (None | int): Number of input frames. Default: None.
         num_output_frames (None | int): Number of output frames. Default: None.
         fixed_seq_len (None | int): The fixed sequence length.
             If None, BasicFramesDataset will obtain the length of each
             sequence.
```

### Comparing `mmagic-1.0.0/mmagic/datasets/basic_image_dataset.py` & `mmagic-1.0.1/mmagic/datasets/basic_image_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         pipeline (list, optional): Processing pipeline. Defaults to [].
         test_mode (bool, optional): ``test_mode=True`` means in test phase.
             Defaults to False.
         filename_tmpl (dict): Template for each filename. Note that the
             template excludes the file extension. Default: dict().
         search_key (str): The key used for searching the folder to get
             data_list. Default: 'gt'.
-        backend_args (dict, optional): Arguments to instantiate the preifx of
+        backend_args (dict, optional): Arguments to instantiate the prefix of
             uri corresponding backend. Defaults to None.
         suffix (str or tuple[str], optional):  File suffix
             that we are interested in. Default: None.
         recursive (bool): If set to True, recursively scan the
             directory. Default: False.
 
     Note:
```

### Comparing `mmagic-1.0.0/mmagic/datasets/categories.py` & `mmagic-1.0.1/mmagic/datasets/categories.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/cifar10_dataset.py` & `mmagic-1.0.1/mmagic/datasets/cifar10_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/comp1k_dataset.py` & `mmagic-1.0.1/mmagic/datasets/comp1k_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,16 @@
     # TODO: Support parsing folder structures without annotation files.
 
     METAINFO = dict(dataset_type='matting_dataset', task_name='matting')
 
     def load_data_list(self) -> List[dict]:
         """Load annotations from an annotation file named as ``self.ann_file``
 
-        In order to be compoatible to both new and old annotation format,
-        we copy implementations from mmengine and do some modificatoins.
+        In order to be compatible to both new and old annotation format,
+        we copy implementations from mmengine and do some modifications.
 
         Returns:
             list[dict]: A list of annotation.
         """  # noqa: E501
         # `self.ann_file` denotes the absolute annotation file path if
         # `self.root=None` or relative path if `self.root=/path/to/data/`.
         annotations = load(self.ann_file)
```

### Comparing `mmagic-1.0.0/mmagic/datasets/controlnet_dataset.py` & `mmagic-1.0.1/mmagic/datasets/controlnet_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/data_utils.py` & `mmagic-1.0.1/mmagic/datasets/data_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/dreambooth_dataset.py` & `mmagic-1.0.1/mmagic/datasets/dreambooth_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/grow_scale_image_dataset.py` & `mmagic-1.0.1/mmagic/datasets/grow_scale_image_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     def __getitem__(self, idx):
         """Get the idx-th image and data information of dataset after
         ``self.pipeline``, and ``full_init`` will be called if the dataset has
         not been fully initialized.
 
         During training phase, if ``self.pipeline`` get ``None``,
         ``self._rand_another`` will be called until a valid image is fetched or
-         the maximum limit of refetech is reached.
+         the maximum limit of refetch is reached.
 
         Args:
             idx (int): The index of self.data_list.
 
         Returns:
             dict: The idx-th image and data information of dataset after
             ``self.pipeline``.
```

### Comparing `mmagic-1.0.0/mmagic/datasets/imagenet_dataset.py` & `mmagic-1.0.1/mmagic/datasets/imagenet_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/mscoco_dataset.py` & `mmagic-1.0.1/mmagic/datasets/mscoco_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/paired_image_dataset.py` & `mmagic-1.0.1/mmagic/datasets/paired_image_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/singan_dataset.py` & `mmagic-1.0.1/mmagic/datasets/singan_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     def full_init(self):
         """Skip the full init process for SinGANDataset."""
 
         self.load_data_list(self.min_size, self.max_size,
                             self.scale_factor_init)
 
     def load_data_list(self, min_size, max_size, scale_factor_init):
-        """Load annatations for SinGAN Dataset.
+        """Load annotations for SinGAN Dataset.
 
         Args:
             min_size (int): The minimum size for the image pyramid.
             max_size (int): The maximum size for the image pyramid.
             scale_factor_init (float): The initial scale factor.
         """
         real = mmcv.imread(self.data_root)
```

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/__init__.py` & `mmagic-1.0.1/mmagic/datasets/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/alpha.py` & `mmagic-1.0.1/mmagic/datasets/transforms/alpha.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
         Returns:
             dict: A dict containing the processed data and information.
         """
         alpha = results['alpha']
         trimap = results['trimap']
 
-        # generete segmentation mask
+        # generate segmentation mask
         kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE,
                                            (self.kernel_size,
                                             self.kernel_size))
         seg = (alpha > 0.5).astype(np.float32)
         seg = cv2.erode(
             seg, kernel, iterations=np.random.randint(*self.erode_iter_range))
         seg = cv2.dilate(
```

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/aug_frames.py` & `mmagic-1.0.1/mmagic/datasets/transforms/aug_frames.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/aug_pixel.py` & `mmagic-1.0.1/mmagic/datasets/transforms/aug_pixel.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/aug_shape.py` & `mmagic-1.0.1/mmagic/datasets/transforms/aug_shape.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/blur_kernels.py` & `mmagic-1.0.1/mmagic/datasets/transforms/blur_kernels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is referenced from BasicSR with modifications.
 # Reference: https://github.com/xinntao/BasicSR/blob/master/basicsr/data/degradations.py  # noqa
-# Original licence: Copyright (c) 2020 xinntao, under the Apache 2.0 license.
+# Original license: Copyright (c) 2020 xinntao, under the Apache 2.0 license.
 
 import numpy as np
 from scipy import special
 
 
 def get_rotated_sigma_matrix(sig_x, sig_y, theta):
     """Calculate the rotated sigma matrix (two dimensional matrix).
```

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/crop.py` & `mmagic-1.0.1/mmagic/datasets/transforms/crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
         repr_str += f'(key={self.key})'
 
         return repr_str
 
 
 @TRANSFORMS.register_module()
 class PairedRandomCrop(BaseTransform):
-    """Paried random crop.
+    """Paired random crop.
 
     It crops a pair of img and gt images with corresponding locations.
     It also supports accepting img list and gt list.
     Required keys are "scale", "lq_key", and "gt_key",
     added or modified keys are "lq_key" and "gt_key".
 
     Args:
```

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/fgbg.py` & `mmagic-1.0.1/mmagic/datasets/transforms/fgbg.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/formatting.py` & `mmagic-1.0.1/mmagic/datasets/transforms/formatting.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/generate_assistant.py` & `mmagic-1.0.1/mmagic/datasets/transforms/generate_assistant.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/generate_frame_indices.py` & `mmagic-1.0.1/mmagic/datasets/transforms/generate_frame_indices.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/get_masked_image.py` & `mmagic-1.0.1/mmagic/datasets/transforms/get_masked_image.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/loading.py` & `mmagic-1.0.1/mmagic/datasets/transforms/loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         use_cache (bool): If True, load all images at once. Default: False.
         to_float32 (bool): Whether to convert the loaded image to a float32
             numpy array. If set to False, the loaded image is an uint8 array.
             Defaults to False.
         to_y_channel (bool): Whether to convert the loaded image to y channel.
             Only support 'rgb2ycbcr' and 'rgb2ycbcr'
             Defaults to False.
-        backend_args (dict, optional): Arguments to instantiate the preifx of
+        backend_args (dict, optional): Arguments to instantiate the prefix of
             uri corresponding backend. Defaults to None.
     """
 
     def __init__(
         self,
         key: str,
         color_type: str = 'color',
@@ -461,15 +461,15 @@
         use_cache (bool): If True, load all images at once. Default: False.
         to_float32 (bool): Whether to convert the loaded image to a float32
             numpy array. If set to False, the loaded image is an uint8 array.
             Defaults to False.
         to_y_channel (bool): Whether to convert the loaded image to y channel.
             Only support 'rgb2ycbcr' and 'rgb2ycbcr'
             Defaults to False.
-        backend_args (dict, optional): Arguments to instantiate the preifx of
+        backend_args (dict, optional): Arguments to instantiate the prefix of
             uri corresponding backend. Defaults to None.
         io_backend (str, optional): io backend where images are store. Defaults
             to None.
     """
 
     def __init__(self,
                  key: str,
```

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/matlab_like_resize.py` & `mmagic-1.0.1/mmagic/datasets/transforms/matlab_like_resize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This code is referenced from matlab_imresize with modifications
 # Reference:
 # https://github.com/fatheral/matlab_imresize/blob/master/imresize.py
-# Original licence: Copyright (c) 2020 fatheral, under the MIT License.
+# Original license: Copyright (c) 2020 fatheral, under the MIT License.
 import numpy as np
 from mmcv.transforms import BaseTransform
 
 from mmagic.registry import TRANSFORMS
 
 
 def get_size_from_scale(input_size, scale_factor):
```

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/normalization.py` & `mmagic-1.0.1/mmagic/datasets/transforms/normalization.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/random_degradations.py` & `mmagic-1.0.1/mmagic/datasets/transforms/random_degradations.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
         """This is the function used to randomly resize images for training
         augmentation.
 
         Args:
             imgs (Tensor): training images.
 
         Returns:
-            Tensor: images after radomly resized
+            Tensor: images after randomly resized
         """
         is_single_image = False
         if isinstance(imgs, np.ndarray):
             is_single_image = True
             imgs = [imgs]
 
         h, w = imgs[0].shape[:2]
```

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/random_down_sampling.py` & `mmagic-1.0.1/mmagic/datasets/transforms/random_down_sampling.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/trimap.py` & `mmagic-1.0.1/mmagic/datasets/transforms/trimap.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/datasets/transforms/values.py` & `mmagic-1.0.1/mmagic/datasets/transforms/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     Added keys are the keys in the dictionary.
 
     Required Keys:
 
     - None
 
-    Added or Modifyed Keys:
+    Added or Modified Keys:
 
     - keys in the dictionary
 
     Args:
         dictionary (dict): The dictionary to update.
     """
```

### Comparing `mmagic-1.0.0/mmagic/datasets/unpaired_image_dataset.py` & `mmagic-1.0.1/mmagic/datasets/unpaired_image_dataset.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/engine/hooks/__init__.py` & `mmagic-1.0.1/mmagic/engine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/engine/hooks/ema.py` & `mmagic-1.0.1/mmagic/engine/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/engine/hooks/iter_time_hook.py` & `mmagic-1.0.1/mmagic/engine/hooks/iter_time_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         """
         # Update iteration time in `runner.message_hub`.
         message_hub = runner.message_hub
         message_hub.update_scalar(f'{mode}/time', time.time() - self.t)
         self.t = time.time()
         window_size = runner.log_processor.window_size
         # Calculate eta every `window_size` iterations. Since test and val
-        # loop will not update runner.iter, use `every_n_innter_iters`to check
+        # loop will not update runner.iter, use `every_n_inner_iters`to check
         # the interval.
         if self.every_n_inner_iters(batch_idx, window_size):
             iter_time = message_hub.get_scalar(f'{mode}/time').mean(
                 window_size)
             if mode == 'train':
                 self.time_sec_tot += iter_time * window_size
                 # Calculate average iterative time.
```

### Comparing `mmagic-1.0.0/mmagic/engine/hooks/pggan_fetch_data_hook.py` & `mmagic-1.0.1/mmagic/engine/hooks/pggan_fetch_data_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             runner.train_loop.dataloader = new_dataloader
             if isinstance(runner.train_loop, IterBasedTrainLoop):
                 runner.train_loop.dataloader_iterator = \
                     _InfiniteDataloaderIterator(new_dataloader)
 
     def update_dataloader(self, dataloader: DataLoader,
                           curr_scale: int) -> Optional[DataLoader]:
-        """Updata the data loader.
+        """Update the data loader.
 
         Args:
             dataloader (DataLoader): The dataloader to be updated.
             curr_scale (int): The current scale of the generated image.
 
         Returns:
             Optional[DataLoader]: The updated dataloader. If the dataloader do
```

### Comparing `mmagic-1.0.0/mmagic/engine/hooks/pickle_data_hook.py` & `mmagic-1.0.1/mmagic/engine/hooks/pickle_data_hook.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/engine/hooks/reduce_lr_scheduler_hook.py` & `mmagic-1.0.1/mmagic/engine/hooks/reduce_lr_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/engine/hooks/visualization_hook.py` & `mmagic-1.0.1/mmagic/engine/hooks/visualization_hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
             outputs: outputs of the generation model
         """
         return
 
     @master_only
     def after_test_iter(self, runner: Runner, batch_idx: int, data_batch: dict,
                         outputs):
-        """Visualize samples after test iteraiton.
+        """Visualize samples after test iteration.
 
         Args:
             runner (Runner): The runner of the training process.
             batch_idx (int): The index of the current batch in the test loop.
             data_batch (dict, optional): Data from dataloader.
                 Defaults to None.
             outputs: outputs of the generation model Defaults to None.
@@ -295,15 +295,15 @@
                    runner: Runner,
                    batch_idx: int,
                    data_batch: dict,
                    outputs: Optional[dict] = None) -> None:
         """Visualize samples.
 
         Args:
-            runner (Runner): The runner conatians model to visualize.
+            runner (Runner): The runner contains model to visualize.
             batch_idx (int): The index of the current batch in loop.
             data_batch (dict): Data from dataloader.
                 Defaults to None.
             outputs (dict, optional): Outputs from model. Defaults to None.
         """
         # this function will only called in training process
         num_batches = runner.train_dataloader.batch_size
```

### Comparing `mmagic-1.0.0/mmagic/engine/optimizers/multi_optimizer_constructor.py` & `mmagic-1.0.1/mmagic/engine/optimizers/multi_optimizer_constructor.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
     def __init__(self, optim_wrapper_cfg: dict, paramwise_cfg=None):
 
         if not isinstance(optim_wrapper_cfg, dict):
             raise TypeError('optimizer_cfg should be a dict',
                             f'but got {type(optim_wrapper_cfg)}')
         assert paramwise_cfg is None, (
-            'parawise_cfg should be set in each optimizer separately')
+            'paramwise_cfg should be set in each optimizer separately')
         self.optim_cfg = optim_wrapper_cfg
 
         if 'modules' in optim_wrapper_cfg:
             # single optimizer with multi param groups
             cfg_ = optim_wrapper_cfg.copy()
             self.modules = cfg_.pop('modules')
             paramwise_cfg_ = cfg_.pop('paramwise_cfg', None)
```

### Comparing `mmagic-1.0.0/mmagic/engine/optimizers/pggan_optimizer_constructor.py` & `mmagic-1.0.1/mmagic/engine/optimizers/pggan_optimizer_constructor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 @OPTIM_WRAPPER_CONSTRUCTORS.register_module()
 class PGGANOptimWrapperConstructor:
     """OptimizerConstructor for PGGAN models. Set optimizers for each
     stage of PGGAN. All submodule must be contained in a
     :class:`torch.nn.ModuleList` named 'blocks'. And we access each submodule
-    by `MODEL.blocks[SCALE]`, where `MODLE` is generator or discriminator, and
+    by `MODEL.blocks[SCALE]`, where `MODEL` is generator or discriminator, and
     the scale is the index of the resolution scale.
 
     More detail about the resolution scale and naming rule please refers to
     :class:`~mmagic.models.editors.pggan.PGGANGenerator` and
     :class:`~mmagic.models.editors.pggan.PGGANDiscriminator`.
 
     Example:
@@ -76,15 +76,15 @@
     def __init__(self,
                  optim_wrapper_cfg: dict,
                  paramwise_cfg: Optional[dict] = None):
         if not isinstance(optim_wrapper_cfg, dict):
             raise TypeError('optimizer_cfg should be a dict',
                             f'but got {type(optim_wrapper_cfg)}')
         assert paramwise_cfg is None, (
-            'parawise_cfg should be set in each optimizer separately')
+            'paramwise_cfg should be set in each optimizer separately')
         self.optim_cfg = deepcopy(optim_wrapper_cfg)
 
         self.reset_optim = self.optim_cfg.pop('reset_optim_for_new_scale',
                                               True)
         print(self.reset_optim)
         self.lr_schedule = self.optim_cfg.pop('lr_schedule', dict())
         self.constructors = {}
```

### Comparing `mmagic-1.0.0/mmagic/engine/optimizers/singan_optimizer_constructor.py` & `mmagic-1.0.1/mmagic/engine/optimizers/singan_optimizer_constructor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 @OPTIM_WRAPPER_CONSTRUCTORS.register_module()
 class SinGANOptimWrapperConstructor:
     """OptimizerConstructor for SinGAN models. Set optimizers for each
     submodule of SinGAN. All submodule must be contained in a
     :class:`torch.nn.ModuleList` named 'blocks'. And we access each submodule
-    by `MODEL.blocks[SCALE]`, where `MODLE` is generator or discriminator, and
+    by `MODEL.blocks[SCALE]`, where `MODEL` is generator or discriminator, and
     the scale is the index of the resolution scale.
 
     More detail about the resolution scale and naming rule please refers to
     :class:`~mmagic.models.editors.singan.SinGANMultiScaleGenerator` and
     :class:`~mmagic.models.editors.singan.SinGANMultiScaleDiscriminator`.
 
     Example:
@@ -56,15 +56,15 @@
     def __init__(self,
                  optim_wrapper_cfg: dict,
                  paramwise_cfg: Optional[dict] = None):
         if not isinstance(optim_wrapper_cfg, dict):
             raise TypeError('optimizer_cfg should be a dict',
                             f'but got {type(optim_wrapper_cfg)}')
         assert paramwise_cfg is None, (
-            'parawise_cfg should be set in each optimizer separately')
+            'paramwise_cfg should be set in each optimizer separately')
         self.optim_cfg = optim_wrapper_cfg
         self.constructors = {}
         for key, cfg in self.optim_cfg.items():
             cfg_ = cfg.copy()
             paramwise_cfg_ = cfg_.pop('paramwise_cfg', None)
             self.constructors[key] = DefaultOptimWrapperConstructor(
                 cfg_, paramwise_cfg_)
```

### Comparing `mmagic-1.0.0/mmagic/engine/runner/log_processor.py` & `mmagic-1.0.1/mmagic/engine/runner/log_processor.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/engine/runner/loop_utils.py` & `mmagic-1.0.1/mmagic/engine/runner/loop_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Args:
         evaluator (Union[Evaluator, dict, list]): The evaluator instance or
             config dict.
     """
     # check Evaluator instance
     warning_template = ('Evaluator type for current config is \'{}\'. '
                         'If you want to use MultiValLoop, we strongly '
-                        'recommand you to use \'Evaluator\' provided by '
+                        'recommend you to use \'Evaluator\' provided by '
                         '\'MMagic\'. Otherwise, there maybe some potential '
                         'bugs.')
     if isinstance(evaluator, Evaluator):
         cls_name = evaluator.__class__.__name__
         if cls_name != 'Evaluator':
             print_log(warning_template.format(cls_name), 'current', WARNING)
         return evaluator
```

### Comparing `mmagic-1.0.0/mmagic/engine/runner/multi_loops.py` & `mmagic-1.0.1/mmagic/engine/runner/multi_loops.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         self._total_length = None  # length for all dataloaders
 
     @property
     def total_length(self) -> int:
         if self._total_length is not None:
             return self._total_length
 
-        warnings.warn('\'total_length\' has not been initializeda and return '
+        warnings.warn('\'total_length\' has not been initialized and return '
                       '\'0\' for safety. This result is likely to be incorrect'
                       ' and we recommend you to call \'total_length\' after '
                       '\'self.run\' is called.')
         return 0
 
     def _build_dataloaders(self,
                            dataloader: DATALOADER_TYPE) -> List[DataLoader]:
@@ -152,15 +152,15 @@
         # 3. Multi evaluator without type: [[dict, ...], [dict, ...]]
         # 4. Multi evaluator with type: [dict(type=xx, metrics=xx), dict(...)]
         if is_evaluator(evaluator):
             evaluator = [update_and_check_evaluator(evaluator)]
         else:
             assert all([
                 is_evaluator(cfg) for cfg in evaluator
-            ]), ('Unsupport evaluator type, please check your input and '
+            ]), ('Unsupported evaluator type, please check your input and '
                  'the docstring.')
             evaluator = [update_and_check_evaluator(cfg) for cfg in evaluator]
 
         evaluators = [runner.build_evaluator(eval) for eval in evaluator]
 
         return evaluators
 
@@ -347,15 +347,15 @@
         self._total_length = None
 
     @property
     def total_length(self) -> int:
         if self._total_length is not None:
             return self._total_length
 
-        warnings.warn('\'total_length\' has not been initializeda and return '
+        warnings.warn('\'total_length\' has not been initialized and return '
                       '\'0\' for safety. This result is likely to be incorrect'
                       ' and we recommend you to call \'total_length\' after '
                       '\'self.run\' is called.')
         return 0
 
     def _build_dataloaders(self,
                            dataloader: DATALOADER_TYPE) -> List[DataLoader]:
@@ -403,15 +403,15 @@
         # 3. Multi evaluator without type: [[dict, ...], [dict, ...]]
         # 4. Multi evaluator with type: [dict(type=xx, metrics=xx), dict(...)]
         if is_evaluator(evaluator):
             evaluator = [update_and_check_evaluator(evaluator)]
         else:
             assert all([
                 is_evaluator(cfg) for cfg in evaluator
-            ]), ('Unsupport evaluator type, please check your input and '
+            ]), ('Unsupported evaluator type, please check your input and '
                  'the docstring.')
             evaluator = [update_and_check_evaluator(cfg) for cfg in evaluator]
 
         evaluators = [runner.build_evaluator(eval) for eval in evaluator]
 
         return evaluators
```

### Comparing `mmagic-1.0.0/mmagic/engine/schedulers/linear_lr_scheduler_with_interval.py` & `mmagic-1.0.1/mmagic/engine/schedulers/linear_lr_scheduler_with_interval.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/engine/schedulers/reduce_lr_scheduler.py` & `mmagic-1.0.1/mmagic/engine/schedulers/reduce_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/__init__.py` & `mmagic-1.0.1/mmagic/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/evaluator.py` & `mmagic-1.0.1/mmagic/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/functional/fid_inception.py` & `mmagic-1.0.1/mmagic/evaluation/functional/fid_inception.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/functional/gaussian_funcs.py` & `mmagic-1.0.1/mmagic/evaluation/functional/gaussian_funcs.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/functional/inception_utils.py` & `mmagic-1.0.1/mmagic/evaluation/functional/inception_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 
 def load_inception(inception_args, metric):
     """Load Inception Model from given ``inception_args`` and ``metric``.
 
     This function would try to load Inception under the guidance of 'type'
     given in `inception_args`, if not given, we would try best to load Tero's
-    ones. In detailly, we would first try to load the model from disk with
+    ones. In detail, we would first try to load the model from disk with
     the given 'inception_path', and then try to download the checkpoint from
     'inception_url'. If both method are failed, pytorch version of Inception
     would be loaded.
 
     Args:
         inception_args (dict): Keyword args for inception net.
         metric (string): Metric to use the Inception. This argument would
@@ -163,21 +163,21 @@
                                            metric: BaseMetric, real_nums: int,
                                            capture_mean_cov: bool,
                                            capture_all: bool
                                            ) -> Tuple[str, dict]:
     """Get the name and meta info of the inception feature cache file
     corresponding to the input dataloader and metric.
 
-    The meta info includs
+    The meta info includes
     'data_root', 'data_prefix', 'meta_info' and 'pipeline' of the dataset, and
     'inception_style' and 'inception_args' of the metric. Then we calculate the
     hash value of the meta info dict with md5, and the name of the inception
     feature cache will be 'inception_feat_{HASH}.pkl'.
     Args:
-        datalaoder (Dataloader): The dataloader of real images.
+        dataloader (Dataloader): The dataloader of real images.
         metric (BaseMetric): The metric which needs inception features.
         real_nums (int): Number of images used to extract inception feature.
         capture_mean_cov (bool): Whether save the mean and covariance of
             inception feature. Defaults to False.
         capture_all (bool): Whether save the raw inception feature. Defaults
             to False.
     Returns:
@@ -227,21 +227,21 @@
 
 
 def get_vgg_feat_cache_name_and_args(dataloader: DataLoader,
                                      metric: BaseMetric) -> Tuple[str, dict]:
     """Get the name and meta info of the vgg feature cache file corresponding
     to the input dataloader and metric.
 
-    The meta info includs 'data_root',
+    The meta info includes 'data_root',
     'data_prefix', 'meta_info' and 'pipeline' of the dataset, and
     'use_tero_scirpt' of the metric. Then we calculate the hash value of the
     meta info dict with md5, and the name of the vgg feature cache will be
     'vgg_feat_{HASH}.pkl'.
     Args:
-        datalaoder (Dataloader): The dataloader of real images.
+        dataloader (Dataloader): The dataloader of real images.
         metric (BaseMetric): The metric which needs inception features.
     Returns:
         Tuple[str, dict]: Filename and meta info dict of the inception feature
             cache.
     """
 
     dataset: BaseDataset = dataloader.dataset
@@ -282,19 +282,19 @@
 
     - If `metric.inception_pkl` is an online path, try to download and load
       it. If cannot download or load, corresponding error will be raised.
     - If `metric.inception_pkl` is local path and file exists, try to load the
       file. If cannot load, corresponding error will be raised.
     - If `metric.inception_pkl` is local path and file not exists, we will
       extract the inception feature manually and save to 'inception_pkl'.
-    - If `metric.inception_pkl` is not defined, we will extrace the inception
+    - If `metric.inception_pkl` is not defined, we will extract the inception
       feature and save it to default cache dir with default name.
 
     Args:
-        datalaoder (Dataloader): The dataloader of real images.
+        dataloader (Dataloader): The dataloader of real images.
         metric (BaseMetric): The metric which needs inception features.
         data_preprocessor (Optional[nn.Module]): Data preprocessor of the
             module. Used to preprocess the real images. If not passed, real
             images will automatically normalized to [-1, 1]. Defaults to None.
         capture_mean_cov (bool): Whether save the mean and covariance of
             inception feature. Defaults to False.
         capture_all (bool): Whether save the raw inception feature. If true,
@@ -455,19 +455,19 @@
 
     - If `metric.vgg_pkl` is an online path, try to download and load
       it. If cannot download or load, corresponding error will be raised.
     - If `metric.vgg_pkl` is local path and file exists, try to load the
       file. If cannot load, corresponding error will be raised.
     - If `metric.vgg_pkl` is local path and file not exists, we will
       extract the vgg feature manually and save to 'vgg_pkl'.
-    - If `metric.vgg_pkl` is not defined, we will extrace the vgg
+    - If `metric.vgg_pkl` is not defined, we will extract the vgg
       feature and save it to default cache dir with default name.
 
     Args:
-        datalaoder (Dataloader): The dataloader of real images.
+        dataloader (Dataloader): The dataloader of real images.
         metric (BaseMetric): The metric which needs vgg features.
         data_preprocessor (Optional[nn.Module]): Data preprocessor of the
             module. Used to preprocess the real images. If not passed, real
             images will automatically normalized to [-1, 1]. Defaults to None.
         Returns:
             np.ndarray: Loaded vgg feature.
     """
@@ -477,15 +477,15 @@
 
     if isinstance(vgg_pkl, str):
         if is_filepath(vgg_pkl) and osp.exists(vgg_pkl):
             with open(vgg_pkl, 'rb') as file:
                 vgg_state = pickle.load(file)
             print_log(
                 f'\'{metric.prefix}\' successful load VGG feature '
-                f'from \'{vgg_pkl}\'', 'currnet')
+                f'from \'{vgg_pkl}\'', 'current')
             return vgg_state['vgg_feat']
         elif vgg_pkl.startswith('s3'):
             try:
                 raise NotImplementedError(
                     'Not support download from Ceph currently')
             except Exception as exp:
                 raise exp('Not support download from Ceph currently')
```

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/__init__.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/base_gen_metric.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/base_gen_metric.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/base_sample_wise_metric.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/base_sample_wise_metric.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/connectivity_error.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/connectivity_error.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/equivariance.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/equivariance.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/fid.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/fid.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
             real_cov) - 2 * np.trace(cov_sqrt)
 
         fid = mean_norm + trace
 
         return float(fid), float(mean_norm), float(trace)
 
     def compute_metrics(self, fake_results: list) -> dict:
-        """Compulate the result of FID metric.
+        """Compute the result of FID metric.
 
         Args:
             fake_results (list): List of image feature of fake images.
 
         Returns:
             dict: A dict of the computed FID metric and its mean and
                 covariance.
```

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/gradient_error.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/gradient_error.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/inception_score.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/inception_score.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/mae.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/mae.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/matting_mse.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/matting_mse.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/metrics_utils.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/ms_ssim.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/ms_ssim.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/mse.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/mse.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/niqe.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/niqe.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/niqe_pris_params.npz` & `mmagic-1.0.1/mmagic/evaluation/metrics/niqe_pris_params.npz`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/ppl.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/ppl.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/precision_and_recall.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/precision_and_recall.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/psnr.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/psnr.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/sad.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/sad.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/snr.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/snr.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/ssim.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/ssim.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/evaluation/metrics/swd.py` & `mmagic-1.0.1/mmagic/evaluation/metrics/swd.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,15 @@
             result_collected = [res for res in result_collected]
             results_collected.append(result_collected)
 
         self._num_processed = 0
         return results_collected
 
     def compute_metrics(self, results_fake, results_real) -> dict:
-        """Compulate the result of SWD metric.
+        """Compute the result of SWD metric.
 
         Args:
             fake_results (list): List of image feature of fake images.
             real_results (list): List of image feature of real images.
 
         Returns:
             dict: A dict of the computed SWD metric.
```

### Comparing `mmagic-1.0.0/mmagic/models/__init__.py` & `mmagic-1.0.1/mmagic/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/__init__.py` & `mmagic-1.0.1/mmagic/models/archs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .multi_layer_disc import MultiLayerDiscriminator
 from .patch_disc import PatchDiscriminator
 from .resnet import ResNet
 from .separable_conv_module import DepthwiseSeparableConvModule
 from .simple_encoder_decoder import SimpleEncoderDecoder
 from .smpatch_disc import SoftMaskPatchDiscriminator
 from .sr_backbone import ResidualBlockNoBN
+from .tokenizer import TokenizerWrapper
 from .upsample import PixelShufflePack
 from .vgg import VGG16
 from .wrapper import DiffusersWrapper
 
 
 def register_diffusers_models() -> List[str]:
     """Register models in ``diffusers.models`` to the ``MODELS`` registry.
@@ -69,9 +70,9 @@
 __all__ = [
     'ASPP', 'DepthwiseSeparableConvModule', 'SimpleGatedConvModule',
     'LinearModule', 'pixel_unshuffle', 'PixelShufflePack', 'ImgNormalize',
     'SpatialTemporalEnsemble', 'SoftMaskPatchDiscriminator',
     'SimpleEncoderDecoder', 'MultiLayerDiscriminator', 'PatchDiscriminator',
     'VGG16', 'ResNet', 'AllGatherLayer', 'ResidualBlockNoBN', 'LoRAWrapper',
     'set_lora', 'set_lora_disable', 'set_lora_enable',
-    'set_only_lora_trainable'
+    'set_only_lora_trainable', 'TokenizerWrapper'
 ]
```

### Comparing `mmagic-1.0.0/mmagic/models/archs/all_gather_layer.py` & `mmagic-1.0.1/mmagic/models/archs/all_gather_layer.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/aspp.py` & `mmagic-1.0.1/mmagic/models/archs/aspp.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/downsample.py` & `mmagic-1.0.1/mmagic/models/archs/downsample.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/ensemble.py` & `mmagic-1.0.1/mmagic/models/archs/ensemble.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/gated_conv_module.py` & `mmagic-1.0.1/mmagic/models/archs/gated_conv_module.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/img_normalize.py` & `mmagic-1.0.1/mmagic/models/archs/img_normalize.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/linear_module.py` & `mmagic-1.0.1/mmagic/models/archs/linear_module.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/lora.py` & `mmagic-1.0.1/mmagic/models/archs/lora.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/multi_layer_disc.py` & `mmagic-1.0.1/mmagic/models/archs/multi_layer_disc.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/patch_disc.py` & `mmagic-1.0.1/mmagic/models/archs/patch_disc.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/resnet.py` & `mmagic-1.0.1/mmagic/models/archs/resnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
             # the convolution with stride
 
             if m.stride == (2, 2):
                 m.stride = (1, 1)
                 if m.kernel_size == (3, 3):
                     m.dilation = (dilate // 2, dilate // 2)
                     m.padding = (dilate // 2, dilate // 2)
-            # other convoluions
+            # other convolutions
             else:
                 if m.kernel_size == (3, 3):
                     m.dilation = (dilate, dilate)
                     m.padding = (dilate, dilate)
 
     def init_weights(self, pretrained: Optional[str] = None) -> None:
         """Init weights for the model.
```

### Comparing `mmagic-1.0.0/mmagic/models/archs/separable_conv_module.py` & `mmagic-1.0.1/mmagic/models/archs/separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/simple_encoder_decoder.py` & `mmagic-1.0.1/mmagic/models/archs/simple_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/smpatch_disc.py` & `mmagic-1.0.1/mmagic/models/archs/smpatch_disc.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/sr_backbone.py` & `mmagic-1.0.1/mmagic/models/archs/sr_backbone.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/upsample.py` & `mmagic-1.0.1/mmagic/models/archs/upsample.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/vgg.py` & `mmagic-1.0.1/mmagic/models/archs/vgg.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/archs/wrapper.py` & `mmagic-1.0.1/mmagic/models/archs/wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import os
 from logging import WARNING
 from typing import Any, List, Optional, Union
 
+import torch
 from mmengine import print_log
 from mmengine.model import BaseModule
+from torch import dtype as TORCH_DTYPE
+
+dtype_mapping = {
+    'float32': torch.float32,
+    'float16': torch.float16,
+    'fp32': torch.float32,
+    'fp16': torch.float16,
+    'half': torch.float16,
+}
 
 
 class DiffusersWrapper(BaseModule):
     """Wrapper for models from HuggingFace Diffusers. This wrapper will be set
     a attribute called `_module_cls` by wrapping function and will be used to
     initialize the model structure.
 
@@ -58,14 +68,15 @@
             function.  Otherwise, *args and **kwargs will be used to
             initialize the model by `self._module_cls(*args, **kwargs)`.
     """
 
     def __init__(self,
                  from_pretrained: Optional[Union[str, os.PathLike]] = None,
                  from_config: Optional[Union[str, os.PathLike]] = None,
+                 dtype: Optional[Union[str, TORCH_DTYPE]] = None,
                  init_cfg: Union[dict, List[dict], None] = None,
                  *args,
                  **kwargs):
         super().__init__(init_cfg)
 
         module_cls = self._module_cls
         assert not (from_pretrained and from_config), (
@@ -83,14 +94,23 @@
             self._is_init = True
         elif from_config is not None:
             _config = module_cls.load_config(from_config, *args, **kwargs)
             self.model = module_cls(**_config)
         else:
             self.model = module_cls(*args, **kwargs)
 
+        if dtype is not None:
+            if isinstance(dtype, str):
+                assert dtype in dtype_mapping, (
+                    'Only support following dtype string: '
+                    f'{list(dtype_mapping.keys())}, but receive {dtype}.')
+                dtype = dtype_mapping[dtype]
+            self.model.to(dtype)
+            print_log(f'Set model dtype to \'{dtype}\'.', 'current')
+
         self.config = self.model.config
 
     def init_weights(self):
         """Initialize the weights.
 
         If type is 'Pretrained' but the model has be loaded from `repo_id`, a
         warning will be raised.
```

### Comparing `mmagic-1.0.0/mmagic/models/base_models/__init__.py` & `mmagic-1.0.1/mmagic/models/base_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/base_models/average_model.py` & `mmagic-1.0.1/mmagic/models/base_models/average_model.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/base_models/base_conditional_gan.py` & `mmagic-1.0.1/mmagic/models/base_models/base_conditional_gan.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,22 +132,22 @@
                 num_classes_disc = discriminator.get('num_classes', None)
             else:
                 num_classes_disc = getattr(discriminator, 'num_classes', None)
 
         # check consistency between gen and disc
         if num_classes_gen is not None and num_classes_disc is not None:
             assert num_classes_disc == num_classes_gen, (
-                '\'num_classes\' is unconsistency between generator and '
+                '\'num_classes\' is inconsistent between generator and '
                 f'discriminator. Receive \'{num_classes_gen}\' and '
                 f'\'{num_classes_disc}\'.')
         model_num_classes = num_classes_gen or num_classes_disc
 
         if num_classes is not None and model_num_classes is not None:
             assert num_classes == model_num_classes, (
-                'Input \'num_classes\' is unconsistency with '
+                'Input \'num_classes\' is inconsistent with '
                 f'model\'s ones. Receive \'{num_classes}\' and '
                 f'\'{model_num_classes}\'.')
 
         num_classes = num_classes or model_num_classes
         return num_classes
 
     def forward(self,
```

### Comparing `mmagic-1.0.0/mmagic/models/base_models/base_edit_model.py` & `mmagic-1.0.1/mmagic/models/base_models/base_edit_model.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/base_models/base_gan.py` & `mmagic-1.0.1/mmagic/models/base_models/base_gan.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         If loss_config is a dict, we allow kinds of value for each field.
 
         1. `loss_config` is None: Users will implement all loss calculations
             in their own function. Weights for each loss terms are hard coded.
         2. `loss_config` is dict of scalar or string: Users will implement all
             loss calculations and use passed `loss_config` to control the
             weight or behavior of the loss calculation. Users will unpack and
-            use each field in this dict by themself.
+            use each field in this dict by themselves.
 
             loss_config = dict(gp_norm_mode='HWC', gp_loss_weight=10)
 
         3. `loss_config` is dict of dict: Each field in `loss_config` will
             used to build a corresponding loss module. And use loss calculation
             function predefined by :class:`BaseGAN` to calculate the loss.
 
@@ -392,29 +392,29 @@
 
         Calls ``self.data_preprocessor(data)`` and
         ``self(inputs, data_sample, mode=None)`` in order. Return the
         generated results which will be passed to evaluator.
 
         Args:
             data (dict): Data sampled from metric specific
-                sampler. More detials in `Metrics` and `Evaluator`.
+                sampler. More details in `Metrics` and `Evaluator`.
 
         Returns:
             SampleList: Generated image or image dict.
         """
         data = self.data_preprocessor(data)
         outputs = self(**data)
         return outputs
 
     def test_step(self, data: dict) -> SampleList:
         """Gets the generated image of given data. Same as :meth:`val_step`.
 
         Args:
             data (dict): Data sampled from metric specific
-                sampler. More detials in `Metrics` and `Evaluator`.
+                sampler. More details in `Metrics` and `Evaluator`.
 
         Returns:
             List[DataSample]: Generated image or image dict.
         """
         data = self.data_preprocessor(data)
         outputs = self(**data)
         return outputs
```

### Comparing `mmagic-1.0.0/mmagic/models/base_models/base_mattor.py` & `mmagic-1.0.1/mmagic/models/base_models/base_mattor.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/base_models/base_translation_model.py` & `mmagic-1.0.1/mmagic/models/base_models/base_translation_model.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/base_models/basic_interpolator.py` & `mmagic-1.0.1/mmagic/models/base_models/basic_interpolator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/base_models/one_stage.py` & `mmagic-1.0.1/mmagic/models/base_models/one_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,16 @@
 
             1. get fake res/image
             2. optimize discriminator (if have)
             3. optimize generator
 
         If `self.train_cfg.disc_step > 1`, the train step will contain multiple
         iterations for optimizing discriminator with different input data and
-        only one iteration for optimizing gerator after `disc_step` iterations
-        for discriminator.
+        only one iteration for optimizing generator after `disc_step`
+        iterations for discriminator.
 
         Args:
             data (List[dict]): Batch of data as input.
             optim_wrapper (dict[torch.optim.Optimizer]): Dict with optimizers
                 for generator and discriminator (if have).
 
         Returns:
```

### Comparing `mmagic-1.0.0/mmagic/models/base_models/two_stage.py` & `mmagic-1.0.1/mmagic/models/base_models/two_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,16 +227,16 @@
         the pipeline:
         1. get fake res/image
         2. optimize discriminator (if have)
         3. optimize generator
 
         If `self.train_cfg.disc_step > 1`, the train step will contain multiple
         iterations for optimizing discriminator with different input data and
-        only one iteration for optimizing gerator after `disc_step` iterations
-        for discriminator.
+        only one iteration for optimizing generator after `disc_step`
+        iterations for discriminator.
 
         Args:
             data (List[dict]): Batch of data as input.
             optim_wrapper (dict[torch.optim.Optimizer]): Dict with optimizers
                 for generator and discriminator (if have).
 
         Returns:
```

### Comparing `mmagic-1.0.0/mmagic/models/data_preprocessors/data_preprocessor.py` & `mmagic-1.0.1/mmagic/models/data_preprocessors/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/data_preprocessors/mattor_preprocessor.py` & `mmagic-1.0.1/mmagic/models/data_preprocessors/mattor_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/diffusion_schedulers/__init__.py` & `mmagic-1.0.1/mmagic/models/diffusion_schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/diffusion_schedulers/ddim_scheduler.py` & `mmagic-1.0.1/mmagic/models/diffusion_schedulers/ddim_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
         self.alphas = 1.0 - self.betas
         self.alphas_cumprod = np.cumprod(self.alphas, axis=0)
 
         # At every step in ddim, we are looking into the
         # previous alphas_cumprod. For the final step,
         # there is no previous alphas_cumprod because we are already
-        # at 0 `set_alpha_to_one` decides whether we set this paratemer
+        # at 0 `set_alpha_to_one` decides whether we set this parameter
         # simply to one or whether we use the final alpha of the
         # "non-previous" one.
         self.final_alpha_cumprod = np.array(
             1.0) if set_alpha_to_one else self.alphas_cumprod[0]
 
         # standard deviation of the initial noise distribution
         self.init_noise_sigma = 1.0
```

### Comparing `mmagic-1.0.0/mmagic/models/diffusion_schedulers/ddpm_scheduler.py` & `mmagic-1.0.1/mmagic/models/diffusion_schedulers/ddpm_scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,19 +211,15 @@
             'noise': noise
         }
 
     def add_noise(self, original_samples, noise, timesteps):
         """add noise."""
 
         sqrt_alpha_prod = self.alphas_cumprod[timesteps]**0.5
-        sqrt_alpha_prod = self.match_shape(sqrt_alpha_prod, original_samples)
         sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps])**0.5
-        sqrt_one_minus_alpha_prod = self.match_shape(sqrt_one_minus_alpha_prod,
-                                                     original_samples)
-
         noisy_samples = (
             sqrt_alpha_prod * original_samples +
             sqrt_one_minus_alpha_prod * noise)
         return noisy_samples
 
     def training_loss(self, model, x_0, t):
         raise NotImplementedError(
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/__init__.py` & `mmagic-1.0.1/mmagic/models/editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/aotgan/aot_decoder.py` & `mmagic-1.0.1/mmagic/models/editors/aotgan/aot_decoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/aotgan/aot_encoder.py` & `mmagic-1.0.1/mmagic/models/editors/aotgan/aot_encoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/aotgan/aot_encoder_decoder.py` & `mmagic-1.0.1/mmagic/models/editors/aotgan/aot_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/aotgan/aot_inpaintor.py` & `mmagic-1.0.1/mmagic/models/editors/aotgan/aot_inpaintor.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/aotgan/aot_neck.py` & `mmagic-1.0.1/mmagic/models/editors/aotgan/aot_neck.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/arcface/arcface_modules.py` & `mmagic-1.0.1/mmagic/models/editors/arcface/arcface_modules.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/arcface/id_loss.py` & `mmagic-1.0.1/mmagic/models/editors/arcface/id_loss.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/arcface/model_irse.py` & `mmagic-1.0.1/mmagic/models/editors/arcface/model_irse.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/basicvsr/basicvsr.py` & `mmagic-1.0.1/mmagic/models/editors/basicvsr/basicvsr.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/basicvsr/basicvsr_net.py` & `mmagic-1.0.1/mmagic/models/editors/basicvsr/basicvsr_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/basicvsr_plusplus_net/basicvsr_plusplus_net.py` & `mmagic-1.0.1/mmagic/models/editors/basicvsr_plusplus_net/basicvsr_plusplus_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/biggan/__init__.py` & `mmagic-1.0.1/mmagic/models/editors/biggan/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/biggan/biggan.py` & `mmagic-1.0.1/mmagic/models/editors/biggan/biggan.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ModelType = Union[Dict, nn.Module]
 TrainInput = Union[dict, Tensor]
 
 
 @MODELS.register_module()
 class BigGAN(BaseConditionalGAN):
-    """Impelmentation of `Large Scale GAN Training for High Fidelity Natural
+    """Implementation of `Large Scale GAN Training for High Fidelity Natural
     Image Synthesis <https://arxiv.org/abs/1809.11096>`_ (BigGAN).
 
     Detailed architecture can be found in
     :class:`~mmagic.models.editors.biggan.BigGANGenerator`
     and
     :class:`~mmagic.models.editors.biggan.BigGANDiscriminator`
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/biggan/biggan_deep_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/biggan/biggan_deep_discriminator.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         with_spectral_norm (bool, optional): Whether to use spectral
             normalization. Defaults to True.
         blocks_cfg (dict, optional): Config for the convolution block.
             Defaults to dict(type='BigGANDiscResBlock').
         arch_cfg (dict, optional): Config for the architecture of this
             discriminator. Defaults to None.
         pretrained (str | dict, optional): Path for the pretrained model or
-            dict containing information for pretained models whose necessary
+            dict containing information for pretrained models whose necessary
             key is 'ckpt_path'. Besides, you can also provide 'prefix' to load
             the generator part from the whole state dict. Defaults to None.
     """
 
     def __init__(self,
                  input_scale,
                  num_classes=0,
@@ -249,15 +249,15 @@
         return out
 
     def init_weights(self, pretrained=None, init_type='ortho'):
         """Init weights for models.
 
         Args:
             pretrained (str | dict, optional): Path for the pretrained model or
-                dict containing information for pretained models whose
+                dict containing information for pretrained models whose
                 necessary key is 'ckpt_path'. Besides, you can also provide
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
             init_type (str, optional): The name of an initialization method:
                 ortho | N02 | xavier. Defaults to 'ortho'.
         """
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/biggan/biggan_deep_generator.py` & `mmagic-1.0.1/mmagic/models/editors/biggan/biggan_deep_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         blocks_cfg (dict, optional): Config for the convolution block. Defaults
             to dict(type='BigGANGenResBlock').
         arch_cfg (dict, optional): Config for the architecture of this
             generator. Defaults to None.
         out_norm_cfg (dict, optional): Config for the norm of output layer.
             Defaults to dict(type='BN').
         pretrained (str | dict, optional): Path for the pretrained model or
-            dict containing information for pretained models whose necessary
+            dict containing information for pretrained models whose necessary
             key is 'ckpt_path'. Besides, you can also provide 'prefix' to load
             the generator part from the whole state dict. Defaults to None.
         rgb2bgr (bool, optional): Whether to reformat the output channels
                 with order `bgr`. We provide several pre-trained BigGAN-Deep
                 weights whose output channels order is `rgb`. You can set
                 this argument to True to use the weights.
     """
@@ -354,15 +354,15 @@
 
         if self.num_classes == 0:
             label_batch = None
 
         elif isinstance(label, torch.Tensor):
             if not use_outside_embedding:
                 assert label.ndim == 1, (
-                    'The label shoube be in shape of (n, )'
+                    'The label should be in shape of (n, )'
                     f'but got {label.shape}.')
             label_batch = label
         elif callable(label):
             label_generator = label
             assert num_batches > 0
             label_batch = label_generator((num_batches, ))
         else:
@@ -421,15 +421,15 @@
         return out_img
 
     def init_weights(self, pretrained=None, init_type='ortho'):
         """Init weights for models.
 
         Args:
             pretrained (str | dict, optional): Path for the pretrained model or
-                dict containing information for pretained models whose
+                dict containing information for pretrained models whose
                 necessary key is 'ckpt_path'. Besides, you can also provide
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
             init_type (str, optional): The name of an initialization method:
                 ortho | N02 | xavier. Defaults to 'ortho'.
         """
         if isinstance(pretrained, str):
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/biggan/biggan_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/biggan/biggan_discriminator.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         with_spectral_norm (bool, optional): Whether to use spectral
             normalization. Defaults to True.
         blocks_cfg (dict, optional): Config for the convolution block.
             Defaults to dict(type='BigGANDiscResBlock').
         arch_cfg (dict, optional): Config for the architecture of this
             discriminator. Defaults to None.
         pretrained (str | dict, optional): Path for the pretrained model or
-            dict containing information for pretained models whose necessary
+            dict containing information for pretrained models whose necessary
             key is 'ckpt_path'. Besides, you can also provide 'prefix' to load
             the generator part from the whole state dict. Defaults to None.
     """
 
     def __init__(self,
                  input_scale,
                  num_classes=0,
@@ -230,15 +230,15 @@
         return out
 
     def init_weights(self, pretrained=None, init_type='ortho'):
         """Init weights for models.
 
         Args:
             pretrained (str | dict, optional): Path for the pretrained model or
-                dict containing information for pretained models whose
+                dict containing information for pretrained models whose
                 necessary key is 'ckpt_path'. Besides, you can also provide
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
             init_type (str, optional): The name of an initialization method:
                 ortho | N02 | xavier. Defaults to 'ortho'.
         """
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/biggan/biggan_generator.py` & `mmagic-1.0.1/mmagic/models/editors/biggan/biggan_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         blocks_cfg (dict, optional): Config for the convolution block. Defaults
             to dict(type='BigGANGenResBlock').
         arch_cfg (dict, optional): Config for the architecture of this
             generator. Defaults to None.
         out_norm_cfg (dict, optional): Config for the norm of output layer.
             Defaults to dict(type='BN').
         pretrained (str | dict, optional): Path for the pretrained model or
-            dict containing information for pretained models whose necessary
+            dict containing information for pretrained models whose necessary
             key is 'ckpt_path'. Besides, you can also provide 'prefix' to load
             the generator part from the whole state dict. Defaults to None.
         rgb2bgr (bool, optional): Whether to reformat the output channels
                 with order `bgr`. We provide several pre-trained BigGAN
                 weights whose output channels order is `rgb`. You can set
                 this argument to True to use the weights.
     """
@@ -344,15 +344,15 @@
 
         elif isinstance(label, torch.Tensor):
             if not use_outside_embedding:
                 if label.ndim != 1:
                     assert all([s == 1 for s in label.shape[1:]])
                     label = label.view(-1)
                 assert label.ndim == 1, (
-                    'The label shoube be in shape of (n, )'
+                    'The label should be in shape of (n, )'
                     f'but got {label.shape}.')
             label_batch = label
         elif callable(label):
             label_generator = label
             assert num_batches > 0
             label_batch = label_generator((num_batches, ))
         else:
@@ -409,15 +409,15 @@
         return out_img
 
     def init_weights(self, pretrained=None, init_type='ortho'):
         """Init weights for models.
 
         Args:
             pretrained (str | dict, optional): Path for the pretrained model or
-                dict containing information for pretained models whose
+                dict containing information for pretrained models whose
                 necessary key is 'ckpt_path'. Besides, you can also provide
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
             init_type (str, optional): The name of an initialization method:
                 ortho | N02 | xavier. Defaults to 'ortho'.
         """
         if isinstance(pretrained, str):
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/biggan/biggan_modules.py` & `mmagic-1.0.1/mmagic/models/editors/biggan/biggan_modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,15 +647,15 @@
         x0 = self.conv1(x0)
 
         x0 = self.bn2(x0, y)
         x0 = self.activation(x0)
         # Drop channels in x  if necessary
         if self.in_channels != self.out_channels:
             x = x[:, :self.out_channels]
-        # unsample both h and x at this point
+        # upsample both h and x at this point
         if self.with_upsample:
             x0 = self.upsample_layer(x0)
             x = self.upsample_layer(x)
         x0 = self.conv2(x0)
 
         x0 = self.bn3(x0, y)
         x0 = self.activation(x0)
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/biggan/biggan_snmodule.py` & `mmagic-1.0.1/mmagic/models/editors/biggan/biggan_snmodule.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/cain/cain.py` & `mmagic-1.0.1/mmagic/models/editors/cain/cain.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/cain/cain_net.py` & `mmagic-1.0.1/mmagic/models/editors/cain/cain_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/controlnet/controlnet.py` & `mmagic-1.0.1/mmagic/models/editors/controlnet/controlnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             ControlNet.
         schedule (Union[dict, nn.Module]): The config or module for diffusion
             scheduler.
         test_scheduler (Union[dict, nn.Module], optional): The config or
             module for diffusion scheduler in test stage (`self.infer`). If not
             passed, will use the same scheduler as `schedule`. Defaults to
             None.
+        dtype (str, optional): The dtype for the model. Defaults to 'fp16'.
         enable_xformers (bool, optional): Whether to use xformers.
             Defaults to True.
         data_preprocessor (dict, optional): The pre-process config of
             :class:`BaseDataPreprocessor`. Defaults to
                 dict(type='DataPreprocessor').
         init_cfg (dict, optional): The weight initialized config for
             :class:`BaseModule`. Defaults to None/
@@ -56,22 +57,29 @@
                  vae: ModelType,
                  text_encoder: ModelType,
                  tokenizer: str,
                  unet: ModelType,
                  controlnet: ModelType,
                  scheduler: ModelType,
                  test_scheduler: Optional[ModelType] = None,
+                 dtype: str = 'fp32',
                  enable_xformers: bool = True,
+                 tomesd_cfg: Optional[dict] = None,
                  data_preprocessor=dict(type='DataPreprocessor'),
                  init_cfg: Optional[dict] = None):
         super().__init__(vae, text_encoder, tokenizer, unet, scheduler,
-                         test_scheduler, enable_xformers, data_preprocessor,
-                         init_cfg)
+                         test_scheduler, dtype, enable_xformers, tomesd_cfg,
+                         data_preprocessor, init_cfg)
 
-        self.controlnet = build_module(controlnet, MODELS)
+        default_args = dict()
+        if dtype is not None:
+            default_args['dtype'] = dtype
+        self.controlnet = build_module(
+            controlnet, MODELS, default_args=default_args)
+        self.set_xformers(self.controlnet)
 
         self.vae.requires_grad_(False)
         self.text_encoder.requires_grad_(False)
         self.unet.requires_grad_(False)
 
     def init_weights(self):
         """Initialize the weights. Noted that this function will only be called
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/controlnet/controlnet_utils.py` & `mmagic-1.0.1/mmagic/models/editors/controlnet/controlnet_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/cyclegan/cyclegan.py` & `mmagic-1.0.1/mmagic/models/editors/cyclegan/cyclegan.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         return log_vars
 
     def test_step(self, data: dict) -> SampleList:
         """Gets the generated image of given data. Same as :meth:`val_step`.
 
         Args:
             data (dict): Data sampled from metric specific
-                sampler. More detials in `Metrics` and `Evaluator`.
+                sampler. More details in `Metrics` and `Evaluator`.
 
         Returns:
             SampleList: A list of ``DataSample`` contain generated results.
         """
         data = self.data_preprocessor(data)
         inputs_dict, data_samples = data['inputs'], data['data_samples']
 
@@ -253,15 +253,15 @@
         return batch_sample_list
 
     def val_step(self, data: dict) -> SampleList:
         """Gets the generated image of given data. Same as :meth:`val_step`.
 
         Args:
             data (dict): Data sampled from metric specific
-                sampler. More detials in `Metrics` and `Evaluator`.
+                sampler. More details in `Metrics` and `Evaluator`.
 
         Returns:
             SampleList: A list of ``DataSample`` contain generated results.
         """
         data = self.data_preprocessor(data)
         inputs_dict, data_samples = data['inputs'], data['data_samples']
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/cyclegan/cyclegan_generator.py` & `mmagic-1.0.1/mmagic/models/editors/cyclegan/cyclegan_generator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/cyclegan/cyclegan_modules.py` & `mmagic-1.0.1/mmagic/models/editors/cyclegan/cyclegan_modules.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/dcgan/dcgan.py` & `mmagic-1.0.1/mmagic/models/editors/dcgan/dcgan.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from mmagic.registry import MODELS
 from mmagic.structures import DataSample
 from ...base_models import BaseGAN
 
 
 @MODELS.register_module()
 class DCGAN(BaseGAN):
-    """Impelmentation of `Unsupervised Representation Learning with Deep
+    """Implementation of `Unsupervised Representation Learning with Deep
     Convolutional Generative Adversarial Networks`.
 
     Paper link:
         <https://arxiv.org/abs/1511.06434>`_ (DCGAN).
 
     Detailed architecture can be found in
     :class:`~mmagic.models.editors.dcgan.DCGANGenerator`  # noqa
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/dcgan/dcgan_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/dcgan/dcgan_discriminator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/dcgan/dcgan_generator.py` & `mmagic-1.0.1/mmagic/models/editors/dcgan/dcgan_generator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/ddpm/attention.py` & `mmagic-1.0.1/mmagic/models/editors/ddpm/attention.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/ddpm/denoising_unet.py` & `mmagic-1.0.1/mmagic/models/editors/ddpm/denoising_unet.py`

 * *Files 0% similar despite different names*

```diff
@@ -776,23 +776,23 @@
             embedding layer and label embedding layer. If not passed (or
             passed ``-1``), output channels of the embedding layers will set
             as four times of ``base_channels``. Defaults to ``-1``.
         num_classes (int, optional): The number of conditional classes. If set
             to 0, this model will be degraded to an unconditional model.
             Defaults to 0.
         channels_cfg (list | dict[list], optional): Config for input channels
-            of the intermedia blocks. If list is passed, each element of the
+            of the intermediate blocks. If list is passed, each element of the
             list indicates the scale factor for the input channels of the
             current block with regard to the ``base_channels``. For block
             ``i``, the input and output channels should be
             ``channels_cfg[i] * base_channels`` and
             ``channels_cfg[i+1] * base_channels`` If dict is provided, the key
             of the dict should be the output scale and corresponding value
             should be a list to define channels. Default: Please refer to
-            ``_defualt_channels_cfg``.
+            ``_default_channels_cfg``.
         output_cfg (dict, optional): Config for output variables. Defaults to
             ``dict(mean='eps', var='learned_range')``.
         norm_cfg (dict, optional): The config for normalization layers.
             Defaults to ``dict(type='GN', num_groups=32)``.
         act_cfg (dict, optional): The config for activation layers. Defaults
             to ``dict(type='SiLU', inplace=False)``.
         shortcut_kernel_size (int, optional): The kernel size for shortcut
@@ -817,15 +817,15 @@
         upsample_cfg (dict, optional): Config for upsample blocks.
             Defaults to ``dict(type='DenoisingDownsample')``.
         downsample_cfg (dict, optional): Config for downsample blocks.
             Defaults to ``dict(type='DenoisingUpsample')``.
         attention_res (int | list[int], optional): Resolution of feature maps
             to apply attention operation. Defaults to ``[16, 8]``.
         pretrained (str | dict, optional): Path for the pretrained model or
-            dict containing information for pretained models whose necessary
+            dict containing information for pretrained models whose necessary
             key is 'ckpt_path'. Besides, you can also provide 'prefix' to load
             the generator part from the whole state dict.  Defaults to None.
     """
 
     _default_channels_cfg = {
         512: [0.5, 1, 1, 2, 2, 4, 4],
         256: [1, 1, 2, 2, 4, 4],
@@ -1157,15 +1157,15 @@
 
         Returns:
             torch.Tensor | dict: If not ``return_noise``
         """
         # By default samples have to be AT least a multiple of t
         # he overall upsampling factor.
         # The overall upsampling factor is equal
-        # to 2 ** (# num of upsampling layears).
+        # to 2 ** (# num of upsampling layers).
         # However, the upsampling interpolation output size
         # can be forced to fit any upsampling size
         # on the fly if necessary.
         default_overall_up_factor = 2**self.num_upsamplers
 
         # upsample size should be forwarded when sample is not
         # a multiple of `default_overall_up_factor`
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/ddpm/embeddings.py` & `mmagic-1.0.1/mmagic/models/editors/ddpm/embeddings.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/ddpm/res_blocks.py` & `mmagic-1.0.1/mmagic/models/editors/ddpm/res_blocks.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/ddpm/unet_blocks.py` & `mmagic-1.0.1/mmagic/models/editors/ddpm/unet_blocks.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/deepfillv1/__init__.py` & `mmagic-1.0.1/mmagic/models/editors/deepfillv1/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/deepfillv1/contextual_attention.py` & `mmagic-1.0.1/mmagic/models/editors/deepfillv1/contextual_attention.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/deepfillv1/contextual_attention_neck.py` & `mmagic-1.0.1/mmagic/models/editors/deepfillv1/contextual_attention_neck.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/deepfillv1/deepfill_decoder.py` & `mmagic-1.0.1/mmagic/models/editors/deepfillv1/deepfill_decoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/deepfillv1/deepfill_disc.py` & `mmagic-1.0.1/mmagic/models/editors/deepfillv1/deepfill_disc.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/deepfillv1/deepfill_encoder.py` & `mmagic-1.0.1/mmagic/models/editors/deepfillv1/deepfill_encoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/deepfillv1/deepfill_refiner.py` & `mmagic-1.0.1/mmagic/models/editors/deepfillv1/deepfill_refiner.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/deepfillv1/deepfillv1.py` & `mmagic-1.0.1/mmagic/models/editors/deepfillv1/deepfillv1.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,16 +259,16 @@
 
             1. get fake res/image
             2. optimize discriminator (if have)
             3. optimize generator
 
         If `self.train_cfg.disc_step > 1`, the train step will contain multiple
         iterations for optimizing discriminator with different input data and
-        only one iteration for optimizing gerator after `disc_step` iterations
-        for discriminator.
+        only one iteration for optimizing generator after `disc_step`
+        iterations for discriminator.
 
         Args:
             data (List[dict]): Batch of data as input.
             optim_wrapper (dict[torch.optim.Optimizer]): Dict with optimizers
                 for generator and discriminator (if have).
 
         Returns:
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/deepfillv2/two_stage_encoder_decoder.py` & `mmagic-1.0.1/mmagic/models/editors/deepfillv2/two_stage_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/dic/dic.py` & `mmagic-1.0.1/mmagic/models/editors/dic/dic.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/dic/dic_net.py` & `mmagic-1.0.1/mmagic/models/editors/dic/dic_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/dic/feedback_hour_glass.py` & `mmagic-1.0.1/mmagic/models/editors/dic/feedback_hour_glass.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/dic/light_cnn.py` & `mmagic-1.0.1/mmagic/models/editors/dic/light_cnn.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/dim/dim.py` & `mmagic-1.0.1/mmagic/models/editors/dim/dim.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/disco_diffusion/disco.py` & `mmagic-1.0.1/mmagic/models/editors/disco_diffusion/disco.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/disco_diffusion/guider.py` & `mmagic-1.0.1/mmagic/models/editors/disco_diffusion/guider.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/disco_diffusion/secondary_model.py` & `mmagic-1.0.1/mmagic/models/editors/disco_diffusion/secondary_model.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/dreambooth/dreambooth.py` & `mmagic-1.0.1/mmagic/models/editors/dreambooth/dreambooth.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,21 +69,22 @@
                  val_prompts: Union[str, List[str]] = None,
                  class_prior_prompt: Optional[str] = None,
                  num_class_images: Optional[int] = 3,
                  prior_loss_weight: float = 0,
                  finetune_text_encoder: bool = False,
                  dtype: str = 'fp16',
                  enable_xformers: bool = True,
+                 tomesd_cfg: Optional[dict] = None,
                  data_preprocessor: Optional[ModelType] = dict(
                      type='DataPreprocessor'),
                  init_cfg: Optional[dict] = None):
 
         super().__init__(vae, text_encoder, tokenizer, unet, scheduler,
-                         test_scheduler, enable_xformers, data_preprocessor,
-                         init_cfg)
+                         test_scheduler, dtype, enable_xformers, tomesd_cfg,
+                         data_preprocessor, init_cfg)
         self.num_class_images = num_class_images
         self.class_prior_prompt = class_prior_prompt
         self.prior_loss_weight = prior_loss_weight
         self.class_images = []
 
         self.dtype = torch.float32
         if dtype == 'fp16':
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/duf/duf.py` & `mmagic-1.0.1/mmagic/models/editors/duf/duf.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/edsr/edsr_net.py` & `mmagic-1.0.1/mmagic/models/editors/edsr/edsr_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/edvr/edvr.py` & `mmagic-1.0.1/mmagic/models/editors/edvr/edvr.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             dict: Dict of losses.
         """
 
         if self.step_counter == 0 and self.with_tsa:
             if self.tsa_iter is None:
                 raise KeyError(
                     'In TSA mode, train_cfg must contain "tsa_iter".')
-            # only train TSA module at the beginging if with TSA module
+            # only train TSA module at the beginning if with TSA module
             for k, v in self.generator.named_parameters():
                 if 'fusion' not in k:
                     v.requires_grad = False
 
         if self.with_tsa and (self.step_counter == self.tsa_iter):
             # train all the parameters
             for v in self.generator.parameters():
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/edvr/edvr_net.py` & `mmagic-1.0.1/mmagic/models/editors/edvr/edvr_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/eg3d/camera.py` & `mmagic-1.0.1/mmagic/models/editors/eg3d/camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
         Args:
             fov (Optional[float], optional): FOV (field of view) in degree. If
                 not passed, :attr:`self.fov` will be used. Defaults to None.
             focal (Optional[float], optional): Focal in pixel. If
                 not passed, :attr:`self.focal` will be used. Defaults to None.
             batch_size (int): The batch size of the output. Defaults to 1.
-            device (DeviceType, optional): Device to put the intrinstic
+            device (DeviceType, optional): Device to put the intrinsic
                 matrix. If not passed, :attr:`self.device` will be used.
                 Defaults to None.
 
         Returns:
             torch.Tensor: Intrinsic matrix.
         """
         # 1. check if foc and focal is both passed
@@ -131,26 +131,26 @@
                          fov: Optional[float] = None,
                          device: DeviceType = None) -> torch.Tensor:
         """Calculate intrinsic matrix from FOV (field of view).
 
         Args:
             fov (Optional[float], optional): FOV (field of view) in degree. If
                 not passed, :attr:`self.fov` will be used. Defaults to None.
-            device (DeviceType, optional): Device to put the intrinstic
+            device (DeviceType, optional): Device to put the intrinsic
                 matrix. If not passed, :attr:`self.device` will be used.
                 Defaults to None.
 
         Returns:
             torch.Tensor: Intrinsic matrix.
         """
         fov = self.fov if fov is None else fov
         assert fov is not None, (
             '\'fov\' and \'self.fov\' should not be None at the same time.')
         # device = self.device if device is None else device
-        # NOTE: EG3D multpile '1 / 1.414' as `image_width` to `focal`, we
+        # NOTE: EG3D multiplies '1 / 1.414' as `image_width` to `focal`, we
         # retain this operation
         focal = float(1 / (math.tan(fov * math.pi / 360) * 1.414))
         intrinsics = [[focal, 0, 0.5], [0, focal, 0.5], [0, 0, 1]]
         intrinsics = torch.tensor(intrinsics, device=device)
         return intrinsics
 
     def focal_to_instrinsic(self,
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/eg3d/dual_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/eg3d/dual_discriminator.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 
 @MODELS.register_module('EG3DDiscriminator')
 @MODELS.register_module()
 class DualDiscriminator(StyleGAN2Discriminator):
     """Dual Discriminator for EG3D. DualDiscriminator shares the same network
     structure with StyleGAN2's Discriminator. However, DualDiscriminator take
-    volume rendered low-resolution image and super-resolutioned image at the
-    same time. The LR image will be upsampled and concatenate with SR ones, and
-    then feed to the discruminator together.
+    volume rendered low-resolution image and super-resolved image at the same
+    time. The LR image will be upsampled and concatenate with SR ones, and then
+    feed to the discriminator together.
 
     Args:
         img_channels (int): The number of the image channels. Defaults to 3.
         use_dual_disc (bool): Whether use dual discriminator as EG3D. If True,
             the input channel of the first conv block will be set as
             `2 * img_channels`. Defaults to True.
         disc_c_noise (float): The factor of noise's standard deviation add to
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/eg3d/eg3d.py` & `mmagic-1.0.1/mmagic/models/editors/eg3d/eg3d.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/eg3d/eg3d_generator.py` & `mmagic-1.0.1/mmagic/models/editors/eg3d/eg3d_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     EG3D generator contains three components:
 
     * A StyleGAN2 based backbone to generate a triplane feature
     * A neural renderer to sample and render low-resolution 2D feature and
       image from generated triplane feature
     * A super resolution module to upsample low-resolution image to
-      high-resolition one
+      high-resolution one
 
     Args:
         out_size (int): The resolution of the generated 2D image.
         noise_size (int): The size of the noise vector of the StyleGAN2
             backbone. Defaults to 512.
         style_channels (int): The number of channels for style code.
             Defaults to 512.
@@ -225,15 +225,15 @@
         # Reshape into 'raw' neural-rendered image
         H = W = self.neural_rendering_resolution
         feature_image = feature_samples.permute(0, 2, 1).reshape(
             batch_size, feature_samples.shape[-1], H, W).contiguous()
         depth_image = depth_samples.permute(0, 2,
                                             1).reshape(batch_size, 1, H, W)
 
-        # Run superresolution to get final image
+        # Run super resolution to get final image
         rgb_image = feature_image[:, :3]
         sr_image = self.sr_model(
             rgb_image, feature_image, styles, add_noise=self.sr_add_noise)
 
         if self.rgb2bgr:
             sr_image = sr_image.flip(1)
             rgb_image = rgb_image.flip(1)
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/eg3d/eg3d_modules.py` & `mmagic-1.0.1/mmagic/models/editors/eg3d/eg3d_modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             label (Optional[torch.Tensor]): Conditional inputs.
                 Defaults to None.
             truncation (float, optional): Truncation factor. Give value less
                 than 1., the truncation trick will be adopted. Defaults to 1.
             num_truncation_layer (int, optional): Number of layers use
                 truncated latent. Defaults to None.
             update_ws (bool): Whether update latent code with EMA. Only work
-                when `w_avg` is registeried. Defaults to False.
+                when `w_avg` is registered. Defaults to False.
 
         Returns:
             torch.Tensor: Style codes after mapping.
         """
         assert noise.shape[1] == self.noise_size
         noise = self.pixel_norm(noise)
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/eg3d/eg3d_utils.py` & `mmagic-1.0.1/mmagic/models/editors/eg3d/eg3d_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/eg3d/ray_sampler.py` & `mmagic-1.0.1/mmagic/models/editors/eg3d/ray_sampler.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/eg3d/renderer.py` & `mmagic-1.0.1/mmagic/models/editors/eg3d/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             The box is axis-aligned, centered at the origin. The range of each
             axis is `[-box_warp/2, box_warp/2]`. If `box_warp=1.8`, it has
             vertices at the range of axis is `[-0.9, 0.9]`. Defaults to 1.
         depth_resolution (int): Resolution of depth, as well as the number of
             points per ray. Defaults to 64.
         depth_resolution_importance (int): Resolution of depth in hierarchical
             sampling. Defaults to 64.
-        clamp_mode (str): The clamp mode for density predicted by nerural
+        clamp_mode (str): The clamp mode for density predicted by neural
             renderer. Defaults to 'softplus'.
         white_back (bool): Whether render a white background. Defaults to True.
         projection_mode (str): The projection method to mapping coordinates of
             render points to plane feature. The usage of this argument please
             refer to :meth:`self.project_onto_planes` and
             https://github.com/NVlabs/eg3d/issues/67. Defaults to 'Official'.
     """
@@ -308,15 +308,15 @@
         """Project 3D points to plane formed by coordinate axes. In this
         function, we use indexing operation to replace matrix multiplication to
         achieve higher calculation performance.
 
         In the original implementation, the mapping matrix is incorrect.
         Therefore we support users to define `projection_mode` to control
         projection behavior in the initialization function of
-        :class:`~EG3DRenderer`. If you want to run inference with the offifical
+        :class:`~EG3DRenderer`. If you want to run inference with the official
         pretrained model, please remember to set
         `projection_mode = 'official'`. More information please refer to
         https://github.com/NVlabs/eg3d/issues/67.
 
         If the project mode `official`, the equivalent projection matrix is
         inverse matrix of:
 
@@ -361,19 +361,19 @@
         Args:
             depths_c (torch.Tensor): Coarse depths shape like
                 (bz, NeRF_res * NeRF_res, N_depth, 1).
             colors_c (torch.Tensor): Coarse color features shape like
                 (bz, NeRF_res * NeRF_res, N_depth, N_feat).
             densities_c (torch.Tensor): Coarse densities shape like
                 (bz, NeRF_res * NeRF_res, N_depth, 1).
-            depths_f (torch.Tensro): Fine depths shape like
+            depths_f (torch.Tensor): Fine depths shape like
                 (bz, NeRF_res * NeRF_res, N_depth_fine, 1).
             colors_f (torch.Tensor): Fine colors features shape like
                 (bz, NeRF_res * NeRF_res, N_depth_fine, N_feat).
-            densities_f (torch.Tensor): Fine densites shape like
+            densities_f (torch.Tensor): Fine densities shape like
                 (bz, NeRF_res * NeRF_res, N_depth_fine, 1).
 
         Returns:
             Tuple[torch.Tensor]: Unified depths, color features and densities.
                 The third dimension of returns are `N_depth + N_depth_fine`.
         """
         all_depths = torch.cat([depths_c, depths_f], dim=-2)
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/esrgan/esrgan.py` & `mmagic-1.0.1/mmagic/models/editors/esrgan/esrgan.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/esrgan/rrdb_net.py` & `mmagic-1.0.1/mmagic/models/editors/esrgan/rrdb_net.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             Tensor: Forward results.
         """
         x1 = self.lrelu(self.conv1(x))
         x2 = self.lrelu(self.conv2(torch.cat((x, x1), 1)))
         x3 = self.lrelu(self.conv3(torch.cat((x, x1, x2), 1)))
         x4 = self.lrelu(self.conv4(torch.cat((x, x1, x2, x3), 1)))
         x5 = self.conv5(torch.cat((x, x1, x2, x3, x4), 1))
-        # Emperically, we use 0.2 to scale the residual for better performance
+        # Empirically, we use 0.2 to scale the residual for better performance
         return x5 * 0.2 + x
 
 
 class RRDB(nn.Module):
     """Residual in Residual Dense Block.
 
     Used in RRDB-Net in ESRGAN.
@@ -179,9 +179,9 @@
 
         Returns:
             Tensor: Forward results.
         """
         out = self.rdb1(x)
         out = self.rdb2(out)
         out = self.rdb3(out)
-        # Emperically, we use 0.2 to scale the residual for better performance
+        # Empirically, we use 0.2 to scale the residual for better performance
         return out * 0.2 + x
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/fba/fba_decoder.py` & `mmagic-1.0.1/mmagic/models/editors/fba/fba_decoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/fba/fba_encoder.py` & `mmagic-1.0.1/mmagic/models/editors/fba/fba_encoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/flavr/flavr.py` & `mmagic-1.0.1/mmagic/models/editors/flavr/flavr.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/flavr/flavr_net.py` & `mmagic-1.0.1/mmagic/models/editors/flavr/flavr_net.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,15 +566,15 @@
         out += residual
         out = self.relu(out)
 
         return out
 
 
 class SEGating(nn.Module):
-    """Gatting of SE attention.
+    """Gating of SE attention.
 
     Args:
         in_channels (int): Number of channels in the input feature map.
     """
 
     def __init__(self, in_channels):
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/gca/gca.py` & `mmagic-1.0.1/mmagic/models/editors/gca/gca.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/gca/gca_module.py` & `mmagic-1.0.1/mmagic/models/editors/gca/gca_module.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/gca/resgca_dec.py` & `mmagic-1.0.1/mmagic/models/editors/gca/resgca_dec.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/gca/resgca_enc.py` & `mmagic-1.0.1/mmagic/models/editors/gca/resgca_enc.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/ggan/ggan.py` & `mmagic-1.0.1/mmagic/models/editors/ggan/ggan.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from mmagic.registry import MODELS
 from mmagic.structures import DataSample
 from ...base_models import BaseGAN
 
 
 @MODELS.register_module()
 class GGAN(BaseGAN):
-    """Impelmentation of `Geomoetric GAN`.
+    """Implementation of `Geometric GAN`.
 
     <https://arxiv.org/abs/1705.02894>`_(GGAN).
     """
 
     def disc_loss(self, disc_pred_fake: Tensor,
                   disc_pred_real: Tensor) -> Tuple:
         r"""Get disc loss. GGAN use hinge loss to train
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/glean/glean_styleganv2.py` & `mmagic-1.0.1/mmagic/models/editors/glean/glean_styleganv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,25 +18,25 @@
         GLEAN: Generative Latent Bank for Large-Factor Image Super-Resolution,
         CVPR, 2021
 
     This method makes use of StyleGAN2 and hence the arguments mostly follow
     that in 'StyleGAN2v2Generator'.
 
     In StyleGAN2, we use a static architecture composing of a style mapping
-    module and number of covolutional style blocks. More details can be found
+    module and number of convolutional style blocks. More details can be found
     in: Analyzing and Improving the Image Quality of StyleGAN CVPR2020.
 
     You can load pretrained model through passing information into
     ``pretrained`` argument. We have already offered official weights as
     follows:
 
-    - styelgan2-ffhq-config-f: http://download.openmmlab.com/mmediting/stylegan2/official_weights/stylegan2-ffhq-config-f-official_20210327_171224-bce9310c.pth  # noqa
+    - stylegan2-ffhq-config-f: http://download.openmmlab.com/mmediting/stylegan2/official_weights/stylegan2-ffhq-config-f-official_20210327_171224-bce9310c.pth  # noqa
     - stylegan2-horse-config-f: http://download.openmmlab.com/mmediting/stylegan2/official_weights/stylegan2-horse-config-f-official_20210327_173203-ef3e69ca.pth  # noqa
     - stylegan2-car-config-f: http://download.openmmlab.com/mmediting/stylegan2/official_weights/stylegan2-car-config-f-official_20210327_172340-8cfe053c.pth  # noqa
-    - styelgan2-cat-config-f: http://download.openmmlab.com/mmediting/stylegan2/official_weights/stylegan2-cat-config-f-official_20210327_172444-15bc485b.pth  # noqa
+    - stylegan2-cat-config-f: http://download.openmmlab.com/mmediting/stylegan2/official_weights/stylegan2-cat-config-f-official_20210327_172444-15bc485b.pth  # noqa
     - stylegan2-church-config-f: http://download.openmmlab.com/mmediting/stylegan2/official_weights/stylegan2-church-config-f-official_20210327_172657-1d42b7d1.pth  # noqa
 
     If you want to load the ema model, you can just use following codes:
 
     .. code-block:: python
 
         # ckpt_http is one of the valid path from http source
@@ -60,22 +60,22 @@
             image and 1 for grayscale image. Default: 3.
         rrdb_channels (int): Number of channels of the RRDB features.
             Default: 64.
         num_rrdbs (int): Number of RRDB blocks in the encoder. Default: 23.
         style_channels (int): The number of channels for style code.
             Default: 512.
         num_mlps (int, optional): The number of MLP layers. Defaults to 8.
-        channel_multiplier (int, optional): The mulitiplier factor for the
+        channel_multiplier (int, optional): The multiplier factor for the
             channel number. Defaults to 2.
         blur_kernel (list, optional): The blurry kernel. Defaults
             to [1, 3, 3, 1].
         lr_mlp (float, optional): The learning rate for the style mapping
             layer. Defaults to 0.01.
         default_style_mode (str, optional): The default mode of style mixing.
-            In training, we defaultly adopt mixing style mode. However, in the
+            In training, we adopt mixing style mode in default. However, in the
             evaluation, we use 'single' style mode. `['mix', 'single']` are
             currently supported. Defaults to 'mix'.
         eval_style_mode (str, optional): The evaluation mode of style mixing.
             Defaults to 'single'.
         mix_prob (float, optional): Mixing probability. The value should be
             in range of [0, 1]. Defaults to 0.9.
         init_cfg (dict, optional): Initialization config dict. Default: None.
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/global_local/gl_decoder.py` & `mmagic-1.0.1/mmagic/models/editors/global_local/gl_decoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/global_local/gl_dilation.py` & `mmagic-1.0.1/mmagic/models/editors/global_local/gl_dilation.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/global_local/gl_disc.py` & `mmagic-1.0.1/mmagic/models/editors/global_local/gl_disc.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/global_local/gl_encoder.py` & `mmagic-1.0.1/mmagic/models/editors/global_local/gl_encoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/global_local/gl_encoder_decoder.py` & `mmagic-1.0.1/mmagic/models/editors/global_local/gl_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/global_local/gl_inpaintor.py` & `mmagic-1.0.1/mmagic/models/editors/global_local/gl_inpaintor.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,25 +39,25 @@
             start_iter=0,
             disc_step=1,
             iter_tc=90000,
             iter_td=100000
         )
 
     `iter_tc` and `iter_td` correspond to the notation :math:`T_C` and
-    :math:`T_D` of theoriginal paper.
+    :math:`T_D` of the original paper.
 
     Args:
         generator (dict): Config for encoder-decoder style generator.
         disc (dict): Config for discriminator.
         loss_gan (dict): Config for adversarial loss.
         loss_gp (dict): Config for gradient penalty loss.
         loss_disc_shift (dict): Config for discriminator shift loss.
         loss_composed_percep (dict): Config for perceptural and style loss with
             composed image as input.
-        loss_out_percep (dict): Config for perceptural and style loss with
+        loss_out_percep (dict): Config for perceptual and style loss with
             direct output as input.
         loss_l1_hole (dict): Config for l1 loss in the hole.
         loss_l1_valid (dict): Config for l1 loss in the valid region.
         loss_tv (dict): Config for total variation loss.
         train_cfg (dict): Configs for training scheduler. `disc_step` must be
             contained for indicates the discriminator updating steps in each
             training step.
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/guided_diffusion/adm.py` & `mmagic-1.0.1/mmagic/models/editors/guided_diffusion/adm.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,29 +243,29 @@
 
         Calls ``self.data_preprocessor(data)`` and
         ``self(inputs, data_sample, mode=None)`` in order. Return the
         generated results which will be passed to evaluator.
 
         Args:
             data (dict): Data sampled from metric specific
-                sampler. More detials in `Metrics` and `Evaluator`.
+                sampler. More details in `Metrics` and `Evaluator`.
 
         Returns:
             SampleList: Generated image or image dict.
         """
         data = self.data_preprocessor(data)
         outputs = self(**data)
         return outputs
 
     def test_step(self, data: dict) -> SampleList:
         """Gets the generated image of given data. Same as :meth:`val_step`.
 
         Args:
             data (dict): Data sampled from metric specific
-                sampler. More detials in `Metrics` and `Evaluator`.
+                sampler. More details in `Metrics` and `Evaluator`.
 
         Returns:
             List[DataSample]: Generated image or image dict.
         """
         data = self.data_preprocessor(data)
         outputs = self(**data)
         return outputs
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/guided_diffusion/classifier.py` & `mmagic-1.0.1/mmagic/models/editors/guided_diffusion/classifier.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/iconvsr/iconvsr_net.py` & `mmagic-1.0.1/mmagic/models/editors/iconvsr/iconvsr_net.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
         # activation function
         self.lrelu = nn.LeakyReLU(negative_slope=0.1, inplace=True)
 
         self._raised_warning = False
 
     def spatial_padding(self, lrs):
-        """Apply pdding spatially.
+        """Apply padding spatially.
 
         Since the PCD module in EDVR requires that the resolution is a multiple
         of 4, we apply padding to the input LR images if their resolution is
         not divisible by 4.
 
         Args:
             lrs (Tensor): Input LR sequence with shape (n, t, c, h, w).
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/indexnet/indexnet.py` & `mmagic-1.0.1/mmagic/models/editors/indexnet/indexnet.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/indexnet/indexnet_decoder.py` & `mmagic-1.0.1/mmagic/models/editors/indexnet/indexnet_decoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/indexnet/indexnet_encoder.py` & `mmagic-1.0.1/mmagic/models/editors/indexnet/indexnet_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,19 +30,19 @@
         out_channels (int): The output channels of the block.
         kernel_size (int): The kernel size of the block.
         stride (int, optional): The stride of the block. Defaults to 2.
         padding (int, optional): The padding of the block. Defaults to 0.
         groups (int, optional): The groups of the block. Defaults to 1.
         norm_cfg (dict, optional): The norm config of the block.
             Defaults to dict(type='BN').
-        use_nonlinear (bool, optional): Whether use nonlinearty in the block.
+        use_nonlinear (bool, optional): Whether use nonlinearity in the block.
             If true, a ConvModule with kernel size 1 will be appended and an
-            ``ReLU6`` nonlinearty will be added to the origin ConvModule.
+            ``ReLU6`` nonlinearity will be added to the origin ConvModule.
             Defaults to False.
-        expansion (int, optional): Expandsion ratio of the middle channels.
+        expansion (int, optional): Expansion ratio of the middle channels.
             Effective when ``use_nonlinear`` is true. Defaults to 1.
 
     Returns:
         nn.Module: The built conv block.
     """
     if use_nonlinear:
         return nn.Sequential(
@@ -337,15 +337,15 @@
             network. Defaults to 'm2o'.
         aspp (bool, optional): Whether use ASPP module to augment output
             feature. Defaults to True.
         norm_cfg (None | dict, optional): Config dict for normalization
             layer. Defaults to dict(type='BN').
         freeze_bn (bool, optional): Whether freeze batch norm layer.
             Defaults to False.
-        use_nonlinear (bool, optional): Whether use nonlinearty in index
+        use_nonlinear (bool, optional): Whether use nonlinearity in index
             network. Refer to the paper for more information.
             Defaults to True.
         use_context (bool, optional): Whether use larger kernel size in
             index network. Refer to the paper for more information.
             Defaults to True.
         init_cfg (dict, optional): Initialization config dict. Default: None.
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/inst_colorization/color_utils.py` & `mmagic-1.0.1/mmagic/models/editors/inst_colorization/color_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/inst_colorization/colorization_net.py` & `mmagic-1.0.1/mmagic/models/editors/inst_colorization/colorization_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/inst_colorization/fusion_net.py` & `mmagic-1.0.1/mmagic/models/editors/inst_colorization/fusion_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/inst_colorization/inst_colorization.py` & `mmagic-1.0.1/mmagic/models/editors/inst_colorization/inst_colorization.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/inst_colorization/weight_layer.py` & `mmagic-1.0.1/mmagic/models/editors/inst_colorization/weight_layer.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/liif/liif.py` & `mmagic-1.0.1/mmagic/models/editors/liif/liif.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/liif/liif_net.py` & `mmagic-1.0.1/mmagic/models/editors/liif/liif_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/liif/mlp_refiner.py` & `mmagic-1.0.1/mmagic/models/editors/liif/mlp_refiner.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/lsgan/lsgan.py` & `mmagic-1.0.1/mmagic/models/editors/lsgan/lsgan.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from mmagic.registry import MODELS
 from mmagic.structures import DataSample
 from ...base_models import BaseGAN
 
 
 @MODELS.register_module()
 class LSGAN(BaseGAN):
-    """Impelmentation of `Least Squares Generative Adversarial Networks`.
+    """Implementation of `Least Squares Generative Adversarial Networks`.
 
     Paper link: https://arxiv.org/pdf/1611.04076.pdf
 
     Detailed architecture can be found in
     :class:`~mmagic.models.editors.lsgan.LSGANGenerator`
     and
     :class:`~mmagic.models.editors.lsgan.LSGANDiscriminator`
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/lsgan/lsgan_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/lsgan/lsgan_discriminator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/lsgan/lsgan_generator.py` & `mmagic-1.0.1/mmagic/models/editors/lsgan/lsgan_generator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/mspie/__init__.py` & `mmagic-1.0.1/mmagic/models/editors/mspie/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/mspie/mspie_stylegan2.py` & `mmagic-1.0.1/mmagic/models/editors/mspie/mspie_stylegan2.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/mspie/mspie_stylegan2_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/mspie/mspie_stylegan2_discriminator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/mspie/mspie_stylegan2_generator.py` & `mmagic-1.0.1/mmagic/models/editors/mspie/mspie_stylegan2_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         channel_multiplier (int, optional): The multiplier factor for the
             channel number. Defaults to 2.
         blur_kernel (list, optional): The blurry kernel. Defaults
             to [1, 3, 3, 1].
         lr_mlp (float, optional): The learning rate for the style mapping
             layer. Defaults to 0.01.
         default_style_mode (str, optional): The default mode of style mixing.
-            In training, we defaultly adopt mixing style mode. However, in the
+            In training, we adopt mixing style mode in default. However, in the
             evaluation, we use 'single' style mode. `['mix', 'single']` are
             currently supported. Defaults to 'mix'.
         eval_style_mode (str, optional): The evaluation mode of style mixing.
             Defaults to 'single'.
         mix_prob (float, optional): Mixing probability. The value should be
             in range of [0, 1]. Defaults to 0.9.
     """
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/mspie/mspie_stylegan2_modules.py` & `mmagic-1.0.1/mmagic/models/editors/mspie/mspie_stylegan2_modules.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/mspie/pe_singan.py` & `mmagic-1.0.1/mmagic/models/editors/mspie/pe_singan.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/mspie/pe_singan_generator.py` & `mmagic-1.0.1/mmagic/models/editors/mspie/pe_singan_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ..singan.singan_modules import GeneratorBlock
 
 
 @MODELS.register_module()
 class SinGANMSGeneratorPE(SinGANMultiScaleGenerator):
     """Multi-Scale Generator used in SinGAN with positional encoding.
 
-    More details can be found in: Positional Encoding as Spatial Inductvie Bias
+    More details can be found in: Positional Encoding as Spatial Inductive Bias
     in GANs, CVPR'2021.
 
     Notes:
 
     - In this version, we adopt the interpolation function from the official
       PyTorch APIs, which is different from the original implementation by the
       authors. However, in our experiments, this influence can be ignored.
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/mspie/positional_encoding.py` & `mmagic-1.0.1/mmagic/models/editors/mspie/positional_encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class SinusoidalPositionalEmbedding(nn.Module):
     """Sinusoidal Positional Embedding 1D or 2D (SPE/SPE2d).
 
     This module is a modified from:
     https://github.com/pytorch/fairseq/blob/master/fairseq/modules/sinusoidal_positional_embedding.py # noqa
 
     Based on the original SPE in single dimension, we implement a 2D sinusoidal
-    positional encodding (SPE2d), as introduced in Positional Encoding as
+    positional encoding (SPE2d), as introduced in Positional Encoding as
     Spatial Inductive Bias in GANs, CVPR'2021.
 
     Args:
         embedding_dim (int): The number of dimensions for the positional
             encoding.
         padding_idx (int | list[int]): The index for the padding contents. The
             padding positions will obtain an encoding vector filling in zeros.
@@ -204,15 +204,15 @@
 @MODELS.register_module()
 class CatersianGrid(nn.Module):
     """Catersian Grid for 2d tensor.
 
     The Catersian Grid is a common-used positional encoding in deep learning.
     In this implementation, we follow the convention of ``grid_sample`` in
     PyTorch. In other words, ``[-1, -1]`` denotes the left-top corner while
-    ``[1, 1]`` denotes the right-botton corner.
+    ``[1, 1]`` denotes the right-bottom corner.
     """
 
     def forward(self, x, **kwargs):
         assert x.dim() == 4
         return self.make_grid2d_like(x, **kwargs)
 
     def make_grid2d(self, height, width, num_batches=1, requires_grad=False):
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/nafnet/naf_avgpool2d.py` & `mmagic-1.0.1/mmagic/models/editors/nafnet/naf_avgpool2d.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/nafnet/naf_layerNorm2d.py` & `mmagic-1.0.1/mmagic/models/editors/nafnet/naf_layerNorm2d.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/nafnet/nafbaseline_net.py` & `mmagic-1.0.1/mmagic/models/editors/nafnet/nafbaseline_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/nafnet/nafnet_net.py` & `mmagic-1.0.1/mmagic/models/editors/nafnet/nafnet_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/pconv/mask_conv_module.py` & `mmagic-1.0.1/mmagic/models/editors/pconv/mask_conv_module.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/pconv/partial_conv.py` & `mmagic-1.0.1/mmagic/models/editors/pconv/partial_conv.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/pconv/pconv_decoder.py` & `mmagic-1.0.1/mmagic/models/editors/pconv/pconv_decoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/pconv/pconv_encoder.py` & `mmagic-1.0.1/mmagic/models/editors/pconv/pconv_encoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/pconv/pconv_encoder_decoder.py` & `mmagic-1.0.1/mmagic/models/editors/pconv/pconv_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/pconv/pconv_inpaintor.py` & `mmagic-1.0.1/mmagic/models/editors/pconv/pconv_inpaintor.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
             1. get fake res/image
             2. optimize discriminator (if have)
             3. optimize generator
 
         If `self.train_cfg.disc_step > 1`, the train step will contain multiple
         iterations for optimizing discriminator with different input data and
-        only one iteration for optimizing gerator after `disc_step` iterations
-        for discriminator.
+        only one iteration for optimizing generator after `disc_step`
+        iterations for discriminator.
 
         Args:
             data (List[dict]): Batch of data as input.
             optim_wrapper (dict[torch.optim.Optimizer]): Dict with optimizers
                 for generator and discriminator (if have).
 
         Returns:
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/pggan/__init__.py` & `mmagic-1.0.1/mmagic/models/editors/pggan/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/pggan/pggan.py` & `mmagic-1.0.1/mmagic/models/editors/pggan/pggan.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             # sanity check for the order of scales
             assert len(self.scales) == 0 or k[0] > self.scales[-1][0]
             self.scales.append(k)
             self.nkimgs.append(v)
 
         self.cum_nkimgs = np.cumsum(self.nkimgs)
         self.curr_stage = 0
-        # dirty walkround for avoiding optimizer bug in resuming
+        # dirty workaround for avoiding optimizer bug in resuming
         self.prev_stage = prev_stage
         # actually nkimgs shown at the end of per training stage
         self._actual_nkimgs = []
         # In each scale, transit from previous torgb layer to newer torgb layer
         # with `transition_kimgs` imgs
         self.transition_kimgs = transition_kimgs
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/pggan/pggan_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/pggan/pggan_discriminator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/pggan/pggan_generator.py` & `mmagic-1.0.1/mmagic/models/editors/pggan/pggan_generator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/pggan/pggan_modules.py` & `mmagic-1.0.1/mmagic/models/editors/pggan/pggan_modules.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/pix2pix/pix2pix.py` & `mmagic-1.0.1/mmagic/models/editors/pix2pix/pix2pix.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         return log_vars
 
     def test_step(self, data: dict) -> SampleList:
         """Gets the generated image of given data. Same as :meth:`val_step`.
 
         Args:
             data (dict): Data sampled from metric specific
-                sampler. More detials in `Metrics` and `Evaluator`.
+                sampler. More details in `Metrics` and `Evaluator`.
 
         Returns:
             List[DataSample]: Generated image or image dict.
         """
         data = self.data_preprocessor(data)
         inputs_dict, data_samples = data['inputs'], data['data_samples']
         target_domain = self._reachable_domains[0]
@@ -196,18 +196,18 @@
         return batch_sample_list
 
     def val_step(self, data: dict) -> SampleList:
         """Gets the generated image of given data. Same as :meth:`val_step`.
 
         Args:
             data (dict): Data sampled from metric specific
-                sampler. More detials in `Metrics` and `Evaluator`.
+                sampler. More details in `Metrics` and `Evaluator`.
 
         Returns:
-            List[DataSampleenerated image or image dict.
+            List[DataSample]: Generated image or image dict.
         """
         data = self.data_preprocessor(data)
         inputs_dict, data_samples = data['inputs'], data['data_samples']
         target_domain = self._reachable_domains[0]
         source_domain = self.get_other_domains(target_domain)[0]
         outputs = self.forward_test(
             inputs_dict[f'img_{source_domain}'], target_domain=target_domain)
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/pix2pix/pix2pix_generator.py` & `mmagic-1.0.1/mmagic/models/editors/pix2pix/pix2pix_generator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/pix2pix/pix2pix_modules.py` & `mmagic-1.0.1/mmagic/models/editors/pix2pix/pix2pix_modules.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/plain/plain_decoder.py` & `mmagic-1.0.1/mmagic/models/editors/plain/plain_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
 @MODELS.register_module()
 class PlainDecoder(BaseModule):
     """Simple decoder from Deep Image Matting.
 
     Args:
         in_channels (int): Channel num of input features.
-        init_cfg (dict, optional): Initialization config dict. efaults to None.
+        init_cfg (dict, optional): Initialization config dict. Default: None.
     """
 
     def __init__(self, in_channels, init_cfg: Optional[dict] = None):
         super().__init__(init_cfg=init_cfg)
 
         self.deconv6_1 = nn.Conv2d(in_channels, 512, kernel_size=1)
         self.deconv5_1 = nn.Conv2d(512, 512, kernel_size=5, padding=2)
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/plain/plain_refiner.py` & `mmagic-1.0.1/mmagic/models/editors/plain/plain_refiner.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/rdn/rdn_net.py` & `mmagic-1.0.1/mmagic/models/editors/rdn/rdn_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/real_basicvsr/real_basicvsr.py` & `mmagic-1.0.1/mmagic/models/editors/real_basicvsr/real_basicvsr.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/real_basicvsr/real_basicvsr_net.py` & `mmagic-1.0.1/mmagic/models/editors/real_basicvsr/real_basicvsr_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/real_esrgan/real_esrgan.py` & `mmagic-1.0.1/mmagic/models/editors/real_esrgan/real_esrgan.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/real_esrgan/unet_disc.py` & `mmagic-1.0.1/mmagic/models/editors/real_esrgan/unet_disc.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/restormer/restormer_net.py` & `mmagic-1.0.1/mmagic/models/editors/restormer/restormer_net.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     def forward(self, x):
         """Forward function.
 
         Args:
             x (Tensor): Input tensor with shape (B, C, H, W).
 
         Returns:
-            Tesnor: Forward results.
+            Tensor: Forward results.
         """
         x = x + self.attn(self.norm1(x))
         x = x + self.ffn(self.norm2(x))
 
         return x
 
 
@@ -287,15 +287,15 @@
     def forward(self, x):
         """Forward function.
 
         Args:
             x (Tensor): Input tensor with shape (B, C, H, W).
 
         Returns:
-            Tesnor: Forward results.
+            Tensor: Forward results.
         """
         x = self.proj(x)
 
         return x
 
 
 class Downsample(BaseModule):
@@ -320,15 +320,15 @@
     def forward(self, x):
         """Forward function.
 
         Args:
             x (Tensor): Input tensor with shape (B, C, H, W).
 
         Returns:
-            Tesnor: Forward results.
+            Tensor: Forward results.
         """
         return self.body(x)
 
 
 class Upsample(BaseModule):
     """Upsample modules.
 
@@ -351,15 +351,15 @@
     def forward(self, x):
         """Forward function.
 
         Args:
             x (Tensor): Input tensor with shape (B, C, H, W).
 
         Returns:
-            Tesnor: Forward results.
+            Tensor: Forward results.
         """
         return self.body(x)
 
 
 @MODELS.register_module()
 class Restormer(BaseModule):
     """Restormer A PyTorch impl of: `Restormer: Efficient Transformer for High-
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/sagan/sagan.py` & `mmagic-1.0.1/mmagic/models/editors/sagan/sagan.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ModelType = Union[Dict, nn.Module]
 TrainInput = Union[dict, Tensor]
 
 
 @MODELS.register_module('SNGAN')
 @MODELS.register_module()
 class SAGAN(BaseConditionalGAN):
-    """Impelmentation of `Self-Attention Generative Adversarial Networks`.
+    """Implementation of `Self-Attention Generative Adversarial Networks`.
 
     <https://arxiv.org/abs/1805.08318>`_ (SAGAN), `Spectral Normalization for
     Generative Adversarial Networks <https://arxiv.org/abs/1802.05957>`_
     (SNGAN), and `cGANs with Projection Discriminator
     <https://arxiv.org/abs/1802.05637>`_ (Proj-GAN).
 
     Detailed architecture can be found in
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/sagan/sagan_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/sagan/sagan_discriminator.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     The overall structure of the projection discriminator can be split into a
     ``from_rgb`` layer, a group of ResBlocks, a linear decision layer, and a
     projection layer. To support defining custom layers, we introduce
     ``from_rgb_cfg`` and ``blocks_cfg``.
 
     The design of the model structure is highly corresponding to the output
     resolution. Therefore, we provide `channels_cfg` and `downsample_cfg` to
-    control the input channels and the downsample behavior of the intermedia
+    control the input channels and the downsample behavior of the intermediate
     blocks.
 
     ``downsample_cfg``: In default config of SNGAN / Proj-GAN, whether to apply
-        downsample in each intermedia blocks is quite flexible and
+        downsample in each intermediate blocks is quite flexible and
         corresponding to the resolution of the output image. Therefore, we
         support user to define the ``downsample_cfg`` by themselves, and to
         control the structure of the discriminator.
 
     ``channels_cfg``: In default config of SNGAN / Proj-GAN, the number of
         ResBlocks and the channels of those blocks are corresponding to the
         resolution of the output image. Therefore, we allow user to define
@@ -59,33 +59,33 @@
             block would be added after which *ConvBlock* (including the head
             block). If ``int`` is passed, only one attention block would be
             added. If ``list`` is passed, self-attention blocks would be added
             after multiple ConvBlocks. To be noted that if the input is
             smaller than ``1``, self-attention corresponding to this index
             would be ignored. Default to 0.
         channels_cfg (list | dict[list], optional): Config for input channels
-            of the intermedia blocks. If list is passed, each element of the
+            of the intermediate blocks. If list is passed, each element of the
             list means the input channels of current block is how many times
             compared to the ``base_channels``. For block ``i``, the input and
             output channels should be ``channels_cfg[i]`` and
             ``channels_cfg[i+1]`` If dict is provided, the key of the dict
             should be the output scale and corresponding value should be a list
             to define channels.  Default: Please refer to
             ``_defualt_channels_cfg``.
         downsample_cfg (list[bool] | dict[list], optional): Config for
-            downsample behavior of the intermedia layers. If a list is passed,
-            ``downsample_cfg[idx] == True`` means apply downsample in idx-th
-            block, and vice versa. If dict is provided, the key dict should
-            be the input scale of the image and corresponding value should be
-            a list ti define the downsample behavior. Default: Please refer
-            to ``_default_downsample_cfg``.
+            downsample behavior of the intermediate layers. If a list is
+            passed, ``downsample_cfg[idx] == True`` means apply downsample in
+            idx-th block, and vice versa. If dict is provided, the key dict
+            should be the input scale of the image and corresponding value
+            should be a list ti define the downsample behavior. Default: Please
+            refer to ``_default_downsample_cfg``.
         from_rgb_cfg (dict, optional): Config for the first layer to convert
             rgb image to feature map. Defaults to
             ``dict(type='SNGANDiscHeadResBlock')``.
-        blocks_cfg (dict, optional): Config for the intermedia blocks.
+        blocks_cfg (dict, optional): Config for the intermediate blocks.
             Defaults to ``dict(type='SNGANDiscResBlock')``
         act_cfg (dict, optional): Activation config for the final output
             layer. Defaults to ``dict(type='ReLU')``.
         with_spectral_norm (bool, optional): Whether use spectral norm for
             all conv blocks or not. Default to True.
         sn_style (str, optional): The style of spectral normalization.
             If set to `ajbrock`, implementation by
@@ -94,15 +94,15 @@
             If set to `torch`, implementation by `PyTorch` will be adopted.
             Defaults to `torch`.
         sn_eps (float, optional): eps for spectral normalization operation.
             Defaults to `1e-12`.
         init_cfg (dict, optional): Config for weight initialization.
             Default to ``dict(type='BigGAN')``.
         pretrained (str | dict , optional): Path for the pretrained model or
-            dict containing information for pretained models whose necessary
+            dict containing information for pretrained models whose necessary
             key is 'ckpt_path'. Besides, you can also provide 'prefix' to load
             the generator part from the whole state dict.  Defaults to None.
     """
 
     # default channel factors
     _defualt_channels_cfg = {
         32: [1, 1, 1],
@@ -288,15 +288,15 @@
         provide BigGAN's and Pytorch-StudioGAN's style initialization
         (``INIT_TYPE.upper() == BIGGAN`` and ``INIT_TYPE.upper() == STUDIO``).
         Please refer to https://github.com/ajbrock/BigGAN-PyTorch and
         https://github.com/POSTECH-CVLab/PyTorch-StudioGAN.
 
         Args:
             pretrained (str | dict, optional): Path for the pretrained model or
-                dict containing information for pretained models whose
+                dict containing information for pretrained models whose
                 necessary key is 'ckpt_path'. Besides, you can also provide
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
         """
         if isinstance(pretrained, str):
             logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=strict, logger=logger)
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/sagan/sagan_generator.py` & `mmagic-1.0.1/mmagic/models/editors/sagan/sagan_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,18 @@
         generalize, we support defining ``blocks_cfg`` by users and loading
         the blocks by calling the build_module method.
 
     Args:
         output_scale (int): Output scale for the generated image.
         num_classes (int, optional): The number classes you would like to
             generate. This arguments would influence the structure of the
-            intermedia blocks and label sampling operation in ``forward``
+            intermediate blocks and label sampling operation in ``forward``
             (e.g. If num_classes=0, ConditionalNormalization layers would
             degrade to unconditional ones.). This arguments would be passed
-            to intermedia blocks by overwrite their config. Defaults to 0.
+            to intermediate blocks by overwrite their config. Defaults to 0.
         base_channels (int, optional): The basic channel number of the
             generator. The other layers contains channels based on this number.
             Default to 64.
         out_channels (int, optional): Channels of the output images.
             Default to 3.
         input_scale (int, optional): Input scale for the features.
             Defaults to 4.
@@ -62,23 +62,23 @@
             block would be added after which *ConvBlock*. If ``int`` is passed,
             only one attention block would be added. If ``list`` is passed,
             self-attention blocks would be added after multiple ConvBlocks.
             To be noted that if the input is smaller than ``1``,
             self-attention corresponding to this index would be ignored.
             Default to 0.
         channels_cfg (list | dict[list], optional): Config for input channels
-            of the intermedia blocks. If list is passed, each element of the
+            of the intermediate blocks. If list is passed, each element of the
             list means the input channels of current block is how many times
             compared to the ``base_channels``. For block ``i``, the input and
             output channels should be ``channels_cfg[i]`` and
             ``channels_cfg[i+1]`` If dict is provided, the key of the dict
             should be the output scale and corresponding value should be a list
             to define channels.  Default: Please refer to
             ``_defualt_channels_cfg``.
-        blocks_cfg (dict, optional): Config for the intermedia blocks.
+        blocks_cfg (dict, optional): Config for the intermediate blocks.
             Defaults to ``dict(type='SNGANGenResBlock')``
         act_cfg (dict, optional): Activation config for the final output
             layer. Defaults to ``dict(type='ReLU')``.
         use_cbn (bool, optional): Whether use conditional normalization. This
             argument would pass to norm layers. Defaults to True.
         auto_sync_bn (bool, optional): Whether convert Batch Norm to
             Synchronized ones when Distributed training is on. Defaults to
@@ -99,15 +99,15 @@
         norm_eps (float, optional): eps for Normalization layers (both
             conditional and non-conditional ones). Default to `1e-4`.
         sn_eps (float, optional): eps for spectral normalization operation.
             Defaults to `1e-12`.
         init_cfg (string, optional): Config for weight initialization.
             Defaults to ``dict(type='BigGAN')``.
         pretrained (str | dict, optional): Path for the pretrained model or
-            dict containing information for pretained models whose necessary
+            dict containing information for pretrained models whose necessary
             key is 'ckpt_path'. Besides, you can also provide 'prefix' to load
             the generator part from the whole state dict.  Defaults to None.
         rgb_to_bgr (bool, optional): Whether to reformat the output channels
                 with order `bgr`. We provide several pre-trained BigGAN
                 weights whose output channels order is `rgb`. You can set
                 this argument to True to use the weights.
     """
@@ -275,15 +275,15 @@
             assert num_batches > 0
             noise_batch = torch.randn((num_batches, self.noise_size))
 
         if isinstance(label, torch.Tensor):
             if label.ndim != 1:
                 assert all([s == 1 for s in label.shape[1:]])
                 label = label.view(-1)
-            assert label.ndim == 1, ('The label shoube be in shape of (n, )'
+            assert label.ndim == 1, ('The label should be in shape of (n, )'
                                      f'but got {label.shape}.')
             label_batch = label
         elif callable(label):
             label_generator = label
             assert num_batches > 0
             label_batch = label_generator(num_batches)
         elif self.num_classes == 0:
@@ -335,15 +335,15 @@
         provide BigGAN's and Pytorch-StudioGAN's style initialization
         (``INIT_TYPE.upper() == BIGGAN`` and ``INIT_TYPE.upper() == STUDIO``).
         Please refer to https://github.com/ajbrock/BigGAN-PyTorch and
         https://github.com/POSTECH-CVLab/PyTorch-StudioGAN.
 
         Args:
             pretrained (str | dict, optional): Path for the pretrained model or
-                dict containing information for pretained models whose
+                dict containing information for pretrained models whose
                 necessary key is 'ckpt_path'. Besides, you can also provide
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
         """
         if isinstance(pretrained, str):
             logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=strict, logger=logger)
@@ -419,9 +419,9 @@
                         if 'bias' in n:
                             constant_init(m, 0)
             else:
                 raise NotImplementedError('Unknown initialization method: '
                                           f'\'{self.init_type}\'')
 
         else:
-            raise TypeError("'pretrined' must be a str or None. "
+            raise TypeError("'pretrained' must be a str or None. "
                             f'But receive {type(pretrained)}.')
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/sagan/sagan_modules.py` & `mmagic-1.0.1/mmagic/models/editors/sagan/sagan_modules.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/singan/singan.py` & `mmagic-1.0.1/mmagic/models/editors/singan/singan.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
         """Train step for SinGAN model. SinGAN is trained with multi-resolution
         images, and each resolution is trained for `:attr:self.iters_per_scale`
         times.
 
         We initialize the weight and learning rate scheduler of the
         corresponding module at the start of each resolution's training. At
         the end of each resolution's training, we update the weight of the
-        noise of current resolution by mse loss between reconstruced image and
+        noise of current resolution by mse loss between reconstructed image and
         real image.
 
         Args:
             data (dict): Data sampled from dataloader.
             optim_wrapper (OptimWrapperDict): OptimWrapperDict instance
                 contains OptimWrapper of generator and discriminator.
 
@@ -640,15 +640,15 @@
     def test_step(self, data: dict) -> SampleList:
         """Gets the generated image of given data in test progress. Before
         generate images, we call `:meth:self.load_test_pkl` to load the fixed
         noise and current stage of the model from the pickle file.
 
         Args:
             data (dict): Data sampled from metric specific
-                sampler. More detials in `Metrics` and `Evaluator`.
+                sampler. More details in `Metrics` and `Evaluator`.
 
         Returns:
             SampleList: A list of ``DataSample`` contain generated results.
         """
         if not self.loaded_test_pkl:
             self.load_test_pkl()
         return super().test_step(data)
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/singan/singan_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/singan/singan_discriminator.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,11 +75,11 @@
         if curr_scale == 0:
             return
         prev_ch = self.blocks[curr_scale - 1].base_channels
         curr_ch = self.blocks[curr_scale].base_channels
         if prev_ch == curr_ch:
             self.blocks[curr_scale].load_state_dict(
                 self.blocks[curr_scale - 1].state_dict())
-            print_log('Successfully load pretrianed model from last scale.')
+            print_log('Successfully load pretrained model from last scale.')
         else:
             print_log('Cannot load pretrained model from last scale since'
                       f' prev_ch({prev_ch}) != curr_ch({curr_ch})')
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/singan/singan_generator.py` & `mmagic-1.0.1/mmagic/models/editors/singan/singan_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,13 +173,13 @@
         prev_in_ch = self.blocks[curr_scale - 1].in_channels
         curr_in_ch = self.blocks[curr_scale].in_channels
         if prev_ch == curr_ch and prev_in_ch == curr_in_ch:
             load_state_dict(
                 self.blocks[curr_scale],
                 self.blocks[curr_scale - 1].state_dict(),
                 logger=MMLogger.get_current_instance())
-            logger.info('Successfully load pretrianed model from last scale.')
+            logger.info('Successfully load pretrained model from last scale.')
         else:
             logger.info(
                 'Cannot load pretrained model from last scale since'
                 f' prev_ch({prev_ch}) != curr_ch({curr_ch})'
                 f' or prev_in_ch({prev_in_ch}) != curr_in_ch({curr_in_ch})')
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/singan/singan_modules.py` & `mmagic-1.0.1/mmagic/models/editors/singan/singan_modules.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/srcnn/srcnn_net.py` & `mmagic-1.0.1/mmagic/models/editors/srcnn/srcnn_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/srgan/modified_vgg.py` & `mmagic-1.0.1/mmagic/models/editors/srgan/modified_vgg.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/srgan/sr_resnet.py` & `mmagic-1.0.1/mmagic/models/editors/srgan/sr_resnet.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/srgan/srgan.py` & `mmagic-1.0.1/mmagic/models/editors/srgan/srgan.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stable_diffusion/clip_wrapper.py` & `mmagic-1.0.1/mmagic/models/editors/stable_diffusion/clip_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         return torch.mm(normalized_image_embeds, normalized_text_embeds.t())
 
     class StableDiffusionSafetyChecker(PreTrainedModel):
         config_class = CLIPConfig
         _no_split_modules = ['CLIPEncoderLayer']
 
         def __init__(self, config: CLIPConfig):
-            """check result image for stable diffsuion to prevent NSFW content
+            """check result image for stable diffusion to prevent NSFW content
             generated.
 
             Args:
                 config(CLIPConfig): config for transformers clip.
             """
 
             super().__init__(config)
@@ -179,9 +179,9 @@
                     os.path.join(pretrained_model_path, 'safety_checker'))
 
         return tokenizer, feature_extractor, text_encoder, safety_checker
 
 else:
 
     def load_clip_submodels(init_cfg, submodels, requires_safety_checker):
-        raise ImportError('Please install tranformers via '
+        raise ImportError('Please install transformers via '
                           '\'pip install transformers\'')
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/stable_diffusion/stable_diffusion.py` & `mmagic-1.0.1/mmagic/models/editors/stable_diffusion/stable_diffusion.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from mmengine.logging import MMLogger
 from mmengine.model import BaseModel
 from mmengine.runner import set_random_seed
 from PIL import Image
 from tqdm.auto import tqdm
-from transformers import CLIPTokenizer
 
-from mmagic.models.utils import build_module, set_xformers
+from mmagic.models.archs import TokenizerWrapper
+from mmagic.models.utils import build_module, set_tomesd, set_xformers
 from mmagic.registry import DIFFUSION_SCHEDULERS, MODELS
 from mmagic.structures import DataSample
 from mmagic.utils.typing import SampleList
 
 logger = MMLogger.get_current_instance()
 
 ModelType = Union[Dict, nn.Module]
@@ -39,14 +39,16 @@
         tokenizer (str): The **name** for CLIP tokenizer.
         schedule (Union[dict, nn.Module]): The config or module for diffusion
             scheduler.
         test_scheduler (Union[dict, nn.Module], optional): The config or
             module for diffusion scheduler in test stage (`self.infer`). If not
             passed, will use the same scheduler as `schedule`. Defaults to
             None.
+        dtype (str, optional): The dtype for the model This argument will not work
+            when dtype is defined for submodels. Defaults to None.
         enable_xformers (bool, optional): Whether to use xformers.
             Defaults to True.
         data_preprocessor (dict, optional): The pre-process config of
             :class:`BaseDataPreprocessor`.
         init_cfg (dict, optional): The weight initialized config for
             :class:`BaseModule`.
     """
@@ -54,53 +56,72 @@
     def __init__(self,
                  vae: ModelType,
                  text_encoder: ModelType,
                  tokenizer: str,
                  unet: ModelType,
                  scheduler: ModelType,
                  test_scheduler: Optional[ModelType] = None,
+                 dtype: Optional[str] = None,
                  enable_xformers: bool = True,
+                 tomesd_cfg: Optional[dict] = None,
                  data_preprocessor: Optional[ModelType] = dict(
                      type='DataPreprocessor'),
                  init_cfg: Optional[dict] = None):
 
         # TODO: support `from_pretrained` for this class
         super().__init__(data_preprocessor, init_cfg)
 
-        self.vae = build_module(vae, MODELS)
-        self.unet = build_module(unet, MODELS)
+        default_args = dict()
+        if dtype is not None:
+            default_args['dtype'] = dtype
+        self.dtype = dtype
+        self.vae = build_module(vae, MODELS, default_args=default_args)
+        self.unet = build_module(unet, MODELS, default_args=default_args)
         self.scheduler = build_module(scheduler, DIFFUSION_SCHEDULERS)
         if test_scheduler is None:
             self.test_scheduler = deepcopy(self.scheduler)
         else:
             self.test_scheduler = build_module(test_scheduler,
                                                DIFFUSION_SCHEDULERS)
         self.text_encoder = build_module(text_encoder, MODELS)
-        if isinstance(tokenizer, nn.Module):
+        if not isinstance(tokenizer, str):
             self.tokenizer = tokenizer
         else:
             # NOTE: here we assume tokenizer is an string
-            # TODO: maybe support a tokenizer wrapper later
-            self.tokenizer = CLIPTokenizer.from_pretrained(
-                tokenizer, subfolder='tokenizer')
+            self.tokenizer = TokenizerWrapper(tokenizer, subfolder='tokenizer')
 
         self.unet_sample_size = self.unet.sample_size
         self.vae_scale_factor = 2**(len(self.vae.block_out_channels) - 1)
 
         self.enable_xformers = enable_xformers
         self.set_xformers()
 
-    def set_xformers(self) -> nn.Module:
+        self.tomesd_cfg = tomesd_cfg
+        self.set_tomesd()
+
+    def set_xformers(self, module: Optional[nn.Module] = None) -> nn.Module:
         """Set xformers for the model.
 
         Returns:
             nn.Module: The model with xformers.
         """
         if self.enable_xformers:
-            set_xformers(self)
+            if module is None:
+                set_xformers(self)
+            else:
+                set_xformers(module)
+
+    def set_tomesd(self) -> nn.Module:
+        """Set ToMe for the stable diffusion model.
+
+        Returns:
+            nn.Module: The model with ToMe.
+        """
+        if self.tomesd_cfg is not None:
+            set_tomesd(self, **self.tomesd_cfg)
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     @torch.no_grad()
     def infer(self,
@@ -313,21 +334,23 @@
             removed_text = self.tokenizer.batch_decode(
                 untruncated_ids[:, self.tokenizer.model_max_length - 1:-1])
             logger.warning(
                 'The following part of your input was truncated because CLIP'
                 ' can only handle sequences up to'
                 f' {self.tokenizer.model_max_length} tokens: {removed_text}')
 
-        if hasattr(self.text_encoder.config, 'use_attention_mask'
-                   ) and self.text_encoder.config.use_attention_mask:
+        text_encoder = self.text_encoder.module if hasattr(
+            self.text_encoder, 'module') else self.text_encoder
+        if hasattr(text_encoder.config, 'use_attention_mask'
+                   ) and text_encoder.config.use_attention_mask:
             attention_mask = text_inputs.attention_mask.to(device)
         else:
             attention_mask = None
 
-        text_embeddings = self.text_encoder(
+        text_embeddings = text_encoder(
             text_input_ids.to(device),
             attention_mask=attention_mask,
         )
         text_embeddings = text_embeddings[0]
 
         # duplicate text embeddings for each generation per prompt,
         bs_embed, seq_len, _ = text_embeddings.shape
@@ -362,21 +385,21 @@
                 uncond_tokens,
                 padding='max_length',
                 max_length=max_length,
                 truncation=True,
                 return_tensors='pt',
             )
 
-            if hasattr(self.text_encoder.config, 'use_attention_mask'
-                       ) and self.text_encoder.config.use_attention_mask:
+            if hasattr(text_encoder.config, 'use_attention_mask'
+                       ) and text_encoder.config.use_attention_mask:
                 attention_mask = uncond_input.attention_mask.to(device)
             else:
                 attention_mask = None
 
-            uncond_embeddings = self.text_encoder(
+            uncond_embeddings = text_encoder(
                 uncond_input.input_ids.to(device),
                 attention_mask=attention_mask,
             )
             uncond_embeddings = uncond_embeddings[0]
 
             # duplicate unconditional embeddings for
             # each generation per prompt, using mps friendly method
@@ -566,15 +589,14 @@
         data = self.data_preprocessor(data)
         inputs, data_samples = data['inputs'], data['data_samples']
 
         vae = self.vae.module if hasattr(self.vae, 'module') else self.vae
 
         optim_wrapper = optim_wrapper_dict['unet']
         with optim_wrapper.optim_context(self.unet):
-            # image = inputs['img']  # image for new concept
             image = inputs
             prompt = data_samples.prompt
             num_batches = image.shape[0]
 
             image = image.to(self.dtype)
             latents = vae.encode(image).latent_dist.sample()
             latents = latents * vae.config.scaling_factor
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/stable_diffusion/vae.py` & `mmagic-1.0.1/mmagic/models/editors/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan1/__init__.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan1/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan1/stylegan1.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan1/stylegan1.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 @MODELS.register_module('StyleGANv1')
 @MODELS.register_module()
 class StyleGAN1(ProgressiveGrowingGAN):
     """Implementation of `A Style-Based Generator Architecture for Generative
     Adversarial Networks`.
 
     <https://openaccess.thecvf.com/content_CVPR_2019/html/Karras_A_Style-Based_Generator_Architecture_for_Generative_Adversarial_Networks_CVPR_2019_paper.html>`_  # noqa
-    (StyleGANv1). This class is inheriant from
+    (StyleGANv1). This class is inherited from
     :class:`~ProgressiveGrowingGAN` to support progressive training.
 
     Detailed architecture can be found in
     :class:`~mmagic.models.editors.stylegan1.StyleGAN1Generator`
     and
     :class:`~mmagic.models.editors.stylegan1.StyleGAN1Discriminator`
 
@@ -68,15 +68,15 @@
         if isinstance(generator, dict):
             model_style_channels = generator.get('style_channels', None)
         else:
             model_style_channels = getattr(generator, 'style_channels', None)
 
         if style_channels is not None and model_style_channels is not None:
             assert style_channels == model_style_channels, (
-                'Input \'style_channels\' is unconsistency with '
+                'Input \'style_channels\' is inconsistent with '
                 f'\'generator.style_channels\'. Receive \'{style_channels}\' '
                 f'and \'{model_style_channels}\'.')
         else:
             style_channels = style_channels or model_style_channels
 
         super().__init__(generator, discriminator, data_preprocessor,
                          nkimgs_per_scale, None, interp_real, transition_kimgs,
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan1/stylegan1_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan1/stylegan1_discriminator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan1/stylegan1_generator.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan1/stylegan1_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         style_channels (int): The number of channels for style code.
         num_mlps (int, optional): The number of MLP layers. Defaults to 8.
         blur_kernel (list, optional): The blurry kernel. Defaults
             to [1, 2, 1].
         lr_mlp (float, optional): The learning rate for the style mapping
             layer. Defaults to 0.01.
         default_style_mode (str, optional): The default mode of style mixing.
-            In training, we defaultly adopt mixing style mode. However, in the
+            In training, we adopt mixing style mode in default. However, in the
             evaluation, we use 'single' style mode. `['mix', 'single']` are
             currently supported. Defaults to 'mix'.
         eval_style_mode (str, optional): The evaluation mode of style mixing.
             Defaults to 'single'.
         mix_prob (float, optional): Mixing probability. The value should be
             in range of [0, 1]. Defaults to 0.9.
     """
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan1/stylegan1_modules.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan1/stylegan1_modules.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan1/stylegan_utils.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan1/stylegan_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan2/__init__.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan2/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan2/ada/augment.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan2/ada/augment.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan2/ada/grid_sample_gradfix.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan2/ada/grid_sample_gradfix.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan2/ada/misc.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan2/ada/misc.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan2/ada/upfirdn2d.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan2/ada/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan2/stylegan2.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan2/stylegan2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ...utils import set_requires_grad
 
 ModelType = Union[Dict, nn.Module]
 
 
 @MODELS.register_module()
 class StyleGAN2(BaseGAN):
-    """Impelmentation of `Analyzing and Improving the Image Quality of
+    """Implementation of `Analyzing and Improving the Image Quality of
     Stylegan`. # noqa.
 
     Paper link: https://openaccess.thecvf.com/content_CVPR_2020/html/Karras_Analyzing_and_Improving_the_Image_Quality_of_StyleGAN_CVPR_2020_paper.html. # noqa
 
     :class:`~mmagic.models.editors.stylegan2.StyleGAN2Generator`
     and
     :class:`~mmagic.models.editors.stylegan2.StyleGAN2Discriminator`
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan2/stylegan2_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan2/stylegan2_discriminator.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             fp32 if not `fp16_enabled`. This argument is designed to deal with
             the cases where some modules are run in FP16 and others in FP32.
             Defaults to True.
         input_bgr2rgb (bool, optional): Whether to reformat the input channels
             with order `rgb`. Since we provide several converted weights,
             whose input order is `rgb`. You can set this argument to True if
             you want to finetune on converted weights. Defaults to False.
-        pretrained (dict | None, optional): Information for pretained models.
+        pretrained (dict | None, optional): Information for pretrained models.
             The necessary key is 'ckpt_path'. Besides, you can also provide
             'prefix' to load the generator part from the whole state dict.
             Defaults to None.
     """
 
     def __init__(self,
                  in_size,
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan2/stylegan2_generator.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan2/stylegan2_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         channel_multiplier (int, optional): The multiplier factor for the
             channel number. Defaults to 2.
         blur_kernel (list, optional): The blurry kernel. Defaults
             to [1, 3, 3, 1].
         lr_mlp (float, optional): The learning rate for the style mapping
             layer. Defaults to 0.01.
         default_style_mode (str, optional): The default mode of style mixing.
-            In training, we defaultly adopt mixing style mode. However, in the
+            In training, we adopt mixing style mode in default. However, in the
             evaluation, we use 'single' style mode. `['mix', 'single']` are
             currently supported. Defaults to 'mix'.
         eval_style_mode (str, optional): The evaluation mode of style mixing.
             Defaults to 'single'.
         mix_prob (float, optional): Mixing probability. The value should be
             in range of [0, 1]. Defaults to ``0.9``.
         update_mean_latent_with_ema (bool, optional): Whether update mean
@@ -89,15 +89,15 @@
             fp16 training. Different from ``fp16_enabled``, this argument
             allows users to adopt FP16 training only in several blocks.
             This behaviour is much more similar to the official implementation
             by Tero. Defaults to 0.
         fp16_enabled (bool, optional): Whether to use fp16 training in this
             module. If this flag is `True`, the whole module will be wrapped
             with ``auto_fp16``. Defaults to False.
-        pretrained (dict | None, optional): Information for pretained models.
+        pretrained (dict | None, optional): Information for pretrained models.
             The necessary key is 'ckpt_path'. Besides, you can also provide
             'prefix' to load the generator part from the whole state dict.
             Defaults to None.
     """
 
     def __init__(self,
                  out_size,
@@ -205,15 +205,15 @@
 
         blk_in_channels_ = self.channels[4]  # in channels of the conv blocks
 
         for i in range(3, self.log_size + 1):
             blk_out_channels_ = self.channels[2**i]
 
             # If `fp16_enabled` is True, all of layers will be run in auto
-            # FP16. In the case of `num_fp16_sacles` > 0, only partial
+            # FP16. In the case of `num_fp16_scales` > 0, only partial
             # layers will be run in fp16.
             _use_fp16 = (self.log_size - i) < num_fp16_scales or fp16_enabled
 
             self.convs.append(
                 ModulatedStyleConv(
                     blk_in_channels_,
                     blk_out_channels_,
@@ -382,15 +382,15 @@
                 random noise will be fixed as this input injected noise.
                 Defaults to None.
             add_noise (bool): Whether apply noise injection. Defaults to True.
             randomize_noise (bool, optional): If `False`, images are sampled
                 with the buffered noise tensor injected to the style conv
                 block. Defaults to True.
             update_ws (bool): Whether update latent code with EMA. Only work
-                when `w_avg` is registeried. Defaults to False.
+                when `w_avg` is registered. Defaults to False.
 
         Returns:
             torch.Tensor | dict: Generated image tensor or dictionary \
                 containing more data.
         """
         input_dim = self.style_channels if input_is_latent else self.noise_size
         # receive noise and conduct sanity check.
@@ -432,17 +432,17 @@
             if self.cond_size is not None and self.cond_size > 0:
                 assert label is not None, (
                     '\'cond_channels\' is not None, \'cond\' must be passed.')
                 assert label.shape[1] == self.cond_size
                 embedding = self.embed(label)
                 # NOTE: If conditional input is passed, do norm for cond
                 # embedding and noise input respectively
-                # do pixel_norm (2nd_momuent_norm) to cond embedding
+                # do pixel_norm (2nd_moment_norm) to cond embedding
                 embedding = self.pixel_norm(embedding)
-                # do pixel_norm (2nd_momuent_norm) to noise input
+                # do pixel_norm (2nd_moment_norm) to noise input
                 styles = [self.pixel_norm(s) for s in styles]
 
             styles_list = []
             for s in styles:
                 if self.cond_size is not None and self.cond_size > 0:
                     s = torch.cat([s, embedding], dim=1)
                 styles_list.append(self.style_mapping(s))
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan2/stylegan2_modules.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan2/stylegan2_modules.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan3/stylegan3.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan3/stylegan3.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                               apply_integer_translation, rotation_matrix)
 
 ModelType = Union[Dict, nn.Module]
 
 
 @MODELS.register_module()
 class StyleGAN3(StyleGAN2):
-    """Impelmentation of `Alias-Free Generative Adversarial Networks`. # noqa.
+    """Implementation of `Alias-Free Generative Adversarial Networks`. # noqa.
 
     Paper link: https://nvlabs-fi-cdn.nvidia.com/stylegan3/stylegan3-paper.pdf # noqa
 
     Detailed architecture can be found in
 
     :class:`~mmagic.models.editors.stylegan3.StyleGAN3Generator`
     and
@@ -56,15 +56,15 @@
         self.forward_kwargs = forward_kwargs
 
     def test_step(self, data: dict) -> SampleList:
         """Gets the generated image of given data. Same as :meth:`val_step`.
 
         Args:
             data (dict): Data sampled from metric specific
-                sampler. More detials in `Metrics` and `Evaluator`.
+                sampler. More details in `Metrics` and `Evaluator`.
 
         Returns:
             SampleList: A list of ``DataSample`` contain generated results.
         """
         data = self.data_preprocessor(data)
         inputs_dict, data_samples = data['inputs'], data['data_samples']
         # hard code to compute equivarience
@@ -80,15 +80,15 @@
         return outputs
 
     def val_step(self, data: dict) -> SampleList:
         """Gets the generated image of given data. Same as :meth:`val_step`.
 
         Args:
             data (dict): Data sampled from metric specific
-                sampler. More detials in `Metrics` and `Evaluator`.
+                sampler. More details in `Metrics` and `Evaluator`.
 
         Returns:
             SampleList: A list of ``DataSample`` contain generated results.
         """
         data = self.data_preprocessor(data)
         inputs_dict, data_samples = data['inputs'], data['data_samples']
         # hard code to compute equivarience
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan3/stylegan3_generator.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan3/stylegan3_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 @MODELS.register_module('StyleGANv3Generator')
 @MODELS.register_module()
 class StyleGAN3Generator(nn.Module):
     """StyleGAN3 Generator.
 
     In StyleGAN3, we make several changes to StyleGANv2's generator which
-    include transformed fourier features, filtered nonlinearities and
+    include transformed fourier features, filtered nonlinearity and
     non-critical sampling, etc. More details can be found in: Alias-Free
     Generative Adversarial Networks NeurIPS'2021.
 
     Ref: https://github.com/NVlabs/stylegan3
 
     Args:
         out_size (int): The output size of the StyleGAN3 generator.
@@ -30,15 +30,15 @@
         noise_size (int, optional): Size of the input noise vector.
             Defaults to 512.
         rgb2bgr (bool, optional): Whether to reformat the output channels
                 with order `bgr`. We provide several pre-trained StyleGAN3
                 weights whose output channels order is `rgb`. You can set
                 this argument to True to use the weights.
         pretrained (str | dict, optional): Path for the pretrained model or
-            dict containing information for pretained models whose necessary
+            dict containing information for pretrained models whose necessary
             key is 'ckpt_path'. Besides, you can also provide 'prefix' to load
             the generator part from the whole state dict. Defaults to None.
         synthesis_cfg (dict, optional): Config for synthesis network. Defaults
             to dict(type='SynthesisNetwork').
         mapping_cfg (dict, optional): Config for mapping network. Defaults to
             dict(type='MappingNetwork').
     """
@@ -178,15 +178,15 @@
         """
         if hasattr(self.style_mapping, 'w_avg'):
             return self.style_mapping.w_avg
         return get_mean_latent(self, num_samples, **kwargs)
 
     def get_training_kwargs(self, phase):
         """Get training kwargs. In StyleGANv3, we enable fp16, and update
-        mangitude ema during training of discriminator. This function is used
+        magnitude ema during training of discriminator. This function is used
         to pass related arguments.
 
         Args:
             phase (str): Current training phase.
 
         Returns:
             dict: Training kwargs.
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan3/stylegan3_modules.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan3/stylegan3_modules.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/stylegan3/stylegan3_utils.py` & `mmagic-1.0.1/mmagic/models/editors/stylegan3/stylegan3_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/swinir/swinir_modules.py` & `mmagic-1.0.1/mmagic/models/editors/swinir/swinir_modules.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/swinir/swinir_net.py` & `mmagic-1.0.1/mmagic/models/editors/swinir/swinir_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/swinir/swinir_rstb.py` & `mmagic-1.0.1/mmagic/models/editors/swinir/swinir_rstb.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/swinir/swinir_utils.py` & `mmagic-1.0.1/mmagic/models/editors/swinir/swinir_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/tdan/tdan.py` & `mmagic-1.0.1/mmagic/models/editors/tdan/tdan.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/tdan/tdan_net.py` & `mmagic-1.0.1/mmagic/models/editors/tdan/tdan_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/tof/tof_vfi_net.py` & `mmagic-1.0.1/mmagic/models/editors/tof/tof_vfi_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/tof/tof_vsr_net.py` & `mmagic-1.0.1/mmagic/models/editors/tof/tof_vsr_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/ttsr/lte.py` & `mmagic-1.0.1/mmagic/models/editors/ttsr/lte.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class LTE(BaseModule):
     """Learnable Texture Extractor.
 
     Based on pretrained VGG19. Generate features in 3 levels.
 
     Args:
         requires_grad (bool): Require grad or not. Default: True.
-        pixel_range (float): Pixel range of geature. Default: 1.
+        pixel_range (float): Pixel range of feature. Default: 1.
         load_pretrained_vgg (bool): Load pretrained VGG from torchvision.
             Default: True.
             Train: must load pretrained VGG.
             Eval: needn't load pretrained VGG, because we will load pretrained
             LTE.
     """
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/ttsr/search_transformer.py` & `mmagic-1.0.1/mmagic/models/editors/ttsr/search_transformer.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/ttsr/ttsr.py` & `mmagic-1.0.1/mmagic/models/editors/ttsr/ttsr.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/ttsr/ttsr_disc.py` & `mmagic-1.0.1/mmagic/models/editors/ttsr/ttsr_disc.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/ttsr/ttsr_net.py` & `mmagic-1.0.1/mmagic/models/editors/ttsr/ttsr_net.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/wgan_gp/wgan_discriminator.py` & `mmagic-1.0.1/mmagic/models/editors/wgan_gp/wgan_discriminator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/wgan_gp/wgan_generator.py` & `mmagic-1.0.1/mmagic/models/editors/wgan_gp/wgan_generator.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/editors/wgan_gp/wgan_gp.py` & `mmagic-1.0.1/mmagic/models/editors/wgan_gp/wgan_gp.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from mmagic.models.losses import gradient_penalty_loss
 from mmagic.registry import MODELS
 from mmagic.structures import DataSample
 
 
 @MODELS.register_module()
 class WGANGP(BaseGAN):
-    """Impelmentation of `Improved Training of Wasserstein GANs`.
+    """Implementation of `Improved Training of Wasserstein GANs`.
 
     Paper link: https://arxiv.org/pdf/1704.00028
 
     Detailed architecture can be found in
     :class:`~mmagic.models.editors.wgan_gp.WGANGPGenerator`
     and
     :class:`~mmagic.models.editors.wgan_gp.WGANGPDiscriminator`
```

### Comparing `mmagic-1.0.0/mmagic/models/editors/wgan_gp/wgan_gp_module.py` & `mmagic-1.0.1/mmagic/models/editors/wgan_gp/wgan_gp_module.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/__init__.py` & `mmagic-1.0.1/mmagic/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/clip_loss.py` & `mmagic-1.0.1/mmagic/models/losses/clip_loss.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/composition_loss.py` & `mmagic-1.0.1/mmagic/models/losses/composition_loss.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/face_id_loss.py` & `mmagic-1.0.1/mmagic/models/losses/face_id_loss.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/feature_loss.py` & `mmagic-1.0.1/mmagic/models/losses/feature_loss.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/gan_loss.py` & `mmagic-1.0.1/mmagic/models/losses/gan_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,15 +498,15 @@
                          weight: float = 1.,
                          pl_batch_size: Optional[int] = None,
                          sync_mean_buffer: bool = False,
                          loss_scaler: Optional[GradScaler] = None,
                          use_apex_amp: bool = False) -> Tuple[torch.Tensor]:
     """Generator Path Regularization.
 
-    Path regularization is proposed in StyelGAN2, which can help the improve
+    Path regularization is proposed in StyleGAN2, which can help the improve
     the continuity of the latent space. More details can be found in:
     Analyzing and Improving the Image Quality of StyleGAN, CVPR2020.
 
     Args:
         generator (nn.Module): The generator module. Note that this loss
             requires that the generator contains ``return_latents`` interface,
             with which we can get the latent code of the current sample.
@@ -516,15 +516,15 @@
         pl_batch_shrink (int, optional): The factor of shrinking the batch size
             for saving GPU memory. Defaults to 1.
         decay (float, optional): Decay for moving average of mean path length.
             Defaults to 0.01.
         weight (float, optional): Weight of this loss item. Defaults to ``1.``.
         pl_batch_size (int | None, optional): The batch size in calculating
             generator path. Once this argument is set, the ``num_batches`` will
-            be overridden with this argument and won't be affectted by
+            be overridden with this argument and won't be affected by
             ``pl_batch_shrink``. Defaults to None.
         sync_mean_buffer (bool, optional): Whether to sync mean path length
             across all of GPUs. Defaults to False.
 
     Returns:
         tuple[Tensor]: The penalty loss, detached mean path tensor, and \
             current path length.
@@ -550,15 +550,15 @@
             outputs=loss,
             inputs=latents,
             grad_outputs=torch.ones(()).to(loss),
             create_graph=True,
             retain_graph=True,
             only_inputs=True)[0]
 
-        # unsacle the grad
+        # unscale the grad
         inv_scale = 1. / loss_scaler.get_scale()
         grad = grad * inv_scale
     elif use_apex_amp:
         from apex.amp._amp_state import _amp_state
 
         # by default, we use loss_scalers[0] for discriminator and
         # loss_scalers[1] for generator
@@ -569,15 +569,15 @@
             outputs=loss,
             inputs=latents,
             grad_outputs=torch.ones(()).to(loss),
             create_graph=True,
             retain_graph=True,
             only_inputs=True)[0]
 
-        # unsacle the grad
+        # unscale the grad
         inv_scale = 1. / _loss_scaler.loss_scale()
         grad = grad * inv_scale
     else:
         grad = autograd.grad(
             outputs=(fake_img * noise).sum(),
             inputs=latents,
             grad_outputs=torch.ones(()).to(fake_img),
```

### Comparing `mmagic-1.0.0/mmagic/models/losses/gradient_loss.py` & `mmagic-1.0.1/mmagic/models/losses/gradient_loss.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/loss_comps/__init__.py` & `mmagic-1.0.1/mmagic/models/losses/loss_comps/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/loss_comps/clip_loss_comps.py` & `mmagic-1.0.1/mmagic/models/losses/loss_comps/clip_loss_comps.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/loss_comps/disc_auxiliary_loss_comps.py` & `mmagic-1.0.1/mmagic/models/losses/loss_comps/disc_auxiliary_loss_comps.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/loss_comps/face_id_loss_comps.py` & `mmagic-1.0.1/mmagic/models/losses/loss_comps/face_id_loss_comps.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/loss_comps/gan_loss_comps.py` & `mmagic-1.0.1/mmagic/models/losses/loss_comps/gan_loss_comps.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/loss_comps/gen_auxiliary_loss_comps.py` & `mmagic-1.0.1/mmagic/models/losses/loss_comps/gen_auxiliary_loss_comps.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..gan_loss import gen_path_regularizer
 
 
 @MODELS.register_module()
 class GeneratorPathRegularizerComps(nn.Module):
     """Generator Path Regularizer.
 
-    Path regularization is proposed in StyelGAN2, which can help the improve
+    Path regularization is proposed in StyleGAN2, which can help the improve
     the continuity of the latent space. More details can be found in:
     Analyzing and Improving the Image Quality of StyleGAN, CVPR2020.
 
     Users can achieve lazy regularization by setting ``interval`` arguments
     here.
 
     **Note for the design of ``data_info``:**
@@ -56,15 +56,15 @@
             Defaults to ``1.``.
         pl_batch_shrink (int, optional): The factor of shrinking the batch size
             for saving GPU memory. Defaults to 1.
         decay (float, optional): Decay for moving average of mean path length.
             Defaults to 0.01.
         pl_batch_size (int | None, optional): The batch size in calculating
             generator path. Once this argument is set, the ``num_batches`` will
-            be overridden with this argument and won't be affectted by
+            be overridden with this argument and won't be affected by
             ``pl_batch_shrink``. Defaults to None.
         sync_mean_buffer (bool, optional): Whether to sync mean path length
             across all of GPUs. Defaults to False.
         interval (int, optional): The interval of calculating this loss. This
             argument is used to support lazy regularization. Defaults to 1.
         data_info (dict, optional): Dictionary contains the mapping between
             loss input args and data dictionary. If ``None``, this module will
```

### Comparing `mmagic-1.0.0/mmagic/models/losses/loss_wrapper.py` & `mmagic-1.0.1/mmagic/models/losses/loss_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/perceptual_loss.py` & `mmagic-1.0.1/mmagic/models/losses/perceptual_loss.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/losses/pixelwise_loss.py` & `mmagic-1.0.1/mmagic/models/losses/pixelwise_loss.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/utils/__init__.py` & `mmagic-1.0.1/mmagic/models/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
 from .bbox_utils import extract_around_bbox, extract_bbox_patch
 from .flow_warp import flow_warp
 from .model_utils import (build_module, default_init_weights,
                           generation_init_weights, get_module_device,
                           get_valid_noise_size, get_valid_num_batches,
-                          make_layer, set_requires_grad, set_xformers,
-                          xformers_is_enable)
+                          make_layer, remove_tomesd, set_requires_grad,
+                          set_tomesd, set_xformers, xformers_is_enable)
 from .sampling_utils import label_sample_fn, noise_sample_fn
 from .tensor_utils import get_unknown_tensor, normalize_vecs
 
 __all__ = [
     'default_init_weights', 'make_layer', 'flow_warp',
     'generation_init_weights', 'set_requires_grad', 'extract_bbox_patch',
     'extract_around_bbox', 'get_unknown_tensor', 'noise_sample_fn',
     'label_sample_fn', 'get_valid_num_batches', 'get_valid_noise_size',
     'get_module_device', 'normalize_vecs', 'build_module', 'set_xformers',
-    'xformers_is_enable'
+    'xformers_is_enable', 'set_tomesd', 'remove_tomesd'
 ]
```

### Comparing `mmagic-1.0.0/mmagic/models/utils/bbox_utils.py` & `mmagic-1.0.1/mmagic/models/utils/bbox_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/utils/diffusion_utils.py` & `mmagic-1.0.1/mmagic/models/utils/diffusion_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import math
 
 import numpy as np
 
 
 def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999):
-    """Create a beta schedule that discretizes the given alpha_t_bar
+    """Create a beta schedule that discretized the given alpha_t_bar
     function, which defines the cumulative product of
     (1-beta) over time from t = [0,1].
 
     Source: https://github.com/huggingface/diffusers/blob/main/src/diffusers/schedulers/scheduling_ddim.py#L49 # noqa
     """
 
     def alpha_bar(time_step):
```

### Comparing `mmagic-1.0.0/mmagic/models/utils/flow_warp.py` & `mmagic-1.0.1/mmagic/models/utils/flow_warp.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/utils/model_utils.py` & `mmagic-1.0.1/mmagic/models/utils/model_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from mmengine.registry import Registry
 from mmengine.utils.dl_utils.parrots_wrapper import _BatchNorm
 from torch import Tensor
 from torch.nn import init
 
 from mmagic.structures import DataSample
 from mmagic.utils.typing import ForwardInputs
+from .tome_utils import (add_tome_cfg_hook, build_mmagic_tomesd_block,
+                         build_mmagic_wrapper_tomesd_block, isinstance_str)
 
 
 def default_init_weights(module, scale=1):
     """Initialize network weights.
 
     Args:
         modules (nn.Module): Modules to be initialized.
@@ -152,15 +154,15 @@
         model_noise_size = generator.get('noise_size', None)
     else:
         model_noise_size = getattr(generator, 'noise_size', None)
 
     # get noise_size
     if noise_size is not None and model_noise_size is not None:
         assert noise_size == model_noise_size, (
-            'Input \'noise_size\' is unconsistency with '
+            'Input \'noise_size\' is inconsistent with '
             f'\'generator.noise_size\'. Receive \'{noise_size}\' and '
             f'\'{model_noise_size}\'.')
     else:
         noise_size = noise_size or model_noise_size
 
     return noise_size
 
@@ -190,29 +192,29 @@
         int: The batch size of samples to generate.
     """
     # attempt to infer num_batches from batch_inputs
     if batch_inputs is not None:
         if isinstance(batch_inputs, Tensor):
             return batch_inputs.shape[0]
 
-        # get num_batces from batch_inputs
+        # get num_batches from batch_inputs
         num_batches_dict = {
             k: v.shape[0]
             for k, v in batch_inputs.items() if isinstance(v, Tensor)
         }
         if 'num_batches' in batch_inputs:
             num_batches_dict['num_batches'] = batch_inputs['num_batches']
 
         if num_batches_dict:
             num_batches_inputs = list(num_batches_dict.values())[0]
             # ensure all num_batches are same
             assert all([
                 bz == num_batches_inputs for bz in num_batches_dict.values()
             ]), ('\'num_batches\' is inconsistency among the preprocessed '
-                 f'input. \'num_batches\' parsed resutls: {num_batches_dict}')
+                 f'input. \'num_batches\' parsed results: {num_batches_dict}')
         else:
             num_batches_inputs = None
     else:
         num_batches_inputs = None
 
     # attempt to infer num_batches from data_samples
     if data_samples is not None:
@@ -278,15 +280,15 @@
         module (nn.Module): The module to set xformers.
         prefix (str): The prefix of the module name.
 
     Returns:
         nn.Module: The module with xformers' efficient Attention.
     """
 
-    if not xformers_is_enable:
+    if not xformers_is_enable():
         print_log('Do not support Xformers. Please install Xformers first. '
                   'The program will run without Xformers.')
         return
 
     for n, m in module.named_children():
         if hasattr(m, 'set_use_memory_efficient_attention_xformers'):
             # set xformers for Diffusers' Cross Attention
@@ -295,7 +297,122 @@
             print_log(
                 'Enable Xformers for HuggingFace Diffusers\' '
                 f'module \'{module_name}\'.', 'current')
         else:
             set_xformers(m, prefix=n)
 
     return module
+
+
+def set_tomesd(model: torch.nn.Module,
+               ratio: float = 0.5,
+               max_downsample: int = 1,
+               sx: int = 2,
+               sy: int = 2,
+               use_rand: bool = True,
+               merge_attn: bool = True,
+               merge_crossattn: bool = False,
+               merge_mlp: bool = False):
+    """Patches a stable diffusion model with ToMe. Apply this to the highest
+    level stable diffusion object.
+
+    Refer to: https://github.com/dbolya/tomesd/blob/main/tomesd/patch.py#L173 # noqa
+
+    Args:
+        model (torch.nn.Module): A top level Stable Diffusion module to patch in place.
+        ratio (float): The ratio of tokens to merge. I.e., 0.4 would reduce the total
+            number of tokens by 40%.The maximum value for this is 1-(1/(`sx` * `sy`)). By default,
+            the max ratio is 0.75 (usually <= 0.5 is recommended). Higher values result in more speed-up,
+            but with more visual quality loss.
+        max_downsample (int): Apply ToMe to layers with at most this amount of downsampling.
+            E.g., 1 only applies to layers with no downsampling, while 8 applies to all layers.
+            Should be chosen from [1, 2, 4, or 8]. 1 and 2 are recommended.
+        sx, sy (int, int): The stride for computing dst sets. A higher stride means you can merge
+            more tokens, default setting of (2, 2) works well in most cases.
+            `sx` and `sy` do not need to divide image size.
+        use_rand (bool): Whether or not to allow random perturbations when computing dst sets.
+            By default: True, but if you're having weird artifacts you can try turning this off.
+        merge_attn (bool): Whether or not to merge tokens for attention (recommended).
+        merge_crossattn (bool): Whether or not to merge tokens for cross attention (not recommended).
+        merge_mlp (bool): Whether or not to merge tokens for the mlp layers (particular not recommended).
+
+    Returns:
+        model (torch.nn.Module): Model patched by ToMe.
+    """
+
+    # Make sure the module is not currently patched
+    remove_tomesd(model)
+
+    is_mmagic = isinstance_str(model, 'StableDiffusion') or isinstance_str(
+        model, 'BaseModel')
+
+    if is_mmagic:
+        # Supports "StableDiffusion.unet" and "unet"
+        diffusion_model = model.unet if hasattr(model, 'unet') else model
+        if isinstance_str(diffusion_model, 'DenoisingUnet'):
+            is_wrapper = False
+        else:
+            is_wrapper = True
+    else:
+        if not hasattr(model, 'model') or not hasattr(model.model,
+                                                      'diffusion_model'):
+            # Provided model not supported
+            print('Expected a Stable Diffusion / Latent Diffusion model.')
+            raise RuntimeError('Provided model was not supported.')
+        diffusion_model = model.model.diffusion_model
+        # TODO: can support more diffusion models, like Stability AI
+        is_wrapper = None
+
+    diffusion_model._tome_info = {
+        'size': None,
+        'hooks': [],
+        'args': {
+            'ratio': ratio,
+            'max_downsample': max_downsample,
+            'sx': sx,
+            'sy': sy,
+            'use_rand': use_rand,
+            'merge_attn': merge_attn,
+            'merge_crossattn': merge_crossattn,
+            'merge_mlp': merge_mlp
+        }
+    }
+    add_tome_cfg_hook(diffusion_model)
+
+    for _, module in diffusion_model.named_modules():
+        if isinstance_str(module, 'BasicTransformerBlock'):
+            # TODO: can support more stable diffusion based models
+            if is_mmagic:
+                if is_wrapper is None:
+                    raise NotImplementedError(
+                        'Specific ToMe block not implemented')
+                elif not is_wrapper:
+                    make_tome_block_fn = build_mmagic_tomesd_block
+                elif is_wrapper:
+                    make_tome_block_fn = build_mmagic_wrapper_tomesd_block
+            else:
+                raise TypeError(
+                    'Currently `tome` only support *stable-diffusion* model!')
+            module.__class__ = make_tome_block_fn(module.__class__)
+            module._tome_info = diffusion_model._tome_info
+
+    return model
+
+
+def remove_tomesd(model: torch.nn.Module):
+    """Removes a patch from a ToMe Diffusion module if it was already patched.
+
+    Refer to: https://github.com/dbolya/tomesd/blob/main/tomesd/patch.py#L251 # noqa
+    """
+    # For mmagic Stable Diffusion models
+    model = model.unet if hasattr(model, 'unet') else model
+
+    for _, module in model.named_modules():
+        if hasattr(module, '_tome_info'):
+            for hook in module._tome_info['hooks']:
+                hook.remove()
+            module._tome_info['hooks'].clear()
+
+        if module.__class__.__name__ == 'ToMeBlock':
+            module.__class__ = module._parent
+
+    return model
```

### Comparing `mmagic-1.0.0/mmagic/models/utils/sampling_utils.py` & `mmagic-1.0.1/mmagic/models/utils/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/models/utils/tensor_utils.py` & `mmagic-1.0.1/mmagic/models/utils/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/registry.py` & `mmagic-1.0.1/mmagic/registry.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/structures/data_sample.py` & `mmagic-1.0.1/mmagic/structures/data_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     Args:
         value (torch.Tensor | numpy.ndarray | Sequence | int): Label value.
         num_classes (int, optional): The number of classes. If not None, set
             it to the metainfo. Defaults to None.
 
     Returns:
-        :obj:`mmengine.LabelData`: The foramtted label data.
+        :obj:`mmengine.LabelData`: The formatted label data.
     """
     # Handle single number
     if isinstance(value, (torch.Tensor, np.ndarray)) and value.ndim == 0:
         value = int(value.item())
 
     if isinstance(value, np.ndarray):
         value = torch.from_numpy(value)
```

### Comparing `mmagic-1.0.0/mmagic/utils/__init__.py` & `mmagic-1.0.1/mmagic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/utils/cli.py` & `mmagic-1.0.1/mmagic/utils/cli.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/utils/img_utils.py` & `mmagic-1.0.1/mmagic/utils/img_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/utils/io_utils.py` & `mmagic-1.0.1/mmagic/utils/io_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     if dest_path is None:
         filename = url.split('/')[-1]
         dest_path = os.path.join(dest_dir, filename)
 
     if dest_path.startswith('~'):
         dest_path = os.path.expanduser('~') + dest_path[1:]
 
-    # advoid downloading existed file
+    # avoid downloading existed file
     if os.path.exists(dest_path):
         return dest_path
 
     rank, ws = get_dist_info()
 
     # only download from the master process
     if rank == 0:
```

### Comparing `mmagic-1.0.0/mmagic/utils/logger.py` & `mmagic-1.0.1/mmagic/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/utils/sampler.py` & `mmagic-1.0.1/mmagic/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/utils/setup_env.py` & `mmagic-1.0.1/mmagic/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/utils/trans_utils.py` & `mmagic-1.0.1/mmagic/utils/trans_utils.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/visualization/concat_visualizer.py` & `mmagic-1.0.1/mmagic/visualization/concat_visualizer.py`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/mmagic/visualization/vis_backend.py` & `mmagic-1.0.1/mmagic/visualization/vis_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             Default to 'vis_image'.
         config_save_file (str): The file name to save config.
             Default to 'config.py'.
         scalar_save_file (str):  The file name to save scalar values.
             Default to 'scalars.json'.
         ceph_path (Optional[str]): The remote path of Ceph cloud storage.
             Defaults to None.
-        delete_local (bool): Whether eelete local after uploading to ceph or
+        delete_local (bool): Whether delete local after uploading to ceph or
             not. If ``ceph_path`` is None, this will be ignored. Defaults to
             True.
     """
 
     def __init__(self,
                  save_dir: str,
                  img_save_dir: str = 'vis_image',
```

### Comparing `mmagic-1.0.0/mmagic/visualization/visualizer.py` & `mmagic-1.0.1/mmagic/visualization/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         vis_results = []
         for sample in sample_dict.values():
             if padding_tensor is not None:
                 vis_results.append(torch.cat([sample, padding_tensor], dim=0))
             else:
                 vis_results.append(sample)
 
-        # concatnate along batch size
+        # concatenate along batch size
         vis_results = torch.cat(vis_results)
         vis_results = [
             make_grid(vis_results[:, t, ...].cpu(),
                       nrow=n_row).cpu().permute(1, 2, 0)
             for t in range(num_timesteps)
         ]
         vis_results = torch.stack(vis_results, dim=0)  # [t, H, W, 3]
@@ -176,15 +176,15 @@
             gen_samples (SampleList): List of data samples to visualize
             target_keys (Union[str, List[str], None]): Keys of the
                 visualization target in data samples.
             color_order (str): The color order of the passed images.
             target_mean (Sequence[Union[float, int]]): The target mean of the
                 visualization results.
             target_std (Sequence[Union[float, int]]): The target std of the
-                visualization resutts.
+                visualization results.
             n_rows (int, optional): Number of images in one row.
 
         Returns:
             np.ndarray: The visualization results.
         """
         if target_keys is None:
             # get all key of image tensor automatically
@@ -213,15 +213,15 @@
         vis_results = []
         for sample in sample_dict.values():
             if padding_tensor is not None:
                 vis_results.append(torch.cat([sample, padding_tensor], dim=0))
             else:
                 vis_results.append(sample)
 
-        # concatnate along batch size
+        # concatenate along batch size
         vis_results = torch.cat(vis_results, dim=0)
         vis_results = make_grid(vis_results, nrow=n_row).cpu().permute(1, 2, 0)
         vis_results = vis_results.numpy().astype(np.uint8)
         return vis_results
 
     def _get_vis_data_by_key(self, sample: DataSample, key: str) -> Tensor:
         """Get tensor in ``DataSample`` by the given key.
@@ -289,15 +289,15 @@
             n_rows (int, optional): Number of images in one row.
                 Defaults to None.
             color_order (str): The color order of the passed images. Defaults
                 to 'bgr'.
             target_mean (Sequence[Union[float, int]]): The target mean of the
                 visualization results. Defaults to 127.5.
             target_std (Sequence[Union[float, int]]): The target std of the
-                visualization resutts. Defaults to 127.5.
+                visualization results. Defaults to 127.5.
             show (bool): Whether to display the drawn image. Default to False.
             wait_time (float): The interval of show (s). Defaults to 0.
             step (int): Global step value to record. Defaults to 0.
         """
 
         # get visualize function
         if vis_mode is None:
```

### Comparing `mmagic-1.0.0/mmagic.egg-info/PKG-INFO` & `mmagic-1.0.1/mmagic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmagic
-Version: 1.0.0
+Version: 1.0.1
 Summary: OpenMMLab Multimodal Advanced, Generative, and Intelligent Creation Toolbox
 Home-page: https://github.com/open-mmlab/mmagic
 Maintainer: MMagic Contributors
 Maintainer-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div id="top" align="center">
           <img src="docs/en/_static/image/mmagic-logo.png" width="500px"/>
@@ -61,15 +61,21 @@
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
         </div>
         
         ## 🚀 What's New <a><img width="35" height="20" src="https://user-images.githubusercontent.com/12782558/212848161-5e783dd6-11e8-4fe0-bbba-39ffb77730be.png"></a>
         
-        ### New release [**MMagic v1.0.0**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.0) \[25/04/2023\]:
+        ### New release [**MMagic v1.0.1**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.1) \[26/05/2023\]:
+        
+        - Support tomesd for StableDiffusion speed-up.
+        - Support all inpainting/matting/image restoration models inferencer.
+        - Support animated drawings.
+        - Support Style-Based Global Appearance Flow for Virtual Try-On.
+        - Fix inferencer in pip-install.
         
         We are excited to announce the release of MMagic v1.0.0 that inherits from [MMEditing](https://github.com/open-mmlab/mmediting) and [MMGeneration](https://github.com/open-mmlab/mmgeneration).
         
         After iterative updates with OpenMMLab 2.0 framework and merged with MMGeneration, MMEditing has become a powerful tool that supports low-level algorithms based on both GAN and CNN. Today, MMEditing embraces Generative AI and transforms into a more advanced and comprehensive AIGC toolkit: **MMagic** (**M**ultimodal **A**dvanced, **G**enerative, and **I**ntelligent **C**reation). MMagic will provide more agile and flexible experimental support for researchers and AIGC enthusiasts, and help you on your AIGC exploration journey.
         
         We highlight the following new features.
         
@@ -380,14 +386,15 @@
                 <ul>
                   <li><a href="projects/glide/configs/README.md">GLIDE (NeurIPS'2021)</a></li>
                   <li><a href="configs/guided_diffusion/README.md">Guided Diffusion (NeurIPS'2021)</a></li>
                   <li><a href="configs/disco_diffusion/README.md">Disco-Diffusion (2022)</a></li>
                   <li><a href="configs/stable_diffusion/README.md">Stable-Diffusion (2022)</a></li>
                   <li><a href="configs/dreambooth/README.md">DreamBooth (2022)</a></li>
                   <li><a href="configs/controlnet/README.md">ControlNet (2023)</a></li>
+                  <li><a href="configs/controlnet_animation/README.md">ControlNet Animation (2023)</a></li>
                 </ul>
               </td>
               <td>
                 <ul>
                   <li><a href="configs/eg3d/README.md">EG3D (CVPR'2022)</a></li>
                 </ul>
               </td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmagic Version: 1.0.0 Summary: OpenMMLab Multimodal
+Metadata-Version: 2.1 Name: mmagic Version: 1.0.1 Summary: OpenMMLab Multimodal
 Advanced, Generative, and Intelligent Creation Toolbox Home-page: https://
 github.com/open-mmlab/mmagic Maintainer: MMagic Contributors Maintainer-email:
 openmmlab@gmail.com License: Apache License 2.0 Description:
                     [docs/en/_static/image/mmagic-logo.png]
                                         
       Multimodal Advanced, Generative, and Intelligent Creation (MMagic
                                 [em'mÃ¦dÊÉªk])
@@ -26,28 +26,31 @@
  News](https://mmagic.readthedocs.io/en/latest/changelog.html) | [ðOngoing
    Projects](https://github.com/open-mmlab/mmagic/projects) | [ð¤Reporting
  Issues](https://github.com/open-mmlab/mmagic/issues) English | [ç®ä½ä¸­æ]
                                (README_zh-CN.md)
 
 ## ð What's New [https://user-images.githubusercontent.com/12782558/
 212848161-5e783dd6-11e8-4fe0-bbba-39ffb77730be.png] ### New release [**MMagic
-v1.0.0**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.0) \[25/04/
-2023\]: We are excited to announce the release of MMagic v1.0.0 that inherits
-from [MMEditing](https://github.com/open-mmlab/mmediting) and [MMGeneration]
-(https://github.com/open-mmlab/mmgeneration). After iterative updates with
-OpenMMLab 2.0 framework and merged with MMGeneration, MMEditing has become a
-powerful tool that supports low-level algorithms based on both GAN and CNN.
-Today, MMEditing embraces Generative AI and transforms into a more advanced and
-comprehensive AIGC toolkit: **MMagic** (**M**ultimodal **A**dvanced,
-**G**enerative, and **I**ntelligent **C**reation). MMagic will provide more
-agile and flexible experimental support for researchers and AIGC enthusiasts,
-and help you on your AIGC exploration journey. We highlight the following new
-features. **1. New Models** We support 11 new models in 4 new tasks. -
-Text2Image / Diffusion - ControlNet - DreamBooth - Stable Diffusion - Disco
-Diffusion - GLIDE - Guided Diffusion - 3D-aware Generation - EG3D - Image
+v1.0.1**](https://github.com/open-mmlab/mmagic/releases/tag/v1.0.1) \[26/05/
+2023\]: - Support tomesd for StableDiffusion speed-up. - Support all
+inpainting/matting/image restoration models inferencer. - Support animated
+drawings. - Support Style-Based Global Appearance Flow for Virtual Try-On. -
+Fix inferencer in pip-install. We are excited to announce the release of MMagic
+v1.0.0 that inherits from [MMEditing](https://github.com/open-mmlab/mmediting)
+and [MMGeneration](https://github.com/open-mmlab/mmgeneration). After iterative
+updates with OpenMMLab 2.0 framework and merged with MMGeneration, MMEditing
+has become a powerful tool that supports low-level algorithms based on both GAN
+and CNN. Today, MMEditing embraces Generative AI and transforms into a more
+advanced and comprehensive AIGC toolkit: **MMagic** (**M**ultimodal
+**A**dvanced, **G**enerative, and **I**ntelligent **C**reation). MMagic will
+provide more agile and flexible experimental support for researchers and AIGC
+enthusiasts, and help you on your AIGC exploration journey. We highlight the
+following new features. **1. New Models** We support 11 new models in 4 new
+tasks. - Text2Image / Diffusion - ControlNet - DreamBooth - Stable Diffusion -
+Disco Diffusion - GLIDE - Guided Diffusion - 3D-aware Generation - EG3D - Image
 Restoration - NAFNet - Restormer - SwinIR - Image Colorization -
 InstColorization **2. Magic Diffusion Model** For the Diffusion Model, we
 provide the following "magic" : - Support image generation based on Stable
 Diffusion and Disco Diffusion. - Support Finetune methods such as Dreambooth
 and DreamBooth LoRA. - Support controllability in text-to-image generation
 using ControlNet. - Support acceleration and optimization strategies based on
 xFormers to improve training and inference efficiency. - Support video
@@ -187,14 +190,16 @@
       (ECCV'2018)        (AAAI'2020)          (2022)
     * DeepFillv2_                           * Stable-Diffusion
       (CVPR'2019)                             (2022)
     * AOT-GAN_                              * DreamBooth_
       (TVCG'2019)                             (2022)
                                             * ControlNet_
                                               (2023)
+                                            * ControlNet
+                                              Animation_(2023)
 Please refer to [model_zoo](https://mmagic.readthedocs.io/en/latest/model_zoo/
 overview.html) for more details.
                                                                 ðBack_to_top
 ## ð¤ Acknowledgement MMagic is an open source project that is contributed by
 researchers and engineers from various colleges and companies. We wish that the
 toolbox and benchmark could serve the growing research community by providing a
 flexible toolkit to reimplement existing methods and develop their own new
```

### Comparing `mmagic-1.0.0/mmagic.egg-info/SOURCES.txt` & `mmagic-1.0.1/mmagic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -276,14 +276,15 @@
 mmagic/.mim/configs/sngan_proj/sngan-proj_woReLUinplace_lr2e-4-ndisc5-1xb64_cifar10-32x32.py
 mmagic/.mim/configs/srcnn/metafile.yml
 mmagic/.mim/configs/srcnn/srcnn_x4k915_1xb16-1000k_div2k.py
 mmagic/.mim/configs/srgan_resnet/metafile.yml
 mmagic/.mim/configs/srgan_resnet/msrresnet_x4c64b16_1xb16-1000k_div2k.py
 mmagic/.mim/configs/srgan_resnet/srgan_x4c64b16_1xb16-1000k_div2k.py
 mmagic/.mim/configs/stable_diffusion/metafile.yml
+mmagic/.mim/configs/stable_diffusion/stable-diffusion_ddim_denoisingunet-tomesd_5e-1.py
 mmagic/.mim/configs/stable_diffusion/stable-diffusion_ddim_denoisingunet.py
 mmagic/.mim/configs/styleganv1/metafile.yml
 mmagic/.mim/configs/styleganv1/styleganv1_ffhq-1024x1024_8xb4-25Mimgs.py
 mmagic/.mim/configs/styleganv1/styleganv1_ffhq-256x256_8xb4-25Mimgs.py
 mmagic/.mim/configs/styleganv2/metafile.yml
 mmagic/.mim/configs/styleganv2/stylegan2_c2-PL-R1_8xb4-apex-fp16-no-scaler-800kiters_ffhq-256x256.py
 mmagic/.mim/configs/styleganv2/stylegan2_c2-PL-R1_8xb4-fp16-globalG-partialD-no-scaler-800kiters_ffhq-256x256.py
@@ -385,15 +386,14 @@
 mmagic/.mim/tools/dataset_converters/vimeo90k/preprocess_vimeo90k_dataset.py
 mmagic/.mim/tools/gui/component.py
 mmagic/.mim/tools/gui/gui.py
 mmagic/.mim/tools/gui/page_general.py
 mmagic/.mim/tools/gui/page_sr.py
 mmagic/.mim/tools/gui/utils.py
 mmagic/.mim/tools/model_converters/publish_model.py
-mmagic/.mim/tools/model_converters/pytorch2onnx.py
 mmagic/apis/__init__.py
 mmagic/apis/mmagic_inferencer.py
 mmagic/apis/inferencers/__init__.py
 mmagic/apis/inferencers/base_mmagic_inferencer.py
 mmagic/apis/inferencers/colorization_inferencer.py
 mmagic/apis/inferencers/conditional_inferencer.py
 mmagic/apis/inferencers/controlnet_animation_inferencer.py
@@ -503,14 +503,15 @@
 mmagic/models/archs/multi_layer_disc.py
 mmagic/models/archs/patch_disc.py
 mmagic/models/archs/resnet.py
 mmagic/models/archs/separable_conv_module.py
 mmagic/models/archs/simple_encoder_decoder.py
 mmagic/models/archs/smpatch_disc.py
 mmagic/models/archs/sr_backbone.py
+mmagic/models/archs/tokenizer.py
 mmagic/models/archs/upsample.py
 mmagic/models/archs/vgg.py
 mmagic/models/archs/wrapper.py
 mmagic/models/base_models/__init__.py
 mmagic/models/base_models/average_model.py
 mmagic/models/base_models/base_conditional_gan.py
 mmagic/models/base_models/base_edit_model.py
@@ -782,14 +783,15 @@
 mmagic/models/utils/__init__.py
 mmagic/models/utils/bbox_utils.py
 mmagic/models/utils/diffusion_utils.py
 mmagic/models/utils/flow_warp.py
 mmagic/models/utils/model_utils.py
 mmagic/models/utils/sampling_utils.py
 mmagic/models/utils/tensor_utils.py
+mmagic/models/utils/tome_utils.py
 mmagic/structures/__init__.py
 mmagic/structures/data_sample.py
 mmagic/utils/__init__.py
 mmagic/utils/cli.py
 mmagic/utils/collect_env.py
 mmagic/utils/img_utils.py
 mmagic/utils/io_utils.py
```

### Comparing `mmagic-1.0.0/mmagic.egg-info/requires.txt` & `mmagic-1.0.1/mmagic.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 av
+controlnet_aux
 diffusers>=0.12.0
 einops
 face-alignment
 facexlib
 lmdb
 lpips
+mediapipe
 mmcv>=2.0.0rc1
 mmengine
 numpy
 opencv-python!=4.5.5.62,!=4.5.5.64
 Pillow
 resize_right
 tensorboard
+transformers>=4.27.4
 
 [:python_version < "3.7"]
 av==8.0.3
 
 [all]
 av
+controlnet_aux
 diffusers>=0.12.0
 einops
 face-alignment
 facexlib
 lmdb
 lpips
+mediapipe
 mmcv>=2.0.0rc1
 mmengine
 numpy
 opencv-python!=4.5.5.62,!=4.5.5.64
 Pillow
 resize_right
 tensorboard
+transformers>=4.27.4
 clip
 controlnet_aux
 coverage<7.0.0
 imageio-ffmpeg==0.4.4
 interrogate
 mmdet>=3.0.0
 pytest
 transformers
 clip
-controlnet_aux
 imageio-ffmpeg==0.4.4
 mmdet>=3.0.0
 open_clip_torch
 PyQt5
-transformers
 
 [all:python_version < "3.7"]
 av==8.0.3
 
 [mim]
 mmcv>=2.0.0
 mmengine>=0.4.0
```

### Comparing `mmagic-1.0.0/setup.cfg` & `mmagic-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmagic-1.0.0/setup.py` & `mmagic-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     return extension(
         name=f'{module}.{name}',
         sources=[os.path.join(*module.split('.'), p) for p in sources],
         define_macros=define_macros,
         extra_compile_args=extra_compile_args)
 
 
-def add_mim_extention():
+def add_mim_extension():
     """Add extra files that are required to support MIM into the package.
 
     These files will be added by creating a symlink to the originals if the
     package is installed in `editable` mode (e.g. pip install -e .), or by
     copying from the originals otherwise.
     """
 
@@ -226,15 +226,15 @@
                 else:
                     warnings.warn(f'Cannot copy file {src_path}.')
             else:
                 raise ValueError(f'Invalid mode {mode}')
 
 
 if __name__ == '__main__':
-    add_mim_extention()
+    add_mim_extension()
     setup(
         name='mmagic',
         version=get_version(),
         description='OpenMMLab Multimodal Advanced, Generative, and '
         'Intelligent Creation Toolbox',
         long_description=readme(),
         long_description_content_type='text/markdown',
```

