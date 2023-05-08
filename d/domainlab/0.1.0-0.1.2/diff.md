# Comparing `tmp/domainlab-0.1.0.tar.gz` & `tmp/domainlab-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domainlab-0.1.0.tar", max compression
+gzip compressed data, was "domainlab-0.1.2.tar", max compression
```

## Comparing `domainlab-0.1.0.tar` & `domainlab-0.1.2.tar`

### file list

```diff
@@ -1,128 +1,145 @@
--rw-r--r--   0        0        0     1067 2023-02-22 15:17:12.758698 domainlab-0.1.0/LICENSE
--rw-r--r--   0        0        0       27 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/.gitignore
--rw-r--r--   0        0        0      178 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/.pylintrc
--rw-r--r--   0        0        0      632 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/__init__.py
--rw-r--r--   0        0        0        0 2023-02-12 17:14:36.932061 domainlab-0.1.0/domainlab/algos/__init__.py
--rw-r--r--   0        0        0     1139 2023-02-22 15:03:23.670904 domainlab-0.1.0/domainlab/algos/a_algo_builder.py
--rw-r--r--   0        0        0     4658 2023-02-12 15:45:54.828094 domainlab-0.1.0/domainlab/algos/builder_custom.py
--rw-r--r--   0        0        0     2624 2023-01-29 12:41:05.994218 domainlab-0.1.0/domainlab/algos/builder_dann.py
--rw-r--r--   0        0        0     1476 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/builder_deepall.py
--rw-r--r--   0        0        0     1606 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/algos/builder_dial.py
--rw-r--r--   0        0        0     2559 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/algos/builder_diva.py
--rw-r--r--   0        0        0     1965 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/builder_hduva.py
--rw-r--r--   0        0        0     3248 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/algos/builder_jigen1.py
--rw-r--r--   0        0        0     2557 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/algos/builder_matchdg.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/compos/__init__.py
--rw-r--r--   0        0        0      812 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/compos/matchdg_args.py
--rw-r--r--   0        0        0     4249 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/compos/matchdg_base.py
--rw-r--r--   0        0        0    12482 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/compos/matchdg_ctr_erm.py
--rw-r--r--   0        0        0    16067 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/compos/matchdg_match.py
--rw-r--r--   0        0        0     3961 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/compos/matchdg_utils.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/msels/__init__.py
--rw-r--r--   0        0        0      556 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/msels/a_model_sel.py
--rw-r--r--   0        0        0      981 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/msels/c_msel.py
--rw-r--r--   0        0        0     1233 2023-01-29 12:41:05.994218 domainlab-0.1.0/domainlab/algos/msels/c_msel_oracle.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/observers/__init__.py
--rw-r--r--   0        0        0      639 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/observers/a_observer.py
--rw-r--r--   0        0        0     3658 2023-01-29 12:41:05.994218 domainlab-0.1.0/domainlab/algos/observers/b_obvisitor.py
--rw-r--r--   0        0        0      494 2023-01-29 12:41:05.994218 domainlab-0.1.0/domainlab/algos/observers/c_obvisitor_cleanup.py
--rw-r--r--   0        0        0     1186 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/observers/c_obvisitor_gen.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/trainers/__init__.py
--rw-r--r--   0        0        0     1404 2023-01-29 12:41:05.994218 domainlab-0.1.0/domainlab/algos/trainers/a_trainer.py
--rw-r--r--   0        0        0      782 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/algos/trainers/args_dial.py
--rw-r--r--   0        0        0     1245 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/algos/trainers/train_basic.py
--rw-r--r--   0        0        0     2833 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/algos/trainers/train_dial.py
--rw-r--r--   0        0        0     1552 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/algos/trainers/train_matchdg.py
--rw-r--r--   0        0        0     3302 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/algos/trainers/train_visitor.py
--rw-r--r--   0        0        0     1696 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/algos/zoo_algos.py
--rw-r--r--   0        0        0     7852 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/arg_parser.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/__init__.py
--rw-r--r--   0        0        0     1474 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/a_nn_builder.py
--rw-r--r--   0        0        0     1485 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/builder_nn_alex.py
--rw-r--r--   0        0        0     1582 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/builder_nn_conv_bn_relu_2.py
--rw-r--r--   0        0        0     1505 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/builder_nn_external_from_file.py
--rw-r--r--   0        0        0      750 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/exp/exp_cuda_seed.py
--rwxr-xr-x   0        0        0     3759 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/compos/exp/exp_main.py
--rw-r--r--   0        0        0     6775 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/compos/exp/exp_utils.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/nn_zoo/__init__.py
--rw-r--r--   0        0        0      853 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/nn_zoo/net_adversarial.py
--rw-r--r--   0        0        0      739 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/nn_zoo/net_classif.py
--rw-r--r--   0        0        0     2799 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py
--rw-r--r--   0        0        0     1888 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/nn_zoo/net_gated.py
--rw-r--r--   0        0        0     1061 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/nn_zoo/nn.py
--rw-r--r--   0        0        0     2743 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/nn_zoo/nn_alex.py
--rw-r--r--   0        0        0      764 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/nn_zoo/nn_torchvision.py
--rw-r--r--   0        0        0     4637 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/pcr/p_chain_handler.py
--rw-r--r--   0        0        0      794 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/pcr/request.py
--rw-r--r--   0        0        0      617 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/utils_conv_get_flat_dim.py
--rw-r--r--   0        0        0      799 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/vae/a_model_builder.py
--rw-r--r--   0        0        0     1326 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/vae/a_vae_builder.py
--rw-r--r--   0        0        0     1886 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/vae/c_vae_adaptor_model_recon.py
--rw-r--r--   0        0        0     1343 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/vae/c_vae_builder_classif.py
--rw-r--r--   0        0        0     3441 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/vae/c_vae_recon.py
--rw-r--r--   0        0        0     2195 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py
--rw-r--r--   0        0        0     2244 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py
--rw-r--r--   0        0        0     1484 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/vae/compos/decoder_cond_prior.py
--rw-r--r--   0        0        0     1495 2023-01-23 10:37:17.607822 domainlab-0.1.0/domainlab/compos/vae/compos/decoder_losses.py
--rw-r--r--   0        0        0     3398 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/vae/compos/encoder.py
--rw-r--r--   0        0        0      671 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/vae/compos/encoder_dirichlet.py
--rw-r--r--   0        0        0     1917 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/vae/compos/encoder_domain_topic.py
--rw-r--r--   0        0        0     2111 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py
--rw-r--r--   0        0        0     2279 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py
--rw-r--r--   0        0        0     5204 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/vae/compos/encoder_xyd_parallel.py
--rw-r--r--   0        0        0     5016 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/vae/compos/encoder_xydt_elevator.py
--rw-r--r--   0        0        0     1891 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/vae/compos/encoder_zy.py
--rw-r--r--   0        0        0     1207 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/vae/utils_request_chain_builder.py
--rw-r--r--   0        0        0     3203 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/vae/zoo_vae_builders_classif.py
--rw-r--r--   0        0        0     1562 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/vae/zoo_vae_builders_classif_topic.py
--rw-r--r--   0        0        0     1594 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/compos/zoo_nn.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/dsets/__init__.py
--rw-r--r--   0        0        0     6116 2023-02-05 10:55:35.735388 domainlab-0.1.0/domainlab/dsets/a_dset_mnist_color_rgb_solo.py
--rw-r--r--   0        0        0     1314 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/dsets/dset_img_path_list.py
--rw-r--r--   0        0        0      843 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/dsets/dset_mnist_color_solo_default.py
--rw-r--r--   0        0        0     1487 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/dsets/dset_poly_domains_mnist_color_default.py
--rw-r--r--   0        0        0     5759 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/dsets/dset_subfolder.py
--rw-r--r--   0        0        0      449 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/dsets/utils_color_palette.py
--rw-r--r--   0        0        0     2278 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/dsets/utils_data.py
--rw-r--r--   0        0        0     5958 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/dsets/utils_wrapdset_patches.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/models/__init__.py
--rw-r--r--   0        0        0     1103 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/models/a_model.py
--rw-r--r--   0        0        0     5885 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/models/a_model_classif.py
--rw-r--r--   0        0        0      855 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/models/args_jigen.py
--rw-r--r--   0        0        0     2482 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/models/args_vae.py
--rw-r--r--   0        0        0     1458 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/models/model_custom.py
--rw-r--r--   0        0        0     1951 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/models/model_dann.py
--rw-r--r--   0        0        0     1209 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/models/model_deep_all.py
--rw-r--r--   0        0        0     3186 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/models/model_diva.py
--rw-r--r--   0        0        0     4867 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/models/model_hduva.py
--rw-r--r--   0        0        0     2335 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/models/model_jigen.py
--rw-r--r--   0        0        0     2091 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/models/model_vae_xyd_classif.py
--rw-r--r--   0        0        0     1256 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/models/wrapper_matchdg.py
--rw-r--r--   0        0        0       58 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/tasks/__init__.py
--rw-r--r--   0        0        0     5628 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/tasks/a_task_classif.py
--rw-r--r--   0        0        0     4815 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/tasks/b_task.py
--rw-r--r--   0        0        0     4035 2023-01-26 17:13:55.056713 domainlab-0.1.0/domainlab/tasks/task_folder.py
--rw-r--r--   0        0        0     2748 2023-01-26 17:13:55.056713 domainlab-0.1.0/domainlab/tasks/task_folder_mk.py
--rw-r--r--   0        0        0     2327 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/tasks/task_mnist_color.py
--rw-r--r--   0        0        0     4299 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/tasks/task_pathlist.py
--rw-r--r--   0        0        0      897 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/tasks/task_utils.py
--rw-r--r--   0        0        0     8668 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/tasks/utils_task.py
--rw-r--r--   0        0        0      690 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/tasks/utils_task_dset.py
--rw-r--r--   0        0        0     3733 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/tasks/zoo_tasks.py
--rw-r--r--   0        0        0     1840 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/uml/libDG.uml
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/__init__.py
--rw-r--r--   0        0        0     4713 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/flows_gen_img_model.py
--rw-r--r--   0        0        0     1057 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/get_git_tag.py
--rw-r--r--   0        0        0      801 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/override_interface.py
--rw-r--r--   0        0        0     2201 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/perf.py
--rw-r--r--   0        0        0     3848 2023-02-22 15:03:23.674904 domainlab-0.1.0/domainlab/utils/perf_metrics.py
--rw-r--r--   0        0        0      899 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/test_img.py
--rw-r--r--   0        0        0      336 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/u_import.py
--rw-r--r--   0        0        0     1949 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/u_import_net_module.py
--rw-r--r--   0        0        0      901 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/utils_class.py
--rw-r--r--   0        0        0     1303 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/utils_classif.py
--rw-r--r--   0        0        0      250 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/utils_cuda.py
--rw-r--r--   0        0        0     1098 2023-01-23 10:37:17.611822 domainlab-0.1.0/domainlab/utils/utils_img_sav.py
--rw-r--r--   0        0        0      655 2023-02-22 15:03:23.678904 domainlab-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1268 1970-01-01 00:00:00.000000 domainlab-0.1.0/setup.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 domainlab-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-03-26 11:30:13.727342 domainlab-0.1.2/LICENSE
+-rw-r--r--   0        0        0       27 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/.gitignore
+-rw-r--r--   0        0        0      178 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/.pylintrc
+-rw-r--r--   0        0        0      730 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-12 17:14:36.932061 domainlab-0.1.2/domainlab/algos/__init__.py
+-rw-r--r--   0        0        0     1139 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/a_algo_builder.py
+-rw-r--r--   0        0        0     4689 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_custom.py
+-rw-r--r--   0        0        0     2955 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_dann.py
+-rw-r--r--   0        0        0     1612 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_deepall.py
+-rw-r--r--   0        0        0     1547 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_deepall_mldg.py
+-rw-r--r--   0        0        0     1633 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_dial.py
+-rw-r--r--   0        0        0     2304 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_diva.py
+-rw-r--r--   0        0        0     2095 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_hduva.py
+-rw-r--r--   0        0        0     3275 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_jigen1.py
+-rw-r--r--   0        0        0     3212 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_match_hduva.py
+-rw-r--r--   0        0        0     2814 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_matchdg.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/compos/__init__.py
+-rw-r--r--   0        0        0      621 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/compos/matchdg_args.py
+-rw-r--r--   0        0        0     3905 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/compos/matchdg_base.py
+-rw-r--r--   0        0        0    12409 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/compos/matchdg_ctr_erm.py
+-rw-r--r--   0        0        0    16853 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/compos/matchdg_match.py
+-rw-r--r--   0        0        0     3961 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/compos/matchdg_utils.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/msels/__init__.py
+-rw-r--r--   0        0        0      602 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/msels/a_model_sel.py
+-rw-r--r--   0        0        0     1092 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/msels/c_msel.py
+-rw-r--r--   0        0        0     1233 2023-01-29 12:41:05.994218 domainlab-0.1.2/domainlab/algos/msels/c_msel_oracle.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/observers/__init__.py
+-rw-r--r--   0        0        0      647 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/observers/a_observer.py
+-rw-r--r--   0        0        0     4562 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/observers/b_obvisitor.py
+-rw-r--r--   0        0        0      501 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/observers/c_obvisitor_cleanup.py
+-rw-r--r--   0        0        0     1186 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/observers/c_obvisitor_gen.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/trainers/__init__.py
+-rw-r--r--   0        0        0     3286 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/trainers/a_trainer.py
+-rw-r--r--   0        0        0      782 2023-02-23 11:55:38.957077 domainlab-0.1.2/domainlab/algos/trainers/args_dial.py
+-rw-r--r--   0        0        0     1775 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/trainers/train_basic.py
+-rw-r--r--   0        0        0     2833 2023-02-23 11:55:38.957077 domainlab-0.1.2/domainlab/algos/trainers/train_dial.py
+-rw-r--r--   0        0        0     1741 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/trainers/train_matchdg.py
+-rw-r--r--   0        0        0     3661 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/trainers/train_mldg.py
+-rw-r--r--   0        0        0     3302 2023-02-23 11:55:38.957077 domainlab-0.1.2/domainlab/algos/trainers/train_visitor.py
+-rw-r--r--   0        0        0     1608 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/algos/trainers/zoo_trainer.py
+-rw-r--r--   0        0        0     1945 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/algos/zoo_algos.py
+-rw-r--r--   0        0        0     9237 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/arg_parser.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/__init__.py
+-rw-r--r--   0        0        0     1474 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/a_nn_builder.py
+-rw-r--r--   0        0        0     1485 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/builder_nn_alex.py
+-rw-r--r--   0        0        0     1582 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/builder_nn_conv_bn_relu_2.py
+-rw-r--r--   0        0        0     1505 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/builder_nn_external_from_file.py
+-rw-r--r--   0        0        0      750 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/exp/exp_cuda_seed.py
+-rwxr-xr-x   0        0        0     2396 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/compos/exp/exp_main.py
+-rw-r--r--   0        0        0     8124 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/compos/exp/exp_utils.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/__init__.py
+-rw-r--r--   0        0        0      853 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/net_adversarial.py
+-rw-r--r--   0        0        0      739 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/net_classif.py
+-rw-r--r--   0        0        0     2799 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py
+-rw-r--r--   0        0        0     1888 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/net_gated.py
+-rw-r--r--   0        0        0     1061 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/nn.py
+-rw-r--r--   0        0        0     2743 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/nn_alex.py
+-rw-r--r--   0        0        0      764 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/nn_torchvision.py
+-rw-r--r--   0        0        0     4637 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/pcr/p_chain_handler.py
+-rw-r--r--   0        0        0      794 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/pcr/request.py
+-rw-r--r--   0        0        0      617 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/utils_conv_get_flat_dim.py
+-rw-r--r--   0        0        0      799 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/a_model_builder.py
+-rw-r--r--   0        0        0     1326 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/a_vae_builder.py
+-rw-r--r--   0        0        0     1886 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/c_vae_adaptor_model_recon.py
+-rw-r--r--   0        0        0     1343 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/c_vae_builder_classif.py
+-rw-r--r--   0        0        0     3441 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/c_vae_recon.py
+-rw-r--r--   0        0        0     2195 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py
+-rw-r--r--   0        0        0     2244 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py
+-rw-r--r--   0        0        0     1484 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/compos/decoder_cond_prior.py
+-rw-r--r--   0        0        0     1598 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/compos/vae/compos/decoder_losses.py
+-rw-r--r--   0        0        0     3398 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder.py
+-rw-r--r--   0        0        0      671 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_dirichlet.py
+-rw-r--r--   0        0        0     1917 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic.py
+-rw-r--r--   0        0        0     2111 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py
+-rw-r--r--   0        0        0     2279 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py
+-rw-r--r--   0        0        0     5204 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_xyd_parallel.py
+-rw-r--r--   0        0        0     5016 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_xydt_elevator.py
+-rw-r--r--   0        0        0     1891 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_zy.py
+-rw-r--r--   0        0        0     1207 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/utils_request_chain_builder.py
+-rw-r--r--   0        0        0     3203 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/zoo_vae_builders_classif.py
+-rw-r--r--   0        0        0     1562 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/zoo_vae_builders_classif_topic.py
+-rw-r--r--   0        0        0     1581 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/compos/zoo_nn.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/dsets/__init__.py
+-rw-r--r--   0        0        0     6116 2023-02-05 10:55:35.735388 domainlab-0.1.2/domainlab/dsets/a_dset_mnist_color_rgb_solo.py
+-rw-r--r--   0        0        0     1314 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/dsets/dset_img_path_list.py
+-rw-r--r--   0        0        0      843 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/dsets/dset_mnist_color_solo_default.py
+-rw-r--r--   0        0        0     1487 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/dsets/dset_poly_domains_mnist_color_default.py
+-rw-r--r--   0        0        0     5759 2023-02-23 11:55:38.957077 domainlab-0.1.2/domainlab/dsets/dset_subfolder.py
+-rw-r--r--   0        0        0      449 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/dsets/utils_color_palette.py
+-rw-r--r--   0        0        0     2278 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/dsets/utils_data.py
+-rw-r--r--   0        0        0     5958 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/dsets/utils_wrapdset_patches.py
+-rw-r--r--   0        0        0        0 2023-02-24 09:24:49.305369 domainlab-0.1.2/domainlab/exp_protocol/__init__.py
+-rw-r--r--   0        0        0     1711 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/exp_protocol/aggregate_results.py
+-rw-r--r--   0        0        0     5731 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/exp_protocol/benchmark.smk
+-rw-r--r--   0        0        0     4511 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/exp_protocol/run_experiment.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/models/__init__.py
+-rw-r--r--   0        0        0     1108 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/models/a_model.py
+-rw-r--r--   0        0        0     7623 2023-03-26 11:36:12.379054 domainlab-0.1.2/domainlab/models/a_model_classif.py
+-rw-r--r--   0        0        0      855 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/models/args_jigen.py
+-rw-r--r--   0        0        0     2482 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/models/args_vae.py
+-rw-r--r--   0        0        0     1402 2023-04-04 08:28:24.062639 domainlab-0.1.2/domainlab/models/interface_vae_xyd.py
+-rw-r--r--   0        0        0     1458 2023-02-23 11:55:38.957077 domainlab-0.1.2/domainlab/models/model_custom.py
+-rw-r--r--   0        0        0     1951 2023-02-23 11:55:38.961078 domainlab-0.1.2/domainlab/models/model_dann.py
+-rw-r--r--   0        0        0     1209 2023-02-23 11:55:38.961078 domainlab-0.1.2/domainlab/models/model_deep_all.py
+-rw-r--r--   0        0        0     3543 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/models/model_diva.py
+-rw-r--r--   0        0        0     4870 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/models/model_hduva.py
+-rw-r--r--   0        0        0     2335 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/models/model_jigen.py
+-rw-r--r--   0        0        0     1082 2023-04-04 08:28:24.062639 domainlab-0.1.2/domainlab/models/model_vae_xyd_classif.py
+-rw-r--r--   0        0        0      714 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/models/model_wrapper_matchdg4net.py
+-rw-r--r--   0        0        0      752 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/models/model_wrapper_matchdg4vae.py
+-rw-r--r--   0        0        0     1508 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/models/wrapper_matchdg.py
+-rw-r--r--   0        0        0       58 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/tasks/__init__.py
+-rw-r--r--   0        0        0     4879 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/tasks/a_task.py
+-rw-r--r--   0        0        0     1453 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/a_task_classif.py
+-rw-r--r--   0        0        0     2982 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/b_task.py
+-rw-r--r--   0        0        0     1474 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/b_task_classif.py
+-rw-r--r--   0        0        0     1826 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/tasks/task_dset.py
+-rw-r--r--   0        0        0     4057 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/task_folder.py
+-rw-r--r--   0        0        0     2748 2023-01-26 17:13:55.056713 domainlab-0.1.2/domainlab/tasks/task_folder_mk.py
+-rw-r--r--   0        0        0     2349 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/task_mnist_color.py
+-rw-r--r--   0        0        0     5085 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/task_pathlist.py
+-rw-r--r--   0        0        0      897 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/task_utils.py
+-rw-r--r--   0        0        0     8773 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/utils_task.py
+-rw-r--r--   0        0        0     1828 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/utils_task_dset.py
+-rw-r--r--   0        0        0     3733 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/tasks/zoo_tasks.py
+-rw-r--r--   0        0        0     3060 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/uml/libDG.uml
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/__init__.py
+-rw-r--r--   0        0        0     4713 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/flows_gen_img_model.py
+-rw-r--r--   0        0        0    20727 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/utils/generate_benchmark_plots.py
+-rw-r--r--   0        0        0     1057 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/get_git_tag.py
+-rw-r--r--   0        0        0     9420 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/utils/hyperparameter_sampling.py
+-rw-r--r--   0        0        0      801 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/override_interface.py
+-rw-r--r--   0        0        0     2168 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/utils/perf.py
+-rw-r--r--   0        0        0     3847 2023-03-26 11:36:42.932263 domainlab-0.1.2/domainlab/utils/perf_metrics.py
+-rw-r--r--   0        0        0     3131 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/utils/sanity_check.py
+-rw-r--r--   0        0        0      899 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/test_img.py
+-rw-r--r--   0        0        0      336 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/u_import.py
+-rw-r--r--   0        0        0     1949 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/u_import_net_module.py
+-rw-r--r--   0        0        0      901 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/utils_class.py
+-rw-r--r--   0        0        0     1303 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/utils_classif.py
+-rw-r--r--   0        0        0      446 2023-05-08 09:57:19.632046 domainlab-0.1.2/domainlab/utils/utils_cuda.py
+-rw-r--r--   0        0        0     1098 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/utils_img_sav.py
+-rw-r--r--   0        0        0      695 2023-05-08 10:14:38.024078 domainlab-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 domainlab-0.1.2/setup.py
+-rw-r--r--   0        0        0      810 1970-01-01 00:00:00.000000 domainlab-0.1.2/PKG-INFO
```

### Comparing `domainlab-0.1.0/LICENSE` & `domainlab-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/algos/a_algo_builder.py` & `domainlab-0.1.2/domainlab/algos/a_algo_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/algos/builder_custom.py` & `domainlab-0.1.2/domainlab/algos/builder_custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,16 @@
 
         def init_business(self, exp):
             """
             return trainer, model, observer
             """
             task = exp.task
             args = exp.args
-            device = get_device(args.nocu)
+            device = get_device(args)
             model_sel = MSelOracleVisitor(MSelTrLoss(max_es=args.es))
             observer = ObVisitor(exp, model_sel, device)
             model = class_name_model(list_str_y=task.list_str_y)
             self.set_nets_from_dictionary(args, task, model)
-            trainer = TrainerBasic(model, task, observer, device, args)
+            trainer = TrainerBasic()
+            trainer.init_business(model, task, observer, device, args)
             return trainer
     return NodeAlgoBuilderCustom
```

### Comparing `domainlab-0.1.0/domainlab/algos/builder_dann.py` & `domainlab-0.1.2/domainlab/algos/builder_dann.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+"""
+builder for Domain Adversarial Neural Network: accept different training scheme
+"""
 from domainlab.algos.a_algo_builder import NodeAlgoBuilder
 from domainlab.algos.msels.c_msel import MSelTrLoss
 from domainlab.algos.msels.c_msel_oracle import MSelOracleVisitor
 from domainlab.algos.observers.b_obvisitor import ObVisitor
 from domainlab.algos.observers.c_obvisitor_cleanup import ObVisitorCleanUp
 from domainlab.algos.trainers.train_visitor import TrainerVisitor
 from domainlab.algos.trainers.train_visitor import HyperSchedulerAneal
+from domainlab.algos.trainers.train_dial import TrainerDIAL
+from domainlab.algos.trainers.zoo_trainer import TrainerChainNodeGetter
 from domainlab.compos.nn_zoo.net_classif import ClassifDropoutReluLinear
 from domainlab.compos.utils_conv_get_flat_dim import get_flat_dim
 from domainlab.compos.zoo_nn import FeatExtractNNBuilderChainNodeGetter
 from domainlab.models.model_dann import mk_dann
 from domainlab.utils.utils_cuda import get_device
 
 
@@ -18,15 +23,15 @@
     """
     def init_business(self, exp):
         """
         return trainer, model, observer
         """
         task = exp.task
         args = exp.args
-        device = get_device(args.nocu)
+        device = get_device(args)
         msel = MSelOracleVisitor(MSelTrLoss(max_es=args.es))
         observer = ObVisitor(exp, msel, device)
         observer = ObVisitorCleanUp(observer)
 
         builder = FeatExtractNNBuilderChainNodeGetter(
             args, arg_name_of_net="nname",
             arg_path_of_net="npath")()  # request, @FIXME, constant string
@@ -49,14 +54,15 @@
 
         model = mk_dann()(list_str_y=task.list_str_y,
                           list_str_d=task.list_domain_tr,
                           alpha=args.gamma_reg,
                           net_encoder=net_encoder,
                           net_classifier=net_classifier,
                           net_discriminator=net_discriminator)
-
-        trainer = TrainerVisitor(model, task, observer, device, args)
-        trainer.set_scheduler(HyperSchedulerAneal,
-                              total_steps=trainer.num_batches*args.epos,
-                              flag_update_epoch=False,
-                              flag_update_batch=True)
+        trainer = TrainerChainNodeGetter(args)(default="visitor")
+        trainer.init_business(model, task, observer, device, args)
+        if trainer.name == "visitor":
+            trainer.set_scheduler(HyperSchedulerAneal,
+                                  total_steps=trainer.num_batches*args.epos,
+                                  flag_update_epoch=False,
+                                  flag_update_batch=True)
         return trainer
```

### Comparing `domainlab-0.1.0/domainlab/algos/builder_deepall.py` & `domainlab-0.1.2/domainlab/algos/builder_dial.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,41 @@
+"""
+builder for domain invariant adversarial learning
+"""
 from domainlab.algos.a_algo_builder import NodeAlgoBuilder
 from domainlab.algos.msels.c_msel import MSelTrLoss
 from domainlab.algos.msels.c_msel_oracle import MSelOracleVisitor
 from domainlab.algos.observers.b_obvisitor import ObVisitor
-from domainlab.algos.trainers.train_basic import TrainerBasic
+from domainlab.algos.trainers.train_dial import TrainerDIAL
 from domainlab.compos.zoo_nn import FeatExtractNNBuilderChainNodeGetter
 from domainlab.models.model_deep_all import mk_deepall
 from domainlab.utils.utils_cuda import get_device
 
 
-class NodeAlgoBuilderDeepAll(NodeAlgoBuilder):
+class NodeAlgoBuilderDeepAll_DIAL(NodeAlgoBuilder):
+    """
+    builder for domain invariant adversarial learning
+    """
     def init_business(self, exp):
         """
         return trainer, model, observer
         """
         task = exp.task
         args = exp.args
-        device = get_device(args.nocu)
+        device = get_device(args)
         model_sel = MSelOracleVisitor(MSelTrLoss(max_es=args.es))
         observer = ObVisitor(exp, model_sel, device)
 
         builder = FeatExtractNNBuilderChainNodeGetter(
             args, arg_name_of_net="nname",
             arg_path_of_net="npath")()  # request, # @FIXME, constant string
 
         net = builder.init_business(flag_pretrain=True, dim_out=task.dim_y,
                                     remove_last_layer=False, args=args,
                                     i_c=task.isize.i_c,
                                     i_h=task.isize.i_h,
                                     i_w=task.isize.i_w)
 
         model = mk_deepall()(net, list_str_y=task.list_str_y)
-        trainer = TrainerBasic(model, task, observer, device, args)
+        trainer = TrainerDIAL()
+        trainer.init_business(model, task, observer, device, args)
         return trainer
```

### Comparing `domainlab-0.1.0/domainlab/algos/builder_dial.py` & `domainlab-0.1.2/domainlab/algos/builder_deepall_mldg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
 builder for domain invariant adversarial learning
 """
 from domainlab.algos.a_algo_builder import NodeAlgoBuilder
 from domainlab.algos.msels.c_msel import MSelTrLoss
-from domainlab.algos.msels.c_msel_oracle import MSelOracleVisitor
 from domainlab.algos.observers.b_obvisitor import ObVisitor
-from domainlab.algos.trainers.train_dial import TrainerDIAL
+from domainlab.algos.trainers.train_mldg import TrainerMLDG
 from domainlab.compos.zoo_nn import FeatExtractNNBuilderChainNodeGetter
 from domainlab.models.model_deep_all import mk_deepall
 from domainlab.utils.utils_cuda import get_device
 
 
-class NodeAlgoBuilderDeepAll_DIAL(NodeAlgoBuilder):
+class NodeAlgoBuilderDeepAllMLDG(NodeAlgoBuilder):
     """
     builder for domain invariant adversarial learning
     """
     def init_business(self, exp):
         """
         return trainer, model, observer
         """
         task = exp.task
         args = exp.args
-        device = get_device(args.nocu)
-        model_sel = MSelOracleVisitor(MSelTrLoss(max_es=args.es))
+        device = get_device(args)
+        model_sel = MSelTrLoss(max_es=args.es)
         observer = ObVisitor(exp, model_sel, device)
 
         builder = FeatExtractNNBuilderChainNodeGetter(
             args, arg_name_of_net="nname",
             arg_path_of_net="npath")()  # request, # @FIXME, constant string
 
         net = builder.init_business(flag_pretrain=True, dim_out=task.dim_y,
                                     remove_last_layer=False, args=args,
                                     i_c=task.isize.i_c,
                                     i_h=task.isize.i_h,
                                     i_w=task.isize.i_w)
 
         model = mk_deepall()(net, list_str_y=task.list_str_y)
-        trainer = TrainerDIAL(model, task, observer, device, args)
+        trainer = TrainerMLDG()
+        trainer.init_business(model, task, observer, device, args)
         return trainer
```

### Comparing `domainlab-0.1.0/domainlab/algos/builder_diva.py` & `domainlab-0.1.2/domainlab/algos/builder_diva.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 """
 from domainlab.algos.a_algo_builder import NodeAlgoBuilder
 from domainlab.algos.msels.c_msel import MSelTrLoss
 from domainlab.algos.msels.c_msel_oracle import MSelOracleVisitor
 from domainlab.algos.observers.b_obvisitor import ObVisitor
 from domainlab.algos.observers.c_obvisitor_cleanup import ObVisitorCleanUp
 from domainlab.algos.observers.c_obvisitor_gen import ObVisitorGen
-from domainlab.algos.trainers.train_visitor import TrainerVisitor
-from domainlab.algos.trainers.train_dial import TrainerDIAL
+from domainlab.algos.trainers.zoo_trainer import TrainerChainNodeGetter
 
 from domainlab.compos.pcr.request import RequestVAEBuilderCHW
 from domainlab.compos.vae.utils_request_chain_builder import VAEChainNodeGetter
 from domainlab.models.model_diva import mk_diva
 from domainlab.utils.utils_cuda import get_device
 
 
@@ -36,26 +35,22 @@
                           list_str_y=task.list_str_y,
                           list_d_tr=task.list_domain_tr,
                           gamma_d=args.gamma_d,
                           gamma_y=args.gamma_y,
                           beta_x=args.beta_x,
                           beta_y=args.beta_y,
                           beta_d=args.beta_d)
-        device = get_device(args.nocu)
+        device = get_device(args)
         model_sel = MSelOracleVisitor(MSelTrLoss(max_es=args.es))
         if not args.gen:
             observer = ObVisitorCleanUp(
                 ObVisitor(exp,
                           model_sel,
                           device))
         else:
             observer = ObVisitorCleanUp(
                 ObVisitorGen(exp,
                              model_sel,
                              device))
-        if args.trainer == "dial":
-            trainer = TrainerDIAL(model, task, observer, device, args)
-        elif args.trainer is None:
-            trainer = TrainerVisitor(model, task, observer, device, args)
-        else:
-            raise NotImplementedError("diva does not support trainers other than default and dial")
+        trainer = TrainerChainNodeGetter(args)(default="visitor")
+        trainer.init_business(model, task, observer, device, args)
         return trainer
```

### Comparing `domainlab-0.1.0/domainlab/algos/builder_hduva.py` & `domainlab-0.1.2/domainlab/algos/builder_hduva.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from domainlab.algos.a_algo_builder import NodeAlgoBuilder
 from domainlab.algos.msels.c_msel import MSelTrLoss
 from domainlab.algos.msels.c_msel_oracle import MSelOracleVisitor
 from domainlab.algos.observers.b_obvisitor import ObVisitor
 from domainlab.algos.observers.c_obvisitor_cleanup import ObVisitorCleanUp
 from domainlab.algos.trainers.train_visitor import TrainerVisitor
+from domainlab.algos.trainers.zoo_trainer import TrainerChainNodeGetter
 from domainlab.compos.pcr.request import RequestVAEBuilderCHW
 from domainlab.compos.vae.utils_request_chain_builder import VAEChainNodeGetter
 from domainlab.models.model_hduva import mk_hduva
 from domainlab.utils.utils_cuda import get_device
 
 
 class NodeAlgoBuilderHDUVA(NodeAlgoBuilder):
@@ -18,15 +19,15 @@
         """
         return trainer, model, observer
         """
         task = exp.task
         args = exp.args
         request = RequestVAEBuilderCHW(
             task.isize.c, task.isize.h, task.isize.w, args)
-        device = get_device(args.nocu)
+        device = get_device(args)
         node = VAEChainNodeGetter(request, args.topic_dim)()
         model = mk_hduva()(node,
                            zd_dim=args.zd_dim,
                            zy_dim=args.zy_dim,
                            zx_dim=args.zx_dim,
                            device=device,
                            topic_dim=args.topic_dim,
@@ -37,9 +38,10 @@
                            beta_t=args.beta_t,
                            beta_x=args.beta_x,
                            beta_y=args.beta_y,
                            beta_d=args.beta_d)
         model_sel = MSelOracleVisitor(MSelTrLoss(max_es=args.es))
         observer = ObVisitorCleanUp(
             ObVisitor(exp, model_sel, device))
-        trainer = TrainerVisitor(model, task, observer, device, args)
+        trainer = TrainerChainNodeGetter(args)(default="visitor")
+        trainer.init_business(model, task, observer, device, args)
         return trainer
```

### Comparing `domainlab-0.1.0/domainlab/algos/builder_jigen1.py` & `domainlab-0.1.2/domainlab/algos/builder_jigen1.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     def init_business(self, exp):
         """
         return trainer, model, observer
         """
         task = exp.task
         args = exp.args
-        device = get_device(args.nocu)
+        device = get_device(args)
         msel = MSelOracleVisitor(MSelTrLoss(max_es=args.es))
         observer = ObVisitor(exp, msel, device)
         observer = ObVisitorCleanUp(observer)
 
         builder = FeatExtractNNBuilderChainNodeGetter(
             args, arg_name_of_net="nname",
             arg_path_of_net="npath")()  # request, @FIXME, constant string
@@ -66,13 +66,14 @@
         model = mk_jigen()(list_str_y=task.list_str_y,
                            list_str_d=task.list_domain_tr,
                            coeff_reg=args.gamma_reg,
                            net_encoder=net_encoder,
                            net_classifier_class=net_classifier,
                            net_classifier_permutation=net_classifier_perm)
 
-        trainer = TrainerVisitor(model, task, observer, device, args)
+        trainer = TrainerVisitor()
+        trainer.init_business(model, task, observer, device, args)
         trainer.set_scheduler(HyperSchedulerAneal,
                               total_steps=trainer.num_batches*args.epos,
                               flag_update_epoch=False,
                               flag_update_batch=True)
         return trainer
```

### Comparing `domainlab-0.1.0/domainlab/algos/builder_matchdg.py` & `domainlab-0.1.2/domainlab/algos/builder_matchdg.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+"""
+builder for mathcdg with deepall
+"""
 from domainlab.algos.a_algo_builder import NodeAlgoBuilder
 from domainlab.algos.msels.c_msel import MSelTrLoss
 from domainlab.algos.msels.c_msel_oracle import MSelOracleVisitor
 from domainlab.algos.observers.b_obvisitor import ObVisitor
 from domainlab.algos.trainers.train_matchdg import TrainerMatchDG
 from domainlab.compos.zoo_nn import FeatExtractNNBuilderChainNodeGetter
 from domainlab.models.model_deep_all import mk_deepall
 from domainlab.models.wrapper_matchdg import ModelWrapMatchDGLogit
+from domainlab.models.model_wrapper_matchdg4net import ModelWrapMatchDGNet
 from domainlab.utils.utils_cuda import get_device
 from domainlab.tasks.utils_task_dset import DsetIndDecorator4XYD
 
 
 class NodeAlgoBuilderMatchDG(NodeAlgoBuilder):
     """
     algorithm builder for matchDG
@@ -20,46 +24,53 @@
 
     def init_business(self, exp):
         """
         return trainer, model, observer
         """
         task = exp.task
         args = exp.args
-        device = get_device(args.nocu)
+        device = get_device(args)
 
         erm_builder = FeatExtractNNBuilderChainNodeGetter(
             args,
             arg_name_of_net="nname",
             arg_path_of_net="npath")()  # request, # @FIXME: constant string
+
         erm_net = erm_builder.init_business(
-            flag_pretrain=True, dim_out=task.dim_y,
-            remove_last_layer=False, args=args,
-            i_c=task.isize.i_c, i_h=task.isize.i_h,
+            flag_pretrain=True,
+            dim_out=task.dim_y,
+            remove_last_layer=False,
+            args=args,
+            i_c=task.isize.i_c,
+            i_h=task.isize.i_h,
             i_w=task.isize.i_w)
 
         model = mk_deepall()(erm_net, list_str_y=task.list_str_y)
         model = ModelWrapMatchDGLogit(model, list_str_y=task.list_str_y)
-
         model = model.to(device)
+
         ctr_builder = FeatExtractNNBuilderChainNodeGetter(
             args,
             arg_name_of_net="nname",
             arg_path_of_net="npath")()  # request, # @FIXME constant string
         ctr_net = ctr_builder.init_business(
             flag_pretrain=True,
             dim_out=task.dim_y,
             # @FIXME: ctr_model should not rely on task.dim_y so it could
             # support more tasks? maybe use task.feat_num?
             remove_last_layer=True,
             args=args,
             i_c=task.isize.i_c,
             i_h=task.isize.i_h,
             i_w=task.isize.i_w)
-        ctr_model = ctr_net.to(device)
+        ctr_model = ModelWrapMatchDGNet(ctr_net, list_str_y=task.list_str_y)
+        ctr_model = ctr_model.to(device)
 
         model_sel = MSelOracleVisitor(MSelTrLoss(max_es=args.es))
         observer = ObVisitor(exp,
                              model_sel,
                              device)
-        trainer = TrainerMatchDG(exp, task, ctr_model, model, observer, args,
-                                 device)
+
+        trainer = TrainerMatchDG()
+        trainer.init_business(exp, task, ctr_model, model, observer, args,
+                              device)
         return trainer
```

### Comparing `domainlab-0.1.0/domainlab/algos/compos/matchdg_base.py` & `domainlab-0.1.2/domainlab/algos/compos/matchdg_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import torch
-from torch import optim
 from domainlab.algos.compos.matchdg_match import MatchPair
 
 
 class MatchAlgoBase():
-    def __init__(self, task, phi, args, device, exp):
+    def __init__(self, task, phi, args, device, exp, opt):
         self.bs_match = args.bs  # use the same batch size for match tensor
         self.exp = exp
         self.task = task
         self.num_domain_tr = len(self.task.list_domain_tr)
         train_domains = self.task.list_domain_tr
         self.list_tr_domain_size = [len(self.task.dict_dset[key]) \
             for key in train_domains]
@@ -20,16 +19,15 @@
         # @FIXME: training loader always drop the last batch,
         # so inside matchdg, for the data storage tensor,
         # loader is re-initialized by disabling drop
         self.loader = task.loader_tr
         self.device = device
         self.phi = phi.to(self.device)
         #
-        self.opt = self.get_opt_sgd()
-        self.scheduler = torch.optim.lr_scheduler.StepLR(self.opt, step_size=25)
+        self.opt = opt
         self.ctr_mpath = self.exp.visitor.model_path + "_ctr"
         #
         self.tensor_ref_domain2each_domain_x = None
         self.tensor_ref_domain2each_domain_y = None
 
     def init_erm_phase(self):
         """
@@ -44,22 +42,14 @@
         # ctr(contrastive learning) phase
         self.phi = self.phi.to(self.device)
         # len((ctr_phi.state_dict()).keys()): 122,
         # extra fields are fc.weight, fc.bias
         self.phi.eval()  # @FIXME
         self.mk_match_tensor(epoch=0)
 
-    def get_opt_sgd(self):
-        opt = optim.SGD([{'params': filter(
-                         lambda p: p.requires_grad,
-                         self.phi.parameters())}, ],
-                        lr=self.args.lr, weight_decay=5e-4,
-                        momentum=0.9, nesterov=True)
-        return opt
-
     def save_model_ctr_phase(self):
         # Store the weights of the model
         # dirname = os.path.dirname(self.ctr_mpath)
         # Path(dirname).mkdir(parents=True, exist_ok=True)
         torch.save(self.phi.state_dict(), self.ctr_mpath)
 
     def save_model_erm_phase(self):
@@ -76,15 +66,19 @@
                               self.bs_match,
                               virtual_ref_dset_size=self.base_domain_size,
                               num_domains_tr=self.num_domain_tr,
                               list_tr_domain_size=self.list_tr_domain_size)
 
         # @FIXME: what is the usefulness of (epoch > 0) as argument
         self.tensor_ref_domain2each_domain_x, self.tensor_ref_domain2each_domain_y = \
-            obj_match(self.device, self.loader, self.phi, (epoch > 0))
+        obj_match(
+            self.device,
+            self.loader,
+            lambda x: self.phi.extract_semantic_feat(x),
+            (epoch > 0))
 
 
 def get_base_domain_size4match_dg(task):
     """
     Base domain is a dataset where each class
     set come from one of the nominal domains
     """
```

### Comparing `domainlab-0.1.0/domainlab/algos/compos/matchdg_ctr_erm.py` & `domainlab-0.1.2/domainlab/algos/compos/matchdg_ctr_erm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 import torch
 
 from domainlab.algos.compos.matchdg_base import MatchAlgoBase
 from domainlab.algos.compos.matchdg_utils import (dist_cosine_agg,
                                                   dist_pairwise_cosine)
+from domainlab.algos.trainers.a_trainer import mk_opt
 
 
 class MatchCtrErm(MatchAlgoBase):
     """
     Contrastive Learning
     """
-    def __init__(self, task, phi, args, device, exp, flag_erm=False):
+    def __init__(self, task, phi, args, device, exp, flag_erm=False, opt=None):
         """
         """
-        super().__init__(task, phi, args, device, exp)
+        if opt is None:
+            opt = mk_opt(phi, args)
+        super().__init__(task, phi, args, device, exp, opt)
         self.epo_loss_tr = 0
         self.flag_erm = flag_erm
         self.epos = self.args.epochs_ctr
         self.epos_per_match = self.args.epos_per_match_update
         self.str_phase = "ctr"
         self.lambda_ctr = 1.0
         if self.flag_erm:
-            self.lambda_ctr = self.args.penalty_ws
-            self.epos = self.args.epochs_erm
+            self.lambda_ctr = self.args.gamma_reg
+            self.epos = self.args.epos - self.args.epochs_ctr
             self.str_phase = "erm"
             self.init_erm_phase()
         else:
             self.mk_match_tensor(epoch=0)
+        self.flag_stop = False
+        self.tuple_tensor_ref_domain2each_y = None
+        self.tuple_tensor_refdomain2each = None
 
     def train(self):
+        """
+        train self.epos number of epochs
+        """
         for epoch in range(self.epos):
             self.tr_epoch(epoch)
 
     def tr_epoch(self, epoch):
         """
         # data in one batch comes from two sources: one part from loader,
         # the other part from match tensor
@@ -40,208 +49,221 @@
         print(self.str_phase, "epoch", epoch)
         # update match tensor
         if (epoch + 1) % self.epos_per_match == 0:
             self.mk_match_tensor(epoch)
 
         inds_shuffle = torch.randperm(self.tensor_ref_domain2each_domain_x.size(0))
         # NOTE: match tensor size: N(ref domain size) * #(train domains) * (image size: c*h*w)
-        # self.tensor_ref_domain2each_domain_x[inds_shuffle] shuffles the match tensor at the first dimension
-        tuple_tensor_refdomain2each = torch.split(self.tensor_ref_domain2each_domain_x[inds_shuffle],
-                                                  self.args.bs, dim=0)
-        # Splits the tensor into chunks. Each chunk is a view of the original tensor of batch size self.args.bs
+        # self.tensor_ref_domain2each_domain_x[inds_shuffle]
+        # shuffles the match tensor at the first dimension
+        self.tuple_tensor_refdomain2each = torch.split(
+            self.tensor_ref_domain2each_domain_x[inds_shuffle],
+            self.args.bs, dim=0)
+        # Splits the tensor into chunks.
+        # Each chunk is a view of the original tensor of batch size self.args.bs
         # return is a tuple of the splited chunks
-        tuple_tensor_ref_domain2each_y = torch.split(self.tensor_ref_domain2each_domain_y[inds_shuffle],
-                                                     self.args.bs, dim=0)
-        print("number of batches in match tensor: ", len(tuple_tensor_refdomain2each))
-        print("single batch match tensor size: ", tuple_tensor_refdomain2each[0].shape)
+        self.tuple_tensor_ref_domain2each_y = torch.split(
+            self.tensor_ref_domain2each_domain_y[inds_shuffle],
+            self.args.bs, dim=0)
+        print("number of batches in match tensor: ", len(self.tuple_tensor_refdomain2each))
+        print("single batch match tensor size: ", self.tuple_tensor_refdomain2each[0].shape)
 
         for batch_idx, (x_e, y_e, d_e, *_) in enumerate(self.loader):
-        # random loader with same batch size as the match tensor loader
-        # the 4th output of self.loader is not used at all,
-        # is only used for creating the match tensor
-            self.opt.zero_grad()
-            x_e = x_e.to(self.device)  # 64 * 1 * 224 * 224
-            # y_e_scalar = torch.argmax(y_e, dim=1).to(self.device)
-            y_e = y_e.to(self.device)
-            # d_e = torch.argmax(d_e, dim=1).numpy()
-            d_e = d_e.to(self.device)
-            # for each batch, the list loss is re-initialized
-
-            # CTR (contrastive) loss for CTR/ERM phase are different
-            list_batch_loss_ctr = []
-            # for a single batch,  loss need to be
-            # aggregated across different combinations of domains.
-            # Defining a leaf node can cause problem by loss_ctr += xxx,
-            # a list with python built-in "sum" can aggregate
-            # these losses within one batch
-
-            if self.flag_erm:
-                # logit_yhat = self.phi(x_e)  # @FIXME
-                # loss_erm_rnd_loader = F.cross_entropy(logit_yhat, y_e.long()).to(self.device)
-                loss_erm_rnd_loader = self.phi.cal_loss(x_e, y_e, d_e)
-
-            num_batches = len(tuple_tensor_refdomain2each)
-
-            if batch_idx >= num_batches:
+            # random loader with same batch size as the match tensor loader
+            # the 4th output of self.loader is not used at all,
+            # is only used for creating the match tensor
+            self.update_batch(epoch, batch_idx, x_e, y_e, d_e)
+            if self.flag_stop is True:
                 print("ref/base domain vs each domain match \
                       traversed one sweep, starting new epoch")
                 break
+        if not self.flag_erm:
+            # Save ctr model's weights post each epoch
+            self.save_model_ctr_phase()
 
-            curr_batch_size = tuple_tensor_refdomain2each[batch_idx].shape[0]
+    def update_batch(self, epoch, batch_idx, x_e, y_e, d_e):
+        """
+        update network for each batch
+        """
+        self.opt.zero_grad()
+        x_e = x_e.to(self.device)  # 64 * 1 * 224 * 224
+        # y_e_scalar = torch.argmax(y_e, dim=1).to(self.device)
+        y_e = y_e.to(self.device)
+        # d_e = torch.argmax(d_e, dim=1).numpy()
+        d_e = d_e.to(self.device)
+        # for each batch, the list loss is re-initialized
+
+        # CTR (contrastive) loss for CTR/ERM phase are different
+        list_batch_loss_ctr = []
+        # for a single batch,  loss need to be
+        # aggregated across different combinations of domains.
+        # Defining a leaf node can cause problem by loss_ctr += xxx,
+        # a list with python built-in "sum" can aggregate
+        # these losses within one batch
 
-            batch_tensor_ref_domain2each = tuple_tensor_refdomain2each[batch_idx].to(self.device)
-            # make order 5 tensor: (ref_domain, domain, channel, img_h, img_w)
-            # with first dimension as batch size
-
-            # clamp the first two dimensions so the phi network could map image to feature
-            batch_tensor_ref_domain2each = batch_tensor_ref_domain2each.view(
-                batch_tensor_ref_domain2each.shape[0]*batch_tensor_ref_domain2each.shape[1],
-                batch_tensor_ref_domain2each.shape[2],   # channel
-                batch_tensor_ref_domain2each.shape[3],   # img_h
-                batch_tensor_ref_domain2each.shape[4])   # img_w
-            # now batch_tensor_ref_domain2each first dim will not be batch_size!
-            # batch_tensor_ref_domain2each.shape torch.Size([40, channel, 224, 224])
-
-            # @FIXME: change to extract_feature?
-            batch_feat_ref_domain2each = self.phi(batch_tensor_ref_domain2each)
-            # batch_feat_ref_domain2each.shape torch.Size[40, 512]
-            # torch.sum(torch.isnan(batch_tensor_ref_domain2each))
-            # assert not torch.sum(torch.isnan(batch_feat_ref_domain2each))
-            flag_isnan = torch.any(torch.isnan(batch_feat_ref_domain2each))
-            if flag_isnan:
-                # usually because learning rate is too big
-                raise RuntimeError("batch_feat_ref_domain2each NAN!")
-
-            # for contrastive training phase,
-            # the last layer of the model is replaced with identity
-
-            batch_ref_domain2each_y = tuple_tensor_ref_domain2each_y[batch_idx].to(self.device)
-            batch_ref_domain2each_y = batch_ref_domain2each_y.view(batch_ref_domain2each_y.shape[0]*batch_ref_domain2each_y.shape[1])
-
-            # @FIXME:
-            # self.phi.cal_loss(batch_tensor_ref_domain2each,
-            # batch_ref_domain2each_y)
-
-            if self.flag_erm:
-                # loss_erm_match_tensor = F.cross_entropy(batch_feat_ref_domain2each, batch_ref_domain2each_y.long()).to(self.device)
-                # @FIXME: check if batch_ref_domain2each_y is
-                # continuous number which means it is at its initial value,
-                # not yet filled
-                # FIMXE: shall we leave batch_ref_domain2each_y scalar so it
-                # takes less memory?
-                loss_erm_match_tensor = self.phi.cal_loss(batch_tensor_ref_domain2each, batch_ref_domain2each_y.long())
-
-            # Creating tensor of shape (domain size, total domains, feat size )
-            # The match tensor's first two dimension
-            # [(Ref domain size) * (# train domains)]
-            # has been clamped together to get features extracted
-            # through self.phi
-
-            # it has to be reshaped into the match tensor shape, the same
-            # for the extracted feature here, it has to reshaped into
-            # the shape of the match tensor
-            # to make sure that the reshape only happens at the
-            # first two dimension, the feature dim has to be kept intact
-            dim_feat = batch_feat_ref_domain2each.shape[1]
-            batch_feat_ref_domain2each = batch_feat_ref_domain2each.view(curr_batch_size, self.num_domain_tr, dim_feat)
-
-            batch_ref_domain2each_y = batch_ref_domain2each_y.view(curr_batch_size, self.num_domain_tr)
-
-            # The match tensor's first two dimension
-            # [(Ref domain size) * (# train domains)] has been clamped
-            # together to get features extracted through self.phi
-            batch_tensor_ref_domain2each = \
-                batch_tensor_ref_domain2each.view(curr_batch_size,
-                                                  self.num_domain_tr,
-                                                  batch_tensor_ref_domain2each.shape[1],   # channel
-                                                  batch_tensor_ref_domain2each.shape[2],   # img_h
-                                                  batch_tensor_ref_domain2each.shape[3])   # img_w
-
-            # Contrastive Loss: class \times domain \times domain
-            counter_same_cls_diff_domain = 1
-            for y_c in range(self.dim_y):
-
-                subset_same_cls = (batch_ref_domain2each_y[:, 0] == y_c)
-                subset_diff_cls = (batch_ref_domain2each_y[:, 0] != y_c)
-                feat_same_cls = batch_feat_ref_domain2each[subset_same_cls]
-                feat_diff_cls = batch_feat_ref_domain2each[subset_diff_cls]
-                #print('class', y_c, "with same class and different class: ",
-                #      feat_same_cls.shape[0], feat_diff_cls.shape[0])
-
-                if feat_same_cls.shape[0] == 0 or feat_diff_cls.shape[0] == 0:
-                    # print("no instances of label",
-                    # y_c,
-                    # "in the current batch, continue")
-                    continue
-
-                if torch.sum(torch.isnan(feat_diff_cls)):
-                    raise RuntimeError('feat_diff_cls has nan entrie(s)')
-
-                feat_diff_cls = feat_diff_cls.view(
-                    feat_diff_cls.shape[0]*feat_diff_cls.shape[1],
-                    feat_diff_cls.shape[2])
-
-                for d_i in range(feat_same_cls.shape[1]):
-                    dist_diff_cls_same_domain = dist_pairwise_cosine(
-                        feat_same_cls[:, d_i, :], feat_diff_cls[:, :])
-
-                    if torch.sum(torch.isnan(dist_diff_cls_same_domain)):
-                        raise RuntimeError('dist_diff_cls_same_domain NAN')
-
-                    # iterate other domains
-                    for d_j in range(feat_same_cls.shape[1]):
-                        if d_i >= d_j:
-                            continue
-                        dist_same_cls_diff_domain = dist_cosine_agg(feat_same_cls[:, d_i, :],
-                                                                    feat_same_cls[:, d_j, :])
-
-                        if torch.sum(torch.isnan(dist_same_cls_diff_domain)):
-                            raise RuntimeError('dist_same_cls_diff_domain NAN')
-
-                        # CTR (contrastive) loss is exclusive for
-                        # CTR phase and ERM phase
-
-                        if self.flag_erm:
-                            list_batch_loss_ctr.append(torch.sum(dist_same_cls_diff_domain))
-                        else:
-                            i_dist_same_cls_diff_domain = 1.0 - dist_same_cls_diff_domain
-                            i_dist_same_cls_diff_domain = i_dist_same_cls_diff_domain / self.args.tau
-                            partition = torch.log(torch.exp(i_dist_same_cls_diff_domain) + dist_diff_cls_same_domain)
-                            list_batch_loss_ctr.append(-1 * torch.sum(i_dist_same_cls_diff_domain - partition))
-
-                        counter_same_cls_diff_domain += dist_same_cls_diff_domain.shape[0]
-
-            loss_ctr = sum(list_batch_loss_ctr) / counter_same_cls_diff_domain
-
-            coeff = (epoch + 1)/(self.epos + 1)
-            # loss aggregation is over different domain
-            # combinations of the same batch
-            # https://discuss.pytorch.org/t/leaf-variable-was-used-in-an-inplace-operation/308
-            # Loosely, tensors you create directly are leaf variables.
-            # Tensors that are the result of a differentiable operation are
-            # not leaf variables
-
-            if self.flag_erm:
-                # extra loss of ERM phase: the ERM loss
-                # (the CTR loss for the ctr phase and erm phase are different)
-                # erm loss comes from two different data loaders,
-                # one is rnd (random) data loader
-                # the other one is the data loader from the match tensor
-                loss_e = torch.tensor(0.0, requires_grad=True) + \
-                        torch.mean(loss_erm_rnd_loader) + \
-                        torch.mean(loss_erm_match_tensor) + \
-                        self.lambda_ctr * coeff * loss_ctr
-            else:
-                loss_e = torch.tensor(0.0, requires_grad=True) + \
-                    self.lambda_ctr * coeff * loss_ctr
-            # @FIXME: without torch.tensor(0.0), after a few epochs,
-            # error "'float' object has no attribute 'backward'"
+        if self.flag_erm:
+            loss_erm_rnd_loader = self.phi.cal_loss(x_e, y_e, d_e)
 
-            loss_e.backward(retain_graph=False)
-            self.opt.step()
-            self.epo_loss_tr += loss_e.detach().item()
+        num_batches = len(self.tuple_tensor_refdomain2each)
 
-            torch.cuda.empty_cache()
+        if batch_idx >= num_batches:
+            print("ref/base domain vs each domain match \
+                    traversed one sweep, starting new epoch")
+            self.flag_stop = True
+            return
+
+        curr_batch_size = self.tuple_tensor_refdomain2each[batch_idx].shape[0]
+
+        batch_tensor_ref_domain2each = self.tuple_tensor_refdomain2each[batch_idx].to(self.device)
+        # make order 5 tensor: (ref_domain, domain, channel, img_h, img_w)
+        # with first dimension as batch size
+
+        # clamp the first two dimensions so the phi network could map image to feature
+        batch_tensor_ref_domain2each = batch_tensor_ref_domain2each.view(
+            batch_tensor_ref_domain2each.shape[0]*batch_tensor_ref_domain2each.shape[1],
+            batch_tensor_ref_domain2each.shape[2],   # channel
+            batch_tensor_ref_domain2each.shape[3],   # img_h
+            batch_tensor_ref_domain2each.shape[4])   # img_w
+        # now batch_tensor_ref_domain2each first dim will not be batch_size!
+        # batch_tensor_ref_domain2each.shape torch.Size([40, channel, 224, 224])
+
+        batch_feat_ref_domain2each = self.phi.extract_semantic_feat(
+            batch_tensor_ref_domain2each)
+        # batch_feat_ref_domain2each.shape torch.Size[40, 512]
+        # torch.sum(torch.isnan(batch_tensor_ref_domain2each))
+        # assert not torch.sum(torch.isnan(batch_feat_ref_domain2each))
+        flag_isnan = torch.any(torch.isnan(batch_feat_ref_domain2each))
+        if flag_isnan:
+            print(batch_tensor_ref_domain2each)
+            raise RuntimeError("batch_feat_ref_domain2each NAN! is learning rate too big or \
+                               hyper-parameter tau not set appropriately?")
+
+        # for contrastive training phase,
+        # the last layer of the model is replaced with identity
+
+        batch_ref_domain2each_y = self.tuple_tensor_ref_domain2each_y[batch_idx].to(self.device)
+        batch_ref_domain2each_y = batch_ref_domain2each_y.view(
+            batch_ref_domain2each_y.shape[0]*batch_ref_domain2each_y.shape[1])
 
-        if not self.flag_erm:
-            # Save ctr model's weights post each epoch
-            self.save_model_ctr_phase()
+        if self.flag_erm:
+            # @FIXME: check if batch_ref_domain2each_y is
+            # continuous number which means it is at its initial value,
+            # not yet filled
+            loss_erm_match_tensor = self.phi.cal_loss(
+                batch_tensor_ref_domain2each, batch_ref_domain2each_y.long())
+
+        # Creating tensor of shape (domain size, total domains, feat size )
+        # The match tensor's first two dimension
+        # [(Ref domain size) * (# train domains)]
+        # has been clamped together to get features extracted
+        # through self.phi
+
+        # it has to be reshaped into the match tensor shape, the same
+        # for the extracted feature here, it has to reshaped into
+        # the shape of the match tensor
+        # to make sure that the reshape only happens at the
+        # first two dimension, the feature dim has to be kept intact
+        dim_feat = batch_feat_ref_domain2each.shape[1]
+        batch_feat_ref_domain2each = batch_feat_ref_domain2each.view(
+            curr_batch_size, self.num_domain_tr, dim_feat)
+
+        batch_ref_domain2each_y = batch_ref_domain2each_y.view(
+            curr_batch_size, self.num_domain_tr)
+
+        # The match tensor's first two dimension
+        # [(Ref domain size) * (# train domains)] has been clamped
+        # together to get features extracted through self.phi
+        batch_tensor_ref_domain2each = \
+            batch_tensor_ref_domain2each.view(curr_batch_size,
+                                              self.num_domain_tr,
+                                              batch_tensor_ref_domain2each.shape[1],   # channel
+                                              batch_tensor_ref_domain2each.shape[2],   # img_h
+                                              batch_tensor_ref_domain2each.shape[3])   # img_w
+
+        # Contrastive Loss: class \times domain \times domain
+        counter_same_cls_diff_domain = 1
+        for y_c in range(self.dim_y):
+
+            subset_same_cls = (batch_ref_domain2each_y[:, 0] == y_c)
+            subset_diff_cls = (batch_ref_domain2each_y[:, 0] != y_c)
+            feat_same_cls = batch_feat_ref_domain2each[subset_same_cls]
+            feat_diff_cls = batch_feat_ref_domain2each[subset_diff_cls]
+            # print('class', y_c, "with same class and different class: ",
+            #      feat_same_cls.shape[0], feat_diff_cls.shape[0])
+
+            if feat_same_cls.shape[0] == 0 or feat_diff_cls.shape[0] == 0:
+                # print("no instances of label",
+                # y_c,
+                # "in the current batch, continue")
+                continue
+
+            if torch.sum(torch.isnan(feat_diff_cls)):
+                raise RuntimeError('feat_diff_cls has nan entrie(s)')
+
+            feat_diff_cls = feat_diff_cls.view(
+                feat_diff_cls.shape[0]*feat_diff_cls.shape[1],
+                feat_diff_cls.shape[2])
+
+            for d_i in range(feat_same_cls.shape[1]):
+                dist_diff_cls_same_domain = dist_pairwise_cosine(
+                    feat_same_cls[:, d_i, :], feat_diff_cls[:, :])
+
+                if torch.sum(torch.isnan(dist_diff_cls_same_domain)):
+                    raise RuntimeError('dist_diff_cls_same_domain NAN')
+
+                # iterate other domains
+                for d_j in range(feat_same_cls.shape[1]):
+                    if d_i >= d_j:
+                        continue
+                    dist_same_cls_diff_domain = dist_cosine_agg(feat_same_cls[:, d_i, :],
+                                                                feat_same_cls[:, d_j, :])
+
+                    if torch.sum(torch.isnan(dist_same_cls_diff_domain)):
+                        raise RuntimeError('dist_same_cls_diff_domain NAN')
+
+                    # CTR (contrastive) loss is exclusive for
+                    # CTR phase and ERM phase
+
+                    if self.flag_erm:
+                        list_batch_loss_ctr.append(torch.sum(dist_same_cls_diff_domain))
+                    else:
+                        i_dist_same_cls_diff_domain = 1.0 - dist_same_cls_diff_domain
+                        i_dist_same_cls_diff_domain = \
+                            i_dist_same_cls_diff_domain / self.args.tau
+                        partition = torch.log(torch.exp(i_dist_same_cls_diff_domain) +
+                                              dist_diff_cls_same_domain)
+                        list_batch_loss_ctr.append(
+                            -1 * torch.sum(i_dist_same_cls_diff_domain - partition))
+
+                    counter_same_cls_diff_domain += dist_same_cls_diff_domain.shape[0]
+
+        loss_ctr = sum(list_batch_loss_ctr) / counter_same_cls_diff_domain
+
+        coeff = (epoch + 1)/(self.epos + 1)
+        # loss aggregation is over different domain
+        # combinations of the same batch
+        # https://discuss.pytorch.org/t/leaf-variable-was-used-in-an-inplace-operation/308
+        # Loosely, tensors you create directly are leaf variables.
+        # Tensors that are the result of a differentiable operation are
+        # not leaf variables
+
+        if self.flag_erm:
+            # extra loss of ERM phase: the ERM loss
+            # (the CTR loss for the ctr phase and erm phase are different)
+            # erm loss comes from two different data loaders,
+            # one is rnd (random) data loader
+            # the other one is the data loader from the match tensor
+            loss_e = torch.tensor(0.0, requires_grad=True) + \
+                    torch.mean(loss_erm_rnd_loader) + \
+                    torch.mean(loss_erm_match_tensor) + \
+                    self.lambda_ctr * coeff * loss_ctr
+        else:
+            loss_e = torch.tensor(0.0, requires_grad=True) + \
+                self.lambda_ctr * coeff * loss_ctr
+        # @FIXME: without torch.tensor(0.0), after a few epochs,
+        # error "'float' object has no attribute 'backward'"
+
+        loss_e.backward(retain_graph=False)
+        self.opt.step()
+        self.epo_loss_tr += loss_e.detach().item()
+
+        torch.cuda.empty_cache()
```

### Comparing `domainlab-0.1.0/domainlab/algos/compos/matchdg_match.py` & `domainlab-0.1.2/domainlab/algos/compos/matchdg_match.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,28 +8,32 @@
 from domainlab.tasks.utils_task import mk_loader
 from domainlab.utils.utils_class import store_args
 
 
 class MatchPair():
     @store_args
     def __init__(self,
-                 dim_y,  # @TODO: dim_y is not used here
+                 dim_y,
                  i_c,
                  i_h,
                  i_w,
-                 bs_match,  # @TODO: bs_match is not used here
+                 bs_match,
                  virtual_ref_dset_size,
                  num_domains_tr,
                  list_tr_domain_size):
         """
         :param virtual_ref_dset_size:  sum of biggest class sizes
         :param num_domains_tr:
         :param list_tr_domain_size:
-        :param phi: neural network to generate causal features from input
         """
+        self.dim_y = dim_y
+        self.bs_match = bs_match
+        self.virtual_ref_dset_size = virtual_ref_dset_size
+        self.num_domains_tr = num_domains_tr
+        self.list_tr_domain_size = list_tr_domain_size
         self.dict_cls_ind_base_domain_ind = {}
         self.dict_virtual_dset2each_domain = MatchDictVirtualRefDset2EachDomain(
             virtual_ref_dset_size=virtual_ref_dset_size,
             num_domains_tr=num_domains_tr,
             i_c=i_c, i_h=i_h, i_w=i_w)()
 
         self.dict_domain_data = MatchDictNumDomain2SizeDomain(
@@ -57,15 +61,14 @@
             loader.dataset,
             bsize=loader.batch_size,
             drop_last=False)
         # @FIXME: training loader will always drop the last incomplete batch
         for _, (x_e, y_e, d_e, idx_e) in enumerate(loader_full_data):
             # traverse mixed domain data from loader
             list_idx_several_ds.extend(list(idx_e.cpu().numpy()))
-            x_e = x_e
             y_e = torch.argmax(y_e, dim=1)
             d_e = torch.argmax(d_e, dim=1).numpy()
 
             # get all domains in current batch
             unique_domains = np.unique(d_e)
             for domain_idx in unique_domains:
                 # select all instances belong to one domain
@@ -113,135 +116,158 @@
         # with the max samples of the current class
         # Create dictionary: class label -> list of ordered flag_curr_domain
         """
         for y_c in range(self.dim_y):
             base_domain_size = 0
             base_domain_idx = -1
             for domain_idx in range(self.num_domains_tr):
-                flag_curr_class = (self.dict_domain_data[domain_idx]['label'] == y_c)   # tensor of True/False
-                curr_size = self.dict_domain_data[domain_idx]['label'][flag_curr_class].shape[0]    # flag_curr_class are subset indicator
+                flag_curr_class = \
+                    (self.dict_domain_data[domain_idx]['label'] == y_c)   # tensor of True/False
+                curr_size = \
+                    self.dict_domain_data[domain_idx]['label'][flag_curr_class].shape[0]
+                # flag_curr_class are subset indicator
                 if base_domain_size < curr_size:
                     base_domain_size = curr_size
                     base_domain_idx = domain_idx
             self.dict_cls_ind_base_domain_ind[y_c] = base_domain_idx
             # for each class label, there is a base domain
             print("for class", y_c)
             print("domain index as base domain:", base_domain_idx)
             print("Base Domain size", base_domain_size)
 
-
-
-    def __call__(self, device, loader, phi, flag_match_min_dist):
+    def __call__(self, device, loader, fun_extract_semantic_feat, flag_match_min_dist):
+        """
+        :param fun_extract_semantic_feat: function to generate causal features from input
+        """
         self._fill_data(loader)
         self._cal_base_domain()
         for curr_domain_ind in range(self.num_domains_tr):
             counter_ref_dset_size = 0
             for y_c in range(self.dim_y):
                 # which domain to use as the base domain for the current class
                 base_domain_idx = self.dict_cls_ind_base_domain_ind[y_c]
 
                 # subset indicator
                 flags_base_domain_curr_cls = \
                     (self.dict_domain_data[base_domain_idx]['label'] == y_c)
                 flags_base_domain_curr_cls = flags_base_domain_curr_cls[:, 0]
-                global_inds_base_domain_curr_cls = self.dict_domain_data[base_domain_idx]['idx'][flags_base_domain_curr_cls]
+                global_inds_base_domain_curr_cls = \
+                    self.dict_domain_data[base_domain_idx]['idx'][flags_base_domain_curr_cls]
                 # pick out base domain class label y_c images
                 # the difference of this block is "curr_domain_ind"
                 # in iteration is
                 # used instead of base_domain_idx for current class
 
                 # pick out current domain y_c class images
                 flag_curr_domain_curr_cls = (self.dict_domain_data[curr_domain_ind]['label'] == y_c)
                 # NO label matches y_c
                 flag_curr_domain_curr_cls = flag_curr_domain_curr_cls[:, 0]
-                global_inds_curr_domain_curr_cls = self.dict_domain_data[curr_domain_ind]['idx'][flag_curr_domain_curr_cls]
+                global_inds_curr_domain_curr_cls = \
+                    self.dict_domain_data[curr_domain_ind]['idx'][flag_curr_domain_curr_cls]
                 size_curr_domain_curr_cls = global_inds_curr_domain_curr_cls.shape[0]
                 if size_curr_domain_curr_cls == 0:  # there is no class y_c in current domain
-                    print("current domain",
-                          curr_domain_ind,
-                          " does not contain class ", y_c)
-                    raise RuntimeError("current domain does not contain all classes")
+                    raise RuntimeError(
+                        f"current domain {curr_domain_ind} does not contain class {y_c}")
 
                 # compute base domain features for class label y_c
-                x_base_domain_curr_cls = self.dict_domain_data[base_domain_idx]['data'][flags_base_domain_curr_cls]
+                x_base_domain_curr_cls = \
+                    self.dict_domain_data[base_domain_idx]['data'][flags_base_domain_curr_cls]
                 # pick out base domain class label y_c images
                 # split data into chunks
-                tuple_batch_x_base_domain_curr_cls = torch.split(x_base_domain_curr_cls, self.bs_match, dim=0)
+                tuple_batch_x_base_domain_curr_cls = \
+                    torch.split(x_base_domain_curr_cls, self.bs_match, dim=0)
                 # @FIXME. when x_base_domain_curr_cls is smaller
                 # than the self.bs_match, then there is only one batch
                 list_base_feat = []
                 for batch_x_base_domain_curr_cls in tuple_batch_x_base_domain_curr_cls:
                     with torch.no_grad():
                         batch_x_base_domain_curr_cls = batch_x_base_domain_curr_cls.to(device)
-                        feat = phi(batch_x_base_domain_curr_cls)
+                        feat = fun_extract_semantic_feat(batch_x_base_domain_curr_cls)
                         list_base_feat.append(feat.cpu())
-                tensor_feat_base_domain_curr_cls = torch.cat(list_base_feat)   # base domain features
+                tensor_feat_base_domain_curr_cls = torch.cat(list_base_feat)
+                # base domain features
 
                 if flag_match_min_dist:  # if epoch > 0:flag_match_min_dist=True
-                    x_curr_domain_curr_cls = self.dict_domain_data[curr_domain_ind]['data'][flag_curr_domain_curr_cls]
+                    x_curr_domain_curr_cls = \
+                        self.dict_domain_data[curr_domain_ind]['data'][flag_curr_domain_curr_cls]
                     # indices_curr pick out current domain y_c class images
-                    tuple_x_batch_curr_domain_curr_cls = torch.split(x_curr_domain_curr_cls, self.bs_match, dim=0)
+                    tuple_x_batch_curr_domain_curr_cls = \
+                        torch.split(x_curr_domain_curr_cls, self.bs_match, dim=0)
                     list_feat_x_curr_domain_curr_cls = []
                     for batch_feat in tuple_x_batch_curr_domain_curr_cls:
                         with torch.no_grad():
                             batch_feat = batch_feat.to(device)
-                            out = phi(batch_feat)
+                            out = fun_extract_semantic_feat(batch_feat)
                             list_feat_x_curr_domain_curr_cls.append(out.cpu())
                     tensor_feat_curr_domain_curr_cls = torch.cat(list_feat_x_curr_domain_curr_cls)
                     # feature through inference network for the current domain of class y_c
 
                 tensor_feat_base_domain_curr_cls = tensor_feat_base_domain_curr_cls.unsqueeze(1)
-                tuple_feat_base_domain_curr_cls = torch.split(tensor_feat_base_domain_curr_cls, self.bs_match, dim=0)
+                tuple_feat_base_domain_curr_cls = \
+                    torch.split(tensor_feat_base_domain_curr_cls, self.bs_match, dim=0)
 
                 counter_curr_cls_base_domain = 0
 
                 # tuple_feat_base_domain_curr_cls is a tuple of splitted part
                 for feat_base_domain_curr_cls in tuple_feat_base_domain_curr_cls:
 
                     if flag_match_min_dist:   # if epoch > 0:flag_match_min_dist=True
                         # Need to compute over batches of
                         # feature due to device Memory out errors
                         # Else no need for loop over
                         # tuple_feat_base_domain_curr_cls;
                         # could have simply computed
                         # tensor_feat_curr_domain_curr_cls -
                         # tensor_feat_base_domain_curr_cls
-                        dist_same_class_base_domain_curr_domain = torch.sum((tensor_feat_curr_domain_curr_cls - feat_base_domain_curr_cls)**2, dim=2)
+                        dist_same_class_base_domain_curr_domain = \
+                            torch.sum(
+                                (tensor_feat_curr_domain_curr_cls - feat_base_domain_curr_cls)**2,
+                                dim=2)
                         # tensor_feat_curr_domain_curr_cls.shape torch.Size([184, 512])
                         # feat_base_domain_curr_cls.shape torch.Size([64, 1, 512])
-                        # (tensor_feat_curr_domain_curr_cls - feat_base_domain_curr_cls).shape: torch.Size([64, 184, 512])
+                        # (tensor_feat_curr_domain_curr_cls - feat_base_domain_curr_cls).shape:
+                        # torch.Size([64, 184, 512])
                         # dist_same_class_base_domain_curr_domain.shape:
                         # torch.Size([64, 184]) is the per element distance of
                         # the cartesian product of feat_base_domain_curr_cls vs
                         # tensor_feat_curr_domain_curr_cls
-                        match_ind_base_domain_curr_domain = torch.argmin(dist_same_class_base_domain_curr_domain, dim=1)  # the batch index of the neareast neighbors
+                        match_ind_base_domain_curr_domain = \
+                            torch.argmin(dist_same_class_base_domain_curr_domain, dim=1)
+                        # the batch index of the neareast neighbors
                         # len(match_ind_base_domain_curr_domain)=64
                         # theoretically match_ind_base_domain_curr_domain can
                         # be a permutation of 0 to 183 though of size 64
                         # sort_val, sort_idx = \
                         # torch.sort(dist_same_class_base_domain_curr_domain, dim=1)
                         del dist_same_class_base_domain_curr_domain
 
                     #  feat_base_domain_curr_cls.shape torch.Size([64, 1, 512])
                     for idx in range(feat_base_domain_curr_cls.shape[0]):
                         # counter_curr_cls_base_domain =0 at initialization
 
-                        ### global_inds_base_domain_curr_cls pick out base
+                        # ## global_inds_base_domain_curr_cls pick out base
                         # domain class label y_c images
-                        global_pos_base_domain_curr_cls = global_inds_base_domain_curr_cls[counter_curr_cls_base_domain].item()
+                        global_pos_base_domain_curr_cls = \
+                            global_inds_base_domain_curr_cls[counter_curr_cls_base_domain].item()
                         if curr_domain_ind == base_domain_idx:
                             ind_match_global_curr_domain_curr_cls = global_pos_base_domain_curr_cls
                         else:
                             if flag_match_min_dist:  # if epoch > 0:match_min_dist=True
-                                ind_match_global_curr_domain_curr_cls = global_inds_curr_domain_curr_cls[match_ind_base_domain_curr_domain[idx]].item()
+                                ind_match_global_curr_domain_curr_cls = \
+                                    global_inds_curr_domain_curr_cls[
+                                        match_ind_base_domain_curr_domain[idx]].item()
                             else:  # if epoch == 0
-                                ind_match_global_curr_domain_curr_cls = global_inds_curr_domain_curr_cls[counter_curr_cls_base_domain%size_curr_domain_curr_cls].item()
-
-                        self.dict_virtual_dset2each_domain[counter_ref_dset_size]['data'][curr_domain_ind] = self.dict_domain_data[curr_domain_ind]['data'][ind_match_global_curr_domain_curr_cls]
-                        self.dict_virtual_dset2each_domain[counter_ref_dset_size]['label'][curr_domain_ind] = self.dict_domain_data[curr_domain_ind]['label'][ind_match_global_curr_domain_curr_cls]
+                                ind_match_global_curr_domain_curr_cls = \
+                                    global_inds_curr_domain_curr_cls[
+                                        counter_curr_cls_base_domain%size_curr_domain_curr_cls].item()
+
+                        self.dict_virtual_dset2each_domain[counter_ref_dset_size]['data'][curr_domain_ind] = \
+                            self.dict_domain_data[curr_domain_ind]['data'][ind_match_global_curr_domain_curr_cls]
+                        self.dict_virtual_dset2each_domain[counter_ref_dset_size]['label'][curr_domain_ind] = \
+                            self.dict_domain_data[curr_domain_ind]['label'][ind_match_global_curr_domain_curr_cls]
                         # @FIXME: label initially were set to random continuous
                         # value, which is a technique to check if
                         # every data has been filled
                         counter_curr_cls_base_domain += 1
                         counter_ref_dset_size += 1
 
             if counter_ref_dset_size != self.virtual_ref_dset_size:
```

### Comparing `domainlab-0.1.0/domainlab/algos/compos/matchdg_utils.py` & `domainlab-0.1.2/domainlab/algos/compos/matchdg_utils.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/algos/msels/a_model_sel.py` & `domainlab-0.1.2/domainlab/algos/msels/a_model_sel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+"""
+Abstract Model Selection
+"""
+
 import abc
 
+
 class AMSel(metaclass=abc.ABCMeta):
+    """
+    Abstract Model Selection
+    """
     def __init__(self):
         self.trainer = None
         self.tr_obs = None
 
     def accept(self, trainer, tr_obs):
         """
         Visitor pattern to trainer
@@ -13,14 +21,13 @@
         self.tr_obs = tr_obs
 
     @abc.abstractmethod
     def update(self):
         """
         observer + visitor pattern to trainer
         """
-        raise NotImplementedError
 
     def if_stop(self):
         """
         check if trainer should stop
         """
         raise NotImplementedError
```

### Comparing `domainlab-0.1.0/domainlab/algos/msels/c_msel.py` & `domainlab-0.1.2/domainlab/algos/msels/c_msel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 """
 Model Selection should be decoupled from
 """
+import math
 from domainlab.algos.msels.a_model_sel import AMSel
 
 
 class MSelTrLoss(AMSel):
     """
     1. Model selection using sum of loss across training domains
     2. Visitor pattern to trainer
     """
     def __init__(self, max_es):
         self.best_loss = float("inf")
-        self.es_c = 1
+        self.es_c = 0
         self.max_es = max_es
         super().__init__()
 
     def update(self):
         """
         if the best model should be updated
         """
         loss = self.trainer.epo_loss_tr   # @FIXME
         assert loss is not None
+        assert not math.isnan(loss)
         flag = True
         if loss < self.best_loss:
-            self.es_c = 1  # restore counter
+            self.es_c = 0  # restore counter
             self.best_loss = loss
         else:
             self.es_c += 1
             print("early stop counter: ", self.es_c)
+            print(f"loss:{loss}, best loss: {self.best_loss}")
             flag = False  # do not update best model
         return flag
 
     def if_stop(self):
         """
         if should early stop
         """
```

### Comparing `domainlab-0.1.0/domainlab/algos/msels/c_msel_oracle.py` & `domainlab-0.1.2/domainlab/algos/msels/c_msel_oracle.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/algos/observers/a_observer.py` & `domainlab-0.1.2/domainlab/algos/observers/a_observer.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class AObVisitor(metaclass=abc.ABCMeta):
     """
     Observer + Visitor pattern for model selection
     """
     @abc.abstractmethod
-    def update(self, epoch):
+    def update(self, epoch) -> bool:
         """
         return True/False whether the trainer should stop training
         """
 
     @abc.abstractmethod
     def accept(self, trainer):
         """
```

### Comparing `domainlab-0.1.0/domainlab/algos/observers/b_obvisitor.py` & `domainlab-0.1.2/domainlab/algos/observers/b_obvisitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,59 +37,86 @@
             metric_te = self.host_trainer.model.cal_perf_metric(
                 self.loader_tr, self.device, self.loader_te)
             self.metric_te = metric_te
         if self.model_sel.update():
             print("model selected")
             self.exp.visitor.save(self.host_trainer.model)
             print("persisted")
-        return self.model_sel.if_stop()
+        flag_stop = self.model_sel.if_stop()
+        return flag_stop
 
     def accept(self, trainer):
         """
         accept invitation as a visitor
         """
         self.host_trainer = trainer
         self.perf_metric = self.host_trainer.model.create_perf_obj(self.task)
         self.model_sel.accept(trainer, self)
 
     def after_all(self):
         """
         After training is done
         """
-        self.exp.visitor.save(self.host_trainer.model, "final")
-        model_ld = self.exp.visitor.load()
+        model_ld = None
+        try:
+            model_ld = self.exp.visitor.load()
+        except FileNotFoundError:
+            # this can happen if loss is increasing, model never get selected
+            return
+
         model_ld = model_ld.to(self.device)
         model_ld.eval()
         print("persisted model performance metric: \n")
         metric_te = model_ld.cal_perf_metric(self.loader_tr, self.device, self.loader_te)
+        self.dump_prediction(model_ld, metric_te)
         self.exp.visitor(metric_te)
+        # prediction dump of test domain is essential to verify the prediction results
+
+    def dump_prediction(self, model_ld, metric_te):
+        """
+        given the test domain loader, use the loaded model model_ld to predict each instance
+        """
         flag_task_folder = isinstance(self.exp.task, NodeTaskFolderClassNaMismatch)
         flag_task_path_list = isinstance(self.exp.task, NodeTaskPathListDummy)
         if flag_task_folder or flag_task_path_list:
             fname4model = self.exp.visitor.model_path  # pylint: disable=E1101
-            file_prefix = os.path.splitext(fname4model)[0]  # remove ".csv"
+            file_prefix = os.path.splitext(fname4model)[0]  # remove ".model"
+            dir4preds = os.path.join(self.exp.args.out, "saved_predicts")
+            if not os.path.exists(dir4preds):
+                os.mkdir(dir4preds)
+            file_prefix = os.path.join(dir4preds,
+                                       os.path.basename(file_prefix))
             file_name = file_prefix + "_instance_wise_predictions.txt"
-            self.host_trainer.model.pred2file(
+            model_ld.pred2file(
                 self.loader_te, self.device,
-                filename=file_name)
+                filename=file_name,
+                metric_te=metric_te)
 
     def clean_up(self):
         """
         to be called by a decorator
         """
         if not self.keep_model:
             try:
-                # oracle means use out-of-domain
-                # test accuracy to select the model
+                # oracle means use out-of-domain test accuracy to select the model
                 self.exp.visitor.remove("oracle")  # pylint: disable=E1101
-                # the last epoch
+            except FileNotFoundError:
+                pass
+
+            try:
+                # the last epoch:
+                # have a model to evaluate in case the training stops in between
                 self.exp.visitor.remove("epoch")  # pylint: disable=E1101
-                # epoch exist to still have a model to evaluate
-                # if the training stops in between
-                self.exp.visitor.remove("final")  # pylint: disable=E1101
+            except FileNotFoundError:
+                warnings.warn("failed to remove model_epoch: file not found")
+
+            try:
+                # without suffix: the selected model
                 self.exp.visitor.remove()  # pylint: disable=E1101
             except FileNotFoundError:
                 warnings.warn("failed to remove model")
+
             try:
-                self.exp.visitor.remove("ctr")  # pylint: disable=E1101 For matchdg
+                # for matchdg
+                self.exp.visitor.remove("ctr")  # pylint: disable=E1101
             except FileNotFoundError:
                 pass
```

### Comparing `domainlab-0.1.0/domainlab/algos/observers/c_obvisitor_gen.py` & `domainlab-0.1.2/domainlab/algos/observers/c_obvisitor_gen.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/algos/trainers/args_dial.py` & `domainlab-0.1.2/domainlab/algos/trainers/args_dial.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/algos/trainers/train_dial.py` & `domainlab-0.1.2/domainlab/algos/trainers/train_dial.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/algos/trainers/train_matchdg.py` & `domainlab-0.1.2/domainlab/algos/trainers/train_matchdg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,49 @@
+"""
+trainer for matchDG
+"""
 from domainlab.algos.compos.matchdg_ctr_erm import MatchCtrErm
 from domainlab.algos.trainers.a_trainer import AbstractTrainer
 
 
 class TrainerMatchDG(AbstractTrainer):
-    def __init__(self, exp, task, ctr_model, model, observer, args, device):
-        super().__init__(model, task, observer, device, args)
+    """
+    trainer for matchdg
+    """
+    def init_business(self, exp, task, ctr_model, model, observer, args, device):
+        super().init_business(model, task, observer, device, args)
         self.exp = exp
         self.epo_loss_tr = None
         self.ctr_model = ctr_model
+        self.erm = None
         self.args = self.aconf
 
     def before_tr(self):
         """
         configure trainer accoding to properties of task as well according to algorithm configs
         """
         # @FIXME: aconf and args should be separated
         # phase 1: contrastive learning
         ctr = MatchCtrErm(exp=self.exp,
                           task=self.task,
                           phi=self.ctr_model,
                           args=self.args,
                           device=self.device,
-                          flag_erm=False)
+                          flag_erm=False,
+                          opt=None)
         ctr.train()
         print("Phase 1 finished: ", ctr.ctr_mpath)
         # phase 2: ERM, initialize object
         self.erm = MatchCtrErm(phi=self.model,
                                exp=self.exp,
                                task=self.task,
                                args=self.args,
                                device=self.device,
-                               flag_erm=True)
+                               flag_erm=True,
+                               opt=self.optimizer)
 
     def tr_epoch(self, epoch):
         self.model.train()
         self.erm.tr_epoch(epoch)
         self.epo_loss_tr = self.erm.epo_loss_tr
         flag_stop = self.observer.update(epoch)  # notify observer
         return flag_stop
```

### Comparing `domainlab-0.1.0/domainlab/algos/trainers/train_visitor.py` & `domainlab-0.1.2/domainlab/algos/trainers/train_visitor.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/algos/zoo_algos.py` & `domainlab-0.1.2/domainlab/algos/zoo_algos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from domainlab.algos.builder_dann import NodeAlgoBuilderDANN
 from domainlab.algos.builder_jigen1 import NodeAlgoBuilderJiGen
 from domainlab.algos.builder_deepall import NodeAlgoBuilderDeepAll
 from domainlab.algos.builder_dial import NodeAlgoBuilderDeepAll_DIAL
+from domainlab.algos.builder_deepall_mldg import NodeAlgoBuilderDeepAllMLDG
 from domainlab.algos.builder_diva import NodeAlgoBuilderDIVA
 from domainlab.algos.builder_hduva import NodeAlgoBuilderHDUVA
 from domainlab.algos.builder_matchdg import NodeAlgoBuilderMatchDG
+from domainlab.algos.builder_match_hduva import NodeAlgoBuilderMatchHDUVA
 from domainlab.compos.pcr.request import RequestArgs2ExpCmd
 from domainlab.utils.u_import import import_path
 
 
 class AlgoBuilderChainNodeGetter(object):
     """
     1. Hardcoded chain
@@ -30,14 +32,16 @@
         """
         1. construct the chain, filter out responsible node, create heavy-weight business object
         2. hard code seems to be the best solution
         """
         chain = NodeAlgoBuilderDIVA(None)
         chain = NodeAlgoBuilderDeepAll(chain)
         chain = NodeAlgoBuilderDeepAll_DIAL(chain)
+        chain = NodeAlgoBuilderDeepAllMLDG(chain)
         chain = NodeAlgoBuilderDANN(chain)
         chain = NodeAlgoBuilderJiGen(chain)
         chain = NodeAlgoBuilderHDUVA(chain)
         chain = NodeAlgoBuilderMatchDG(chain)
+        chain = NodeAlgoBuilderMatchHDUVA(chain)
         chain = self.register_external_node(chain)
         node = chain.handle(self.request)
         return node
```

### Comparing `domainlab-0.1.0/domainlab/arg_parser.py` & `domainlab-0.1.2/domainlab/arg_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Command line arguments
 """
 import argparse
 import warnings
+
 import yaml
 
 from domainlab.algos.compos.matchdg_args import add_args2parser_matchdg
 from domainlab.algos.trainers.args_dial import add_args2parser_dial
-from domainlab.models.args_vae import add_args2parser_vae
 from domainlab.models.args_jigen import add_args2parser_jigen
+from domainlab.models.args_vae import add_args2parser_vae
 
 
 def mk_parser_main():
     """
     Args for command line definition
     """
     parser = argparse.ArgumentParser(description='DomainLab')
@@ -32,14 +33,17 @@
 
     parser.add_argument('--seed', type=int, default=0,
                         help='random seed (default: 0)')
 
     parser.add_argument('--nocu', action='store_true', default=False,
                         help='disables CUDA')
 
+    parser.add_argument('--device', type=str, default=None,
+                        help='device name default None')
+
     parser.add_argument('--gen', action='store_true', default=False,
                         help='save generated images')
 
     parser.add_argument('--keep_model', action='store_true', default=False,
                         help='do not delete model at the end of training')
 
     parser.add_argument('--epos', default=2, type=int,
@@ -101,14 +105,20 @@
                         help='tag as prefix of result aggregation file name \
                         e.g. git hash for reproducibility')
 
     parser.add_argument('--aggtag', type=str, default="aggtag",
                         help='tag in each line of result aggregation file \
                         e.g., to specify potential different configurations')
 
+    parser.add_argument('--agg_partial_bm', type=str,
+                        default=None, dest="bm_dir",
+                        help="Aggregates and plots partial data of a snakemake \
+                        benchmark. Requires the benchmark config file. \
+                        Other arguments will be ignored.")
+
     parser.add_argument('--msel', type=str, default=None,
                         help='model selection: val, elbo, recon, the \
                         elbo and recon only make sense for vae models,\
                         will be ignored by other methods')
 
     parser.add_argument('--aname', metavar="an", type=str,
                         default=None,
@@ -154,35 +164,51 @@
     arg_group_jigen = parser.add_argument_group('jigen')
     arg_group_jigen = add_args2parser_jigen(arg_group_jigen)
     args_group_dial = parser.add_argument_group('dial')
     args_group_dial = add_args2parser_dial(args_group_dial)
     return parser
 
 
+def apply_dict_to_args(args, data: dict, extend=False):
+    """
+    Tries to apply the data to the args dict of DomainLab.
+    Unknown keys are silently ignored as long as
+    extend is not set.
+    """
+    arg_dict = args.__dict__
+    for key, value in data.items():
+        if (key in arg_dict) or extend:
+            if isinstance(value, list):
+                cur_val = arg_dict.get(key, None)
+                if not isinstance(cur_val, list):
+                    if cur_val is not None:
+                        raise RuntimeError(f"input dictionary value is list, \
+                                           however, in DomainLab args, we have {cur_val}, \
+                                           going to overrite to list")
+                    arg_dict[key] = []  # if args_dict[key] is None, cast it into a list
+                    # domainlab will take care of it if this argument can not be a list
+                arg_dict[key].extend(value)  # args_dict[key] is already a list
+                # keep existing values for the list arg_dct[key]
+            else:
+                # over-write existing value
+                arg_dict[key] = value
+        else:
+            raise ValueError("Unsupported key: ", key)
+
+
 def parse_cmd_args():
     """
     get args from command line
     """
     parser = mk_parser_main()
     args = parser.parse_args()
     if args.config_file:
-
         data = yaml.safe_load(args.config_file)
         delattr(args, 'config_file')
-        arg_dict = args.__dict__
-
-        for key in data:
-            if key not in arg_dict:
-                raise ValueError("The key is not supported: ", key)
-
-        for key, value in data.items():
-            if isinstance(value, list):
-                arg_dict[key].extend(value)
-            else:
-                arg_dict[key] = value
+        apply_dict_to_args(args, data)
 
-    if args.acon is None:
+    if args.acon is None and args.bm_dir is None:
         print("\n\n")
         warnings.warn("no algorithm conf specified, going to use default")
         print("\n\n")
 
     return args
```

### Comparing `domainlab-0.1.0/domainlab/compos/a_nn_builder.py` & `domainlab-0.1.2/domainlab/compos/a_nn_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/builder_nn_alex.py` & `domainlab-0.1.2/domainlab/compos/builder_nn_alex.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/builder_nn_conv_bn_relu_2.py` & `domainlab-0.1.2/domainlab/compos/builder_nn_conv_bn_relu_2.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/builder_nn_external_from_file.py` & `domainlab-0.1.2/domainlab/compos/builder_nn_external_from_file.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/exp/exp_cuda_seed.py` & `domainlab-0.1.2/domainlab/compos/exp/exp_cuda_seed.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/exp/exp_main.py` & `domainlab-0.1.2/domainlab/compos/exp/exp_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 import datetime
 import os
+import shutil
+
 from torch.utils.data import Subset
 import torch.utils.data as data_utils
 import numpy as np
 
 from domainlab.algos.zoo_algos import AlgoBuilderChainNodeGetter
 from domainlab.compos.exp.exp_utils import AggWriter
 from domainlab.tasks.zoo_tasks import TaskChainNodeGetter
 from domainlab.dsets.utils_data import plot_ds
+from domainlab.utils.sanity_check import SanityCheck
 
 os.environ['CUDA_LAUNCH_BLOCKING'] = "1"  # debug
 
 
 class Exp():
     """
     Exp is combination of Task, Algorithm, and Configuration (including random seed)
     """
-    def __init__(self, args, task=None):
+    def __init__(self, args, task=None, visitor=AggWriter):
         """
         :param args:
         :param task:
         """
         self.task = task
         if task is None:
             self.task = TaskChainNodeGetter(args)()
             if args.san_check:
-                self.dataset_sanity_check(args, args.san_num)
+                sancheck = SanityCheck(args, self.task)
+                sancheck.dataset_sanity_check()
         self.task.init_business(args)
         self.args = args
-        self.visitor = AggWriter(self)
+        self.visitor = visitor(self)
         algo_builder = AlgoBuilderChainNodeGetter(self.args)()  # request
         self.trainer = algo_builder.init_business(self)
         self.epochs = self.args.epos
         self.epoch_counter = 1
 
     def execute(self):
         """
@@ -43,55 +47,24 @@
         print('\n Experiment start at :', str(t_0))
         t_c = t_0
         self.trainer.before_tr()
         for epoch in range(1, self.epochs + 1):
             t_before_epoch = t_c
             flag_stop = self.trainer.tr_epoch(epoch)
             t_c = datetime.datetime.now()
-            print("now: ", str(t_c), "epoch time: ", t_c - t_before_epoch, "used: ", t_c - t_0,
+            print(f"epoch: {epoch} ",
+                  "now: ", str(t_c),
+                  "epoch time: ", t_c - t_before_epoch,
+                  "used: ", t_c - t_0,
                   "model: ", self.visitor.model_name)
             # current time, time since experiment start, epoch time
             if flag_stop:
                 self.epoch_counter = epoch
+                print("early stop trigger")
                 break
             if epoch == self.epochs:
                 self.epoch_counter = self.epochs
             else:
                 self.epoch_counter += 1
         print("Experiment finished at epoch:", self.epoch_counter,
               "with time:", t_c - t_0, "at", t_c)
         self.trainer.post_tr()
-
-    def dataset_sanity_check(self, args, sample_num):
-        """
-        when we load data from folder or a file listing the path of observations,
-        we want to check if the file we loaded are in accordance with our expectations
-        This function dump a subsample of the dataset into hierarchical folder structure.
-        """
-        self.task.init_business(args)
-        f_name = os.path.join(args.out, 'Dset_extraction', self.task.task_name)
-
-        # for each domain do...
-        for domain in self.task.get_list_domains():
-            # generate a dataset for each domain
-            d_dataset = self.task.get_dset_by_domain(args, domain)[0]
-
-            # for each class do...
-            for class_num in range(len(self.task.list_str_y)):
-                num_of_samples = 0
-                loader_domain = data_utils.DataLoader(d_dataset, batch_size=1, shuffle=False)
-                domain_targets = []
-                for num, (_, lab, *_) in enumerate(loader_domain):
-                    if int(np.argmax(lab[0])) == class_num:
-                        domain_targets.append(num)
-                        num_of_samples += 1
-                    if sample_num == num_of_samples:
-                        break
-
-                class_dataset = Subset(d_dataset, domain_targets)
-                os.makedirs(f_name + '/' + str(domain), exist_ok=True)
-                plot_ds(
-                    class_dataset,
-                    f_name + '/' + str(domain) + '/' +
-                    str(self.task.list_str_y[class_num]) + '.jpg',
-                    batchsize=sample_num
-                )
```

### Comparing `domainlab-0.1.0/domainlab/compos/nn_zoo/net_adversarial.py` & `domainlab-0.1.2/domainlab/compos/nn_zoo/net_adversarial.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/nn_zoo/net_classif.py` & `domainlab-0.1.2/domainlab/compos/nn_zoo/net_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py` & `domainlab-0.1.2/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/nn_zoo/net_gated.py` & `domainlab-0.1.2/domainlab/compos/nn_zoo/net_gated.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/nn_zoo/nn.py` & `domainlab-0.1.2/domainlab/compos/nn_zoo/nn.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/nn_zoo/nn_alex.py` & `domainlab-0.1.2/domainlab/compos/nn_zoo/nn_alex.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/nn_zoo/nn_torchvision.py` & `domainlab-0.1.2/domainlab/compos/nn_zoo/nn_torchvision.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/pcr/p_chain_handler.py` & `domainlab-0.1.2/domainlab/compos/pcr/p_chain_handler.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/pcr/request.py` & `domainlab-0.1.2/domainlab/compos/pcr/request.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/utils_conv_get_flat_dim.py` & `domainlab-0.1.2/domainlab/compos/utils_conv_get_flat_dim.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/a_model_builder.py` & `domainlab-0.1.2/domainlab/compos/vae/a_model_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/a_vae_builder.py` & `domainlab-0.1.2/domainlab/compos/vae/a_vae_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/c_vae_adaptor_model_recon.py` & `domainlab-0.1.2/domainlab/compos/vae/c_vae_adaptor_model_recon.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/c_vae_builder_classif.py` & `domainlab-0.1.2/domainlab/compos/vae/c_vae_builder_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/c_vae_recon.py` & `domainlab-0.1.2/domainlab/compos/vae/c_vae_recon.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/decoder_cond_prior.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/decoder_cond_prior.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/decoder_losses.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/decoder_losses.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Upon pixel wise mean and variance
 """
 import torch
+from domainlab import g_inst_component_loss_agg
 
 
 class NLLPixelLogistic256(object):
     """
     Compute pixel wise negative likelihood of image,
     given pixel wise mean and variance.
     Pixel intensity is divided into bins of 256 levels.
@@ -31,12 +32,13 @@
         scale = torch.exp(logvar)
         tensor = (torch.floor(tensor / self.bin_size) * self.bin_size - mean) / scale
         cdf_plus = torch.sigmoid(tensor + self.bin_size/scale)
         cdf_minus = torch.sigmoid(tensor)
 
         # negative log-likelihood for each pixel
         log_logist_256 = - torch.log(cdf_plus - cdf_minus + 1.e-7)
-        nll = torch.sum(log_logist_256, dim=self.reduce_dims)
+        # torch.Size([100, 3, 28, 28])
+        nll = g_inst_component_loss_agg(log_logist_256, dim=self.reduce_dims)
         # NOTE: pixel NLL should always be summed
         # across the whole image of all channels
         # NOTE: result should be order 1 tensor of dim batch_size
         return nll
```

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/encoder.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/encoder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/encoder_dirichlet.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_dirichlet.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/encoder_domain_topic.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/encoder_xyd_parallel.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_xyd_parallel.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/encoder_xydt_elevator.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_xydt_elevator.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/compos/encoder_zy.py` & `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_zy.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/utils_request_chain_builder.py` & `domainlab-0.1.2/domainlab/compos/vae/utils_request_chain_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/zoo_vae_builders_classif.py` & `domainlab-0.1.2/domainlab/compos/vae/zoo_vae_builders_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/vae/zoo_vae_builders_classif_topic.py` & `domainlab-0.1.2/domainlab/compos/vae/zoo_vae_builders_classif_topic.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/compos/zoo_nn.py` & `domainlab-0.1.2/domainlab/compos/zoo_nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import copy
-
 from domainlab.compos.builder_nn_alex import mkNodeFeatExtractNNBuilderNameAlex
 from domainlab.compos.builder_nn_conv_bn_relu_2 import \
     mkNodeFeatExtractNNBuilderNameConvBnRelu2
 from domainlab.compos.builder_nn_external_from_file import \
     mkNodeFeatExtractNNBuilderExternFromFile
```

### Comparing `domainlab-0.1.0/domainlab/dsets/a_dset_mnist_color_rgb_solo.py` & `domainlab-0.1.2/domainlab/dsets/a_dset_mnist_color_rgb_solo.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/dsets/dset_img_path_list.py` & `domainlab-0.1.2/domainlab/dsets/dset_img_path_list.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/dsets/dset_mnist_color_solo_default.py` & `domainlab-0.1.2/domainlab/dsets/dset_mnist_color_solo_default.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/dsets/dset_poly_domains_mnist_color_default.py` & `domainlab-0.1.2/domainlab/dsets/dset_poly_domains_mnist_color_default.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/dsets/dset_subfolder.py` & `domainlab-0.1.2/domainlab/dsets/dset_subfolder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/dsets/utils_data.py` & `domainlab-0.1.2/domainlab/dsets/utils_data.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/dsets/utils_wrapdset_patches.py` & `domainlab-0.1.2/domainlab/dsets/utils_wrapdset_patches.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/models/a_model.py` & `domainlab-0.1.2/domainlab/models/a_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from torch import nn
 
 
 class AModel(nn.Module, metaclass=abc.ABCMeta):
     """
     operations that all models (classification, segmentation, seq2seq)
     """
-    def cal_loss(self, tensor_x, tensor_y, tensor_d, others=None):
+    def cal_loss(self, tensor_x, tensor_y, tensor_d=None, others=None):
         """
         calculate the loss
         """
         return self.cal_task_loss(tensor_x, tensor_y) + \
             self.cal_reg_loss(tensor_x, tensor_y, tensor_d, others)
 
     @abc.abstractmethod
```

### Comparing `domainlab-0.1.0/domainlab/models/a_model_classif.py` & `domainlab-0.1.2/domainlab/models/a_model_classif.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 operations that all claasification model should have
 """
 
 import abc
 import numpy as np
+import math
 import torch
 from torch import nn as nn
 from torch.nn import functional as F
 
 from domainlab.models.a_model import AModel
 from domainlab.utils.utils_class import store_args
 from domainlab.utils.utils_classif import get_label_na, logit2preds_vpic
@@ -31,30 +32,31 @@
         return self.perf_metric
 
     def cal_perf_metric(self, loader_tr, device, loader_te=None):
         """
         classification performance matric
         """
         metric_te = None
-        metric_tr_pool = self.perf_metric.cal_metrics(self, loader_tr, device)
-        confmat = metric_tr_pool.pop("confmat")
-        print("pooled train domains performance:")
-        rprint(metric_tr_pool)
-        print("confusion matrix:")
-        print(pd.DataFrame(confmat))
-        metric_tr_pool["confmat"] = confmat
-        # test set has no domain label, so can be more custom
-        if loader_te is not None:
-            metric_te = self.perf_metric.cal_metrics(self, loader_te, device)
-            confmat = metric_te.pop("confmat")
-            print("out of domain test performance:")
-            rprint(metric_te)
+        with torch.no_grad():
+            metric_tr_pool = self.perf_metric.cal_metrics(self, loader_tr, device)
+            confmat = metric_tr_pool.pop("confmat")
+            print("pooled train domains performance:")
+            rprint(metric_tr_pool)
             print("confusion matrix:")
             print(pd.DataFrame(confmat))
-            metric_te["confmat"] = confmat
+            metric_tr_pool["confmat"] = confmat
+            # test set has no domain label, so can be more custom
+            if loader_te is not None:
+                metric_te = self.perf_metric.cal_metrics(self, loader_te, device)
+                confmat = metric_te.pop("confmat")
+                print("out of domain test performance:")
+                rprint(metric_te)
+                print("confusion matrix:")
+                print(pd.DataFrame(confmat))
+                metric_te["confmat"] = confmat
         return metric_te
 
     def evaluate(self, loader_te, device):
         """
         for classification task, use the current model to cal acc
         """
         acc = PerfClassif.cal_acc(self, loader_te, device)
@@ -116,37 +118,69 @@
         if (tensor_y.shape[-1] == 1) | (len(tensor_y.shape) == 1):
             y_target = tensor_y
         else:
             _, y_target = tensor_y.max(dim=1)
         lc_y = F.cross_entropy(logit_y, y_target, reduction="none")
         return lc_y
 
-    def pred2file(self, loader_te, device,
-                  filename='path_prediction.txt', flag_pred_scalar=False):
+    def pred2file(self, loader_te, device, filename,
+                  metric_te,
+                  spliter="#"):
         """
         pred2file dump predicted label to file as sanity check
         """
         self.eval()
         model_local = self.to(device)
-        for _, (x_s, y_s, *_, path) in enumerate(loader_te):
+        for _, (x_s, y_s, *_, path4instance) in enumerate(loader_te):
             x_s, y_s = x_s.to(device), y_s.to(device)
             _, prob, *_ = model_local.infer_y_vpicn(x_s)
-            # print(path)
-            list_pred_list = prob.tolist()
-            list_label_list = y_s.tolist()
-            if flag_pred_scalar:
-                list_pred_list = [np.asarray(pred).argmax() for pred in list_pred_list]
-                list_label_list = [np.asarray(label).argmax() for label in list_label_list]
-            # label belongs to data
-            list_pair_path_pred = list(zip(path, list_label_list, list_pred_list))
+            list_pred_prob_list = prob.tolist()
+            list_target_list = y_s.tolist()
+            list_target_scalar = [np.asarray(label).argmax() for label in list_target_list]
+            tuple_zip = zip(path4instance, list_target_scalar, list_pred_prob_list)
+            list_pair_path_pred = list(tuple_zip)
             with open(filename, 'a', encoding="utf8") as handle_file:
-                for pair in list_pair_path_pred:
-                    # 1:-1 removes brackets of tuple
-                    print(str(pair)[1:-1], file=handle_file)
+                for list4one_obs_path_prob_target in list_pair_path_pred:
+                    list_str_one_obs_path_target_predprob = [
+                        str(ele) for ele in list4one_obs_path_prob_target]
+                    str_line = (" "+spliter+" ").join(list_str_one_obs_path_target_predprob)
+                    str_line = str_line.replace("[", "")
+                    str_line = str_line.replace("]", "")
+                    print(str_line, file=handle_file)
         print("prediction saved in file ", filename)
+        file_acc = self.read_prediction_file(filename, spliter)
+        acc_metric_te = metric_te['acc']
+        flag1 = math.isclose(file_acc, acc_metric_te, rel_tol=1e-9, abs_tol=0.01)
+        acc_raw1 = PerfClassif.cal_acc(self, loader_te, device)
+        acc_raw2 = PerfClassif.cal_acc(self, loader_te, device)
+        flag_raw_consistency = math.isclose(acc_raw1, acc_raw2, rel_tol=1e-9, abs_tol=0.01)
+        flag2 = math.isclose(file_acc, acc_raw1, rel_tol=1e-9, abs_tol=0.01)
+        if not (flag1 & flag2 & flag_raw_consistency):
+            str_info = f"inconsistent acc:  \
+                prediction file acc {file_acc} \
+                torchmetric acc {acc_metric_te} \
+                raw acc 1 {acc_raw1} \
+                raw acc 2 {acc_raw2}"
+            raise RuntimeError(str_info)
+        return file_acc
+
+    def read_prediction_file(self, filename, spliter):
+        """
+        check if the written fiel could calculate acc
+        """
+        with open(filename, 'r', encoding="utf8") as handle_file:
+            list_lines = [line.strip().split(spliter) for line in handle_file]
+        count_correct = 0
+        for line in list_lines:
+            list_prob = [float(ele) for ele in line[2].split(",")]
+            if np.array(list_prob).argmax() == int(line[1]):
+                count_correct += 1
+        acc = count_correct / len(list_lines)
+        print(f"accuracy from prediction file {acc}")
+        return acc
 
     def cal_loss_gen_adv(self, x_natural, x_adv, vec_y):
         """
         calculate loss function for generation of adversarial images
         """
         x_adv.requires_grad_()
         with torch.enable_grad():
@@ -156,8 +190,7 @@
             prob_natural = F.softmax(logits_natural, dim=1)
             loss_adv_gen_task = self.cal_task_loss(x_adv, vec_y)
             loss_adv_gen = self.loss4gen_adv(prob_adv, prob_natural)
         return loss_adv_gen + loss_adv_gen_task.sum()
 
     def cal_reg_loss(self, tensor_x, tensor_y, tensor_d, others=None):
         return 0
-
```

### Comparing `domainlab-0.1.0/domainlab/models/args_jigen.py` & `domainlab-0.1.2/domainlab/models/args_jigen.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/models/args_vae.py` & `domainlab-0.1.2/domainlab/models/args_vae.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/models/model_custom.py` & `domainlab-0.1.2/domainlab/models/model_custom.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/models/model_dann.py` & `domainlab-0.1.2/domainlab/models/model_dann.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/models/model_deep_all.py` & `domainlab-0.1.2/domainlab/models/model_deep_all.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/models/model_hduva.py` & `domainlab-0.1.2/domainlab/models/model_hduva.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Hierarchical Domain Unsupervised Variational Auto-Encoding
 """
 import torch
 from torch.distributions import Dirichlet
 
 from domainlab.models.model_vae_xyd_classif import VAEXYDClassif
 from domainlab.utils.utils_class import store_args
+from domainlab import g_inst_component_loss_agg
 
 
 def mk_hduva(parent_class=VAEXYDClassif):
     """
     Hierarchical Domain Unsupervised VAE with arbitrary task loss
     """
     class ModelHDUVA(parent_class):
@@ -70,67 +71,65 @@
             self.add_module("net_p_zy",
                             self.chain_node_builder.construct_cond_prior(
                                 self.dim_y, self.zy_dim))
             self.add_module("net_classif_y",
                             self.chain_node_builder.construct_classifier(
                                 self.zy_dim, self.dim_y))
 
-        def cal_logit_y(self, tensor_x):
-            """
-            calculate the logit for softmax classification
-            """
-            _, _, \
-                _, _, \
-                _, _, \
-                _, zy_q = self.encoder(tensor_x)
-            logit_y = self.net_classif_y(zy_q)
-            return logit_y
-
         def init_p_topic_batch(self, batch_size, device):
             """
             flat prior
             """
             prior = Dirichlet(torch.ones(batch_size, self.topic_dim).to(device))
             return prior
 
-        def cal_reg_loss(self, tensor_x, tensor_y, tensor_d, others=None):
+        def cal_reg_loss(self, tensor_x, tensor_y, tensor_d=None, others=None):
             q_topic, topic_q, \
                 qzd, zd_q, \
                 qzx, zx_q, \
                 qzy, zy_q = self.encoder(tensor_x)
 
             batch_size = zd_q.shape[0]
             device = zd_q.device
 
             p_topic = self.init_p_topic_batch(batch_size, device)
 
             # zx KL divergence
             zx_p_minus_q = 0
             if self.zx_dim > 0:
                 p_zx = self.init_p_zx4batch(batch_size, device)
-                zx_p_minus_q = torch.sum(p_zx.log_prob(zx_q) - qzx.log_prob(zx_q), 1)
+                zx_p_minus_q = g_inst_component_loss_agg(
+                    p_zx.log_prob(zx_q) - qzx.log_prob(zx_q), 1)
 
             # @FIXME: does monte-carlo KL makes the performance unstable?
             # from torch.distributions import kl_divergence
 
             # zy KL divergence
             p_zy = self.net_p_zy(tensor_y)
-            zy_p_minus_zy_q = torch.sum(p_zy.log_prob(zy_q) - qzy.log_prob(zy_q), 1)
+            zy_p_minus_zy_q = g_inst_component_loss_agg(p_zy.log_prob(zy_q) - qzy.log_prob(zy_q), 1)
 
             # zd KL diverence
             p_zd = self.net_p_zd(topic_q)
-            zd_p_minus_q = torch.sum(p_zd.log_prob(zd_q) - qzd.log_prob(zd_q), 1)
+            zd_p_minus_q = g_inst_component_loss_agg(p_zd.log_prob(zd_q) - qzd.log_prob(zd_q), 1)
 
             # topic KL divergence
             # @FIXME: why topic is still there?
             topic_p_minus_q = p_topic.log_prob(topic_q) - q_topic.log_prob(topic_q)
 
             # reconstruction
             z_concat = self.decoder.concat_ytdx(zy_q, topic_q, zd_q, zx_q)
             loss_recon_x, _, _ = self.decoder(z_concat, tensor_x)
             batch_loss = loss_recon_x \
                 - self.beta_x * zx_p_minus_q \
                 - self.beta_y * zy_p_minus_zy_q \
                 - self.beta_d * zd_p_minus_q \
                 - self.beta_t * topic_p_minus_q
             return batch_loss
+
+        def extract_semantic_features(self, tensor_x):
+            """
+            :param tensor_x:
+            """
+            zy_q_loc = self.encoder.infer_zy_loc(tensor_x)
+            return zy_q_loc
+
     return ModelHDUVA
```

### Comparing `domainlab-0.1.0/domainlab/models/model_jigen.py` & `domainlab-0.1.2/domainlab/models/model_jigen.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/models/wrapper_matchdg.py` & `domainlab-0.1.2/domainlab/models/wrapper_matchdg.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,30 +6,41 @@
 
 class ModelWrapMatchDGLogit(AModelClassif):
     """
     Wrap an arbitrary model with interface:cal_logit_y
     """
     def __init__(self, net, list_str_y, list_str_d=None):
         super().__init__(list_str_y, list_str_d)
+        self.check_attribute(net)
+        self.net = net
+
+    def check_attribute(self, net):
+        """
+        """
         fun_name = AModelClassif.match_feat_fun_na
         if not hasattr(net, fun_name):
             raise RuntimeError(
                 "model to be wrapped must inherit base class ",
                 str(AModelClassif.__class__),
                 " with attribute:", fun_name)
-        self.net = net
 
     def cal_logit_y(self, tensor_x):
         return self.net.cal_logit_y(tensor_x)
 
     def cal_loss(self, tensor_x, tensor_y, tensor_d=None, others=None):
         return self.net.cal_loss(tensor_x, tensor_y, tensor_d)
 
     def cal_reg_loss(self, tensor_x, tensor_y, tensor_d=None, others=None):
         return self.net.cal_loss(tensor_x, tensor_y, tensor_d)  # @FIXME: this is wrong
 
     def forward(self, tensor_x):
         """
         calculate features to be matched
         """
+        return self.extract_semantic_feat(tensor_x)
+
+    def extract_semantic_feat(self, tensor_x):
+        """
+        extract semantic feature
+        """
         logit_y = self.net.cal_logit_y(tensor_x)  # @FIXME: match other features instead of logit
         return logit_y
```

### Comparing `domainlab-0.1.0/domainlab/tasks/b_task.py` & `domainlab-0.1.2/domainlab/tasks/a_task.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,157 @@
 """
-Use dictionaries to create train and test domain split
+Abstract class for Task
 """
-from collections import Counter
+import warnings
+from abc import abstractmethod
 
-import torch
-from torch.utils.data.dataset import ConcatDataset
+from domainlab.compos.pcr.p_chain_handler import AbstractChainNodeHandler
+from domainlab.tasks.task_utils import parse_domain_id
 
-from domainlab.tasks.a_task_classif import NodeTaskDGClassif
-from domainlab.tasks.utils_task import (DsetDomainVecDecorator, mk_loader,
-                                        mk_onehot)
 
-
-class NodeTaskDict(NodeTaskDGClassif):
+class NodeTaskDG(AbstractChainNodeHandler):
     """
-    Use dictionaries to create train and test domain split
+    Domain Generalization Classification Task
     """
-    @property
-    def list_str_y(self):
-        return self._list_str_y
+    def __init__(self, succ=None):
+        super().__init__(succ)
+        self._loader_tr = None
+        self._loader_te = None
+        self._loader_val = None
+        self._list_domains = None
+        self._list_domain_tr = None
+        self._name = None
+        self._args = None
+        self.dict_dset = {}
+        self.dict_dset_te = {}
+        self.dict_dset_val = {}
+        self.dict_domain_class_count = {}
+        self.dim_d_tr = None  # public
+        self._im_size = None
+        self._dict_domains2imgroot = {}
+        self._dict_domain_folder_name2class = {}  # {"domain1": {"class1":car, "class2":dog}}
+        self._dict_domain_img_trans = {}
+        self.dict_att = {}
+        self.img_trans_te = None
+        self.dict_domain2imgroot = {}
+        self._dict_domain2filepath_list_im_tr = {}  # {"photo": "xxx/yyy/file_of_path2imgs"}
+        self._dict_domain2filepath_list_im_val = {}
+        self._dict_domain2filepath_list_im_te = {}
+        self.dict_class_label_ind2name = None
+
+    @abstractmethod
+    def init_business(self, args):
+        """
+        construct task
+        """
+    def get_list_domains(self):
+        """
+        1. get list of domain names
+        2. better use method than property so new domains can be added
+        """
+        return self._list_domains
 
-    @list_str_y.setter
-    def list_str_y(self, list_str_y):
-        self._list_str_y = list_str_y
+    def set_list_domains(self, list_domains):
+        """
+        setter for self._list_domains
+        """
+        self._list_domains = list_domains
 
     @property
     def isize(self):
+        """
+        getter for input size: isize
+        """
         return self._im_size
 
     @isize.setter
     def isize(self, im_size):
+        """
+        setter for input size: isize
+        """
         self._im_size = im_size
 
-    def get_list_domains(self):
-        return self._list_domains
+    @property
+    def list_domain_tr(self):
+        """
+        property getter of list of domains for this task
+        """
+        if self._list_domain_tr is None:
+            raise RuntimeError("task not intialized!")
+        return self._list_domain_tr
 
-    def set_list_domains(self, list_domains):
+    @property
+    def loader_tr(self):
+        """loader of mixed train domains"""
+        return self._loader_tr
+
+    @property
+    def loader_val(self):
+        """loader of validation dataset on the training domains"""
+        return self._loader_val
+
+    @property
+    def loader_te(self):
+        """loader of mixed test domains"""
+        return self._loader_te
+
+    @property
+    def task_name(self):
         """
-        setter for self._list_domains
+        The basic name of the task, without configurations
         """
-        self._list_domains = list_domains
+        # @FIXME: hardcoded position
+        return type(self).__name__[8:].lower()
 
-    def get_dset_by_domain(self, args, na_domain, split=False):
+    def get_na(self, na_tr, na_te):
         """
-        each domain correspond to one dataset
+        task name appended with configurations
+        :param na_tr: training domain names
+        :param na_te: test domain names
         """
-        raise NotImplementedError
+        _, list_te = self.get_list_domains_tr_te(na_tr, na_te)
+        str_te = "_".join(list_te)
+        # train domain names are too long
+        return "_".join([self.task_name, "te", str_te])
 
-    def decorate_dset(self, model, args):
+    def is_myjob(self, request):
         """
-        dispatch re-organization of data flow to model
+        :param request: string
         """
+        return request == self.task_name
 
-    def init_business(self, args):
+    def get_list_domains_tr_te(self, tr_id, te_id):
         """
-        create a dictionary of datasets
+        For static DG task, get train and test domains list.
+
+        :param tr_id: training domain ids;
+            int or str, or a list of int or str, or None;
+            if None, then assumed to be the complement of te_id.
+        :param te_id: test domain ids;
+            int or str, or a list of int or str; required.
+        :return: list of training domain names, list of test domain names.
         """
-        # @FIXME
-        from domainlab.algos.zoo_algos import AlgoBuilderChainNodeGetter
-        # ImportError: cannot import name 'AlgoBuilderChainNodeGetter'
-        # from partially initialized module 'domainlab.algos.zoo_algos'
-        # (most likely due to a circular import)
-        # (~/domainlab_master/domainlab/algos/zoo_algos.py)
-        node = AlgoBuilderChainNodeGetter(args)()
-        list_domain_tr, list_domain_te = self.get_list_domains_tr_te(args.tr_d, args.te_d)
-        self.dict_dset = {}
-        self.dict_dset_val = {}
-        dim_d = len(list_domain_tr)
-        for (ind_domain_dummy, na_domain) in enumerate(list_domain_tr):
-            # FIXME: specify either split = True or False
-            dset_tr, dset_val = self.get_dset_by_domain(args, na_domain)
-            # @FIXME: currently, different task has different default values for
-            # split, for TaskFolder split default to False, for mnist, split
-            # default to True
-            vec_domain = mk_onehot(dim_d, ind_domain_dummy)
-            ddset_tr = DsetDomainVecDecorator(dset_tr, vec_domain, na_domain)
-            ddset_val = DsetDomainVecDecorator(dset_val, vec_domain, na_domain)
-            ddset_tr = node.dset_decoration_args_algo(args, ddset_tr)
-            ddset_val = node.dset_decoration_args_algo(args, ddset_val)
-            self.dict_dset.update({na_domain: ddset_tr})
-            self.dict_dset_val.update({na_domain: ddset_val})
-        ddset_mix = ConcatDataset(tuple(self.dict_dset.values()))
-        self._loader_tr = mk_loader(ddset_mix, args.bs)
+        list_domains = self.get_list_domains()
 
-        ddset_mix_val = ConcatDataset(tuple(self.dict_dset_val.values()))
-        self._loader_val = mk_loader(ddset_mix_val, args.bs)
+        list_domain_te = parse_domain_id(te_id, list_domains)
+        assert set(list_domain_te).issubset(set(list_domains))
 
-        self.dict_dset_te = {}
-        # No need to have domain Label for test
-        for na_domain in list_domain_te:
-            dset_te, *_ = self.get_dset_by_domain(args, na_domain, split=False)
-            # @FIXME: since get_dset_by_domain always return two datasets,
-            # train and validation, this is not needed in test domain
-            self.dict_dset_te.update({na_domain: dset_te})
-        dset_te = ConcatDataset(tuple(self.dict_dset_te.values()))
-        self._loader_te = mk_loader(dset_te, args.bs, drop_last=False)
-        self.count_domain_class()
-
-    def count_domain_class(self):
-        """
-        iterate all domains and count the class label distribution for each
-        return a double dictionary {"domain1": {"class1":3, "class2": 4,...}, ....}
-        """
-        for key, dset in self.dict_dset.items():
-            dict_class_count = self._count_class_one_hot(dset)
-            self.dict_domain_class_count[key] = dict_class_count
-        for key, dset in self.dict_dset_te.items():
-            dict_class_count = self._count_class_one_hot(dset)
-            self.dict_domain_class_count[key] = dict_class_count
-
-    def _count_class_one_hot(self, dset):
-        labels_count = torch.zeros(self.dim_y, dtype=torch.long)
-        for _, target, *_ in dset:
-            labels_count += target.long()
-
-        list_count = list(labels_count.cpu().numpy())
-        dict_class_count = {}
-        for name, count in zip(self.list_str_y, list_count):
-            dict_class_count[name] = count
-        return dict_class_count
-
-    def _count_class(self, dset):   # @FIXME: remove this
-        labels = dset.targets
-        class_dict = dict(Counter(labels))
-        return class_dict
+        if tr_id is None:
+            list_domain_tr = [did for did in list_domains if
+                              did not in list_domain_te]
+        else:
+            list_domain_tr = parse_domain_id(tr_id, list_domains)
+        if not set(list_domain_tr).issubset(set(list_domains)):
+            raise RuntimeError(
+                f"training domain {list_domain_tr} is not \
+                subset of available domains {list_domains}")
+
+        if set(list_domain_tr) & set(list_domain_te):
+            warnings.warn(
+                "The sets of training and test domains overlap -- \
+                be aware of data leakage or training to the test!",
+                RuntimeWarning
+            )
+
+        self.dim_d_tr = len(list_domain_tr)
+        self._list_domain_tr = list_domain_tr
+        return list_domain_tr, list_domain_te
```

### Comparing `domainlab-0.1.0/domainlab/tasks/task_folder.py` & `domainlab-0.1.2/domainlab/tasks/task_folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 """
 from torchvision import transforms
 
 from domainlab.dsets.dset_subfolder import DsetSubFolder
 from domainlab.dsets.utils_data import (DsetInMemDecorator,
                                         fun_img_path_loader_default,
                                         mk_fun_label2onehot)
-from domainlab.tasks.b_task import NodeTaskDict
+from domainlab.tasks.b_task_classif import NodeTaskDictClassif
 from domainlab.tasks.utils_task import DsetClassVecDecoratorImgPath
 
 
-class NodeTaskFolder(NodeTaskDict):
+class NodeTaskFolder(NodeTaskDictClassif):
     """
     create dataset by loading files from an organized folder
     then each domain correspond to one dataset
     """
     @property
     def dict_domain2imgroot(self):
         """
```

### Comparing `domainlab-0.1.0/domainlab/tasks/task_folder_mk.py` & `domainlab-0.1.2/domainlab/tasks/task_folder_mk.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/tasks/task_mnist_color.py` & `domainlab-0.1.2/domainlab/tasks/task_mnist_color.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Color MNIST with palette
 """
 from torch.utils.data import random_split
 
 from domainlab.dsets.dset_mnist_color_solo_default import \
     DsetMNISTColorSoloDefault
 from domainlab.dsets.utils_color_palette import default_rgb_palette  # @FIXME
-from domainlab.tasks.b_task import NodeTaskDict
+from domainlab.tasks.b_task_classif import NodeTaskDictClassif
 from domainlab.tasks.utils_task import ImSize
 from domainlab.utils.utils_classif import mk_dummy_label_list_str
 
 
-class NodeTaskMNISTColor10(NodeTaskDict):
+class NodeTaskMNISTColor10(NodeTaskDictClassif):
     """
     Use the deafult palette with 10 colors
     """
     @property
     def list_str_y(self):
         return mk_dummy_label_list_str("digit", 10)
```

### Comparing `domainlab-0.1.0/domainlab/tasks/task_pathlist.py` & `domainlab-0.1.2/domainlab/tasks/task_pathlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,69 +5,75 @@
 executed)
 of an image and the second slot contains the class label as a numerical string.
 """
 import os
 
 import torch.multiprocessing
 
-torch.multiprocessing.set_sharing_strategy('file_system')
-# "too many opened files" https://github.com/pytorch/pytorch/issues/11201
-
-from torchvision import transforms
-
 from domainlab.dsets.dset_img_path_list import DsetImPathList
 from domainlab.dsets.utils_data import mk_fun_label2onehot
-from domainlab.tasks.b_task import NodeTaskDict
+from domainlab.tasks.b_task_classif import NodeTaskDictClassif
+
+torch.multiprocessing.set_sharing_strategy('file_system')
+# "too many opened files" https://github.com/pytorch/pytorch/issues/11201
 
 
-class NodeTaskPathListDummy(NodeTaskDict):
-    pass
+class NodeTaskPathListDummy(NodeTaskDictClassif):
+    """
+    typedef class so that other function can use isinstance
+    """
+    def get_dset_by_domain(self, args, na_domain, split=False):
+        raise NotImplementedError
 
 
 def mk_node_task_path_list(isize,
+                           img_trans_te,
                            list_str_y,
-                           trans4all,
-                           dict_class_label2name,
+                           img_trans_tr,
+                           dict_class_label_ind2name,
                            dict_domain2imgroot,
-                           dict_d2filepath_list_img,
+                           dict_d2filepath_list_img_tr,
                            dict_d2filepath_list_img_val,
                            dict_d2filepath_list_img_te,
                            succ=None):
     """mk_node_task_path_list.
 
     :param isize:
     :param list_str_y:
-    :param trans4all:
-    :param dict_class_label2name:
+    :param img_trans_tr:
+    :param dict_class_label_ind2name:
     :param dict_domain2imgroot:
-    :param dict_d2filepath_list_img:
+    :param dict_d2filepath_list_img_tr:
     :param dict_d2filepath_list_img_val:
     :param dict_d2filepath_list_img_te:
     :param succ:
     """
     class NodeTaskPathList(NodeTaskPathListDummy):
         """
         The class TaskPathList provides the user an interface to provide a file
         with each line consisting of a pair separated by comma, where the
         first slot contains the path (either absolute or relative if the user
         knows from where this package is executed) of an image and the second
         slot contains the class label as a numerical string.
         e.g.: /path/2/file/art_painting/dog/pic_376.jpg 1
         """
-        def _get_complete_domain(self, na_domain, list_domain_path):
+        def _get_complete_domain(self, na_domain, dict_domain2pathfilepath):
             """_get_complete_domain.
 
             :param na_domain:
             """
-            if self._dict_domain_img_trans:
-                trans = self._dict_domain_img_trans[na_domain]
+            if na_domain not in self.list_domain_tr:
+                trans = img_trans_te
             else:
-                trans = trans4all
+                if self._dict_domain_img_trans:
+                    trans = self._dict_domain_img_trans[na_domain]
+                else:
+                    trans = img_trans_tr
             root_img = self.dict_domain2imgroot[na_domain]
-            path2filelist = list_domain_path[na_domain]
+            path2filelist = dict_domain2pathfilepath[na_domain]
             path2filelist = os.path.expanduser(path2filelist)
             root_img = os.path.expanduser(root_img)
             dset = DsetImPathList(root_img, path2filelist, trans_img=trans,
                                   trans_target=mk_fun_label2onehot(
                                       len(self.list_str_y)))
             return dset
 
@@ -75,38 +81,44 @@
             """get_dset_by_domain.
 
             :param args:
             :param na_domain:
             :param split: for test set, use the whole
             """
             if not split:  # no train/val split for test domain
+                # the user is required to input tr, val, te file path
+                # if split=False, then only te is used, which contains
+                # the whole dataset
                 dset = self._get_complete_domain(
                     na_domain,
                     self._dict_domain2filepath_list_im_te)
+                # test set contains train+validation
                 return dset, dset  # @FIXME: avoid returning two identical
 
             dset = self._get_complete_domain(
                 na_domain,
-                self._dict_domain2filepath_list_im)
+                # read training set from user configuration
+                self._dict_domain2filepath_list_im_tr)
 
             dset_val = self._get_complete_domain(
                 na_domain,
+                # read validation set from user configuration
                 self._dict_domain2filepath_list_im_val)
 
             return dset, dset_val
 
         def conf(self, args):
             """conf.
-
             :param args:
             """
             self.list_str_y = list_str_y
             self.isize = isize
+            self.dict_class_label_ind2name = dict_class_label_ind2name
             self.dict_domain2imgroot = dict_domain2imgroot
-            self._dict_domain2filepath_list_im = dict_d2filepath_list_img
+            self._dict_domain2filepath_list_im_tr = dict_d2filepath_list_img_tr
             self._dict_domain2filepath_list_im_val = dict_d2filepath_list_img_val
             self._dict_domain2filepath_list_im_te = dict_d2filepath_list_img_te
             self.set_list_domains(list(self.dict_domain2imgroot.keys()))
 
         def init_business(self, args):
             """init_business.
```

### Comparing `domainlab-0.1.0/domainlab/tasks/task_utils.py` & `domainlab-0.1.2/domainlab/tasks/task_utils.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/tasks/utils_task.py` & `domainlab-0.1.2/domainlab/tasks/utils_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,29 @@
     :param ind: index
     """
     eye = torch.eye(dim)
     vec = eye[ind]
     return vec
 
 
-def mk_loader(dset, bsize, drop_last=True, shuffle=True):
+def mk_loader(dset, bsize,
+              drop_last=True,
+              shuffle=True,
+              num_workers=int(0)):
     """
     :param bs: batch size
     """
     if len(dset) < bsize:
         bsize = len(dset)
     loader = torch.utils.data.DataLoader(
         dataset=dset,
         batch_size=bsize,
         shuffle=shuffle,
-        # shuffle must be true so the last incomplete
-        # batch get used in anohter epoch
-        num_workers=int(0),   # @FIXME:
+        # @FIXME: shuffle must be true so the last incomplete batch get used in another epoch?
+        num_workers=num_workers,   # @FIXME: num_workers=int(0) can be slow?
         drop_last=drop_last)
     return loader
 
 
 class DsetDomainVecDecorator(Dataset):
     """
     decorate a pytorch dataset with a fixed vector representation of domain
@@ -234,15 +236,15 @@
     counter = 0
     batches = min(batches, len(l_iter))
     for _ in range(batches):
         img, vec_y, *other_vars = next(l_iter)
         class_label_ind_batch = tensor1hot2ind(vec_y)
 
         # get domain label
-        # Note 1: test loaders don't return domain labels (see NodeTaskDict.init_business)
+        # Note 1: test loaders don't return domain labels (see NodeTaskDictClassif.init_business)
         # Note 2: for train loaders domain label will be the 0th element of other_vars (see DsetDomainVecDecorator class above)
         has_domain_label_ind = False
         if not test:
             if other_vars:
                 domain_label_ind_batch = tensor1hot2ind(other_vars[0])
                 has_domain_label_ind = True
```

### Comparing `domainlab-0.1.0/domainlab/tasks/zoo_tasks.py` & `domainlab-0.1.2/domainlab/tasks/zoo_tasks.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/utils/flows_gen_img_model.py` & `domainlab-0.1.2/domainlab/utils/flows_gen_img_model.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/utils/get_git_tag.py` & `domainlab-0.1.2/domainlab/utils/get_git_tag.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/utils/override_interface.py` & `domainlab-0.1.2/domainlab/utils/override_interface.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/utils/perf_metrics.py` & `domainlab-0.1.2/domainlab/utils/perf_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """Classification Performance"""
+import numpy as np
 import torch
 from torchmetrics.classification import (AUC, AUROC, Accuracy, ConfusionMatrix,
                                          F1Score, Precision, Recall,
                                          Specificity)
 
 
 class PerfMetricClassif():
     """Classification Performance metrics"""
-    def __init__(self, num_classes, average='macro'):
+    def __init__(self, num_classes, agg_precision_recall_f1='macro'):
         super().__init__()
-        self.acc = Accuracy(num_classes=num_classes, average=average)
-        self.precision = Precision(num_classes=num_classes, average=average)
-        self.recall = Recall(num_classes=num_classes, average=average)
-        self.f1_score = F1Score(num_classes=num_classes, average=average)
-        self.auroc = AUROC(num_classes=num_classes, average=average)
+        self.acc = Accuracy(num_classes=num_classes, average='micro')
+        # NOTE: only micro aggregation make sense for acc
+        self.precision = Precision(num_classes=num_classes, average=agg_precision_recall_f1)
+        # Calculate the metric for each class separately, and average the
+        # metrics across classes (with equal weights for each class).
+        self.recall = Recall(num_classes=num_classes, average=agg_precision_recall_f1)
+        self.f1_score = F1Score(num_classes=num_classes, average=agg_precision_recall_f1)
+        # NOTE: auroc does nto support "micro" as aggregation
+        self.auroc = AUROC(num_classes=num_classes, average=agg_precision_recall_f1)
         self.specificity = Specificity(num_classes=num_classes,
-                                       average=average)
+                                       average=agg_precision_recall_f1)
         self.confmat = ConfusionMatrix(num_classes=num_classes)
 
-    def cal_metrics(self, model, loader_te, device, max_batches=None):
+    def cal_metrics(self, model, loader_te, device):
         """
         :param model:
         :param loader_te:
         :param device: for final test, GPU can be used
-        :param max_batches:
-                maximum number of iteration for data loader, used to
-                probe performance with less computation burden.
-                default None, which means to traverse the whole dataset
         """
         self.acc.reset()
         self.precision.reset()
         self.recall.reset()
         self.f1_score.reset()
         self.auroc.reset()
         self.specificity.reset()
@@ -38,35 +39,31 @@
         self.acc = self.acc.to(device)
         self.precision = self.precision.to(device)
         self.recall = self.recall.to(device)
         self.f1_score = self.f1_score.to(device)
         self.auroc = self.auroc.to(device)
         self.specificity = self.specificity.to(device)
         self.confmat = self.confmat.to(device)
-        model.eval()
         model_local = model.to(device)
-        if max_batches is None:
-            max_batches = len(loader_te)
+        model_local.eval()
         with torch.no_grad():
-            for i, (x_s, y_s, *_) in enumerate(loader_te):
+            for _, (x_s, y_s, *_) in enumerate(loader_te):
                 x_s, y_s = x_s.to(device), y_s.to(device)
                 _, prob, _, *_ = model_local.infer_y_vpicn(x_s)
                 _, target_label = torch.max(y_s, 1)
                 # self.acc.update(pred_label, target_label)  # bug found by xinyuejohn
                 # pred_label is (N,C) which we need to convert to (N)
                 # prob is (N,C) which is fine for torchmetrics
                 self.acc.update(prob, target_label)
                 self.precision.update(prob, target_label)
                 self.recall.update(prob, target_label)
                 self.specificity.update(prob, target_label)
                 self.f1_score.update(prob, target_label)
                 self.auroc.update(prob, target_label)
                 self.confmat.update(prob, target_label)
-                if i > max_batches:
-                    break
 
         acc_y = self.acc.compute()
         precision_y = self.precision.compute()
         recall_y = self.recall.compute()
         specificity_y = self.specificity.compute()
         f1_score_y = self.f1_score.compute()
         auroc_y = self.auroc.compute()
```

### Comparing `domainlab-0.1.0/domainlab/utils/test_img.py` & `domainlab-0.1.2/domainlab/utils/test_img.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/utils/u_import_net_module.py` & `domainlab-0.1.2/domainlab/utils/u_import_net_module.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/utils/utils_class.py` & `domainlab-0.1.2/domainlab/utils/utils_class.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/utils/utils_classif.py` & `domainlab-0.1.2/domainlab/utils/utils_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/domainlab/utils/utils_img_sav.py` & `domainlab-0.1.2/domainlab/utils/utils_img_sav.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.0/pyproject.toml` & `domainlab-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [tool.poetry]
 name = "domainlab"
-version = "0.1.0"
+version = "0.1.2"
 description = "Library of Domain Generalization"
 authors = ["Xudong Sun <smilesun.east@gmail.com>", "Alexej Gossmann <alexej.gossmann@fda.hhs.gov>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.23.4"
 matplotlib = "^3.6.1"
+seaborn = "0.12.2"
+snakemake = "7.21.0"
 torchmetrics = "^0.10.0"
 torch = "^1.12.0"
 torchvision = "^0.13.0"
 pillow = "^6.1.0"
 rich = "^13.3.1"
 pandas = "^1.5.1"
 scikit-learn = "^1.2.1"
```

### Comparing `domainlab-0.1.0/setup.py` & `domainlab-0.1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,14 +11,15 @@
  'domainlab.compos',
  'domainlab.compos.exp',
  'domainlab.compos.nn_zoo',
  'domainlab.compos.pcr',
  'domainlab.compos.vae',
  'domainlab.compos.vae.compos',
  'domainlab.dsets',
+ 'domainlab.exp_protocol',
  'domainlab.models',
  'domainlab.tasks',
  'domainlab.utils']
 
 package_data = \
 {'': ['*'], 'domainlab': ['uml/*']}
 
@@ -26,21 +27,23 @@
 ['matplotlib>=3.6.1,<4.0.0',
  'numpy>=1.23.4,<2.0.0',
  'pandas>=1.5.1,<2.0.0',
  'pillow>=6.1.0,<7.0.0',
  'pyyaml>=6.0,<7.0',
  'rich>=13.3.1,<14.0.0',
  'scikit-learn>=1.2.1,<2.0.0',
+ 'seaborn==0.12.2',
+ 'snakemake==7.21.0',
  'torch>=1.12.0,<2.0.0',
  'torchmetrics>=0.10.0,<0.11.0',
  'torchvision>=0.13.0,<0.14.0']
 
 setup_kwargs = {
     'name': 'domainlab',
-    'version': '0.1.0',
+    'version': '0.1.2',
     'description': 'Library of Domain Generalization',
     'long_description': 'None',
     'author': 'Xudong Sun',
     'author_email': 'smilesun.east@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `domainlab-0.1.0/PKG-INFO` & `domainlab-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: domainlab
-Version: 0.1.0
+Version: 0.1.2
 Summary: Library of Domain Generalization
 Author: Xudong Sun
 Author-email: smilesun.east@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: matplotlib (>=3.6.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: pillow (>=6.1.0,<7.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
+Requires-Dist: seaborn (==0.12.2)
+Requires-Dist: snakemake (==7.21.0)
 Requires-Dist: torch (>=1.12.0,<2.0.0)
 Requires-Dist: torchmetrics (>=0.10.0,<0.11.0)
 Requires-Dist: torchvision (>=0.13.0,<0.14.0)
```

