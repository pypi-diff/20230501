# Comparing `tmp/xturing-0.1.1.tar.gz` & `tmp/xturing-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xturing-0.1.1.tar", last modified: Wed Apr 19 13:02:09 2023, max compression
+gzip compressed data, was "xturing-0.1.2.tar", last modified: Mon May  1 17:25:29 2023, max compression
```

## Comparing `xturing-0.1.1.tar` & `xturing-0.1.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.248906 xturing-0.1.1/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    11357 2023-03-20 07:53:44.000000 xturing-0.1.1/LICENSE
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       34 2023-03-29 09:34:15.000000 xturing-0.1.1/MANIFEST.in
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    21624 2023-04-19 13:02:09.248351 xturing-0.1.1/PKG-INFO
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     7162 2023-04-18 12:33:45.000000 xturing-0.1.1/README.md
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2203 2023-04-19 13:01:46.000000 xturing-0.1.1/pyproject.toml
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       38 2023-04-19 13:02:09.249064 xturing-0.1.1/setup.cfg
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.194814 xturing-0.1.1/src/
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.202283 xturing-0.1.1/src/xturing/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       22 2023-04-19 13:01:46.000000 xturing-0.1.1/src/xturing/__about__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      438 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/__init__.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.207892 xturing-0.1.1/src/xturing/cli/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      561 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/cli/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2042 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/cli/api.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      989 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/cli/chat.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      131 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/cli/ui.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.211762 xturing-0.1.1/src/xturing/config/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      569 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/config/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      972 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/config/config_data_classes.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2701 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/config/finetuning_config.yaml
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2739 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/config/generation_config.yaml
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1862 2023-04-15 21:30:16.000000 xturing-0.1.1/src/xturing/config/read_config.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.214383 xturing-0.1.1/src/xturing/datasets/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      436 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/datasets/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      199 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/datasets/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     8179 2023-04-05 17:10:03.000000 xturing-0.1.1/src/xturing/datasets/instruction_dataset.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      222 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/datasets/text2image_dataset.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1830 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/datasets/text_dataset.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.218672 xturing-0.1.1/src/xturing/engines/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3182 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      272 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/engines/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1871 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/bloom_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6746 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/causal.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1923 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/cerebras_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      804 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/distilgpt2_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1755 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/galactica_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1446 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/gpt2_engine.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2885 2023-04-15 21:30:16.000000 xturing-0.1.1/src/xturing/engines/gptj_engine.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.219527 xturing-0.1.1/src/xturing/engines/gptj_utils/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/engines/gptj_utils/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     7690 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/engines/gptj_utils/gptj.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6256 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/llama_engine.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.220496 xturing-0.1.1/src/xturing/engines/llama_utils/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       65 2023-03-26 14:55:44.000000 xturing-0.1.1/src/xturing/engines/llama_utils/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    44486 2023-03-26 14:55:44.000000 xturing-0.1.1/src/xturing/engines/llama_utils/llama.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.222578 xturing-0.1.1/src/xturing/engines/lora_engine/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       73 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/lora_engine/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    42467 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/lora_engine/lora.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3556 2023-04-15 21:30:16.000000 xturing-0.1.1/src/xturing/engines/lora_engine/save_and_load.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-04-15 21:30:16.000000 xturing-0.1.1/src/xturing/engines/lora_engine/test.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1830 2023-04-06 13:15:31.000000 xturing-0.1.1/src/xturing/engines/opt_engine.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.224038 xturing-0.1.1/src/xturing/engines/quant_utils/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       59 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/quant_utils/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6803 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/engines/quant_utils/custom_autotune.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    28505 2023-04-19 13:01:46.000000 xturing-0.1.1/src/xturing/engines/quant_utils/quant.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.226862 xturing-0.1.1/src/xturing/model_apis/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      864 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/model_apis/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1827 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/model_apis/ai21.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      573 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/model_apis/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1847 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/model_apis/cohere.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     4600 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/model_apis/openai.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.232201 xturing-0.1.1/src/xturing/models/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2566 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/models/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2067 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/models/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1084 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/bloom.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     7132 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/causal.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1135 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/cerebras.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      579 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/distilgpt2.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1152 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/galactica.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1033 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/gpt2.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1067 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/gptj.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2100 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/models/llama.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1050 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/models/opt.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      542 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/models/stable_diffusion.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.234366 xturing-0.1.1/src/xturing/preprocessors/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      137 2023-03-26 14:55:44.000000 xturing-0.1.1/src/xturing/preprocessors/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      484 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/preprocessors/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     4582 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/preprocessors/instruction_collator.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2252 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/preprocessors/text_collator.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      642 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/registry.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.237815 xturing-0.1.1/src/xturing/self_instruct/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/self_instruct/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     9891 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/self_instruct/bootstrap_instructions.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     5490 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/self_instruct/generate_instances.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3737 2023-04-03 17:26:37.000000 xturing-0.1.1/src/xturing/self_instruct/identify_if_classification.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    14280 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/self_instruct/prepare_for_finetuning.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2198 2023-04-05 17:10:03.000000 xturing-0.1.1/src/xturing/self_instruct/prepare_seed_tasks.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.239038 xturing-0.1.1/src/xturing/self_instruct/templates/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3580 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/self_instruct/templates/clf_task_template.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    12674 2023-03-29 10:14:08.000000 xturing-0.1.1/src/xturing/self_instruct/templates/instance_gen_template.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.241073 xturing-0.1.1/src/xturing/trainers/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       78 2023-03-26 14:55:44.000000 xturing-0.1.1/src/xturing/trainers/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      233 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/trainers/base.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6049 2023-04-19 13:01:46.000000 xturing-0.1.1/src/xturing/trainers/lightning_trainer.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.242192 xturing-0.1.1/src/xturing/ui/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/ui/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    13646 2023-04-03 17:19:47.000000 xturing-0.1.1/src/xturing/ui/playground.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.247081 xturing-0.1.1/src/xturing/utils/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        0 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/utils/__init__.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      215 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/utils/external_loggers.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3075 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/utils/hub.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      304 2023-03-26 14:55:44.000000 xturing-0.1.1/src/xturing/utils/interactive.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     2147 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/utils/logging.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      621 2023-03-24 13:26:24.000000 xturing-0.1.1/src/xturing/utils/loss_fns.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     1366 2023-04-03 17:19:41.000000 xturing-0.1.1/src/xturing/utils/notebooks.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     6886 2023-04-18 12:33:45.000000 xturing-0.1.1/src/xturing/utils/text_splitter.py
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3803 2023-04-05 17:10:03.000000 xturing-0.1.1/src/xturing/utils/utils.py
-drwxr-xr-x   0 sarthaklangde   (501) staff       (20)        0 2023-04-19 13:02:09.205715 xturing-0.1.1/src/xturing.egg-info/
--rw-r--r--   0 sarthaklangde   (501) staff       (20)    21624 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/PKG-INFO
--rw-r--r--   0 sarthaklangde   (501) staff       (20)     3201 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/SOURCES.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        1 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/dependency_links.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)       48 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/entry_points.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)      237 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/requires.txt
--rw-r--r--   0 sarthaklangde   (501) staff       (20)        8 2023-04-19 13:02:09.000000 xturing-0.1.1/src/xturing.egg-info/top_level.txt
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.384961 xturing-0.1.2/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    11357 2023-03-20 17:06:03.000000 xturing-0.1.2/LICENSE
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       34 2023-03-29 09:39:04.000000 xturing-0.1.2/MANIFEST.in
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    21624 2023-05-01 17:25:29.384961 xturing-0.1.2/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     7162 2023-05-01 17:21:49.000000 xturing-0.1.2/README.md
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2203 2023-05-01 17:21:49.000000 xturing-0.1.2/pyproject.toml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-05-01 17:25:29.384961 xturing-0.1.2/setup.cfg
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.352961 xturing-0.1.2/src/
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.356961 xturing-0.1.2/src/xturing/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       22 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/__about__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      438 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/__init__.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.356961 xturing-0.1.2/src/xturing/cli/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      561 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/cli/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2042 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/cli/api.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      989 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/cli/chat.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      131 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/cli/ui.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.360961 xturing-0.1.2/src/xturing/config/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      569 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/config/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      972 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/config/config_data_classes.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2701 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/config/finetuning_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2517 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/config/generation_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1862 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/config/read_config.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.360961 xturing-0.1.2/src/xturing/datasets/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      436 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/datasets/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      199 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/datasets/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8179 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/datasets/instruction_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      222 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/datasets/text2image_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/datasets/text_dataset.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.364961 xturing-0.1.2/src/xturing/engines/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3182 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      272 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/engines/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1871 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/bloom_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6742 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1923 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/cerebras_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      804 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/distilgpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1755 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/galactica_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1446 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/gpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2885 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/gptj_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.364961 xturing-0.1.2/src/xturing/engines/gptj_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/engines/gptj_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8053 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/gptj_utils/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6438 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/llama_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.364961 xturing-0.1.2/src/xturing/engines/llama_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       65 2023-03-24 15:40:08.000000 xturing-0.1.2/src/xturing/engines/llama_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    44486 2023-03-24 15:40:08.000000 xturing-0.1.2/src/xturing/engines/llama_utils/llama.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.368961 xturing-0.1.2/src/xturing/engines/lora_engine/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       73 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/lora_engine/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    42467 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/lora_engine/lora.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3556 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/lora_engine/save_and_load.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/lora_engine/test.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/opt_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.368961 xturing-0.1.2/src/xturing/engines/quant_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       59 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/quant_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6803 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/quant_utils/custom_autotune.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    28505 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/quant_utils/quant.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.372961 xturing-0.1.2/src/xturing/model_apis/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      864 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/model_apis/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1827 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/model_apis/ai21.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      573 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/model_apis/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1847 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/model_apis/cohere.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4600 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/model_apis/openai.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.376961 xturing-0.1.2/src/xturing/models/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2566 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/models/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2067 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/models/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1084 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/bloom.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     7132 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1135 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/cerebras.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      579 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/distilgpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1152 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/galactica.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1033 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/gpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2100 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/models/llama.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1050 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/opt.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      542 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/models/stable_diffusion.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.376961 xturing-0.1.2/src/xturing/preprocessors/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      137 2023-03-24 15:40:08.000000 xturing-0.1.2/src/xturing/preprocessors/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      484 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/preprocessors/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4582 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/preprocessors/instruction_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2252 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/preprocessors/text_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      642 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/registry.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.380961 xturing-0.1.2/src/xturing/self_instruct/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/self_instruct/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     9891 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/self_instruct/bootstrap_instructions.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     5490 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/self_instruct/generate_instances.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3737 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/self_instruct/identify_if_classification.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    14280 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/self_instruct/prepare_for_finetuning.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2198 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/self_instruct/prepare_seed_tasks.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.380961 xturing-0.1.2/src/xturing/self_instruct/templates/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3580 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/self_instruct/templates/clf_task_template.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    12674 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/self_instruct/templates/instance_gen_template.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.380961 xturing-0.1.2/src/xturing/trainers/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       78 2023-03-24 15:40:08.000000 xturing-0.1.2/src/xturing/trainers/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      233 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/trainers/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6049 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/trainers/lightning_trainer.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.380961 xturing-0.1.2/src/xturing/ui/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/ui/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    13646 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/ui/playground.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.384961 xturing-0.1.2/src/xturing/utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      215 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/utils/external_loggers.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3135 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/utils/hub.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      304 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/utils/interactive.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2147 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/utils/logging.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      621 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/utils/loss_fns.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1366 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/utils/notebooks.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6886 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/utils/text_splitter.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3803 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/utils/utils.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.356961 xturing-0.1.2/src/xturing.egg-info/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    21624 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3201 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/entry_points.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      237 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/requires.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        8 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/top_level.txt
```

### Comparing `xturing-0.1.1/LICENSE` & `xturing-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/PKG-INFO` & `xturing-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xturing-0.1.1/README.md` & `xturing-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/pyproject.toml` & `xturing-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xturing"
-version = "0.1.1"
+version = "0.1.2"
 description = "Fine-tuning, evaluation and data generation for LLMs"
 
 authors = [
     { name = "Glenn Ko", email = "glenn@stochastic.ai" },
     { name = "Yuji Chai", email = "yuji.chai@stochastic.ai" },
     { name = "Roman Ageev", email = "roman.ageev@stochastic.ai" },
     { name = "Toan Do", email = "toan.do@stochastic.ai" },
@@ -39,15 +39,15 @@
     "data-generation",
     "training",
     "distributed",
 ]
 dependencies = [
     "torch >= 1.9.0",
     "pytorch-lightning",
-    "transformers==4.27.3",
+    "transformers==4.28.1",
     "datasets",
     "evaluate",
     "bitsandbytes==0.37.2",
     "sentencepiece",
     "deepspeed",
     "gradio",
     "click",
```

### Comparing `xturing-0.1.1/src/xturing/cli/__init__.py` & `xturing-0.1.2/src/xturing/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/cli/api.py` & `xturing-0.1.2/src/xturing/cli/api.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/cli/chat.py` & `xturing-0.1.2/src/xturing/cli/chat.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/config/__init__.py` & `xturing-0.1.2/src/xturing/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/config/config_data_classes.py` & `xturing-0.1.2/src/xturing/config/config_data_classes.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/config/finetuning_config.yaml` & `xturing-0.1.2/src/xturing/config/finetuning_config.yaml`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/config/generation_config.yaml` & `xturing-0.1.2/src/xturing/config/generation_config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -16,18 +16,16 @@
 # Contrastive search
 llama_lora:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
-# Contrastive search
+# Greedy search
 llama_lora_int8:
-  penalty_alpha: 0.6
-  top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
 llama_lora_int4:
   penalty_alpha: 0.6
   top_k: 4
@@ -44,18 +42,16 @@
 # Contrastive search
 gptj_lora:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
-# Contrastive search
+# Greedy search
 gptj_lora_int8:
-  penalty_alpha: 0.6
-  top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Top-p sampling
 gpt2:
   do_sample: true
   top_k: 0
@@ -100,18 +96,16 @@
 # Contrastive search
 galactica_lora:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
-# Contrastive search
+# Greedy search
 galactica_lora_int8:
-  penalty_alpha: 0.6
-  top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
 opt:
   penalty_alpha: 0.6
   top_k: 4
@@ -121,18 +115,16 @@
 # Contrastive search
 opt_lora:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
-# Contrastive search
+# Greedy search
 opt_lora_int8:
-  penalty_alpha: 0.6
-  top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
 cerebras:
   penalty_alpha: 0.6
   top_k: 4
@@ -142,18 +134,16 @@
 # Contrastive search
 cerebras_lora:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
-# Contrastive search
+# Greedy search
 cerebras_lora_int8:
-  penalty_alpha: 0.6
-  top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
 bloom:
   penalty_alpha: 0.6
   top_k: 4
@@ -163,13 +153,11 @@
 # Contrastive search
 bloom_lora:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
-# Contrastive search
+# Greedy search
 bloom_lora_int8:
-  penalty_alpha: 0.6
-  top_k: 4
   max_new_tokens: 256
   do_sample: false
```

### Comparing `xturing-0.1.1/src/xturing/config/read_config.py` & `xturing-0.1.2/src/xturing/config/read_config.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/datasets/instruction_dataset.py` & `xturing-0.1.2/src/xturing/datasets/instruction_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/datasets/text_dataset.py` & `xturing-0.1.2/src/xturing/datasets/text_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/__init__.py` & `xturing-0.1.2/src/xturing/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/bloom_engine.py` & `xturing-0.1.2/src/xturing/engines/bloom_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/causal.py` & `xturing-0.1.2/src/xturing/engines/causal.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         if weights_path is not None and exists_lora_config_file(weights_path):
             self.model = LoraModel.from_pretrained(self.base_model, weights_path)
         elif weights_path is not None and exists_xturing_config_file(weights_path):
             self.model = LoraModel(lora_config, self.model)
             model_weights_path = str(Path(weights_path).resolve() / "pytorch_model.bin")
             self.model.load_state_dict(
                 torch.load(
-                    model_weights_path  # , map_location=torch.device(DEFAULT_DEVICE)
+                    model_weights_path, map_location=torch.device(DEFAULT_DEVICE)
                 )
             )
         else:
             self.model = LoraModel(lora_config, self.model)
             self.model.print_trainable_parameters()
 
         self.loss_fct = CrossEntropyLoss()
```

### Comparing `xturing-0.1.1/src/xturing/engines/cerebras_engine.py` & `xturing-0.1.2/src/xturing/engines/cerebras_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/distilgpt2_engine.py` & `xturing-0.1.2/src/xturing/engines/distilgpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/galactica_engine.py` & `xturing-0.1.2/src/xturing/engines/galactica_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/gpt2_engine.py` & `xturing-0.1.2/src/xturing/engines/gpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/gptj_engine.py` & `xturing-0.1.2/src/xturing/engines/gptj_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/gptj_utils/gptj.py` & `xturing-0.1.2/src/xturing/engines/gptj_utils/gptj.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,25 @@
+from typing import Optional, Tuple, Union
+
 import torch
 import torch.nn as nn
-from typing import Optional, Union, Tuple
-from transformers.models.gptj.modeling_gptj import (
-    apply_rotary_pos_emb,
-    fixed_pos_embedding,
-)
+from transformers.models.gptj.modeling_gptj import apply_rotary_pos_emb
+
+
+def fixed_pos_embedding(x, seq_dim=1, seq_len=None):
+    dim = x.shape[-1]
+    if seq_len is None:
+        seq_len = x.shape[seq_dim]
+    inv_freq = 1.0 / (10000 ** (torch.arange(0, dim, 2) / dim))
+    sinusoid_inp = (
+        torch.einsum("i , j -> i j", torch.arange(seq_len), inv_freq)
+        .to(x.device)
+        .float()
+    )
+    return torch.sin(sinusoid_inp), torch.cos(sinusoid_inp)
 
 
 class GPTJAttention(nn.Module):
     def __init__(self, config):
         super().__init__()
 
         max_positions = config.max_position_embeddings
```

### Comparing `xturing-0.1.1/src/xturing/engines/llama_engine.py` & `xturing-0.1.2/src/xturing/engines/llama_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
-import transformers
 
 import torch
+import transformers
 from torch import nn
 
 from xturing.engines.causal import CausalEngine, CausalLoraEngine
 from xturing.engines.llama_utils import LlamaConfig, LlamaForCausalLM, LlamaTokenizer
 from xturing.engines.lora_engine import prepare_model_for_int8_training
-from xturing.engines.quant_utils import make_quant, autotune_warmup
+from xturing.engines.quant_utils import autotune_warmup, make_quant
 from xturing.utils.hub import ModelHub
 
+
 class LLamaEngine(CausalEngine):
     config_name: str = "llama_engine"
 
     def __init__(self, weights_path: Optional[Union[str, Path]] = None):
         model_name = "aleksickx/llama-7b-hf"
         model = LlamaForCausalLM.from_pretrained(model_name, torch_dtype=torch.float16)
         tokenizer = LlamaTokenizer.from_pretrained(model_name, add_bos_token=False)
@@ -98,67 +99,76 @@
             weights_path=weights_path,
             model=model,
             tokenizer=tokenizer,
             load_8bit=True,
             target_modules=["q_proj", "v_proj"],
         )
 
-def find_layers(module, layers=[nn.Conv2d, nn.Linear], name=''):
+
+def find_layers(module, layers=[nn.Conv2d, nn.Linear], name=""):
     if type(module) in layers:
         return {name: module}
     res = {}
     for name1, child in module.named_children():
-        res.update(find_layers(
-            child, layers=layers, name=name + '.' + name1 if name != '' else name1
-        ))
+        res.update(
+            find_layers(
+                child, layers=layers, name=name + "." + name1 if name != "" else name1
+            )
+        )
     return res
 
+
 class LlamaLoraInt4Engine(CausalLoraEngine):
     config_name: str = "llama_lora_int4_engine"
 
     def __init__(self, weights_path: Optional[Union[str, Path]] = None):
-        model_name = "decapoda-research/llama-7b-hf" 
+        model_name = "decapoda-research/llama-7b-hf"
 
         if weights_path is None:
-            weights_path = ModelHub().load("x/llama_lora_int4")            
+            weights_path = ModelHub().load("x/llama_lora_int4")
 
         config = LlamaConfig.from_pretrained(model_name)
 
         saved_kaiming_uniform_ = torch.nn.init.kaiming_uniform_
         saved_uniform_ = torch.nn.init.uniform_
         saved_normal_ = torch.nn.init.normal_
 
         def noop(*args, **kwargs):
             pass
-        
-        torch.nn.init.kaiming_uniform_ = noop 
-        torch.nn.init.uniform_ = noop 
-        torch.nn.init.normal_ = noop 
+
+        torch.nn.init.kaiming_uniform_ = noop
+        torch.nn.init.uniform_ = noop
+        torch.nn.init.normal_ = noop
 
         torch.set_default_dtype(torch.half)
         transformers.modeling_utils._init_weights = False
         torch.set_default_dtype(torch.half)
         model = LlamaForCausalLM(config)
         torch.set_default_dtype(torch.float)
         model = model.eval()
 
         layers = find_layers(model)
 
-        for name in ['lm_head']:
+        for name in ["lm_head"]:
             if name in layers:
                 del layers[name]
-        
+
         wbits = 4
         groupsize = 128
-        warmup_autotune=True
-        
+        warmup_autotune = True
+
         make_quant(model, layers, wbits, groupsize)
-        
 
-        model.load_state_dict(torch.load(weights_path / Path("pytorch_model.bin")), strict=False)
+        state_dict = torch.load(
+            weights_path / Path("pytorch_model.bin"), map_location="cpu"
+        )
+        new_state_dict = {}
+        for key, value in state_dict.items():
+            new_state_dict[key[6:]] = value
+        model.load_state_dict(new_state_dict, strict=False)
 
         if warmup_autotune:
             autotune_warmup(model)
 
         model.seqlen = 2048
 
         model.gptq = True
@@ -167,18 +177,18 @@
         model.enable_input_require_grads()
 
         tokenizer = LlamaTokenizer.from_pretrained(model_name, add_bos_token=False)
         tokenizer.pad_token = tokenizer.eos_token
         tokenizer.pad_token_id = tokenizer.eos_token_id
 
         super().__init__(
-            model=model, 
+            model=model,
             tokenizer=tokenizer,
             target_modules=[
                 "q_proj",
                 "v_proj",
-            ]
+            ],
         )
 
         torch.nn.init.kaiming_uniform_ = saved_kaiming_uniform_
         torch.nn.init.uniform_ = saved_uniform_
         torch.nn.init.normal_ = saved_normal_
```

### Comparing `xturing-0.1.1/src/xturing/engines/llama_utils/llama.py` & `xturing-0.1.2/src/xturing/engines/llama_utils/llama.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/lora_engine/lora.py` & `xturing-0.1.2/src/xturing/engines/lora_engine/lora.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/lora_engine/save_and_load.py` & `xturing-0.1.2/src/xturing/engines/lora_engine/save_and_load.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/opt_engine.py` & `xturing-0.1.2/src/xturing/engines/opt_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/quant_utils/custom_autotune.py` & `xturing-0.1.2/src/xturing/engines/quant_utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/engines/quant_utils/quant.py` & `xturing-0.1.2/src/xturing/engines/quant_utils/quant.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/model_apis/__init__.py` & `xturing-0.1.2/src/xturing/model_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/model_apis/ai21.py` & `xturing-0.1.2/src/xturing/model_apis/ai21.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/model_apis/base.py` & `xturing-0.1.2/src/xturing/model_apis/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/model_apis/cohere.py` & `xturing-0.1.2/src/xturing/model_apis/cohere.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/model_apis/openai.py` & `xturing-0.1.2/src/xturing/model_apis/openai.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/__init__.py` & `xturing-0.1.2/src/xturing/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/base.py` & `xturing-0.1.2/src/xturing/models/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/bloom.py` & `xturing-0.1.2/src/xturing/models/bloom.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/causal.py` & `xturing-0.1.2/src/xturing/models/causal.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/cerebras.py` & `xturing-0.1.2/src/xturing/models/cerebras.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/distilgpt2.py` & `xturing-0.1.2/src/xturing/models/distilgpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/galactica.py` & `xturing-0.1.2/src/xturing/models/galactica.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/gpt2.py` & `xturing-0.1.2/src/xturing/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/gptj.py` & `xturing-0.1.2/src/xturing/models/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/llama.py` & `xturing-0.1.2/src/xturing/models/llama.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/opt.py` & `xturing-0.1.2/src/xturing/models/opt.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/models/stable_diffusion.py` & `xturing-0.1.2/src/xturing/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/preprocessors/instruction_collator.py` & `xturing-0.1.2/src/xturing/preprocessors/instruction_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/preprocessors/text_collator.py` & `xturing-0.1.2/src/xturing/preprocessors/text_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/registry.py` & `xturing-0.1.2/src/xturing/registry.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/self_instruct/bootstrap_instructions.py` & `xturing-0.1.2/src/xturing/self_instruct/bootstrap_instructions.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/self_instruct/generate_instances.py` & `xturing-0.1.2/src/xturing/self_instruct/generate_instances.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/self_instruct/identify_if_classification.py` & `xturing-0.1.2/src/xturing/self_instruct/identify_if_classification.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/self_instruct/prepare_for_finetuning.py` & `xturing-0.1.2/src/xturing/self_instruct/prepare_for_finetuning.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/self_instruct/prepare_seed_tasks.py` & `xturing-0.1.2/src/xturing/self_instruct/prepare_seed_tasks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/self_instruct/templates/clf_task_template.py` & `xturing-0.1.2/src/xturing/self_instruct/templates/clf_task_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/self_instruct/templates/instance_gen_template.py` & `xturing-0.1.2/src/xturing/self_instruct/templates/instance_gen_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/trainers/lightning_trainer.py` & `xturing-0.1.2/src/xturing/trainers/lightning_trainer.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/ui/playground.py` & `xturing-0.1.2/src/xturing/ui/playground.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/utils/hub.py` & `xturing-0.1.2/src/xturing/utils/hub.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,22 +51,24 @@
 
                 print(f"Downloaded model {model_name} from {url}")
 
                 # if zip has folder with model, move files to root
 
                 entries = list(model_dir.glob("*"))
 
-                if len(entries) == 1 and entries[0].is_dir():
+                while len(entries) == 1 and entries[0].is_dir():
                     single_folder = entries[0]
 
                     for item in single_folder.iterdir():
                         shutil.move(str(item), str(model_dir / item.name))
 
                     shutil.rmtree(single_folder)
 
+                    entries = list(model_dir.glob("*"))
+
             except Exception as e:
                 print(f"Error downloading model {model_name} from {url}: {e}")
                 raise e
             finally:
                 zip_filename.unlink()
 
         return model_dir
```

### Comparing `xturing-0.1.1/src/xturing/utils/logging.py` & `xturing-0.1.2/src/xturing/utils/logging.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/utils/loss_fns.py` & `xturing-0.1.2/src/xturing/utils/loss_fns.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/utils/notebooks.py` & `xturing-0.1.2/src/xturing/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/utils/text_splitter.py` & `xturing-0.1.2/src/xturing/utils/text_splitter.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing/utils/utils.py` & `xturing-0.1.2/src/xturing/utils/utils.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.1/src/xturing.egg-info/PKG-INFO` & `xturing-0.1.2/src/xturing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xturing-0.1.1/src/xturing.egg-info/SOURCES.txt` & `xturing-0.1.2/src/xturing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

