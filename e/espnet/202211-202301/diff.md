# Comparing `tmp/espnet-202211.tar.gz` & `tmp/espnet-202301.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espnet-202211.tar", last modified: Sun Dec 11 23:52:21 2022, max compression
+gzip compressed data, was "espnet-202301.tar", last modified: Wed Feb  1 10:50:34 2023, max compression
```

## Comparing `espnet-202211.tar` & `espnet-202301.tar`

### file list

```diff
@@ -1,787 +1,877 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.561892 espnet-202211/
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2022-12-11 23:52:12.000000 espnet-202211/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    65341 2022-12-11 23:52:21.561892 espnet-202211/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    57649 2022-12-11 23:52:12.000000 espnet-202211/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.465891 espnet-202211/espnet/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2022-12-11 23:52:12.000000 espnet-202211/espnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.465891 espnet-202211/espnet/asr/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2022-12-11 23:52:12.000000 espnet-202211/espnet/asr/asr_mix_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2022-12-11 23:52:12.000000 espnet-202211/espnet/asr/asr_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.465891 espnet-202211/espnet/asr/chainer_backend/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/asr/chainer_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19572 2022-12-11 23:52:12.000000 espnet-202211/espnet/asr/chainer_backend/asr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.469891 espnet-202211/espnet/asr/pytorch_backend/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/asr/pytorch_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61311 2022-12-11 23:52:12.000000 espnet-202211/espnet/asr/pytorch_backend/asr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10707 2022-12-11 23:52:12.000000 espnet-202211/espnet/asr/pytorch_backend/asr_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    22054 2022-12-11 23:52:12.000000 espnet-202211/espnet/asr/pytorch_backend/asr_mix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2022-12-11 23:52:12.000000 espnet-202211/espnet/asr/pytorch_backend/recog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.469891 espnet-202211/espnet/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13210 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/asr_align.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5778 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/asr_enhance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13800 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/asr_recog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22288 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/asr_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8939 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/lm_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14923 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/mt_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5956 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/mt_trans.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17332 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/st_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5855 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/st_trans.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5267 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/tts_decode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10680 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/tts_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5094 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/vc_decode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10830 2022-12-11 23:52:12.000000 espnet-202211/espnet/bin/vc_train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.469891 espnet-202211/espnet/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-11 23:52:12.000000 espnet-202211/espnet/distributed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.473891 espnet-202211/espnet/lm/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/lm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.473891 espnet-202211/espnet/lm/chainer_backend/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/lm/chainer_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2022-12-11 23:52:12.000000 espnet-202211/espnet/lm/chainer_backend/extlm.py
--rw-r--r--   0 runner    (1001) docker     (123)    18247 2022-12-11 23:52:12.000000 espnet-202211/espnet/lm/chainer_backend/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2022-12-11 23:52:12.000000 espnet-202211/espnet/lm/lm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.473891 espnet-202211/espnet/lm/pytorch_backend/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/lm/pytorch_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2022-12-11 23:52:12.000000 espnet-202211/espnet/lm/pytorch_backend/extlm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2022-12-11 23:52:12.000000 espnet-202211/espnet/lm/pytorch_backend/lm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.473891 espnet-202211/espnet/mt/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/mt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2022-12-11 23:52:12.000000 espnet-202211/espnet/mt/mt_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.473891 espnet-202211/espnet/mt/pytorch_backend/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/mt/pytorch_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2022-12-11 23:52:12.000000 espnet-202211/espnet/mt/pytorch_backend/mt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.477891 espnet-202211/espnet/nets/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/asr_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/batch_beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/batch_beam_search_online.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/batch_beam_search_online_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)    19111 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    30731 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/beam_search_transducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.477891 espnet-202211/espnet/nets/chainer_backend/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/asr_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/ctc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/deterministic_embed_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/e2e_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/e2e_asr_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/nets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.477891 espnet-202211/espnet/nets/chainer_backend/rnn/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/rnn/attentions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/rnn/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11061 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/rnn/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/rnn/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.481891 espnet-202211/espnet/nets/chainer_backend/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/ctc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/decoder_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/encoder_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/label_smoothing_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/positionwise_feed_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/subsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11816 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/chainer_backend/transformer/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    13950 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/ctc_prefix_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/e2e_asr_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/e2e_mt_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/lm_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/mt_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.485891 espnet-202211/espnet/nets/pytorch_backend/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.489891 espnet-202211/espnet/nets/pytorch_backend/conformer/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/conformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/conformer/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/conformer/contextual_block_encoder_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/conformer/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/conformer/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/conformer/encoder_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/conformer/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9928 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/ctc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19379 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_asr_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_asr_maskctc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30840 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_asr_mix.py
--rw-r--r--   0 runner    (1001) docker     (123)    18183 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_asr_mix_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31487 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_asr_mulenc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18123 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_asr_transducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22562 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_asr_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13630 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_mt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16007 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_mt_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24057 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_st.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_st_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22657 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_st_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34348 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_tts_fastspeech.py
--rw-r--r--   0 runner    (1001) docker     (123)    34041 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_tts_tacotron2.py
--rw-r--r--   0 runner    (1001) docker     (123)    45641 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_tts_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30409 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_vc_tacotron2.py
--rw-r--r--   0 runner    (1001) docker     (123)    46109 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/e2e_vc_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.489891 espnet-202211/espnet/nets/pytorch_backend/fastspeech/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/fastspeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/fastspeech/duration_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/fastspeech/duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/fastspeech/length_regulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.489891 espnet-202211/espnet/nets/pytorch_backend/frontends/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/frontends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/frontends/beamformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/frontends/dnn_beamformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/frontends/dnn_wpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/frontends/feature_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/frontends/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/frontends/mask_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/gtn_ctc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.489891 espnet-202211/espnet/nets/pytorch_backend/lm/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/lm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14561 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/lm/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/lm/seq_rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/lm/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.489891 espnet-202211/espnet/nets/pytorch_backend/maskctc/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/maskctc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/maskctc/add_mask_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/maskctc/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    16551 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/nets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.493891 espnet-202211/espnet/nets/pytorch_backend/rnn/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/rnn/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)    66963 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/rnn/attentions.py
--rw-r--r--   0 runner    (1001) docker     (123)    49021 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/rnn/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    14183 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/rnn/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.493891 espnet-202211/espnet/nets/pytorch_backend/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/streaming/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/streaming/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.493891 espnet-202211/espnet/nets/pytorch_backend/tacotron2/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/tacotron2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/tacotron2/cbhg.py
--rw-r--r--   0 runner    (1001) docker     (123)    24496 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/tacotron2/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/tacotron2/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.497891 espnet-202211/espnet/nets/pytorch_backend/transducer/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10628 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    16356 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/conv1d_nets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/custom_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/custom_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/error_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/joint_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18464 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/rnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15051 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/transducer_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/transformer_decoder_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transducer/vgg2l.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.501891 espnet-202211/espnet/nets/pytorch_backend/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/add_sos_eos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)    11646 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/contextual_block_encoder_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13734 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/decoder_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/dynamic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/dynamic_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12758 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/encoder_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/encoder_mix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/label_smoothing_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/lightconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/lightconv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/longformer_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/multi_layer_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/positionwise_feed_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/repeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/subsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/transformer/subsampling_without_posenc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/pytorch_backend/wavenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/scorer_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.501891 espnet-202211/espnet/nets/scorers/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/scorers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/scorers/ctc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/scorers/length_bonus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/scorers/ngram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/st_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/transducer_decoder_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2022-12-11 23:52:12.000000 espnet-202211/espnet/nets/tts_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.501891 espnet-202211/espnet/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2022-12-11 23:52:12.000000 espnet-202211/espnet/optimizer/chainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2022-12-11 23:52:12.000000 espnet-202211/espnet/optimizer/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2022-12-11 23:52:12.000000 espnet-202211/espnet/optimizer/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2022-12-11 23:52:12.000000 espnet-202211/espnet/optimizer/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.505891 espnet-202211/espnet/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2022-12-11 23:52:12.000000 espnet-202211/espnet/scheduler/chainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2022-12-11 23:52:12.000000 espnet-202211/espnet/scheduler/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2022-12-11 23:52:12.000000 espnet-202211/espnet/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.505891 espnet-202211/espnet/st/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/st/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.505891 espnet-202211/espnet/st/pytorch_backend/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/st/pytorch_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22845 2022-12-11 23:52:12.000000 espnet-202211/espnet/st/pytorch_backend/st.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.505891 espnet-202211/espnet/transform/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-11 23:52:12.000000 espnet-202211/espnet/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2022-12-11 23:52:12.000000 espnet-202211/espnet/transform/add_deltas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2022-12-11 23:52:12.000000 espnet-202211/espnet/transform/channel_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2022-12-11 23:52:12.000000 espnet-202211/espnet/transform/cmvn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2022-12-11 23:52:12.000000 espnet-202211/espnet/transform/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2022-12-11 23:52:12.000000 espnet-202211/espnet/transform/perturb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2022-12-11 23:52:12.000000 espnet-202211/espnet/transform/spec_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2022-12-11 23:52:12.000000 espnet-202211/espnet/transform/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2022-12-11 23:52:12.000000 espnet-202211/espnet/transform/transform_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2022-12-11 23:52:12.000000 espnet-202211/espnet/transform/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2022-12-11 23:52:12.000000 espnet-202211/espnet/transform/wpe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.505891 espnet-202211/espnet/tts/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/tts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.505891 espnet-202211/espnet/tts/pytorch_backend/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/tts/pytorch_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26532 2022-12-11 23:52:12.000000 espnet-202211/espnet/tts/pytorch_backend/tts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.509891 espnet-202211/espnet/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/check_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/cli_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/cli_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/deterministic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/dynamic_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/fill_missing_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    24831 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18458 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/spec_augment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.509891 espnet-202211/espnet/utils/training/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18371 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/training/batchfy.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/training/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/training/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/training/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2022-12-11 23:52:12.000000 espnet-202211/espnet/utils/training/train_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-11 23:52:12.000000 espnet-202211/espnet/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.465891 espnet-202211/espnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    65341 2022-12-11 23:52:21.000000 espnet-202211/espnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24754 2022-12-11 23:52:21.000000 espnet-202211/espnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-11 23:52:21.000000 espnet-202211/espnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2022-12-11 23:52:21.000000 espnet-202211/espnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-11 23:52:21.000000 espnet-202211/espnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.509891 espnet-202211/espnet2/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-11 23:52:12.000000 espnet-202211/espnet2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.513892 espnet-202211/espnet2/asr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/ctc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.513892 espnet-202211/espnet2/asr/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/decoder/abs_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/decoder/hugging_face_transformers_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/decoder/mlm_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12121 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/decoder/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/decoder/transducer_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19739 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/decoder/transformer_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.517892 espnet-202211/espnet2/asr/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/abs_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    20919 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/branchformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15076 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/conformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23191 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/contextual_block_conformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    21748 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/contextual_block_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15207 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/e_branchformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/hubert_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15058 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/longformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/rnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/transformer_encoder_multispkr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/vgg_rnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/encoder/wav2vec2_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22181 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/espnet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.517892 espnet-202211/espnet2/asr/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/frontend/abs_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/frontend/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/frontend/fused.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/frontend/s3prl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/frontend/windowing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.517892 espnet-202211/espnet2/asr/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/layers/cgmlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/layers/fastformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/maskctc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/pit_espnet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.517892 espnet-202211/espnet2/asr/postencoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/postencoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/postencoder/abs_postencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.517892 espnet-202211/espnet2/asr/preencoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/preencoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/preencoder/abs_preencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/preencoder/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/preencoder/sinc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.517892 espnet-202211/espnet2/asr/specaug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/specaug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/specaug/abs_specaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/specaug/specaug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.521891 espnet-202211/espnet2/asr/transducer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/transducer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29365 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/transducer/beam_search_transducer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr/transducer/error_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.521891 espnet-202211/espnet2/asr_transducer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23075 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/beam_search_transducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.521891 espnet-202211/espnet2/asr_transducer/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/decoder/abs_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/decoder/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/decoder/stateless_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.521891 espnet-202211/espnet2/asr_transducer/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.525892 espnet-202211/espnet2/asr_transducer/encoder/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/blocks/branchformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/blocks/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/blocks/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/blocks/conv_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/building.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.525892 espnet-202211/espnet2/asr_transducer/encoder/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/modules/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/modules/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/modules/multi_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/modules/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/modules/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/encoder/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/error_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15569 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/espnet_transducer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/joint_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2022-12-11 23:52:12.000000 espnet-202211/espnet2/asr_transducer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.529892 espnet-202211/espnet2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3756 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/aggregate_stats_dirs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32304 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/asr_align.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29613 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/asr_inference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26605 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/asr_inference_k2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/asr_inference_maskctc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21853 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/asr_inference_streaming.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/asr_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26022 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/asr_transducer_inference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      599 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/asr_transducer_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26817 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/diar_inference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      477 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/diar_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21746 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/enh_inference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      467 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/enh_s2t_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6342 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/enh_scoring.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/enh_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      413 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/gan_tts_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      454 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/hubert_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3105 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/hugging_face_export_vocabulary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13042 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/launch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6595 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/lm_calc_perplexity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      383 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/lm_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17194 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/mt_inference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/mt_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2901 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)    23605 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/slu_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/slu_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3394 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/split_scps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17745 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/st_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    20953 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/st_inference_streaming.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/st_train.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/svs_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/svs_train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8005 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/tokenize_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25855 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/tts_inference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      389 2022-12-11 23:52:12.000000 espnet-202211/espnet2/bin/tts_train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.529892 espnet-202211/espnet2/diar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/abs_diar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.529892 espnet-202211/espnet2/diar/attractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/attractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/attractor/abs_attractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/attractor/rnn_attractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.529892 espnet-202211/espnet2/diar/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/decoder/abs_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/decoder/linear_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14924 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/espnet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/label_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.529892 espnet-202211/espnet2/diar/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/layers/abs_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/layers/multi_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/layers/tcn_nomask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.529892 espnet-202211/espnet2/diar/separator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/separator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2022-12-11 23:52:12.000000 espnet-202211/espnet2/diar/separator/tcn_separator_nomask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.529892 espnet-202211/espnet2/enh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/abs_enh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.529892 espnet-202211/espnet2/enh/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/decoder/abs_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/decoder/conv_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/decoder/null_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/decoder/stft_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.529892 espnet-202211/espnet2/enh/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/encoder/abs_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/encoder/conv_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/encoder/null_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/encoder/stft_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19389 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/espnet_enh_s2t_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20148 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/espnet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.533892 espnet-202211/espnet2/enh/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42560 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/beamformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    37809 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/beamformer_th.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/complexnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/conv_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18544 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/dc_crn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23362 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/dnn_beamformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/dnn_wpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/dpmulcat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/dprnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/dptnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/fasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/ifasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/mask_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/skim.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/tcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14467 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/tcndenseunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/layers/wpe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.533892 espnet-202211/espnet2/enh/loss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.533892 espnet-202211/espnet2/enh/loss/criterions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/criterions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/criterions/abs_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    16625 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/criterions/tf_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/criterions/time_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.533892 espnet-202211/espnet2/enh/loss/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/wrappers/abs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/wrappers/dpcl_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/wrappers/fixed_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/wrappers/mixit_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/wrappers/multilayer_pit_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/loss/wrappers/pit_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.537892 espnet-202211/espnet2/enh/separator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/abs_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/asteroid_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/conformer_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/dan_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/dc_crn_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/dccrn_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/dpcl_e2e_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/dpcl_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/dprnn_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/dptnet_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/fasnet_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/ineube_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10439 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/neural_beamformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/rnn_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/skim_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/svoice_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/tcn_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2022-12-11 23:52:12.000000 espnet-202211/espnet2/enh/separator/transformer_separator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.537892 espnet-202211/espnet2/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2022-12-11 23:52:12.000000 espnet-202211/espnet2/fileio/datadir_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2022-12-11 23:52:12.000000 espnet-202211/espnet2/fileio/npy_scp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2022-12-11 23:52:12.000000 espnet-202211/espnet2/fileio/rand_gen_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2022-12-11 23:52:12.000000 espnet-202211/espnet2/fileio/read_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2022-12-11 23:52:12.000000 espnet-202211/espnet2/fileio/rttm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2022-12-11 23:52:12.000000 espnet-202211/espnet2/fileio/score_scp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2022-12-11 23:52:12.000000 espnet-202211/espnet2/fileio/sound_scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.537892 espnet-202211/espnet2/gan_tts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/abs_gan_tts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/espnet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.537892 espnet-202211/espnet2/gan_tts/hifigan/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/hifigan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/hifigan/hifigan.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/hifigan/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/hifigan/residual_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.537892 espnet-202211/espnet2/gan_tts/jets/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/jets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/jets/alignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    35386 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/jets/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24388 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/jets/jets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/jets/length_regulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/jets/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.537892 espnet-202211/espnet2/gan_tts/joint/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/joint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24009 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/joint/joint_text2wav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.537892 espnet-202211/espnet2/gan_tts/melgan/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/melgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16694 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/melgan/melgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/melgan/pqmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/melgan/residual_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.537892 espnet-202211/espnet2/gan_tts/parallel_wavegan/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/parallel_wavegan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/parallel_wavegan/parallel_wavegan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/parallel_wavegan/upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.537892 espnet-202211/espnet2/gan_tts/style_melgan/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/style_melgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/style_melgan/style_melgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/style_melgan/tade_res_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.537892 espnet-202211/espnet2/gan_tts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/utils/get_random_segments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.541892 espnet-202211/espnet2/gan_tts/vits/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    25456 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.541892 espnet-202211/espnet2/gan_tts/vits/monotonic_align/
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/monotonic_align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/monotonic_align/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/posterior_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/residual_coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/vits/vits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.541892 espnet-202211/espnet2/gan_tts/wavenet/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/wavenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/wavenet/residual_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2022-12-11 23:52:12.000000 espnet-202211/espnet2/gan_tts/wavenet/wavenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.541892 espnet-202211/espnet2/hubert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/hubert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2022-12-11 23:52:12.000000 espnet-202211/espnet2/hubert/espnet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2022-12-11 23:52:12.000000 espnet-202211/espnet2/hubert/hubert_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.541892 espnet-202211/espnet2/iterators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/iterators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2022-12-11 23:52:12.000000 espnet-202211/espnet2/iterators/abs_iter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2022-12-11 23:52:12.000000 espnet-202211/espnet2/iterators/chunk_iter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2022-12-11 23:52:12.000000 espnet-202211/espnet2/iterators/multiple_iter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2022-12-11 23:52:12.000000 espnet-202211/espnet2/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.541892 espnet-202211/espnet2/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2022-12-11 23:52:12.000000 espnet-202211/espnet2/layers/abs_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2022-12-11 23:52:12.000000 espnet-202211/espnet2/layers/global_mvn.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-11 23:52:12.000000 espnet-202211/espnet2/layers/inversible_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2022-12-11 23:52:12.000000 espnet-202211/espnet2/layers/label_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2022-12-11 23:52:12.000000 espnet-202211/espnet2/layers/log_mel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2022-12-11 23:52:12.000000 espnet-202211/espnet2/layers/mask_along_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9034 2022-12-11 23:52:12.000000 espnet-202211/espnet2/layers/sinc_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2022-12-11 23:52:12.000000 espnet-202211/espnet2/layers/stft.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2022-12-11 23:52:12.000000 espnet-202211/espnet2/layers/time_warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2022-12-11 23:52:12.000000 espnet-202211/espnet2/layers/utterance_mvn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.541892 espnet-202211/espnet2/lm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/lm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-11 23:52:12.000000 espnet-202211/espnet2/lm/abs_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2022-12-11 23:52:12.000000 espnet-202211/espnet2/lm/espnet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2022-12-11 23:52:12.000000 espnet-202211/espnet2/lm/seq_rnn_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2022-12-11 23:52:12.000000 espnet-202211/espnet2/lm/transformer_lm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.541892 espnet-202211/espnet2/main_funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/main_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2022-12-11 23:52:12.000000 espnet-202211/espnet2/main_funcs/average_nbest_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2022-12-11 23:52:12.000000 espnet-202211/espnet2/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2022-12-11 23:52:12.000000 espnet-202211/espnet2/main_funcs/collect_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2022-12-11 23:52:12.000000 espnet-202211/espnet2/main_funcs/pack_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.541892 espnet-202211/espnet2/mt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/mt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2022-12-11 23:52:12.000000 espnet-202211/espnet2/mt/espnet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/mt/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/mt/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2022-12-11 23:52:12.000000 espnet-202211/espnet2/mt/frontend/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2022-12-11 23:52:12.000000 espnet-202211/espnet2/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2022-12-11 23:52:12.000000 espnet-202211/espnet2/samplers/abs_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2022-12-11 23:52:12.000000 espnet-202211/espnet2/samplers/build_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2022-12-11 23:52:12.000000 espnet-202211/espnet2/samplers/folded_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2022-12-11 23:52:12.000000 espnet-202211/espnet2/samplers/length_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2022-12-11 23:52:12.000000 espnet-202211/espnet2/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2022-12-11 23:52:12.000000 espnet-202211/espnet2/samplers/sorted_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2022-12-11 23:52:12.000000 espnet-202211/espnet2/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2022-12-11 23:52:12.000000 espnet-202211/espnet2/schedulers/abs_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2022-12-11 23:52:12.000000 espnet-202211/espnet2/schedulers/noam_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2022-12-11 23:52:12.000000 espnet-202211/espnet2/schedulers/warmup_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2022-12-11 23:52:12.000000 espnet-202211/espnet2/schedulers/warmup_step_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/slu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/slu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17037 2022-12-11 23:52:12.000000 espnet-202211/espnet2/slu/espnet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/slu/postdecoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/slu/postdecoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2022-12-11 23:52:12.000000 espnet-202211/espnet2/slu/postdecoder/abs_postdecoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2022-12-11 23:52:12.000000 espnet-202211/espnet2/slu/postdecoder/hugging_face_transformers_postdecoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/slu/postencoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/slu/postencoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2022-12-11 23:52:12.000000 espnet-202211/espnet2/slu/postencoder/conformer_postencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2022-12-11 23:52:12.000000 espnet-202211/espnet2/slu/postencoder/transformer_postencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/st/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/st/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16512 2022-12-11 23:52:12.000000 espnet-202211/espnet2/st/espnet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/svs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/svs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2022-12-11 23:52:12.000000 espnet-202211/espnet2/svs/abs_svs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45987 2022-12-11 23:52:12.000000 espnet-202211/espnet2/svs/espnet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/svs/feats_extract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/svs/feats_extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2022-12-11 23:52:12.000000 espnet-202211/espnet2/svs/feats_extract/score_feats_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/svs/naive_rnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/svs/naive_rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21827 2022-12-11 23:52:12.000000 espnet-202211/espnet2/svs/naive_rnn/naive_rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    22844 2022-12-11 23:52:12.000000 espnet-202211/espnet2/svs/naive_rnn/naive_rnn_dp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.545892 espnet-202211/espnet2/svs/xiaoice/
--rw-r--r--   0 runner    (1001) docker     (123)    30828 2022-12-11 23:52:12.000000 espnet-202211/espnet2/svs/xiaoice/XiaoiceSing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/svs/xiaoice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.549892 espnet-202211/espnet2/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68030 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/abs_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    19328 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/asr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/asr_transducer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/diar.py
--rw-r--r--   0 runner    (1001) docker     (123)    18641 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/enh.py
--rw-r--r--   0 runner    (1001) docker     (123)    19866 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/enh_s2t.py
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/gan_tts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13388 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13499 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/mt.py
--rw-r--r--   0 runner    (1001) docker     (123)    20979 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/slu.py
--rw-r--r--   0 runner    (1001) docker     (123)    20374 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/st.py
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/svs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tasks/tts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.549892 espnet-202211/espnet2/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2022-12-11 23:52:12.000000 espnet-202211/espnet2/text/abs_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2022-12-11 23:52:12.000000 espnet-202211/espnet2/text/build_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2022-12-11 23:52:12.000000 espnet-202211/espnet2/text/char_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2022-12-11 23:52:12.000000 espnet-202211/espnet2/text/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2022-12-11 23:52:12.000000 espnet-202211/espnet2/text/hugging_face_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2022-12-11 23:52:12.000000 espnet-202211/espnet2/text/korean_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20902 2022-12-11 23:52:12.000000 espnet-202211/espnet2/text/phoneme_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2022-12-11 23:52:12.000000 espnet-202211/espnet2/text/sentencepiece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2022-12-11 23:52:12.000000 espnet-202211/espnet2/text/token_id_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2022-12-11 23:52:12.000000 espnet-202211/espnet2/text/word_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.549892 espnet-202211/espnet2/torch_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/torch_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2022-12-11 23:52:12.000000 espnet-202211/espnet2/torch_utils/add_gradient_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2022-12-11 23:52:12.000000 espnet-202211/espnet2/torch_utils/device_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2022-12-11 23:52:12.000000 espnet-202211/espnet2/torch_utils/forward_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2022-12-11 23:52:12.000000 espnet-202211/espnet2/torch_utils/get_layer_from_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2022-12-11 23:52:12.000000 espnet-202211/espnet2/torch_utils/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2022-12-11 23:52:12.000000 espnet-202211/espnet2/torch_utils/load_pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2022-12-11 23:52:12.000000 espnet-202211/espnet2/torch_utils/model_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2022-12-11 23:52:12.000000 espnet-202211/espnet2/torch_utils/pytorch_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2022-12-11 23:52:12.000000 espnet-202211/espnet2/torch_utils/recursive_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-11 23:52:12.000000 espnet-202211/espnet2/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.553892 espnet-202211/espnet2/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/abs_espnet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/abs_gan_espnet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/class_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/collate_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17741 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/distributed_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15059 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/gan_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    44547 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19602 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2022-12-11 23:52:12.000000 espnet-202211/espnet2/train/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.553892 espnet-202211/espnet2/tts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/abs_tts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/espnet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.553892 espnet-202211/espnet2/tts/fastspeech/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/fastspeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29711 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/fastspeech/fastspeech.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.553892 espnet-202211/espnet2/tts/fastspeech2/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/fastspeech2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35997 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/fastspeech2/fastspeech2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/fastspeech2/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/fastspeech2/variance_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.553892 espnet-202211/espnet2/tts/feats_extract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/feats_extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/feats_extract/abs_feats_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/feats_extract/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/feats_extract/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/feats_extract/linear_spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/feats_extract/log_mel_fbank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/feats_extract/log_spectrogram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.553892 espnet-202211/espnet2/tts/gst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/gst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/gst/style_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.553892 espnet-202211/espnet2/tts/tacotron2/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/tacotron2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21020 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/tacotron2/tacotron2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.553892 espnet-202211/espnet2/tts/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34927 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/transformer/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.553892 espnet-202211/espnet2/tts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/utils/duration_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2022-12-11 23:52:12.000000 espnet-202211/espnet2/tts/utils/parallel_wavegan_pretrained_vocoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.553892 espnet-202211/espnet2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:12.000000 espnet-202211/espnet2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-11 23:52:12.000000 espnet-202211/espnet2/utils/build_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2022-12-11 23:52:12.000000 espnet-202211/espnet2/utils/config_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2022-12-11 23:52:12.000000 espnet-202211/espnet2/utils/get_default_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2022-12-11 23:52:12.000000 espnet-202211/espnet2/utils/griffin_lim.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2022-12-11 23:52:12.000000 espnet-202211/espnet2/utils/kwargs2args.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2022-12-11 23:52:12.000000 espnet-202211/espnet2/utils/nested_dict_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2022-12-11 23:52:12.000000 espnet-202211/espnet2/utils/sized_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2022-12-11 23:52:12.000000 espnet-202211/espnet2/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2022-12-11 23:52:12.000000 espnet-202211/espnet2/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2022-12-11 23:52:21.561892 espnet-202211/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2022-12-11 23:52:12.000000 espnet-202211/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 23:52:21.561892 espnet-202211/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2022-12-11 23:52:12.000000 espnet-202211/test/test_asr_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2022-12-11 23:52:12.000000 espnet-202211/test/test_asr_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2022-12-11 23:52:12.000000 espnet-202211/test/test_asr_quantize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2022-12-11 23:52:12.000000 espnet-202211/test/test_batch_beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2022-12-11 23:52:12.000000 espnet-202211/test/test_beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2022-12-11 23:52:12.000000 espnet-202211/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21590 2022-12-11 23:52:12.000000 espnet-202211/test/test_custom_transducer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2022-12-11 23:52:12.000000 espnet-202211/test/test_distributed_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26225 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_asr_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_asr_maskctc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_asr_mulenc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14894 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_asr_transducer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_asr_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_mt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_mt_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20475 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_st.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_st_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_st_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21140 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_tts_fastspeech.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_tts_tacotron2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15609 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_tts_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8638 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_vc_tacotron2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2022-12-11 23:52:12.000000 espnet-202211/test/test_e2e_vc_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2022-12-11 23:52:12.000000 espnet-202211/test/test_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2022-12-11 23:52:12.000000 espnet-202211/test/test_io_voxforge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2022-12-11 23:52:12.000000 espnet-202211/test/test_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2022-12-11 23:52:12.000000 espnet-202211/test/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2022-12-11 23:52:12.000000 espnet-202211/test/test_multi_spkrs.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2022-12-11 23:52:12.000000 espnet-202211/test/test_ngram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2022-12-11 23:52:12.000000 espnet-202211/test/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2022-12-11 23:52:12.000000 espnet-202211/test/test_positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2022-12-11 23:52:12.000000 espnet-202211/test/test_recog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2022-12-11 23:52:12.000000 espnet-202211/test/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2022-12-11 23:52:12.000000 espnet-202211/test/test_sentencepiece.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2022-12-11 23:52:12.000000 espnet-202211/test/test_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2022-12-11 23:52:12.000000 espnet-202211/test/test_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2022-12-11 23:52:12.000000 espnet-202211/test/test_train_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2022-12-11 23:52:12.000000 espnet-202211/test/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2022-12-11 23:52:12.000000 espnet-202211/test/test_transformer_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     9830 2022-12-11 23:52:12.000000 espnet-202211/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.499410 espnet-202301/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-02-01 10:50:24.000000 espnet-202301/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    67965 2023-02-01 10:50:34.499410 espnet-202301/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    60025 2023-02-01 10:50:24.000000 espnet-202301/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.427408 espnet-202301/espnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-01 10:50:24.000000 espnet-202301/espnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.427408 espnet-202301/espnet/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-02-01 10:50:24.000000 espnet-202301/espnet/asr/asr_mix_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-02-01 10:50:24.000000 espnet-202301/espnet/asr/asr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.427408 espnet-202301/espnet/asr/chainer_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/asr/chainer_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19572 2023-02-01 10:50:24.000000 espnet-202301/espnet/asr/chainer_backend/asr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.427408 espnet-202301/espnet/asr/pytorch_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/asr/pytorch_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61311 2023-02-01 10:50:24.000000 espnet-202301/espnet/asr/pytorch_backend/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-02-01 10:50:24.000000 espnet-202301/espnet/asr/pytorch_backend/asr_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22054 2023-02-01 10:50:24.000000 espnet-202301/espnet/asr/pytorch_backend/asr_mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-02-01 10:50:24.000000 espnet-202301/espnet/asr/pytorch_backend/recog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.427408 espnet-202301/espnet/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13210 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/asr_align.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5778 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/asr_enhance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13800 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/asr_recog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22288 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/asr_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8939 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/lm_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14923 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/mt_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5956 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/mt_trans.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17332 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/st_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5855 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/st_trans.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5267 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/tts_decode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10680 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/tts_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5094 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/vc_decode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10830 2023-02-01 10:50:24.000000 espnet-202301/espnet/bin/vc_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.427408 espnet-202301/espnet/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-01 10:50:24.000000 espnet-202301/espnet/distributed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.427408 espnet-202301/espnet/lm/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/lm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.427408 espnet-202301/espnet/lm/chainer_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/lm/chainer_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-02-01 10:50:24.000000 espnet-202301/espnet/lm/chainer_backend/extlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18247 2023-02-01 10:50:24.000000 espnet-202301/espnet/lm/chainer_backend/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-02-01 10:50:24.000000 espnet-202301/espnet/lm/lm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.431408 espnet-202301/espnet/lm/pytorch_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/lm/pytorch_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-02-01 10:50:24.000000 espnet-202301/espnet/lm/pytorch_backend/extlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-02-01 10:50:24.000000 espnet-202301/espnet/lm/pytorch_backend/lm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.431408 espnet-202301/espnet/mt/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/mt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-02-01 10:50:24.000000 espnet-202301/espnet/mt/mt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.431408 espnet-202301/espnet/mt/pytorch_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/mt/pytorch_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-02-01 10:50:24.000000 espnet-202301/espnet/mt/pytorch_backend/mt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.431408 espnet-202301/espnet/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/asr_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/batch_beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/batch_beam_search_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/batch_beam_search_online_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19995 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/beam_search_timesync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30731 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/beam_search_transducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.431408 espnet-202301/espnet/nets/chainer_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/asr_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/ctc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/deterministic_embed_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/e2e_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/e2e_asr_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/nets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.431408 espnet-202301/espnet/nets/chainer_backend/rnn/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/rnn/attentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/rnn/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/rnn/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/rnn/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.435408 espnet-202301/espnet/nets/chainer_backend/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/ctc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/decoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/encoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/label_smoothing_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/positionwise_feed_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/subsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/chainer_backend/transformer/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/ctc_prefix_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/e2e_asr_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/e2e_mt_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/lm_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/mt_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.435408 espnet-202301/espnet/nets/pytorch_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.439408 espnet-202301/espnet/nets/pytorch_backend/conformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/conformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/conformer/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/conformer/contextual_block_encoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/conformer/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/conformer/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/conformer/encoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/conformer/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/ctc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19379 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_asr_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_asr_maskctc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30840 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_asr_mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18183 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_asr_mix_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31487 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_asr_mulenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_asr_transducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22562 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_asr_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_mt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_mt_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24057 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_st_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22657 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_st_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34348 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_tts_fastspeech.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34041 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_tts_tacotron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45641 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_tts_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_vc_tacotron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46109 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/e2e_vc_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.439408 espnet-202301/espnet/nets/pytorch_backend/fastspeech/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/fastspeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/fastspeech/duration_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/fastspeech/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/fastspeech/length_regulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.439408 espnet-202301/espnet/nets/pytorch_backend/frontends/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/frontends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/frontends/beamformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/frontends/dnn_beamformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/frontends/dnn_wpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/frontends/feature_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/frontends/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/frontends/mask_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/gtn_ctc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.439408 espnet-202301/espnet/nets/pytorch_backend/lm/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/lm/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/lm/seq_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/lm/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.439408 espnet-202301/espnet/nets/pytorch_backend/maskctc/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/maskctc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/maskctc/add_mask_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/maskctc/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16551 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/nets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.439408 espnet-202301/espnet/nets/pytorch_backend/rnn/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/rnn/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66963 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/rnn/attentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49021 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/rnn/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/rnn/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.439408 espnet-202301/espnet/nets/pytorch_backend/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/streaming/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/streaming/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.439408 espnet-202301/espnet/nets/pytorch_backend/tacotron2/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/tacotron2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/tacotron2/cbhg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24496 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/tacotron2/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/tacotron2/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.443408 espnet-202301/espnet/nets/pytorch_backend/transducer/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/conv1d_nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/custom_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/custom_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/error_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/joint_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18464 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/rnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15051 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/transducer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/transformer_decoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transducer/vgg2l.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.443408 espnet-202301/espnet/nets/pytorch_backend/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/add_sos_eos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/contextual_block_encoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/decoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/dynamic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/dynamic_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12758 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/encoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/encoder_mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/label_smoothing_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/lightconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/lightconv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/longformer_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/multi_layer_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/positionwise_feed_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/subsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/transformer/subsampling_without_posenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/pytorch_backend/wavenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/scorer_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.443408 espnet-202301/espnet/nets/scorers/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/scorers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/scorers/ctc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/scorers/length_bonus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/scorers/ngram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/scorers/uasr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/st_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/transducer_decoder_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-02-01 10:50:24.000000 espnet-202301/espnet/nets/tts_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.447409 espnet-202301/espnet/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-02-01 10:50:24.000000 espnet-202301/espnet/optimizer/chainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-02-01 10:50:24.000000 espnet-202301/espnet/optimizer/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-01 10:50:24.000000 espnet-202301/espnet/optimizer/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-02-01 10:50:24.000000 espnet-202301/espnet/optimizer/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.447409 espnet-202301/espnet/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-02-01 10:50:24.000000 espnet-202301/espnet/scheduler/chainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-02-01 10:50:24.000000 espnet-202301/espnet/scheduler/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-02-01 10:50:24.000000 espnet-202301/espnet/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.447409 espnet-202301/espnet/st/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/st/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.447409 espnet-202301/espnet/st/pytorch_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/st/pytorch_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22845 2023-02-01 10:50:24.000000 espnet-202301/espnet/st/pytorch_backend/st.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.447409 espnet-202301/espnet/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-01 10:50:24.000000 espnet-202301/espnet/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-01 10:50:24.000000 espnet-202301/espnet/transform/add_deltas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-02-01 10:50:24.000000 espnet-202301/espnet/transform/channel_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-02-01 10:50:24.000000 espnet-202301/espnet/transform/cmvn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-01 10:50:24.000000 espnet-202301/espnet/transform/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-02-01 10:50:24.000000 espnet-202301/espnet/transform/perturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-02-01 10:50:24.000000 espnet-202301/espnet/transform/spec_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-02-01 10:50:24.000000 espnet-202301/espnet/transform/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-02-01 10:50:24.000000 espnet-202301/espnet/transform/transform_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-02-01 10:50:24.000000 espnet-202301/espnet/transform/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-02-01 10:50:24.000000 espnet-202301/espnet/transform/wpe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.447409 espnet-202301/espnet/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/tts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.447409 espnet-202301/espnet/tts/pytorch_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/tts/pytorch_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26532 2023-02-01 10:50:24.000000 espnet-202301/espnet/tts/pytorch_backend/tts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.447409 espnet-202301/espnet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/check_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/cli_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/cli_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/deterministic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/dynamic_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/fill_missing_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24831 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18458 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/spec_augment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.447409 espnet-202301/espnet/utils/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/training/batchfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/training/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/training/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/training/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-02-01 10:50:24.000000 espnet-202301/espnet/utils/training/train_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-01 10:50:24.000000 espnet-202301/espnet/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.427408 espnet-202301/espnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    67965 2023-02-01 10:50:34.000000 espnet-202301/espnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27497 2023-02-01 10:50:34.000000 espnet-202301/espnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 10:50:34.000000 espnet-202301/espnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-02-01 10:50:34.000000 espnet-202301/espnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-01 10:50:34.000000 espnet-202301/espnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.451409 espnet-202301/espnet2/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-01 10:50:24.000000 espnet-202301/espnet2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.451409 espnet-202301/espnet2/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/ctc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.451409 espnet-202301/espnet2/asr/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/decoder/abs_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/decoder/hugging_face_transformers_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/decoder/mlm_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/decoder/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/decoder/s4_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/decoder/transducer_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/decoder/transformer_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/decoder/whisper_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.451409 espnet-202301/espnet2/asr/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/abs_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21255 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/branchformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/conformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23191 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/contextual_block_conformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21748 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/contextual_block_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/e_branchformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25131 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/hubert_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/longformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/rnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/transformer_encoder_multispkr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/vgg_rnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/wav2vec2_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/encoder/whisper_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/espnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.451409 espnet-202301/espnet2/asr/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/frontend/abs_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/frontend/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/frontend/fused.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/frontend/s3prl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/frontend/whisper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/frontend/windowing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.451409 espnet-202301/espnet2/asr/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/layers/cgmlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/layers/fastformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/maskctc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/pit_espnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.455409 espnet-202301/espnet2/asr/postencoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/postencoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/postencoder/abs_postencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.455409 espnet-202301/espnet2/asr/preencoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/preencoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/preencoder/abs_preencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/preencoder/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/preencoder/sinc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.455409 espnet-202301/espnet2/asr/specaug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/specaug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/specaug/abs_specaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/specaug/specaug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.455409 espnet-202301/espnet2/asr/state_spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/cauchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/ff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61258 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/s4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/state_spaces/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.455409 espnet-202301/espnet2/asr/transducer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/transducer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29365 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/transducer/beam_search_transducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr/transducer/error_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.455409 espnet-202301/espnet2/asr_transducer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/beam_search_transducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.455409 espnet-202301/espnet2/asr_transducer/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/decoder/abs_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/decoder/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/decoder/stateless_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.455409 espnet-202301/espnet2/asr_transducer/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.459409 espnet-202301/espnet2/asr_transducer/encoder/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/blocks/branchformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/blocks/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/blocks/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/blocks/conv_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.459409 espnet-202301/espnet2/asr_transducer/encoder/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/modules/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/modules/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/modules/multi_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/modules/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/modules/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/encoder/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/error_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/espnet_transducer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/joint_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-02-01 10:50:24.000000 espnet-202301/espnet2/asr_transducer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.463409 espnet-202301/espnet2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3756 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/aggregate_stats_dirs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32304 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/asr_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31745 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/asr_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26605 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/asr_inference_k2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/asr_inference_maskctc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21853 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/asr_inference_streaming.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/asr_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26022 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/asr_transducer_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/asr_transducer_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26817 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/diar_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      477 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/diar_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21746 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/enh_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/enh_s2t_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6342 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/enh_scoring.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/enh_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22718 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/enh_tse_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/enh_tse_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      413 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/gan_svs_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      413 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/gan_tts_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/hubert_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3105 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/hugging_face_export_vocabulary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13042 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/launch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6595 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/lm_calc_perplexity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/lm_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17194 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/mt_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/mt_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3119 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/slu_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/slu_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3394 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/split_scps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17745 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/st_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20953 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/st_inference_streaming.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/st_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/svs_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/svs_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/tokenize_text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25855 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/tts_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/tts_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/uasr_extract_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/uasr_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21667 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/uasr_inference_k2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/uasr_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-02-01 10:50:24.000000 espnet-202301/espnet2/bin/whisper_export_vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.463409 espnet-202301/espnet2/diar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/abs_diar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.463409 espnet-202301/espnet2/diar/attractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/attractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/attractor/abs_attractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/attractor/rnn_attractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.463409 espnet-202301/espnet2/diar/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/decoder/abs_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/decoder/linear_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/espnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/label_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.463409 espnet-202301/espnet2/diar/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/layers/abs_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/layers/multi_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/layers/tcn_nomask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.463409 espnet-202301/espnet2/diar/separator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/separator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-02-01 10:50:24.000000 espnet-202301/espnet2/diar/separator/tcn_separator_nomask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.463409 espnet-202301/espnet2/enh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/abs_enh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.463409 espnet-202301/espnet2/enh/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/decoder/abs_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/decoder/conv_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/decoder/null_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/decoder/stft_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.467409 espnet-202301/espnet2/enh/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/encoder/abs_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/encoder/conv_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/encoder/null_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/encoder/stft_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19389 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/espnet_enh_s2t_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/espnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12815 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/espnet_model_tse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.467409 espnet-202301/espnet2/enh/extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/extractor/abs_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/extractor/td_speakerbeam_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.467409 espnet-202301/espnet2/enh/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/adapt_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42560 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/beamformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37809 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/beamformer_th.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/complexnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/conv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18544 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/dc_crn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23362 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/dnn_beamformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/dnn_wpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/dpmulcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/dprnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/dptnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/fasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/ifasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/mask_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/skim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/tcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/tcndenseunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/layers/wpe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.467409 espnet-202301/espnet2/enh/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.467409 espnet-202301/espnet2/enh/loss/criterions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/criterions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/criterions/abs_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/criterions/tf_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/criterions/time_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.467409 espnet-202301/espnet2/enh/loss/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/wrappers/abs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/wrappers/dpcl_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/wrappers/fixed_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/wrappers/mixit_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/wrappers/multilayer_pit_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/loss/wrappers/pit_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.471409 espnet-202301/espnet2/enh/separator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/abs_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/asteroid_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/conformer_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/dan_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/dc_crn_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/dccrn_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/dpcl_e2e_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/dpcl_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/dprnn_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/dptnet_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/fasnet_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/ineube_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/neural_beamformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/rnn_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/skim_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/svoice_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/tcn_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-02-01 10:50:24.000000 espnet-202301/espnet2/enh/separator/transformer_separator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.471409 espnet-202301/espnet2/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-02-01 10:50:24.000000 espnet-202301/espnet2/fileio/datadir_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-02-01 10:50:24.000000 espnet-202301/espnet2/fileio/npy_scp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-02-01 10:50:24.000000 espnet-202301/espnet2/fileio/rand_gen_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-02-01 10:50:24.000000 espnet-202301/espnet2/fileio/read_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-02-01 10:50:24.000000 espnet-202301/espnet2/fileio/rttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-02-01 10:50:24.000000 espnet-202301/espnet2/fileio/score_scp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-02-01 10:50:24.000000 espnet-202301/espnet2/fileio/sound_scp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-02-01 10:50:24.000000 espnet-202301/espnet2/fileio/vad_scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.471409 espnet-202301/espnet2/fst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/fst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-02-01 10:50:24.000000 espnet-202301/espnet2/fst/lm_rescore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.471409 espnet-202301/espnet2/gan_svs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/abs_gan_svs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45043 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/espnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.475410 espnet-202301/espnet2/gan_svs/vits/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/vits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/vits/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/vits/frame_prior_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26875 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/vits/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/vits/length_regulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/vits/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/vits/phoneme_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/vits/pitch_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/vits/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35487 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_svs/vits/vits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.475410 espnet-202301/espnet2/gan_tts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/abs_gan_tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/espnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.475410 espnet-202301/espnet2/gan_tts/hifigan/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/hifigan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/hifigan/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/hifigan/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/hifigan/residual_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.475410 espnet-202301/espnet2/gan_tts/jets/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/jets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/jets/alignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35386 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/jets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/jets/jets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/jets/length_regulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/jets/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.475410 espnet-202301/espnet2/gan_tts/joint/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/joint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24009 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/joint/joint_text2wav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.475410 espnet-202301/espnet2/gan_tts/melgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/melgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/melgan/melgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/melgan/pqmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/melgan/residual_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.475410 espnet-202301/espnet2/gan_tts/parallel_wavegan/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/parallel_wavegan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/parallel_wavegan/parallel_wavegan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/parallel_wavegan/upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.475410 espnet-202301/espnet2/gan_tts/style_melgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/style_melgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/style_melgan/style_melgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/style_melgan/tade_res_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.475410 espnet-202301/espnet2/gan_tts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/utils/get_random_segments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.475410 espnet-202301/espnet2/gan_tts/vits/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25456 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.479410 espnet-202301/espnet2/gan_tts/vits/monotonic_align/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/monotonic_align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/monotonic_align/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/posterior_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/residual_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/vits/vits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.479410 espnet-202301/espnet2/gan_tts/wavenet/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/wavenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/wavenet/residual_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-02-01 10:50:24.000000 espnet-202301/espnet2/gan_tts/wavenet/wavenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.479410 espnet-202301/espnet2/hubert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/hubert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-02-01 10:50:24.000000 espnet-202301/espnet2/hubert/espnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-02-01 10:50:24.000000 espnet-202301/espnet2/hubert/hubert_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.479410 espnet-202301/espnet2/iterators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/iterators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-01 10:50:24.000000 espnet-202301/espnet2/iterators/abs_iter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-02-01 10:50:24.000000 espnet-202301/espnet2/iterators/chunk_iter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-01 10:50:24.000000 espnet-202301/espnet2/iterators/multiple_iter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-02-01 10:50:24.000000 espnet-202301/espnet2/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.479410 espnet-202301/espnet2/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-01 10:50:24.000000 espnet-202301/espnet2/layers/abs_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-02-01 10:50:24.000000 espnet-202301/espnet2/layers/global_mvn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-01 10:50:24.000000 espnet-202301/espnet2/layers/inversible_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-02-01 10:50:24.000000 espnet-202301/espnet2/layers/label_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-02-01 10:50:24.000000 espnet-202301/espnet2/layers/log_mel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-02-01 10:50:24.000000 espnet-202301/espnet2/layers/mask_along_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9034 2023-02-01 10:50:24.000000 espnet-202301/espnet2/layers/sinc_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-02-01 10:50:24.000000 espnet-202301/espnet2/layers/stft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-02-01 10:50:24.000000 espnet-202301/espnet2/layers/time_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-02-01 10:50:24.000000 espnet-202301/espnet2/layers/utterance_mvn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.479410 espnet-202301/espnet2/lm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-01 10:50:24.000000 espnet-202301/espnet2/lm/abs_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-02-01 10:50:24.000000 espnet-202301/espnet2/lm/espnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-02-01 10:50:24.000000 espnet-202301/espnet2/lm/seq_rnn_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-02-01 10:50:24.000000 espnet-202301/espnet2/lm/transformer_lm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.479410 espnet-202301/espnet2/main_funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/main_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-02-01 10:50:24.000000 espnet-202301/espnet2/main_funcs/average_nbest_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-02-01 10:50:24.000000 espnet-202301/espnet2/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-02-01 10:50:24.000000 espnet-202301/espnet2/main_funcs/collect_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-02-01 10:50:24.000000 espnet-202301/espnet2/main_funcs/pack_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.479410 espnet-202301/espnet2/mt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/mt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-02-01 10:50:24.000000 espnet-202301/espnet2/mt/espnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.479410 espnet-202301/espnet2/mt/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/mt/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-02-01 10:50:24.000000 espnet-202301/espnet2/mt/frontend/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.479410 espnet-202301/espnet2/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-02-01 10:50:24.000000 espnet-202301/espnet2/optimizers/optim_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-01 10:50:24.000000 espnet-202301/espnet2/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.483410 espnet-202301/espnet2/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-01 10:50:24.000000 espnet-202301/espnet2/samplers/abs_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-02-01 10:50:24.000000 espnet-202301/espnet2/samplers/build_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-02-01 10:50:24.000000 espnet-202301/espnet2/samplers/folded_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-02-01 10:50:24.000000 espnet-202301/espnet2/samplers/length_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-02-01 10:50:24.000000 espnet-202301/espnet2/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-02-01 10:50:24.000000 espnet-202301/espnet2/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-02-01 10:50:24.000000 espnet-202301/espnet2/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.483410 espnet-202301/espnet2/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-01 10:50:24.000000 espnet-202301/espnet2/schedulers/abs_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-02-01 10:50:24.000000 espnet-202301/espnet2/schedulers/noam_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-02-01 10:50:24.000000 espnet-202301/espnet2/schedulers/warmup_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-02-01 10:50:24.000000 espnet-202301/espnet2/schedulers/warmup_step_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.483410 espnet-202301/espnet2/slu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/slu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-02-01 10:50:24.000000 espnet-202301/espnet2/slu/espnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.483410 espnet-202301/espnet2/slu/postdecoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/slu/postdecoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-01 10:50:24.000000 espnet-202301/espnet2/slu/postdecoder/abs_postdecoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-02-01 10:50:24.000000 espnet-202301/espnet2/slu/postdecoder/hugging_face_transformers_postdecoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.483410 espnet-202301/espnet2/slu/postencoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/slu/postencoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-02-01 10:50:24.000000 espnet-202301/espnet2/slu/postencoder/conformer_postencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-02-01 10:50:24.000000 espnet-202301/espnet2/slu/postencoder/transformer_postencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.483410 espnet-202301/espnet2/st/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/st/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-02-01 10:50:24.000000 espnet-202301/espnet2/st/espnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.483410 espnet-202301/espnet2/svs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/svs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-02-01 10:50:24.000000 espnet-202301/espnet2/svs/abs_svs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46091 2023-02-01 10:50:24.000000 espnet-202301/espnet2/svs/espnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.483410 espnet-202301/espnet2/svs/feats_extract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/svs/feats_extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-02-01 10:50:24.000000 espnet-202301/espnet2/svs/feats_extract/score_feats_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.483410 espnet-202301/espnet2/svs/naive_rnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/svs/naive_rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21929 2023-02-01 10:50:24.000000 espnet-202301/espnet2/svs/naive_rnn/naive_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22946 2023-02-01 10:50:24.000000 espnet-202301/espnet2/svs/naive_rnn/naive_rnn_dp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.483410 espnet-202301/espnet2/svs/xiaoice/
+-rw-r--r--   0 runner    (1001) docker     (123)    30828 2023-02-01 10:50:24.000000 espnet-202301/espnet2/svs/xiaoice/XiaoiceSing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/svs/xiaoice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.487410 espnet-202301/espnet2/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69028 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/abs_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/asr_transducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/diar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18641 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/enh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19866 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/enh_s2t.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/enh_tse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/gan_svs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/gan_tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/mt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20979 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/slu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20374 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/st.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/svs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tasks/uasr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.487410 espnet-202301/espnet2/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/abs_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/build_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/char_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/hugging_face_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/korean_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20902 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/phoneme_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/token_id_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/whisper_token_id_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/whisper_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-02-01 10:50:24.000000 espnet-202301/espnet2/text/word_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.487410 espnet-202301/espnet2/torch_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/torch_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-02-01 10:50:24.000000 espnet-202301/espnet2/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-02-01 10:50:24.000000 espnet-202301/espnet2/torch_utils/device_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-01 10:50:24.000000 espnet-202301/espnet2/torch_utils/forward_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-01 10:50:24.000000 espnet-202301/espnet2/torch_utils/get_layer_from_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-02-01 10:50:24.000000 espnet-202301/espnet2/torch_utils/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-02-01 10:50:24.000000 espnet-202301/espnet2/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-02-01 10:50:24.000000 espnet-202301/espnet2/torch_utils/model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-01 10:50:24.000000 espnet-202301/espnet2/torch_utils/pytorch_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-02-01 10:50:24.000000 espnet-202301/espnet2/torch_utils/recursive_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-01 10:50:24.000000 espnet-202301/espnet2/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/abs_espnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/abs_gan_espnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/class_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/collate_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/distributed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/gan_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53064 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19602 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35408 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-02-01 10:50:24.000000 espnet-202301/espnet2/train/uasr_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/abs_tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/espnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/tts/fastspeech/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/fastspeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29711 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/fastspeech/fastspeech.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/tts/fastspeech2/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/fastspeech2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35997 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/fastspeech2/fastspeech2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/fastspeech2/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/fastspeech2/variance_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/tts/feats_extract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/feats_extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/feats_extract/abs_feats_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/feats_extract/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/feats_extract/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/feats_extract/linear_spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/feats_extract/log_mel_fbank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/feats_extract/log_spectrogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/tts/gst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/gst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/gst/style_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/tts/prodiff/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/prodiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/prodiff/denoiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/prodiff/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35170 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/prodiff/prodiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/tts/tacotron2/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/tacotron2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21020 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/tacotron2/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/tts/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34927 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/transformer/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/tts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/utils/duration_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-02-01 10:50:24.000000 espnet-202301/espnet2/tts/utils/parallel_wavegan_pretrained_vocoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/uasr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.491410 espnet-202301/espnet2/uasr/discriminator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/discriminator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/discriminator/abs_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/discriminator/conv_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/espnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.495411 espnet-202301/espnet2/uasr/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/generator/abs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/generator/conv_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.495411 espnet-202301/espnet2/uasr/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/loss/abs_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/loss/discriminator_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/loss/gradient_penalty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/loss/phoneme_diversity_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/loss/pseudo_label_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/loss/smoothness_penalty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.495411 espnet-202301/espnet2/uasr/segmenter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/segmenter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/segmenter/abs_segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/segmenter/join_segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-02-01 10:50:24.000000 espnet-202301/espnet2/uasr/segmenter/random_segmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.495411 espnet-202301/espnet2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:24.000000 espnet-202301/espnet2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-01 10:50:24.000000 espnet-202301/espnet2/utils/build_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-02-01 10:50:24.000000 espnet-202301/espnet2/utils/config_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-01 10:50:24.000000 espnet-202301/espnet2/utils/get_default_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-02-01 10:50:24.000000 espnet-202301/espnet2/utils/griffin_lim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-01 10:50:24.000000 espnet-202301/espnet2/utils/kwargs2args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-02-01 10:50:24.000000 espnet-202301/espnet2/utils/nested_dict_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-02-01 10:50:24.000000 espnet-202301/espnet2/utils/sized_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-02-01 10:50:24.000000 espnet-202301/espnet2/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-01 10:50:24.000000 espnet-202301/espnet2/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-01 10:50:34.499410 espnet-202301/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-02-01 10:50:24.000000 espnet-202301/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 10:50:34.499410 espnet-202301/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-02-01 10:50:24.000000 espnet-202301/test/test_asr_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-01 10:50:24.000000 espnet-202301/test/test_asr_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-01 10:50:24.000000 espnet-202301/test/test_asr_quantize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-02-01 10:50:24.000000 espnet-202301/test/test_batch_beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-02-01 10:50:24.000000 espnet-202301/test/test_beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-02-01 10:50:24.000000 espnet-202301/test/test_beam_search_timesync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-02-01 10:50:24.000000 espnet-202301/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21624 2023-02-01 10:50:24.000000 espnet-202301/test/test_custom_transducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-02-01 10:50:24.000000 espnet-202301/test/test_distributed_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26225 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_asr_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_asr_maskctc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_asr_mulenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_asr_transducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_asr_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_mt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_mt_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20475 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_st_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_st_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21140 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_tts_fastspeech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_tts_tacotron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_tts_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_vc_tacotron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-02-01 10:50:24.000000 espnet-202301/test/test_e2e_vc_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-02-01 10:50:24.000000 espnet-202301/test/test_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-01 10:50:24.000000 espnet-202301/test/test_io_voxforge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-02-01 10:50:24.000000 espnet-202301/test/test_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-02-01 10:50:24.000000 espnet-202301/test/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-02-01 10:50:24.000000 espnet-202301/test/test_multi_spkrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-01 10:50:24.000000 espnet-202301/test/test_ngram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-02-01 10:50:24.000000 espnet-202301/test/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-02-01 10:50:24.000000 espnet-202301/test/test_positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-02-01 10:50:24.000000 espnet-202301/test/test_recog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-02-01 10:50:24.000000 espnet-202301/test/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-02-01 10:50:24.000000 espnet-202301/test/test_sentencepiece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-02-01 10:50:24.000000 espnet-202301/test/test_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-01 10:50:24.000000 espnet-202301/test/test_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-02-01 10:50:24.000000 espnet-202301/test/test_train_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-02-01 10:50:24.000000 espnet-202301/test/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-02-01 10:50:24.000000 espnet-202301/test/test_transformer_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-02-01 10:50:24.000000 espnet-202301/test/test_utils.py
```

### Comparing `espnet-202211/LICENSE` & `espnet-202301/LICENSE`

 * *Files identical despite different names*

### Comparing `espnet-202211/PKG-INFO` & `espnet-202301/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espnet
-Version: 202211
+Version: 202301
 Summary: ESPnet: end-to-end speech processing toolkit
 Home-page: http://github.com/espnet/espnet
 Author: Shinji Watanabe
 Author-email: shinjiw@ieee.org
 License: Apache Software License
 Description: <div align="left"><img src="doc/image/espnet_logo1.png" width="550"/></div>
         
@@ -68,15 +68,16 @@
         - Support singing voice synthesis recipe (ofuton_p_utagoe_db)
         
         ### ASR: Automatic Speech Recognition
         - **State-of-the-art performance** in several ASR benchmarks (comparable/superior to hybrid DNN/HMM and CTC)
         - **Hybrid CTC/attention** based end-to-end ASR
           - Fast/accurate training with CTC/attention multitask training
           - CTC/attention joint decoding to boost monotonic alignment decoding
-          - Encoder: VGG-like CNN + BiRNN (LSTM/GRU), sub-sampling BiRNN (LSTM/GRU), Transformer, Conformer or [Branchformer](https://proceedings.mlr.press/v162/peng22a.html)
+          - Encoder: VGG-like CNN + BiRNN (LSTM/GRU), sub-sampling BiRNN (LSTM/GRU), Transformer, Conformer, [Branchformer](https://proceedings.mlr.press/v162/peng22a.html), or [E-Branchformer](https://arxiv.org/abs/2210.00077)
+          - Decoder: RNN (LSTM/GRU), Transformer, or S4
         - Attention: Dot product, location-aware attention, variants of multi-head
         - Incorporate RNNLM/LSTMLM/TransformerLM/N-gram trained only with text data
         - Batch GPU decoding
         - Data augmentation
         - **Transducer** based end-to-end ASR
           - Architecture:
             - RNN-based encoder and decoder.
@@ -100,22 +101,23 @@
         - Non-autoregressive model based on Mask-CTC
         - ASR examples for supporting endangered language documentation (Please refer to egs/puebla_nahuatl and egs/yoloxochitl_mixtec for details)
         - Wav2Vec2.0 pretrained model as Encoder, imported from [FairSeq](https://github.com/pytorch/fairseq/tree/master/fairseq).
         - Self-supervised learning representations as features, using upstream models in [S3PRL](https://github.com/s3prl/s3prl) in frontend.
           - Set `frontend` to be `s3prl`
           - Select any upstream model by setting the `frontend_conf` to the corresponding name.
         - Transfer Learning :
-          - easy usage and transfers from models previously trained by your group, or models from [ESPnet huggingface repository](https://huggingface.co/espnet).
+          - easy usage and transfers from models previously trained by your group, or models from [ESPnet Hugging Face repository](https://huggingface.co/espnet).
           - [Documentation](https://github.com/espnet/espnet/tree/master/egs2/mini_an4/asr1/transfer_learning.md) and [toy example runnable on colab](https://github.com/espnet/notebook/blob/master/espnet2_asr_transfer_learning_demo.ipynb).
         - Streaming Transformer/Conformer ASR with blockwise synchronous beam search.
         - Restricted Self-Attention based on [Longformer](https://arxiv.org/abs/2004.05150) as an encoder for long sequences
+        - OpenAI [Whisper](https://openai.com/blog/whisper/) model, robust ASR based on large-scale, weakly-supervised multitask learning
         
         Demonstration
         - Real-time ASR demo with ESPnet2  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/espnet/notebook/blob/master/espnet2_asr_realtime_demo.ipynb)
-        - [Gradio](https://github.com/gradio-app/gradio) Web Demo on [Huggingface Spaces](https://huggingface.co/docs/hub/spaces). Check out the [Web Demo](https://huggingface.co/spaces/akhaliq/espnet2_asr)
+        - [Gradio](https://github.com/gradio-app/gradio) Web Demo on [Hugging Face Spaces](https://huggingface.co/docs/hub/spaces). Check out the [Web Demo](https://huggingface.co/spaces/akhaliq/espnet2_asr)
         - Streaming Transformer ASR [Local Demo](https://github.com/espnet/notebook/blob/master/espnet2_streaming_asr_demo.ipynb) with ESPnet2.
         
         ### TTS: Text-to-speech
         - Architecture
             - Tacotron2
             - Transformer-TTS
             - FastSpeech
@@ -140,15 +142,15 @@
             - Multi-band MelGAN
             - HiFiGAN
             - StyleMelGAN
             - Mix of the above models
         
         Demonstration
         - Real-time TTS demo with ESPnet2  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/espnet/notebook/blob/master/espnet2_tts_realtime_demo.ipynb)
-        - Integrated to [Huggingface Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/akhaliq/ESPnet2-TTS)
+        - Integrated to [Hugging Face Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/akhaliq/ESPnet2-TTS)
         
         To train the neural vocoder, please check the following repositories:
         - [kan-bayashi/ParallelWaveGAN](https://github.com/kan-bayashi/ParallelWaveGAN)
         - [r9y9/wavenet_vocoder](https://github.com/r9y9/wavenet_vocoder)
         
         > **NOTE**:
         > - We are moving on ESPnet2-based development for TTS.
@@ -178,14 +180,15 @@
         - End-to-end VC based on cascaded ASR+TTS (Baseline system for Voice Conversion Challenge 2020!)
         
         ### SLU: Spoken Language Understanding
         - Architecture
             - Transformer based Encoder
             - Conformer based Encoder
             - [Branchformer](https://proceedings.mlr.press/v162/peng22a.html) based Encoder
+            - [E-Branchformer](https://arxiv.org/abs/2210.00077) based Encoder
             - RNN based Decoder
             - Transformer based Decoder
         - Support Multitasking with ASR
             - Predict both intent and ASR transcript
         - Support Multitasking with NLU
             - Deliberation encoder based 2 pass model
         - Support using pretrained ASR models
@@ -200,38 +203,47 @@
             - En / Jp / Zn / Nl / And more...
         - Supports using context from previous utterances
         - Supports using other tasks like SE in pipeline manner
         - Supports Two Pass SLU that combines audio and ASR transcript
         Demonstration
         - Performing noisy spoken language understanding using speech enhancement model followed by spoken language understanding model.  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14nCrJ05vJcQX0cJuXjbMVFWUHJ3Wfb6N?usp=sharing)
         - Performing two pass spoken language understanding where the second pass model attends on both acoustic and semantic information.  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1p2cbGIPpIIcynuDl4ZVHDpmNPl8Nh_ci?usp=sharing)
-        - Integrated to [Huggingface Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See SLU demo on multiple languages: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Siddhant/ESPnet2-SLU)
+        - Integrated to [Hugging Face Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See SLU demo on multiple languages: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Siddhant/ESPnet2-SLU)
         
         
         ### SUM: Speech Summarization
         - End to End Speech Summarization Recipe for Instructional Videos using Restricted Self-Attention [[Sharma et al., 2022]](https://arxiv.org/abs/2110.06263)
         
         ### SVS: Singing Voice Synthesis
         - Framework merge from [Muskits](https://github.com/SJTMusicTeam/Muskits)
         - Architecture
           - RNN-based non-autoregressive model
           - Xiaoice
           - Sequence-to-sequence Transformer (with GLU-based encoder)
-          - MLP singer
+          - MLP singer (in progress)
           - Tacotron-singing (in progress)
-          - DiffSinger (to be published)
-          - VISinger (in progress)
+          - DiffSinger (in progress)
+          - VISinger
         - Support multi-speaker & multilingual singing synthesis
           - Speaker ID embedding
           - Language ID embedding
-          - Global sytle token (GST) embedding
         - Various language support
           - Jp / En / Kr / Zh
         - Tight integration with neural vocoders (the same as TTS)
         
+        ### SSL: Self-supervised Learning
+        - Support HuBERT Pretraining:
+          * Example recipe: [egs2/LibriSpeech/ssl1](egs2/LibriSpeech/ssl1)
+        
+        ### UASR: Unsupervised ASR (EURO: ESPnet Unsupervised Recognition - Open-source)
+        - Architecture
+          - wav2vec-U (with different self-supervised models)
+          - wav2vec-U 2.0 (in progress)
+        - Support PrefixBeamSearch and K2-based WFST decoding
+        
         ### DNN Framework
         - Flexible network architecture thanks to chainer and pytorch
         - Flexible front-end processing thanks to [kaldiio](https://github.com/nttcslab-sp/kaldiio) and HDF5 support
         - Tensorboard based monitoring
         
         ### ESPnet2
         See [ESPnet2](https://espnet.github.io/espnet/espnet2_tutorial.html).
@@ -289,24 +301,27 @@
         
         
         We list the character error rate (CER) and word error rate (WER) of major ASR tasks.
         
         | Task                                                              |     CER (%)     |     WER (%)     |                                                                              Pretrained model                                                                               |
         | ----------------------------------------------------------------- | :-------------: | :-------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
         | Aishell dev/test                                                  |     4.6/5.1     |       N/A       |                [link](https://github.com/espnet/espnet/blob/master/egs/aishell/asr1/RESULTS.md#conformer-kernel-size--15--specaugment--lm-weight--00-result)                |
-        | **ESPnet2** Aishell dev/test                                      |     4.4/4.7     |       N/A       |                [link](https://github.com/espnet/espnet/tree/master/egs2/aishell/asr1#conformer--specaug--speed-perturbation-featsraw-n_fft512-hop_length128)                |
+        | **ESPnet2** Aishell dev/test                                      |     4.1/4.4     |       N/A       |                [link](https://github.com/espnet/espnet/tree/master/egs2/aishell/asr1#branchformer-initial)                                                                  |
         | Common Voice dev/test                                             |     1.7/1.8     |     2.2/2.3     |    [link](https://github.com/espnet/espnet/blob/master/egs/commonvoice/asr1/RESULTS.md#first-results-default-pytorch-transformer-setting-with-bpe-100-epochs-single-gpu)    |
         | CSJ eval1/eval2/eval3                                             |   5.7/3.8/4.2   |       N/A       |                 [link](https://github.com/espnet/espnet/blob/master/egs/csj/asr1/RESULTS.md#pytorch-backend-transformer-without-any-hyperparameter-tuning)                  |
         | **ESPnet2** CSJ eval1/eval2/eval3                                 |   4.5/3.3/3.6   |       N/A       |                                        [link](https://github.com/espnet/espnet/tree/master/egs2/csj/asr1#initial-conformer-results)                                         |
+        | **ESPnet2** GigaSpeech dev/test                                   |       N/A       |    10.6/10.5    |                                          [link](https://github.com/espnet/espnet/tree/master/egs2/gigaspeech/asr1#e-branchformer)                                           |
         | HKUST dev                                                         |      23.5       |       N/A       |                                  [link](https://github.com/espnet/espnet/blob/master/egs/hkust/asr1/RESULTS.md#transformer-only-20-epochs)                                  |
         | **ESPnet2** HKUST dev                                             |      21.2       |       N/A       |                                    [link](https://github.com/espnet/espnet/tree/master/egs2/hkust/asr1#transformer-asr--transformer-lm)                                     |
         | Librispeech dev_clean/dev_other/test_clean/test_other             |       N/A       | 1.9/4.9/2.1/4.9 | [link](https://github.com/espnet/espnet/blob/master/egs/librispeech/asr1/RESULTS.md#pytorch-large-conformer-with-specaug--speed-perturbation-8-gpus--transformer-lm-4-gpus) |
         | **ESPnet2** Librispeech dev_clean/dev_other/test_clean/test_other | 0.6/1.5/0.6/1.4 | 1.7/3.4/1.8/3.6 |    [link](https://github.com/espnet/espnet/tree/master/egs2/librispeech/asr1#self-supervised-learning-features-hubert_large_ll60k-conformer-utt_mvn-with-transformer-lm)    |
         | Switchboard (eval2000) callhm/swbd                                |       N/A       |    14.0/6.8     |          [link](https://github.com/espnet/espnet/blob/master/egs/swbd/asr1/RESULTS.md#conformer-with-bpe-2000-specaug-speed-perturbation-transformer-lm-decoding)           |
+        | **ESPnet2** Switchboard (eval2000) callhm/swbd                    |       N/A       |    13.4/7.3     |                                             [link](https://github.com/espnet/espnet/tree/master/egs2/swbd/asr1#e-branchformer)                                              |
         | TEDLIUM2 dev/test                                                 |       N/A       |     8.6/7.2     |                 [link](https://github.com/espnet/espnet/blob/master/egs/tedlium2/asr1/RESULTS.md#conformer-large-model--specaug--speed-perturbation--rnnlm)                 |
+        | **ESPnet2** TEDLIUM2 dev/test                                     |       N/A       |     7.3/7.1     |                 [link](https://github.com/espnet/espnet/blob/master/egs2/tedlium2/asr1/README.md#e-branchformer-12-encoder-layers)                                          |
         | TEDLIUM3 dev/test                                                 |       N/A       |     9.6/7.6     |                                              [link](https://github.com/espnet/espnet/blob/master/egs/tedlium3/asr1/RESULTS.md)                                              |
         | WSJ dev93/eval92                                                  |     3.2/2.1     |     7.0/4.7     |                                                                                     N/A                                                                                     |
         | **ESPnet2** WSJ dev93/eval92                                      |     1.1/0.8     |     2.8/1.8     |       [link](https://github.com/espnet/espnet/tree/master/egs2/wsj/asr1#self-supervised-learning-features-wav2vec2_large_ll60k-conformer-utt_mvn-with-transformer-lm)       |
         
         Note that the performance of the CSJ, HKUST, and Librispeech tasks was significantly improved by using the wide network (#units = 1024) and large subword units if necessary reported by [RWTH](https://arxiv.org/pdf/1805.03294.pdf).
         
         If you want to check the results of the other recipes, please check `egs/<name_of_recipe>/asr1/RESULTS.md`.
@@ -829,19 +844,35 @@
           title={{ESPnet-SE}: End-to-End Speech Enhancement and Separation Toolkit Designed for {ASR} Integration},
           author={Chenda Li and Jing Shi and Wangyou Zhang and Aswin Shanmugam Subramanian and Xuankai Chang and Naoyuki Kamo and Moto Hira and Tomoki Hayashi and Christoph Boeddeker and Zhuo Chen and Shinji Watanabe},
           booktitle={Proceedings of IEEE Spoken Language Technology Workshop (SLT)},
           pages={785--792},
           year={2021},
           organization={IEEE},
         }
-        @article{arora2021espnet,
-          title={ESPnet-SLU: Advancing Spoken Language Understanding through ESPnet},
+        @inproceedings{arora2021espnet,
+          title={{ESPnet-SLU}: Advancing Spoken Language Understanding through ESPnet},
           author={Arora, Siddhant and Dalmia, Siddharth and Denisov, Pavel and Chang, Xuankai and Ueda, Yushi and Peng, Yifan and Zhang, Yuekai and Kumar, Sujay and Ganesan, Karthik and Yan, Brian and others},
-          journal={arXiv preprint arXiv:2111.14706},
-          year={2021}
+          booktitle={ICASSP 2022-2022 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
+          pages={7167--7171},
+          year={2022},
+          organization={IEEE}
+        }
+        @inproceedings{shi2022muskits,
+          author={Shi, Jiatong and Guo, Shuai and Qian, Tao and Huo, Nan and Hayashi, Tomoki and Wu, Yuning and Xu, Frank and Chang, Xuankai and Li, Huazhe and Wu, Peter and Watanabe, Shinji and Jin, Qin},
+          title={{Muskits}: an End-to-End Music Processing Toolkit for Singing Voice Synthesis},
+          year={2022},
+          booktitle={Proceedings of Interspeech},
+          pages={4277-4281},
+          url={https://www.isca-speech.org/archive/pdfs/interspeech_2022/shi22d_interspeech.pdf}
+        }
+        @article{gao2022euro,
+          title={{EURO}: {ESPnet} Unsupervised ASR Open-source Toolkit},
+          author={Gao, Dongji and Shi, Jiatong and Chuang, Shun-Po and Garcia, Leibny Paola and Lee, Hung-yi and Watanabe, Shinji and Khudanpur, Sanjeev},
+          journal={arXiv preprint arXiv:2211.17196},
+          year={2022}
         }
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `espnet-202211/README.md` & `espnet-202301/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
 - Support singing voice synthesis recipe (ofuton_p_utagoe_db)
 
 ### ASR: Automatic Speech Recognition
 - **State-of-the-art performance** in several ASR benchmarks (comparable/superior to hybrid DNN/HMM and CTC)
 - **Hybrid CTC/attention** based end-to-end ASR
   - Fast/accurate training with CTC/attention multitask training
   - CTC/attention joint decoding to boost monotonic alignment decoding
-  - Encoder: VGG-like CNN + BiRNN (LSTM/GRU), sub-sampling BiRNN (LSTM/GRU), Transformer, Conformer or [Branchformer](https://proceedings.mlr.press/v162/peng22a.html)
+  - Encoder: VGG-like CNN + BiRNN (LSTM/GRU), sub-sampling BiRNN (LSTM/GRU), Transformer, Conformer, [Branchformer](https://proceedings.mlr.press/v162/peng22a.html), or [E-Branchformer](https://arxiv.org/abs/2210.00077)
+  - Decoder: RNN (LSTM/GRU), Transformer, or S4
 - Attention: Dot product, location-aware attention, variants of multi-head
 - Incorporate RNNLM/LSTMLM/TransformerLM/N-gram trained only with text data
 - Batch GPU decoding
 - Data augmentation
 - **Transducer** based end-to-end ASR
   - Architecture:
     - RNN-based encoder and decoder.
@@ -92,22 +93,23 @@
 - Non-autoregressive model based on Mask-CTC
 - ASR examples for supporting endangered language documentation (Please refer to egs/puebla_nahuatl and egs/yoloxochitl_mixtec for details)
 - Wav2Vec2.0 pretrained model as Encoder, imported from [FairSeq](https://github.com/pytorch/fairseq/tree/master/fairseq).
 - Self-supervised learning representations as features, using upstream models in [S3PRL](https://github.com/s3prl/s3prl) in frontend.
   - Set `frontend` to be `s3prl`
   - Select any upstream model by setting the `frontend_conf` to the corresponding name.
 - Transfer Learning :
-  - easy usage and transfers from models previously trained by your group, or models from [ESPnet huggingface repository](https://huggingface.co/espnet).
+  - easy usage and transfers from models previously trained by your group, or models from [ESPnet Hugging Face repository](https://huggingface.co/espnet).
   - [Documentation](https://github.com/espnet/espnet/tree/master/egs2/mini_an4/asr1/transfer_learning.md) and [toy example runnable on colab](https://github.com/espnet/notebook/blob/master/espnet2_asr_transfer_learning_demo.ipynb).
 - Streaming Transformer/Conformer ASR with blockwise synchronous beam search.
 - Restricted Self-Attention based on [Longformer](https://arxiv.org/abs/2004.05150) as an encoder for long sequences
+- OpenAI [Whisper](https://openai.com/blog/whisper/) model, robust ASR based on large-scale, weakly-supervised multitask learning
 
 Demonstration
 - Real-time ASR demo with ESPnet2  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/espnet/notebook/blob/master/espnet2_asr_realtime_demo.ipynb)
-- [Gradio](https://github.com/gradio-app/gradio) Web Demo on [Huggingface Spaces](https://huggingface.co/docs/hub/spaces). Check out the [Web Demo](https://huggingface.co/spaces/akhaliq/espnet2_asr)
+- [Gradio](https://github.com/gradio-app/gradio) Web Demo on [Hugging Face Spaces](https://huggingface.co/docs/hub/spaces). Check out the [Web Demo](https://huggingface.co/spaces/akhaliq/espnet2_asr)
 - Streaming Transformer ASR [Local Demo](https://github.com/espnet/notebook/blob/master/espnet2_streaming_asr_demo.ipynb) with ESPnet2.
 
 ### TTS: Text-to-speech
 - Architecture
     - Tacotron2
     - Transformer-TTS
     - FastSpeech
@@ -132,15 +134,15 @@
     - Multi-band MelGAN
     - HiFiGAN
     - StyleMelGAN
     - Mix of the above models
 
 Demonstration
 - Real-time TTS demo with ESPnet2  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/espnet/notebook/blob/master/espnet2_tts_realtime_demo.ipynb)
-- Integrated to [Huggingface Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/akhaliq/ESPnet2-TTS)
+- Integrated to [Hugging Face Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/akhaliq/ESPnet2-TTS)
 
 To train the neural vocoder, please check the following repositories:
 - [kan-bayashi/ParallelWaveGAN](https://github.com/kan-bayashi/ParallelWaveGAN)
 - [r9y9/wavenet_vocoder](https://github.com/r9y9/wavenet_vocoder)
 
 > **NOTE**:
 > - We are moving on ESPnet2-based development for TTS.
@@ -170,14 +172,15 @@
 - End-to-end VC based on cascaded ASR+TTS (Baseline system for Voice Conversion Challenge 2020!)
 
 ### SLU: Spoken Language Understanding
 - Architecture
     - Transformer based Encoder
     - Conformer based Encoder
     - [Branchformer](https://proceedings.mlr.press/v162/peng22a.html) based Encoder
+    - [E-Branchformer](https://arxiv.org/abs/2210.00077) based Encoder
     - RNN based Decoder
     - Transformer based Decoder
 - Support Multitasking with ASR
     - Predict both intent and ASR transcript
 - Support Multitasking with NLU
     - Deliberation encoder based 2 pass model
 - Support using pretrained ASR models
@@ -192,38 +195,47 @@
     - En / Jp / Zn / Nl / And more...
 - Supports using context from previous utterances
 - Supports using other tasks like SE in pipeline manner
 - Supports Two Pass SLU that combines audio and ASR transcript
 Demonstration
 - Performing noisy spoken language understanding using speech enhancement model followed by spoken language understanding model.  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14nCrJ05vJcQX0cJuXjbMVFWUHJ3Wfb6N?usp=sharing)
 - Performing two pass spoken language understanding where the second pass model attends on both acoustic and semantic information.  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1p2cbGIPpIIcynuDl4ZVHDpmNPl8Nh_ci?usp=sharing)
-- Integrated to [Huggingface Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See SLU demo on multiple languages: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Siddhant/ESPnet2-SLU)
+- Integrated to [Hugging Face Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See SLU demo on multiple languages: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Siddhant/ESPnet2-SLU)
 
 
 ### SUM: Speech Summarization
 - End to End Speech Summarization Recipe for Instructional Videos using Restricted Self-Attention [[Sharma et al., 2022]](https://arxiv.org/abs/2110.06263)
 
 ### SVS: Singing Voice Synthesis
 - Framework merge from [Muskits](https://github.com/SJTMusicTeam/Muskits)
 - Architecture
   - RNN-based non-autoregressive model
   - Xiaoice
   - Sequence-to-sequence Transformer (with GLU-based encoder)
-  - MLP singer
+  - MLP singer (in progress)
   - Tacotron-singing (in progress)
-  - DiffSinger (to be published)
-  - VISinger (in progress)
+  - DiffSinger (in progress)
+  - VISinger
 - Support multi-speaker & multilingual singing synthesis
   - Speaker ID embedding
   - Language ID embedding
-  - Global sytle token (GST) embedding
 - Various language support
   - Jp / En / Kr / Zh
 - Tight integration with neural vocoders (the same as TTS)
 
+### SSL: Self-supervised Learning
+- Support HuBERT Pretraining:
+  * Example recipe: [egs2/LibriSpeech/ssl1](egs2/LibriSpeech/ssl1)
+
+### UASR: Unsupervised ASR (EURO: ESPnet Unsupervised Recognition - Open-source)
+- Architecture
+  - wav2vec-U (with different self-supervised models)
+  - wav2vec-U 2.0 (in progress)
+- Support PrefixBeamSearch and K2-based WFST decoding
+
 ### DNN Framework
 - Flexible network architecture thanks to chainer and pytorch
 - Flexible front-end processing thanks to [kaldiio](https://github.com/nttcslab-sp/kaldiio) and HDF5 support
 - Tensorboard based monitoring
 
 ### ESPnet2
 See [ESPnet2](https://espnet.github.io/espnet/espnet2_tutorial.html).
@@ -281,24 +293,27 @@
 
 
 We list the character error rate (CER) and word error rate (WER) of major ASR tasks.
 
 | Task                                                              |     CER (%)     |     WER (%)     |                                                                              Pretrained model                                                                               |
 | ----------------------------------------------------------------- | :-------------: | :-------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
 | Aishell dev/test                                                  |     4.6/5.1     |       N/A       |                [link](https://github.com/espnet/espnet/blob/master/egs/aishell/asr1/RESULTS.md#conformer-kernel-size--15--specaugment--lm-weight--00-result)                |
-| **ESPnet2** Aishell dev/test                                      |     4.4/4.7     |       N/A       |                [link](https://github.com/espnet/espnet/tree/master/egs2/aishell/asr1#conformer--specaug--speed-perturbation-featsraw-n_fft512-hop_length128)                |
+| **ESPnet2** Aishell dev/test                                      |     4.1/4.4     |       N/A       |                [link](https://github.com/espnet/espnet/tree/master/egs2/aishell/asr1#branchformer-initial)                                                                  |
 | Common Voice dev/test                                             |     1.7/1.8     |     2.2/2.3     |    [link](https://github.com/espnet/espnet/blob/master/egs/commonvoice/asr1/RESULTS.md#first-results-default-pytorch-transformer-setting-with-bpe-100-epochs-single-gpu)    |
 | CSJ eval1/eval2/eval3                                             |   5.7/3.8/4.2   |       N/A       |                 [link](https://github.com/espnet/espnet/blob/master/egs/csj/asr1/RESULTS.md#pytorch-backend-transformer-without-any-hyperparameter-tuning)                  |
 | **ESPnet2** CSJ eval1/eval2/eval3                                 |   4.5/3.3/3.6   |       N/A       |                                        [link](https://github.com/espnet/espnet/tree/master/egs2/csj/asr1#initial-conformer-results)                                         |
+| **ESPnet2** GigaSpeech dev/test                                   |       N/A       |    10.6/10.5    |                                          [link](https://github.com/espnet/espnet/tree/master/egs2/gigaspeech/asr1#e-branchformer)                                           |
 | HKUST dev                                                         |      23.5       |       N/A       |                                  [link](https://github.com/espnet/espnet/blob/master/egs/hkust/asr1/RESULTS.md#transformer-only-20-epochs)                                  |
 | **ESPnet2** HKUST dev                                             |      21.2       |       N/A       |                                    [link](https://github.com/espnet/espnet/tree/master/egs2/hkust/asr1#transformer-asr--transformer-lm)                                     |
 | Librispeech dev_clean/dev_other/test_clean/test_other             |       N/A       | 1.9/4.9/2.1/4.9 | [link](https://github.com/espnet/espnet/blob/master/egs/librispeech/asr1/RESULTS.md#pytorch-large-conformer-with-specaug--speed-perturbation-8-gpus--transformer-lm-4-gpus) |
 | **ESPnet2** Librispeech dev_clean/dev_other/test_clean/test_other | 0.6/1.5/0.6/1.4 | 1.7/3.4/1.8/3.6 |    [link](https://github.com/espnet/espnet/tree/master/egs2/librispeech/asr1#self-supervised-learning-features-hubert_large_ll60k-conformer-utt_mvn-with-transformer-lm)    |
 | Switchboard (eval2000) callhm/swbd                                |       N/A       |    14.0/6.8     |          [link](https://github.com/espnet/espnet/blob/master/egs/swbd/asr1/RESULTS.md#conformer-with-bpe-2000-specaug-speed-perturbation-transformer-lm-decoding)           |
+| **ESPnet2** Switchboard (eval2000) callhm/swbd                    |       N/A       |    13.4/7.3     |                                             [link](https://github.com/espnet/espnet/tree/master/egs2/swbd/asr1#e-branchformer)                                              |
 | TEDLIUM2 dev/test                                                 |       N/A       |     8.6/7.2     |                 [link](https://github.com/espnet/espnet/blob/master/egs/tedlium2/asr1/RESULTS.md#conformer-large-model--specaug--speed-perturbation--rnnlm)                 |
+| **ESPnet2** TEDLIUM2 dev/test                                     |       N/A       |     7.3/7.1     |                 [link](https://github.com/espnet/espnet/blob/master/egs2/tedlium2/asr1/README.md#e-branchformer-12-encoder-layers)                                          |
 | TEDLIUM3 dev/test                                                 |       N/A       |     9.6/7.6     |                                              [link](https://github.com/espnet/espnet/blob/master/egs/tedlium3/asr1/RESULTS.md)                                              |
 | WSJ dev93/eval92                                                  |     3.2/2.1     |     7.0/4.7     |                                                                                     N/A                                                                                     |
 | **ESPnet2** WSJ dev93/eval92                                      |     1.1/0.8     |     2.8/1.8     |       [link](https://github.com/espnet/espnet/tree/master/egs2/wsj/asr1#self-supervised-learning-features-wav2vec2_large_ll60k-conformer-utt_mvn-with-transformer-lm)       |
 
 Note that the performance of the CSJ, HKUST, and Librispeech tasks was significantly improved by using the wide network (#units = 1024) and large subword units if necessary reported by [RWTH](https://arxiv.org/pdf/1805.03294.pdf).
 
 If you want to check the results of the other recipes, please check `egs/<name_of_recipe>/asr1/RESULTS.md`.
@@ -821,14 +836,30 @@
   title={{ESPnet-SE}: End-to-End Speech Enhancement and Separation Toolkit Designed for {ASR} Integration},
   author={Chenda Li and Jing Shi and Wangyou Zhang and Aswin Shanmugam Subramanian and Xuankai Chang and Naoyuki Kamo and Moto Hira and Tomoki Hayashi and Christoph Boeddeker and Zhuo Chen and Shinji Watanabe},
   booktitle={Proceedings of IEEE Spoken Language Technology Workshop (SLT)},
   pages={785--792},
   year={2021},
   organization={IEEE},
 }
-@article{arora2021espnet,
-  title={ESPnet-SLU: Advancing Spoken Language Understanding through ESPnet},
+@inproceedings{arora2021espnet,
+  title={{ESPnet-SLU}: Advancing Spoken Language Understanding through ESPnet},
   author={Arora, Siddhant and Dalmia, Siddharth and Denisov, Pavel and Chang, Xuankai and Ueda, Yushi and Peng, Yifan and Zhang, Yuekai and Kumar, Sujay and Ganesan, Karthik and Yan, Brian and others},
-  journal={arXiv preprint arXiv:2111.14706},
-  year={2021}
+  booktitle={ICASSP 2022-2022 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
+  pages={7167--7171},
+  year={2022},
+  organization={IEEE}
+}
+@inproceedings{shi2022muskits,
+  author={Shi, Jiatong and Guo, Shuai and Qian, Tao and Huo, Nan and Hayashi, Tomoki and Wu, Yuning and Xu, Frank and Chang, Xuankai and Li, Huazhe and Wu, Peter and Watanabe, Shinji and Jin, Qin},
+  title={{Muskits}: an End-to-End Music Processing Toolkit for Singing Voice Synthesis},
+  year={2022},
+  booktitle={Proceedings of Interspeech},
+  pages={4277-4281},
+  url={https://www.isca-speech.org/archive/pdfs/interspeech_2022/shi22d_interspeech.pdf}
+}
+@article{gao2022euro,
+  title={{EURO}: {ESPnet} Unsupervised ASR Open-source Toolkit},
+  author={Gao, Dongji and Shi, Jiatong and Chuang, Shun-Po and Garcia, Leibny Paola and Lee, Hung-yi and Watanabe, Shinji and Khudanpur, Sanjeev},
+  journal={arXiv preprint arXiv:2211.17196},
+  year={2022}
 }
 ```
```

### Comparing `espnet-202211/espnet/asr/asr_mix_utils.py` & `espnet-202301/espnet/asr/asr_mix_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/asr/asr_utils.py` & `espnet-202301/espnet/asr/asr_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/asr/chainer_backend/asr.py` & `espnet-202301/espnet/asr/chainer_backend/asr.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/asr/pytorch_backend/asr.py` & `espnet-202301/espnet/asr/pytorch_backend/asr.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/asr/pytorch_backend/asr_init.py` & `espnet-202301/espnet/asr/pytorch_backend/asr_init.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/asr/pytorch_backend/asr_mix.py` & `espnet-202301/espnet/asr/pytorch_backend/asr_mix.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/asr/pytorch_backend/recog.py` & `espnet-202301/espnet/asr/pytorch_backend/recog.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/asr_align.py` & `espnet-202301/espnet/bin/asr_align.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/asr_enhance.py` & `espnet-202301/espnet/bin/asr_enhance.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/asr_recog.py` & `espnet-202301/espnet/bin/asr_recog.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/asr_train.py` & `espnet-202301/espnet/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/lm_train.py` & `espnet-202301/espnet/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/mt_train.py` & `espnet-202301/espnet/bin/mt_train.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/mt_trans.py` & `espnet-202301/espnet/bin/mt_trans.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/st_train.py` & `espnet-202301/espnet/bin/st_train.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/st_trans.py` & `espnet-202301/espnet/bin/st_trans.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/tts_decode.py` & `espnet-202301/espnet/bin/tts_decode.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/tts_train.py` & `espnet-202301/espnet/bin/tts_train.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/vc_decode.py` & `espnet-202301/espnet/bin/vc_decode.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/bin/vc_train.py` & `espnet-202301/espnet/bin/vc_train.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/lm/chainer_backend/extlm.py` & `espnet-202301/espnet/lm/chainer_backend/extlm.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/lm/chainer_backend/lm.py` & `espnet-202301/espnet/lm/chainer_backend/lm.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/lm/lm_utils.py` & `espnet-202301/espnet/lm/lm_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/lm/pytorch_backend/extlm.py` & `espnet-202301/espnet/lm/pytorch_backend/extlm.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/lm/pytorch_backend/lm.py` & `espnet-202301/espnet/lm/pytorch_backend/lm.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/mt/mt_utils.py` & `espnet-202301/espnet/mt/mt_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/mt/pytorch_backend/mt.py` & `espnet-202301/espnet/mt/pytorch_backend/mt.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/asr_interface.py` & `espnet-202301/espnet/nets/asr_interface.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/batch_beam_search.py` & `espnet-202301/espnet/nets/batch_beam_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,21 +114,25 @@
 
         """
         init_states = dict()
         init_scores = dict()
         for k, d in self.scorers.items():
             init_states[k] = d.batch_init_state(x)
             init_scores[k] = 0.0
+
+        # NOTE (Shih-Lun): added for OpenAI Whisper ASR
+        primer = [self.sos] if self.hyp_primer is None else self.hyp_primer
+
         return self.batchfy(
             [
                 Hypothesis(
                     score=0.0,
                     scores=init_scores,
                     states=init_states,
-                    yseq=torch.tensor([self.sos], device=x.device),
+                    yseq=torch.tensor(primer, device=x.device),
                 )
             ]
         )
 
     def score_full(
         self, hyp: BatchHypothesis, x: torch.Tensor
     ) -> Tuple[Dict[str, torch.Tensor], Dict[str, Any]]:
```

### Comparing `espnet-202211/espnet/nets/batch_beam_search_online.py` & `espnet-202301/espnet/nets/batch_beam_search_online.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/batch_beam_search_online_sim.py` & `espnet-202301/espnet/nets/batch_beam_search_online_sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -245,14 +245,24 @@
         logging.info(f"total number of ended hypotheses: {len(nbest_hyps)}")
         if self.token_list is not None:
             logging.info(
                 "best hypo: "
                 + "".join([self.token_list[x] for x in best.yseq[1:-1]])
                 + "\n"
             )
+        if best.yseq[1:-1].shape[0] == x.shape[0]:
+            logging.warning(
+                "best hypo length: {} == max output length: {}".format(
+                    best.yseq[1:-1].shape[0], maxlen
+                )
+            )
+            logging.warning(
+                "decoding may be stopped by the max output length limitation, "
+                + "please consider to increase the maxlenratio."
+            )
         return nbest_hyps
 
     def extend(self, x: torch.Tensor, hyps: Hypothesis) -> List[Hypothesis]:
         """Extend probabilities and states with more encoded chunks.
 
         Args:
             x (torch.Tensor): The extended encoder output feature
```

### Comparing `espnet-202211/espnet/nets/beam_search.py` & `espnet-202301/espnet/nets/beam_search.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         beam_size: int,
         vocab_size: int,
         sos: int,
         eos: int,
         token_list: List[str] = None,
         pre_beam_ratio: float = 1.5,
         pre_beam_score_key: str = None,
+        hyp_primer: List[int] = None,
     ):
         """Initialize beam search.
 
         Args:
             scorers (dict[str, ScorerInterface]): Dict of decoder modules
                 e.g., Decoder, CTCPrefixScorer, LM
                 The scorer will be ignored if it is `None`
@@ -83,14 +84,18 @@
                 self.full_scorers[k] = v
             if isinstance(v, torch.nn.Module):
                 self.nn_dict[k] = v
 
         # set configurations
         self.sos = sos
         self.eos = eos
+
+        # added for OpenAI Whisper decoding
+        self.hyp_primer = hyp_primer
+
         self.token_list = token_list
         self.pre_beam_size = int(pre_beam_ratio * beam_size)
         self.beam_size = beam_size
         self.n_vocab = vocab_size
         if (
             pre_beam_score_key is not None
             and pre_beam_score_key != "full"
@@ -100,14 +105,21 @@
         self.pre_beam_score_key = pre_beam_score_key
         self.do_pre_beam = (
             self.pre_beam_score_key is not None
             and self.pre_beam_size < self.n_vocab
             and len(self.part_scorers) > 0
         )
 
+    def set_hyp_primer(self, hyp_primer: List[int] = None) -> None:
+        """Set the primer sequence for decoding.
+
+        Used for OpenAI Whisper models.
+        """
+        self.hyp_primer = hyp_primer
+
     def init_hyp(self, x: torch.Tensor) -> List[Hypothesis]:
         """Get an initial hypothesis data.
 
         Args:
             x (torch.Tensor): The encoder output feature
 
         Returns:
@@ -115,20 +127,24 @@
 
         """
         init_states = dict()
         init_scores = dict()
         for k, d in self.scorers.items():
             init_states[k] = d.init_state(x)
             init_scores[k] = 0.0
+
+        # NOTE (Shih-Lun): added for OpenAI Whisper ASR
+        primer = [self.sos] if self.hyp_primer is None else self.hyp_primer
+
         return [
             Hypothesis(
                 score=0.0,
                 scores=init_scores,
                 states=init_states,
-                yseq=torch.tensor([self.sos], device=x.device),
+                yseq=torch.tensor(primer, device=x.device),
             )
         ]
 
     @staticmethod
     def append_token(xs: torch.Tensor, x: int) -> torch.Tensor:
         """Append new token to prefix tokens.
 
@@ -399,14 +415,24 @@
         logging.info(f"total number of ended hypotheses: {len(nbest_hyps)}")
         if self.token_list is not None:
             logging.info(
                 "best hypo: "
                 + "".join([self.token_list[x] for x in best.yseq[1:-1]])
                 + "\n"
             )
+        if best.yseq[1:-1].shape[0] == x.shape[0]:
+            logging.warning(
+                "best hypo length: {} == max output length: {}".format(
+                    best.yseq[1:-1].shape[0], maxlen
+                )
+            )
+            logging.warning(
+                "decoding may be stopped by the max output length limitation, "
+                + "please consider to increase the maxlenratio."
+            )
         return nbest_hyps
 
     def post_process(
         self,
         i: int,
         maxlen: int,
         maxlenratio: float,
```

### Comparing `espnet-202211/espnet/nets/beam_search_transducer.py` & `espnet-202301/espnet/nets/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/asr_interface.py` & `espnet-202301/espnet/nets/chainer_backend/asr_interface.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/ctc.py` & `espnet-202301/espnet/nets/chainer_backend/ctc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/deterministic_embed_id.py` & `espnet-202301/espnet/nets/chainer_backend/deterministic_embed_id.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/e2e_asr.py` & `espnet-202301/espnet/nets/chainer_backend/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/e2e_asr_transformer.py` & `espnet-202301/espnet/nets/chainer_backend/e2e_asr_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/rnn/attentions.py` & `espnet-202301/espnet/nets/chainer_backend/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/rnn/decoders.py` & `espnet-202301/espnet/nets/chainer_backend/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/rnn/encoders.py` & `espnet-202301/espnet/nets/chainer_backend/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/rnn/training.py` & `espnet-202301/espnet/nets/chainer_backend/rnn/training.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/transformer/attention.py` & `espnet-202301/espnet/nets/chainer_backend/transformer/attention.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/transformer/ctc.py` & `espnet-202301/espnet/nets/chainer_backend/transformer/ctc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/transformer/decoder.py` & `espnet-202301/espnet/nets/chainer_backend/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/transformer/decoder_layer.py` & `espnet-202301/espnet/nets/chainer_backend/transformer/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/transformer/embedding.py` & `espnet-202301/espnet/nets/chainer_backend/transformer/embedding.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/transformer/encoder.py` & `espnet-202301/espnet/nets/chainer_backend/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/transformer/encoder_layer.py` & `espnet-202301/espnet/nets/chainer_backend/transformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/transformer/label_smoothing_loss.py` & `espnet-202301/espnet/nets/chainer_backend/transformer/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/transformer/positionwise_feed_forward.py` & `espnet-202301/espnet/nets/chainer_backend/transformer/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/transformer/subsampling.py` & `espnet-202301/espnet/nets/chainer_backend/transformer/subsampling.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/chainer_backend/transformer/training.py` & `espnet-202301/espnet/nets/chainer_backend/transformer/training.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/ctc_prefix_score.py` & `espnet-202301/espnet/nets/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/e2e_asr_common.py` & `espnet-202301/espnet/nets/e2e_asr_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,20 @@
 
         self.report_cer = report_cer
         self.report_wer = report_wer
 
         self.char_list = char_list
         self.space = sym_space
         self.blank = sym_blank
-        self.idx_blank = self.char_list.index(self.blank)
+        # NOTE (Shih-Lun): else case is for OpenAI Whisper ASR model,
+        #                  which doesn't use <blank> token
+        if self.blank in self.char_list:
+            self.idx_blank = self.char_list.index(self.blank)
+        else:
+            self.idx_blank = None
         if self.space in self.char_list:
             self.idx_space = self.char_list.index(self.space)
         else:
             self.idx_space = None
 
     def __call__(self, ys_hat, ys_pad, is_ctc=False):
         """Calculate sentence-level WER/CER score.
```

### Comparing `espnet-202211/espnet/nets/e2e_mt_common.py` & `espnet-202301/espnet/nets/e2e_mt_common.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/lm_interface.py` & `espnet-202301/espnet/nets/lm_interface.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/mt_interface.py` & `espnet-202301/espnet/nets/mt_interface.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/conformer/argument.py` & `espnet-202301/espnet/nets/pytorch_backend/conformer/argument.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/conformer/contextual_block_encoder_layer.py` & `espnet-202301/espnet/nets/pytorch_backend/conformer/contextual_block_encoder_layer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/conformer/convolution.py` & `espnet-202301/espnet/nets/pytorch_backend/conformer/convolution.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/conformer/encoder.py` & `espnet-202301/espnet/nets/pytorch_backend/conformer/encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/conformer/encoder_layer.py` & `espnet-202301/espnet/nets/pytorch_backend/conformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/ctc.py` & `espnet-202301/espnet/nets/pytorch_backend/ctc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_asr.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_asr_conformer.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_asr_conformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_asr_maskctc.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_asr_maskctc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_asr_mix.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_asr_mix.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_asr_mix_transformer.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_asr_mix_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_asr_mulenc.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_asr_mulenc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_asr_transducer.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_asr_transducer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_asr_transformer.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_asr_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_mt.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_mt.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_mt_transformer.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_mt_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_st.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_st.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_st_conformer.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_st_conformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_st_transformer.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_st_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_tts_fastspeech.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_tts_fastspeech.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_tts_tacotron2.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_tts_tacotron2.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_tts_transformer.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_tts_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_vc_tacotron2.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_vc_tacotron2.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/e2e_vc_transformer.py` & `espnet-202301/espnet/nets/pytorch_backend/e2e_vc_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/fastspeech/duration_calculator.py` & `espnet-202301/espnet/nets/pytorch_backend/fastspeech/duration_calculator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/fastspeech/duration_predictor.py` & `espnet-202301/espnet/nets/pytorch_backend/fastspeech/duration_predictor.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/fastspeech/length_regulator.py` & `espnet-202301/espnet/nets/pytorch_backend/fastspeech/length_regulator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/frontends/beamformer.py` & `espnet-202301/espnet/nets/pytorch_backend/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/frontends/dnn_beamformer.py` & `espnet-202301/espnet/nets/pytorch_backend/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/frontends/dnn_wpe.py` & `espnet-202301/espnet/nets/pytorch_backend/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/frontends/feature_transform.py` & `espnet-202301/espnet/nets/pytorch_backend/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/frontends/frontend.py` & `espnet-202301/espnet/nets/pytorch_backend/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/frontends/mask_estimator.py` & `espnet-202301/espnet/nets/pytorch_backend/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/gtn_ctc.py` & `espnet-202301/espnet/nets/pytorch_backend/gtn_ctc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/initialization.py` & `espnet-202301/espnet/nets/pytorch_backend/initialization.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/lm/default.py` & `espnet-202301/espnet/nets/pytorch_backend/lm/default.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/lm/seq_rnn.py` & `espnet-202301/espnet/nets/pytorch_backend/lm/seq_rnn.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/lm/transformer.py` & `espnet-202301/espnet/nets/pytorch_backend/lm/transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/maskctc/add_mask_token.py` & `espnet-202301/espnet/nets/pytorch_backend/maskctc/add_mask_token.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/maskctc/mask.py` & `espnet-202301/espnet/nets/pytorch_backend/maskctc/mask.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/nets_utils.py` & `espnet-202301/espnet/nets/pytorch_backend/nets_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/rnn/argument.py` & `espnet-202301/espnet/nets/pytorch_backend/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/rnn/attentions.py` & `espnet-202301/espnet/nets/pytorch_backend/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/rnn/decoders.py` & `espnet-202301/espnet/nets/pytorch_backend/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/rnn/encoders.py` & `espnet-202301/espnet/nets/pytorch_backend/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/streaming/segment.py` & `espnet-202301/espnet/nets/pytorch_backend/streaming/segment.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/streaming/window.py` & `espnet-202301/espnet/nets/pytorch_backend/streaming/window.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/tacotron2/cbhg.py` & `espnet-202301/espnet/nets/pytorch_backend/tacotron2/cbhg.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/tacotron2/decoder.py` & `espnet-202301/espnet/nets/pytorch_backend/tacotron2/decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/tacotron2/encoder.py` & `espnet-202301/espnet/nets/pytorch_backend/tacotron2/encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/arguments.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/arguments.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/blocks.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/blocks.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/conv1d_nets.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/conv1d_nets.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/custom_decoder.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/custom_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/custom_encoder.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/custom_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/error_calculator.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/error_calculator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/initializer.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/initializer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/joint_network.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/joint_network.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/rnn_decoder.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/rnn_encoder.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/transducer_tasks.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/transducer_tasks.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/transformer_decoder_layer.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/transformer_decoder_layer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/utils.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transducer/vgg2l.py` & `espnet-202301/espnet/nets/pytorch_backend/transducer/vgg2l.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/add_sos_eos.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/argument.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/argument.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/attention.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/attention.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/contextual_block_encoder_layer.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/contextual_block_encoder_layer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/decoder.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/decoder_layer.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/dynamic_conv.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/dynamic_conv2d.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/embedding.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/embedding.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/encoder.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/encoder_layer.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/encoder_mix.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/encoder_mix.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/initializer.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/initializer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/label_smoothing_loss.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/layer_norm.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/layer_norm.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/lightconv.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/lightconv.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/lightconv2d.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/longformer_attention.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/longformer_attention.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/mask.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/mask.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/multi_layer_conv.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/optimizer.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/optimizer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/plot.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/plot.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/positionwise_feed_forward.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/repeat.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/repeat.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/subsampling.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/subsampling.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         super().__init__(message)
         self.actual_size = actual_size
         self.limit = limit
 
 
 def check_short_utt(ins, size):
     """Check if the utterance is too short for subsampling."""
+    if isinstance(ins, Conv2dSubsampling1) and size < 5:
+        return True, 5
     if isinstance(ins, Conv2dSubsampling2) and size < 7:
         return True, 7
     if isinstance(ins, Conv2dSubsampling) and size < 7:
         return True, 7
     if isinstance(ins, Conv2dSubsampling6) and size < 11:
         return True, 11
     if isinstance(ins, Conv2dSubsampling8) and size < 15:
@@ -90,14 +92,73 @@
 
     def __getitem__(self, key):
         """Get item.
 
         When reset_parameters() is called, if use_scaled_pos_enc is used,
             return the positioning encoding.
 
+        """
+        if key != -1:
+            raise NotImplementedError("Support only `-1` (for `reset_parameters`).")
+        return self.out[key]
+
+
+class Conv2dSubsampling1(torch.nn.Module):
+    """Similar to Conv2dSubsampling module, but without any subsampling performed.
+
+    Args:
+        idim (int): Input dimension.
+        odim (int): Output dimension.
+        dropout_rate (float): Dropout rate.
+        pos_enc (torch.nn.Module): Custom position encoding layer.
+
+    """
+
+    def __init__(self, idim, odim, dropout_rate, pos_enc=None):
+        """Construct an Conv2dSubsampling1 object."""
+        super(Conv2dSubsampling1, self).__init__()
+        self.conv = torch.nn.Sequential(
+            torch.nn.Conv2d(1, odim, 3, 1),
+            torch.nn.ReLU(),
+            torch.nn.Conv2d(odim, odim, 3, 1),
+            torch.nn.ReLU(),
+        )
+        self.out = torch.nn.Sequential(
+            torch.nn.Linear(odim * (idim - 4), odim),
+            pos_enc if pos_enc is not None else PositionalEncoding(odim, dropout_rate),
+        )
+
+    def forward(self, x, x_mask):
+        """Pass x through 2 Conv2d layers without subsampling.
+
+        Args:
+            x (torch.Tensor): Input tensor (#batch, time, idim).
+            x_mask (torch.Tensor): Input mask (#batch, 1, time).
+
+        Returns:
+            torch.Tensor: Subsampled tensor (#batch, time', odim).
+                where time' = time - 4.
+            torch.Tensor: Subsampled mask (#batch, 1, time').
+                where time' = time - 4.
+
+        """
+        x = x.unsqueeze(1)  # (b, c, t, f)
+        x = self.conv(x)
+        b, c, t, f = x.size()
+        x = self.out(x.transpose(1, 2).contiguous().view(b, t, c * f))
+        if x_mask is None:
+            return x, None
+        return x, x_mask[:, :, :-4]
+
+    def __getitem__(self, key):
+        """Get item.
+
+        When reset_parameters() is called, if use_scaled_pos_enc is used,
+            return the positioning encoding.
+
         """
         if key != -1:
             raise NotImplementedError("Support only `-1` (for `reset_parameters`).")
         return self.out[key]
 
 
 class Conv2dSubsampling2(torch.nn.Module):
```

### Comparing `espnet-202211/espnet/nets/pytorch_backend/transformer/subsampling_without_posenc.py` & `espnet-202301/espnet/nets/pytorch_backend/transformer/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/pytorch_backend/wavenet.py` & `espnet-202301/espnet/nets/pytorch_backend/wavenet.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/scorer_interface.py` & `espnet-202301/espnet/nets/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/scorers/ctc.py` & `espnet-202301/espnet/nets/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/scorers/length_bonus.py` & `espnet-202301/espnet/nets/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/scorers/ngram.py` & `espnet-202301/espnet/nets/scorers/ngram.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/st_interface.py` & `espnet-202301/espnet/nets/st_interface.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/transducer_decoder_interface.py` & `espnet-202301/espnet/nets/transducer_decoder_interface.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/nets/tts_interface.py` & `espnet-202301/espnet/nets/tts_interface.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/optimizer/chainer.py` & `espnet-202301/espnet/optimizer/chainer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/optimizer/factory.py` & `espnet-202301/espnet/optimizer/factory.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/optimizer/parser.py` & `espnet-202301/espnet/optimizer/parser.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/optimizer/pytorch.py` & `espnet-202301/espnet/optimizer/pytorch.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/scheduler/chainer.py` & `espnet-202301/espnet/scheduler/chainer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/scheduler/pytorch.py` & `espnet-202301/espnet/scheduler/pytorch.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/scheduler/scheduler.py` & `espnet-202301/espnet/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/st/pytorch_backend/st.py` & `espnet-202301/espnet/st/pytorch_backend/st.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/transform/add_deltas.py` & `espnet-202301/espnet/transform/add_deltas.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/transform/channel_selector.py` & `espnet-202301/espnet/transform/channel_selector.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/transform/cmvn.py` & `espnet-202301/espnet/transform/cmvn.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/transform/functional.py` & `espnet-202301/espnet/transform/functional.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/transform/perturb.py` & `espnet-202301/espnet/transform/perturb.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/transform/spec_augment.py` & `espnet-202301/espnet/transform/spec_augment.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/transform/spectrogram.py` & `espnet-202301/espnet/transform/spectrogram.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/transform/transformation.py` & `espnet-202301/espnet/transform/transformation.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/transform/wpe.py` & `espnet-202301/espnet/transform/wpe.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/tts/pytorch_backend/tts.py` & `espnet-202301/espnet/tts/pytorch_backend/tts.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/check_kwargs.py` & `espnet-202301/espnet/utils/check_kwargs.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/cli_readers.py` & `espnet-202301/espnet/utils/cli_readers.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/cli_utils.py` & `espnet-202301/espnet/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/cli_writers.py` & `espnet-202301/espnet/utils/cli_writers.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/dataset.py` & `espnet-202301/espnet/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/deterministic_utils.py` & `espnet-202301/espnet/utils/deterministic_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/dynamic_import.py` & `espnet-202301/espnet/utils/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/fill_missing_args.py` & `espnet-202301/espnet/utils/fill_missing_args.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/io_utils.py` & `espnet-202301/espnet/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/spec_augment.py` & `espnet-202301/espnet/utils/spec_augment.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/training/batchfy.py` & `espnet-202301/espnet/utils/training/batchfy.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/training/evaluator.py` & `espnet-202301/espnet/utils/training/evaluator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/training/iterators.py` & `espnet-202301/espnet/utils/training/iterators.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/training/tensorboard_logger.py` & `espnet-202301/espnet/utils/training/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet/utils/training/train_utils.py` & `espnet-202301/espnet/utils/training/train_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet.egg-info/PKG-INFO` & `espnet-202301/espnet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espnet
-Version: 202211
+Version: 202301
 Summary: ESPnet: end-to-end speech processing toolkit
 Home-page: http://github.com/espnet/espnet
 Author: Shinji Watanabe
 Author-email: shinjiw@ieee.org
 License: Apache Software License
 Description: <div align="left"><img src="doc/image/espnet_logo1.png" width="550"/></div>
         
@@ -68,15 +68,16 @@
         - Support singing voice synthesis recipe (ofuton_p_utagoe_db)
         
         ### ASR: Automatic Speech Recognition
         - **State-of-the-art performance** in several ASR benchmarks (comparable/superior to hybrid DNN/HMM and CTC)
         - **Hybrid CTC/attention** based end-to-end ASR
           - Fast/accurate training with CTC/attention multitask training
           - CTC/attention joint decoding to boost monotonic alignment decoding
-          - Encoder: VGG-like CNN + BiRNN (LSTM/GRU), sub-sampling BiRNN (LSTM/GRU), Transformer, Conformer or [Branchformer](https://proceedings.mlr.press/v162/peng22a.html)
+          - Encoder: VGG-like CNN + BiRNN (LSTM/GRU), sub-sampling BiRNN (LSTM/GRU), Transformer, Conformer, [Branchformer](https://proceedings.mlr.press/v162/peng22a.html), or [E-Branchformer](https://arxiv.org/abs/2210.00077)
+          - Decoder: RNN (LSTM/GRU), Transformer, or S4
         - Attention: Dot product, location-aware attention, variants of multi-head
         - Incorporate RNNLM/LSTMLM/TransformerLM/N-gram trained only with text data
         - Batch GPU decoding
         - Data augmentation
         - **Transducer** based end-to-end ASR
           - Architecture:
             - RNN-based encoder and decoder.
@@ -100,22 +101,23 @@
         - Non-autoregressive model based on Mask-CTC
         - ASR examples for supporting endangered language documentation (Please refer to egs/puebla_nahuatl and egs/yoloxochitl_mixtec for details)
         - Wav2Vec2.0 pretrained model as Encoder, imported from [FairSeq](https://github.com/pytorch/fairseq/tree/master/fairseq).
         - Self-supervised learning representations as features, using upstream models in [S3PRL](https://github.com/s3prl/s3prl) in frontend.
           - Set `frontend` to be `s3prl`
           - Select any upstream model by setting the `frontend_conf` to the corresponding name.
         - Transfer Learning :
-          - easy usage and transfers from models previously trained by your group, or models from [ESPnet huggingface repository](https://huggingface.co/espnet).
+          - easy usage and transfers from models previously trained by your group, or models from [ESPnet Hugging Face repository](https://huggingface.co/espnet).
           - [Documentation](https://github.com/espnet/espnet/tree/master/egs2/mini_an4/asr1/transfer_learning.md) and [toy example runnable on colab](https://github.com/espnet/notebook/blob/master/espnet2_asr_transfer_learning_demo.ipynb).
         - Streaming Transformer/Conformer ASR with blockwise synchronous beam search.
         - Restricted Self-Attention based on [Longformer](https://arxiv.org/abs/2004.05150) as an encoder for long sequences
+        - OpenAI [Whisper](https://openai.com/blog/whisper/) model, robust ASR based on large-scale, weakly-supervised multitask learning
         
         Demonstration
         - Real-time ASR demo with ESPnet2  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/espnet/notebook/blob/master/espnet2_asr_realtime_demo.ipynb)
-        - [Gradio](https://github.com/gradio-app/gradio) Web Demo on [Huggingface Spaces](https://huggingface.co/docs/hub/spaces). Check out the [Web Demo](https://huggingface.co/spaces/akhaliq/espnet2_asr)
+        - [Gradio](https://github.com/gradio-app/gradio) Web Demo on [Hugging Face Spaces](https://huggingface.co/docs/hub/spaces). Check out the [Web Demo](https://huggingface.co/spaces/akhaliq/espnet2_asr)
         - Streaming Transformer ASR [Local Demo](https://github.com/espnet/notebook/blob/master/espnet2_streaming_asr_demo.ipynb) with ESPnet2.
         
         ### TTS: Text-to-speech
         - Architecture
             - Tacotron2
             - Transformer-TTS
             - FastSpeech
@@ -140,15 +142,15 @@
             - Multi-band MelGAN
             - HiFiGAN
             - StyleMelGAN
             - Mix of the above models
         
         Demonstration
         - Real-time TTS demo with ESPnet2  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/espnet/notebook/blob/master/espnet2_tts_realtime_demo.ipynb)
-        - Integrated to [Huggingface Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/akhaliq/ESPnet2-TTS)
+        - Integrated to [Hugging Face Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/akhaliq/ESPnet2-TTS)
         
         To train the neural vocoder, please check the following repositories:
         - [kan-bayashi/ParallelWaveGAN](https://github.com/kan-bayashi/ParallelWaveGAN)
         - [r9y9/wavenet_vocoder](https://github.com/r9y9/wavenet_vocoder)
         
         > **NOTE**:
         > - We are moving on ESPnet2-based development for TTS.
@@ -178,14 +180,15 @@
         - End-to-end VC based on cascaded ASR+TTS (Baseline system for Voice Conversion Challenge 2020!)
         
         ### SLU: Spoken Language Understanding
         - Architecture
             - Transformer based Encoder
             - Conformer based Encoder
             - [Branchformer](https://proceedings.mlr.press/v162/peng22a.html) based Encoder
+            - [E-Branchformer](https://arxiv.org/abs/2210.00077) based Encoder
             - RNN based Decoder
             - Transformer based Decoder
         - Support Multitasking with ASR
             - Predict both intent and ASR transcript
         - Support Multitasking with NLU
             - Deliberation encoder based 2 pass model
         - Support using pretrained ASR models
@@ -200,38 +203,47 @@
             - En / Jp / Zn / Nl / And more...
         - Supports using context from previous utterances
         - Supports using other tasks like SE in pipeline manner
         - Supports Two Pass SLU that combines audio and ASR transcript
         Demonstration
         - Performing noisy spoken language understanding using speech enhancement model followed by spoken language understanding model.  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14nCrJ05vJcQX0cJuXjbMVFWUHJ3Wfb6N?usp=sharing)
         - Performing two pass spoken language understanding where the second pass model attends on both acoustic and semantic information.  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1p2cbGIPpIIcynuDl4ZVHDpmNPl8Nh_ci?usp=sharing)
-        - Integrated to [Huggingface Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See SLU demo on multiple languages: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Siddhant/ESPnet2-SLU)
+        - Integrated to [Hugging Face Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). See SLU demo on multiple languages: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Siddhant/ESPnet2-SLU)
         
         
         ### SUM: Speech Summarization
         - End to End Speech Summarization Recipe for Instructional Videos using Restricted Self-Attention [[Sharma et al., 2022]](https://arxiv.org/abs/2110.06263)
         
         ### SVS: Singing Voice Synthesis
         - Framework merge from [Muskits](https://github.com/SJTMusicTeam/Muskits)
         - Architecture
           - RNN-based non-autoregressive model
           - Xiaoice
           - Sequence-to-sequence Transformer (with GLU-based encoder)
-          - MLP singer
+          - MLP singer (in progress)
           - Tacotron-singing (in progress)
-          - DiffSinger (to be published)
-          - VISinger (in progress)
+          - DiffSinger (in progress)
+          - VISinger
         - Support multi-speaker & multilingual singing synthesis
           - Speaker ID embedding
           - Language ID embedding
-          - Global sytle token (GST) embedding
         - Various language support
           - Jp / En / Kr / Zh
         - Tight integration with neural vocoders (the same as TTS)
         
+        ### SSL: Self-supervised Learning
+        - Support HuBERT Pretraining:
+          * Example recipe: [egs2/LibriSpeech/ssl1](egs2/LibriSpeech/ssl1)
+        
+        ### UASR: Unsupervised ASR (EURO: ESPnet Unsupervised Recognition - Open-source)
+        - Architecture
+          - wav2vec-U (with different self-supervised models)
+          - wav2vec-U 2.0 (in progress)
+        - Support PrefixBeamSearch and K2-based WFST decoding
+        
         ### DNN Framework
         - Flexible network architecture thanks to chainer and pytorch
         - Flexible front-end processing thanks to [kaldiio](https://github.com/nttcslab-sp/kaldiio) and HDF5 support
         - Tensorboard based monitoring
         
         ### ESPnet2
         See [ESPnet2](https://espnet.github.io/espnet/espnet2_tutorial.html).
@@ -289,24 +301,27 @@
         
         
         We list the character error rate (CER) and word error rate (WER) of major ASR tasks.
         
         | Task                                                              |     CER (%)     |     WER (%)     |                                                                              Pretrained model                                                                               |
         | ----------------------------------------------------------------- | :-------------: | :-------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
         | Aishell dev/test                                                  |     4.6/5.1     |       N/A       |                [link](https://github.com/espnet/espnet/blob/master/egs/aishell/asr1/RESULTS.md#conformer-kernel-size--15--specaugment--lm-weight--00-result)                |
-        | **ESPnet2** Aishell dev/test                                      |     4.4/4.7     |       N/A       |                [link](https://github.com/espnet/espnet/tree/master/egs2/aishell/asr1#conformer--specaug--speed-perturbation-featsraw-n_fft512-hop_length128)                |
+        | **ESPnet2** Aishell dev/test                                      |     4.1/4.4     |       N/A       |                [link](https://github.com/espnet/espnet/tree/master/egs2/aishell/asr1#branchformer-initial)                                                                  |
         | Common Voice dev/test                                             |     1.7/1.8     |     2.2/2.3     |    [link](https://github.com/espnet/espnet/blob/master/egs/commonvoice/asr1/RESULTS.md#first-results-default-pytorch-transformer-setting-with-bpe-100-epochs-single-gpu)    |
         | CSJ eval1/eval2/eval3                                             |   5.7/3.8/4.2   |       N/A       |                 [link](https://github.com/espnet/espnet/blob/master/egs/csj/asr1/RESULTS.md#pytorch-backend-transformer-without-any-hyperparameter-tuning)                  |
         | **ESPnet2** CSJ eval1/eval2/eval3                                 |   4.5/3.3/3.6   |       N/A       |                                        [link](https://github.com/espnet/espnet/tree/master/egs2/csj/asr1#initial-conformer-results)                                         |
+        | **ESPnet2** GigaSpeech dev/test                                   |       N/A       |    10.6/10.5    |                                          [link](https://github.com/espnet/espnet/tree/master/egs2/gigaspeech/asr1#e-branchformer)                                           |
         | HKUST dev                                                         |      23.5       |       N/A       |                                  [link](https://github.com/espnet/espnet/blob/master/egs/hkust/asr1/RESULTS.md#transformer-only-20-epochs)                                  |
         | **ESPnet2** HKUST dev                                             |      21.2       |       N/A       |                                    [link](https://github.com/espnet/espnet/tree/master/egs2/hkust/asr1#transformer-asr--transformer-lm)                                     |
         | Librispeech dev_clean/dev_other/test_clean/test_other             |       N/A       | 1.9/4.9/2.1/4.9 | [link](https://github.com/espnet/espnet/blob/master/egs/librispeech/asr1/RESULTS.md#pytorch-large-conformer-with-specaug--speed-perturbation-8-gpus--transformer-lm-4-gpus) |
         | **ESPnet2** Librispeech dev_clean/dev_other/test_clean/test_other | 0.6/1.5/0.6/1.4 | 1.7/3.4/1.8/3.6 |    [link](https://github.com/espnet/espnet/tree/master/egs2/librispeech/asr1#self-supervised-learning-features-hubert_large_ll60k-conformer-utt_mvn-with-transformer-lm)    |
         | Switchboard (eval2000) callhm/swbd                                |       N/A       |    14.0/6.8     |          [link](https://github.com/espnet/espnet/blob/master/egs/swbd/asr1/RESULTS.md#conformer-with-bpe-2000-specaug-speed-perturbation-transformer-lm-decoding)           |
+        | **ESPnet2** Switchboard (eval2000) callhm/swbd                    |       N/A       |    13.4/7.3     |                                             [link](https://github.com/espnet/espnet/tree/master/egs2/swbd/asr1#e-branchformer)                                              |
         | TEDLIUM2 dev/test                                                 |       N/A       |     8.6/7.2     |                 [link](https://github.com/espnet/espnet/blob/master/egs/tedlium2/asr1/RESULTS.md#conformer-large-model--specaug--speed-perturbation--rnnlm)                 |
+        | **ESPnet2** TEDLIUM2 dev/test                                     |       N/A       |     7.3/7.1     |                 [link](https://github.com/espnet/espnet/blob/master/egs2/tedlium2/asr1/README.md#e-branchformer-12-encoder-layers)                                          |
         | TEDLIUM3 dev/test                                                 |       N/A       |     9.6/7.6     |                                              [link](https://github.com/espnet/espnet/blob/master/egs/tedlium3/asr1/RESULTS.md)                                              |
         | WSJ dev93/eval92                                                  |     3.2/2.1     |     7.0/4.7     |                                                                                     N/A                                                                                     |
         | **ESPnet2** WSJ dev93/eval92                                      |     1.1/0.8     |     2.8/1.8     |       [link](https://github.com/espnet/espnet/tree/master/egs2/wsj/asr1#self-supervised-learning-features-wav2vec2_large_ll60k-conformer-utt_mvn-with-transformer-lm)       |
         
         Note that the performance of the CSJ, HKUST, and Librispeech tasks was significantly improved by using the wide network (#units = 1024) and large subword units if necessary reported by [RWTH](https://arxiv.org/pdf/1805.03294.pdf).
         
         If you want to check the results of the other recipes, please check `egs/<name_of_recipe>/asr1/RESULTS.md`.
@@ -829,19 +844,35 @@
           title={{ESPnet-SE}: End-to-End Speech Enhancement and Separation Toolkit Designed for {ASR} Integration},
           author={Chenda Li and Jing Shi and Wangyou Zhang and Aswin Shanmugam Subramanian and Xuankai Chang and Naoyuki Kamo and Moto Hira and Tomoki Hayashi and Christoph Boeddeker and Zhuo Chen and Shinji Watanabe},
           booktitle={Proceedings of IEEE Spoken Language Technology Workshop (SLT)},
           pages={785--792},
           year={2021},
           organization={IEEE},
         }
-        @article{arora2021espnet,
-          title={ESPnet-SLU: Advancing Spoken Language Understanding through ESPnet},
+        @inproceedings{arora2021espnet,
+          title={{ESPnet-SLU}: Advancing Spoken Language Understanding through ESPnet},
           author={Arora, Siddhant and Dalmia, Siddharth and Denisov, Pavel and Chang, Xuankai and Ueda, Yushi and Peng, Yifan and Zhang, Yuekai and Kumar, Sujay and Ganesan, Karthik and Yan, Brian and others},
-          journal={arXiv preprint arXiv:2111.14706},
-          year={2021}
+          booktitle={ICASSP 2022-2022 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
+          pages={7167--7171},
+          year={2022},
+          organization={IEEE}
+        }
+        @inproceedings{shi2022muskits,
+          author={Shi, Jiatong and Guo, Shuai and Qian, Tao and Huo, Nan and Hayashi, Tomoki and Wu, Yuning and Xu, Frank and Chang, Xuankai and Li, Huazhe and Wu, Peter and Watanabe, Shinji and Jin, Qin},
+          title={{Muskits}: an End-to-End Music Processing Toolkit for Singing Voice Synthesis},
+          year={2022},
+          booktitle={Proceedings of Interspeech},
+          pages={4277-4281},
+          url={https://www.isca-speech.org/archive/pdfs/interspeech_2022/shi22d_interspeech.pdf}
+        }
+        @article{gao2022euro,
+          title={{EURO}: {ESPnet} Unsupervised ASR Open-source Toolkit},
+          author={Gao, Dongji and Shi, Jiatong and Chuang, Shun-Po and Garcia, Leibny Paola and Lee, Hung-yi and Watanabe, Shinji and Khudanpur, Sanjeev},
+          journal={arXiv preprint arXiv:2211.17196},
+          year={2022}
         }
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `espnet-202211/espnet.egg-info/SOURCES.txt` & `espnet-202301/espnet.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 espnet/mt/pytorch_backend/mt.py
 espnet/nets/__init__.py
 espnet/nets/asr_interface.py
 espnet/nets/batch_beam_search.py
 espnet/nets/batch_beam_search_online.py
 espnet/nets/batch_beam_search_online_sim.py
 espnet/nets/beam_search.py
+espnet/nets/beam_search_timesync.py
 espnet/nets/beam_search_transducer.py
 espnet/nets/ctc_prefix_score.py
 espnet/nets/e2e_asr_common.py
 espnet/nets/e2e_mt_common.py
 espnet/nets/lm_interface.py
 espnet/nets/mt_interface.py
 espnet/nets/scorer_interface.py
@@ -191,14 +192,15 @@
 espnet/nets/pytorch_backend/transformer/repeat.py
 espnet/nets/pytorch_backend/transformer/subsampling.py
 espnet/nets/pytorch_backend/transformer/subsampling_without_posenc.py
 espnet/nets/scorers/__init__.py
 espnet/nets/scorers/ctc.py
 espnet/nets/scorers/length_bonus.py
 espnet/nets/scorers/ngram.py
+espnet/nets/scorers/uasr.py
 espnet/optimizer/__init__.py
 espnet/optimizer/chainer.py
 espnet/optimizer/factory.py
 espnet/optimizer/parser.py
 espnet/optimizer/pytorch.py
 espnet/scheduler/__init__.py
 espnet/scheduler/chainer.py
@@ -245,49 +247,66 @@
 espnet2/asr/maskctc_model.py
 espnet2/asr/pit_espnet_model.py
 espnet2/asr/decoder/__init__.py
 espnet2/asr/decoder/abs_decoder.py
 espnet2/asr/decoder/hugging_face_transformers_decoder.py
 espnet2/asr/decoder/mlm_decoder.py
 espnet2/asr/decoder/rnn_decoder.py
+espnet2/asr/decoder/s4_decoder.py
 espnet2/asr/decoder/transducer_decoder.py
 espnet2/asr/decoder/transformer_decoder.py
+espnet2/asr/decoder/whisper_decoder.py
 espnet2/asr/encoder/__init__.py
 espnet2/asr/encoder/abs_encoder.py
 espnet2/asr/encoder/branchformer_encoder.py
 espnet2/asr/encoder/conformer_encoder.py
 espnet2/asr/encoder/contextual_block_conformer_encoder.py
 espnet2/asr/encoder/contextual_block_transformer_encoder.py
 espnet2/asr/encoder/e_branchformer_encoder.py
 espnet2/asr/encoder/hubert_encoder.py
 espnet2/asr/encoder/longformer_encoder.py
 espnet2/asr/encoder/rnn_encoder.py
 espnet2/asr/encoder/transformer_encoder.py
 espnet2/asr/encoder/transformer_encoder_multispkr.py
 espnet2/asr/encoder/vgg_rnn_encoder.py
 espnet2/asr/encoder/wav2vec2_encoder.py
+espnet2/asr/encoder/whisper_encoder.py
 espnet2/asr/frontend/__init__.py
 espnet2/asr/frontend/abs_frontend.py
 espnet2/asr/frontend/default.py
 espnet2/asr/frontend/fused.py
 espnet2/asr/frontend/s3prl.py
+espnet2/asr/frontend/whisper.py
 espnet2/asr/frontend/windowing.py
 espnet2/asr/layers/__init__.py
 espnet2/asr/layers/cgmlp.py
 espnet2/asr/layers/fastformer.py
 espnet2/asr/postencoder/__init__.py
 espnet2/asr/postencoder/abs_postencoder.py
 espnet2/asr/postencoder/hugging_face_transformers_postencoder.py
 espnet2/asr/preencoder/__init__.py
 espnet2/asr/preencoder/abs_preencoder.py
 espnet2/asr/preencoder/linear.py
 espnet2/asr/preencoder/sinc.py
 espnet2/asr/specaug/__init__.py
 espnet2/asr/specaug/abs_specaug.py
 espnet2/asr/specaug/specaug.py
+espnet2/asr/state_spaces/__init__.py
+espnet2/asr/state_spaces/attention.py
+espnet2/asr/state_spaces/base.py
+espnet2/asr/state_spaces/block.py
+espnet2/asr/state_spaces/cauchy.py
+espnet2/asr/state_spaces/components.py
+espnet2/asr/state_spaces/ff.py
+espnet2/asr/state_spaces/model.py
+espnet2/asr/state_spaces/pool.py
+espnet2/asr/state_spaces/registry.py
+espnet2/asr/state_spaces/residual.py
+espnet2/asr/state_spaces/s4.py
+espnet2/asr/state_spaces/utils.py
 espnet2/asr/transducer/__init__.py
 espnet2/asr/transducer/beam_search_transducer.py
 espnet2/asr/transducer/error_calculator.py
 espnet2/asr_transducer/__init__.py
 espnet2/asr_transducer/activation.py
 espnet2/asr_transducer/beam_search_transducer.py
 espnet2/asr_transducer/error_calculator.py
@@ -325,14 +344,17 @@
 espnet2/bin/asr_transducer_train.py
 espnet2/bin/diar_inference.py
 espnet2/bin/diar_train.py
 espnet2/bin/enh_inference.py
 espnet2/bin/enh_s2t_train.py
 espnet2/bin/enh_scoring.py
 espnet2/bin/enh_train.py
+espnet2/bin/enh_tse_inference.py
+espnet2/bin/enh_tse_train.py
+espnet2/bin/gan_svs_train.py
 espnet2/bin/gan_tts_train.py
 espnet2/bin/hubert_train.py
 espnet2/bin/hugging_face_export_vocabulary.py
 espnet2/bin/launch.py
 espnet2/bin/lm_calc_perplexity.py
 espnet2/bin/lm_train.py
 espnet2/bin/mt_inference.py
@@ -345,14 +367,19 @@
 espnet2/bin/st_inference_streaming.py
 espnet2/bin/st_train.py
 espnet2/bin/svs_inference.py
 espnet2/bin/svs_train.py
 espnet2/bin/tokenize_text.py
 espnet2/bin/tts_inference.py
 espnet2/bin/tts_train.py
+espnet2/bin/uasr_extract_feature.py
+espnet2/bin/uasr_inference.py
+espnet2/bin/uasr_inference_k2.py
+espnet2/bin/uasr_train.py
+espnet2/bin/whisper_export_vocabulary.py
 espnet2/diar/__init__.py
 espnet2/diar/abs_diar.py
 espnet2/diar/espnet_model.py
 espnet2/diar/label_processor.py
 espnet2/diar/attractor/__init__.py
 espnet2/diar/attractor/abs_attractor.py
 espnet2/diar/attractor/rnn_attractor.py
@@ -365,25 +392,30 @@
 espnet2/diar/layers/tcn_nomask.py
 espnet2/diar/separator/__init__.py
 espnet2/diar/separator/tcn_separator_nomask.py
 espnet2/enh/__init__.py
 espnet2/enh/abs_enh.py
 espnet2/enh/espnet_enh_s2t_model.py
 espnet2/enh/espnet_model.py
+espnet2/enh/espnet_model_tse.py
 espnet2/enh/decoder/__init__.py
 espnet2/enh/decoder/abs_decoder.py
 espnet2/enh/decoder/conv_decoder.py
 espnet2/enh/decoder/null_decoder.py
 espnet2/enh/decoder/stft_decoder.py
 espnet2/enh/encoder/__init__.py
 espnet2/enh/encoder/abs_encoder.py
 espnet2/enh/encoder/conv_encoder.py
 espnet2/enh/encoder/null_encoder.py
 espnet2/enh/encoder/stft_encoder.py
+espnet2/enh/extractor/__init__.py
+espnet2/enh/extractor/abs_extractor.py
+espnet2/enh/extractor/td_speakerbeam_extractor.py
 espnet2/enh/layers/__init__.py
+espnet2/enh/layers/adapt_layers.py
 espnet2/enh/layers/beamformer.py
 espnet2/enh/layers/beamformer_th.py
 espnet2/enh/layers/complex_utils.py
 espnet2/enh/layers/complexnn.py
 espnet2/enh/layers/conv_utils.py
 espnet2/enh/layers/dc_crn.py
 espnet2/enh/layers/dnn_beamformer.py
@@ -433,14 +465,30 @@
 espnet2/fileio/datadir_writer.py
 espnet2/fileio/npy_scp.py
 espnet2/fileio/rand_gen_dataset.py
 espnet2/fileio/read_text.py
 espnet2/fileio/rttm.py
 espnet2/fileio/score_scp.py
 espnet2/fileio/sound_scp.py
+espnet2/fileio/vad_scp.py
+espnet2/fst/__init__.py
+espnet2/fst/lm_rescore.py
+espnet2/gan_svs/__init__.py
+espnet2/gan_svs/abs_gan_svs.py
+espnet2/gan_svs/espnet_model.py
+espnet2/gan_svs/vits/__init__.py
+espnet2/gan_svs/vits/duration_predictor.py
+espnet2/gan_svs/vits/frame_prior_net.py
+espnet2/gan_svs/vits/generator.py
+espnet2/gan_svs/vits/length_regulator.py
+espnet2/gan_svs/vits/modules.py
+espnet2/gan_svs/vits/phoneme_predictor.py
+espnet2/gan_svs/vits/pitch_predictor.py
+espnet2/gan_svs/vits/text_encoder.py
+espnet2/gan_svs/vits/vits.py
 espnet2/gan_tts/__init__.py
 espnet2/gan_tts/abs_gan_tts.py
 espnet2/gan_tts/espnet_model.py
 espnet2/gan_tts/hifigan/__init__.py
 espnet2/gan_tts/hifigan/hifigan.py
 espnet2/gan_tts/hifigan/loss.py
 espnet2/gan_tts/hifigan/residual_block.py
@@ -509,14 +557,15 @@
 espnet2/main_funcs/collect_stats.py
 espnet2/main_funcs/pack_funcs.py
 espnet2/mt/__init__.py
 espnet2/mt/espnet_model.py
 espnet2/mt/frontend/__init__.py
 espnet2/mt/frontend/embedding.py
 espnet2/optimizers/__init__.py
+espnet2/optimizers/optim_groups.py
 espnet2/optimizers/sgd.py
 espnet2/samplers/__init__.py
 espnet2/samplers/abs_sampler.py
 espnet2/samplers/build_batch_sampler.py
 espnet2/samplers/folded_batch_sampler.py
 espnet2/samplers/length_batch_sampler.py
 espnet2/samplers/num_elements_batch_sampler.py
@@ -550,32 +599,37 @@
 espnet2/tasks/__init__.py
 espnet2/tasks/abs_task.py
 espnet2/tasks/asr.py
 espnet2/tasks/asr_transducer.py
 espnet2/tasks/diar.py
 espnet2/tasks/enh.py
 espnet2/tasks/enh_s2t.py
+espnet2/tasks/enh_tse.py
+espnet2/tasks/gan_svs.py
 espnet2/tasks/gan_tts.py
 espnet2/tasks/hubert.py
 espnet2/tasks/lm.py
 espnet2/tasks/mt.py
 espnet2/tasks/slu.py
 espnet2/tasks/st.py
 espnet2/tasks/svs.py
 espnet2/tasks/tts.py
+espnet2/tasks/uasr.py
 espnet2/text/__init__.py
 espnet2/text/abs_tokenizer.py
 espnet2/text/build_tokenizer.py
 espnet2/text/char_tokenizer.py
 espnet2/text/cleaner.py
 espnet2/text/hugging_face_tokenizer.py
 espnet2/text/korean_cleaner.py
 espnet2/text/phoneme_tokenizer.py
 espnet2/text/sentencepiece_tokenizer.py
 espnet2/text/token_id_converter.py
+espnet2/text/whisper_token_id_converter.py
+espnet2/text/whisper_tokenizer.py
 espnet2/text/word_tokenizer.py
 espnet2/torch_utils/__init__.py
 espnet2/torch_utils/add_gradient_noise.py
 espnet2/torch_utils/device_funcs.py
 espnet2/torch_utils/forward_adaptor.py
 espnet2/torch_utils/get_layer_from_string.py
 espnet2/torch_utils/initialize.py
@@ -592,14 +646,15 @@
 espnet2/train/dataset.py
 espnet2/train/distributed_utils.py
 espnet2/train/gan_trainer.py
 espnet2/train/iterable_dataset.py
 espnet2/train/preprocessor.py
 espnet2/train/reporter.py
 espnet2/train/trainer.py
+espnet2/train/uasr_trainer.py
 espnet2/tts/__init__.py
 espnet2/tts/abs_tts.py
 espnet2/tts/espnet_model.py
 espnet2/tts/fastspeech/__init__.py
 espnet2/tts/fastspeech/fastspeech.py
 espnet2/tts/fastspeech2/__init__.py
 espnet2/tts/fastspeech2/fastspeech2.py
@@ -610,21 +665,44 @@
 espnet2/tts/feats_extract/dio.py
 espnet2/tts/feats_extract/energy.py
 espnet2/tts/feats_extract/linear_spectrogram.py
 espnet2/tts/feats_extract/log_mel_fbank.py
 espnet2/tts/feats_extract/log_spectrogram.py
 espnet2/tts/gst/__init__.py
 espnet2/tts/gst/style_encoder.py
+espnet2/tts/prodiff/__init__.py
+espnet2/tts/prodiff/denoiser.py
+espnet2/tts/prodiff/loss.py
+espnet2/tts/prodiff/prodiff.py
 espnet2/tts/tacotron2/__init__.py
 espnet2/tts/tacotron2/tacotron2.py
 espnet2/tts/transformer/__init__.py
 espnet2/tts/transformer/transformer.py
 espnet2/tts/utils/__init__.py
 espnet2/tts/utils/duration_calculator.py
 espnet2/tts/utils/parallel_wavegan_pretrained_vocoder.py
+espnet2/uasr/__init__.py
+espnet2/uasr/espnet_model.py
+espnet2/uasr/discriminator/__init__.py
+espnet2/uasr/discriminator/abs_discriminator.py
+espnet2/uasr/discriminator/conv_discriminator.py
+espnet2/uasr/generator/__init__.py
+espnet2/uasr/generator/abs_generator.py
+espnet2/uasr/generator/conv_generator.py
+espnet2/uasr/loss/__init__.py
+espnet2/uasr/loss/abs_loss.py
+espnet2/uasr/loss/discriminator_loss.py
+espnet2/uasr/loss/gradient_penalty.py
+espnet2/uasr/loss/phoneme_diversity_loss.py
+espnet2/uasr/loss/pseudo_label_loss.py
+espnet2/uasr/loss/smoothness_penalty.py
+espnet2/uasr/segmenter/__init__.py
+espnet2/uasr/segmenter/abs_segmenter.py
+espnet2/uasr/segmenter/join_segmenter.py
+espnet2/uasr/segmenter/random_segmenter.py
 espnet2/utils/__init__.py
 espnet2/utils/build_dataclass.py
 espnet2/utils/config_argparse.py
 espnet2/utils/get_default_kwargs.py
 espnet2/utils/griffin_lim.py
 espnet2/utils/kwargs2args.py
 espnet2/utils/nested_dict_action.py
@@ -632,14 +710,15 @@
 espnet2/utils/types.py
 espnet2/utils/yaml_no_alias_safe_dump.py
 test/test_asr_init.py
 test/test_asr_interface.py
 test/test_asr_quantize.py
 test/test_batch_beam_search.py
 test/test_beam_search.py
+test/test_beam_search_timesync.py
 test/test_cli.py
 test/test_custom_transducer.py
 test/test_distributed_launch.py
 test/test_e2e_asr.py
 test/test_e2e_asr_conformer.py
 test/test_e2e_asr_maskctc.py
 test/test_e2e_asr_mulenc.py
```

### Comparing `espnet-202211/espnet.egg-info/requires.txt` & `espnet-202301/espnet.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 h5py>=2.10.0
 kaldiio>=2.17.0
 torch>=1.3.0
 torch_complex
 nltk>=3.4.5
 numpy
 protobuf<=3.20.1
+hydra-core
+opt-einsum
 sentencepiece
 ctc-segmentation>=1.6.6
 pyworld>=0.2.10
 pypinyin<=0.44.0
 espnet_tts_frontend
 ci_sdr
 pytorch_wpe
 fast-bss-eval==0.1.3
+editdistance
 importlib-metadata<5.0
 
 [all]
 torchaudio
 torch_optimizer
 fairscale
 transformers
@@ -46,14 +49,16 @@
 nnmnkwii
 museval>=0.2.1
 pystoi>=0.2.2
 mir-eval>=0.6
 fastdtw
 nara_wpe>=0.0.5
 sacrebleu>=1.5.1
+praatio>=5.1.1
+scikit-learn>=1.0.0
 
 [doc]
 Jinja2<3.1
 Sphinx==2.1.2
 sphinx-rtd-theme>=0.2.4
 sphinx-argparse>=0.2.5
 commonmark==0.8.1
@@ -71,14 +76,16 @@
 nnmnkwii
 museval>=0.2.1
 pystoi>=0.2.2
 mir-eval>=0.6
 fastdtw
 nara_wpe>=0.0.5
 sacrebleu>=1.5.1
+praatio>=5.1.1
+scikit-learn>=1.0.0
 
 [test]
 pytest>=3.3.0
 pytest-timeouts>=1.2.1
 pytest-pythonpath>=0.7.3
 pytest-cov>=2.7.1
 hacking>=2.0.0
```

### Comparing `espnet-202211/espnet2/asr/ctc.py` & `espnet-202301/espnet2/asr/ctc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/decoder/hugging_face_transformers_decoder.py` & `espnet-202301/espnet2/asr/decoder/hugging_face_transformers_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/decoder/mlm_decoder.py` & `espnet-202301/espnet2/asr/decoder/mlm_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/decoder/rnn_decoder.py` & `espnet-202301/espnet2/asr/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/decoder/transducer_decoder.py` & `espnet-202301/espnet2/asr/decoder/transducer_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/decoder/transformer_decoder.py` & `espnet-202301/espnet2/asr/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/encoder/branchformer_encoder.py` & `espnet-202301/espnet2/asr/encoder/branchformer_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     RelPositionalEncoding,
     ScaledPositionalEncoding,
 )
 from espnet.nets.pytorch_backend.transformer.layer_norm import LayerNorm
 from espnet.nets.pytorch_backend.transformer.repeat import repeat
 from espnet.nets.pytorch_backend.transformer.subsampling import (
     Conv2dSubsampling,
+    Conv2dSubsampling1,
     Conv2dSubsampling2,
     Conv2dSubsampling6,
     Conv2dSubsampling8,
     TooShortUttError,
     check_short_utt,
 )
 
@@ -362,14 +363,21 @@
         elif input_layer == "conv2d":
             self.embed = Conv2dSubsampling(
                 input_size,
                 output_size,
                 dropout_rate,
                 pos_enc_class(output_size, positional_dropout_rate),
             )
+        elif input_layer == "conv2d1":
+            self.embed = Conv2dSubsampling1(
+                input_size,
+                output_size,
+                dropout_rate,
+                pos_enc_class(output_size, positional_dropout_rate),
+            )
         elif input_layer == "conv2d2":
             self.embed = Conv2dSubsampling2(
                 input_size,
                 output_size,
                 dropout_rate,
                 pos_enc_class(output_size, positional_dropout_rate),
             )
@@ -517,14 +525,15 @@
 
         """
 
         masks = (~make_pad_mask(ilens)[:, None, :]).to(xs_pad.device)
 
         if (
             isinstance(self.embed, Conv2dSubsampling)
+            or isinstance(self.embed, Conv2dSubsampling1)
             or isinstance(self.embed, Conv2dSubsampling2)
             or isinstance(self.embed, Conv2dSubsampling6)
             or isinstance(self.embed, Conv2dSubsampling8)
         ):
             short_status, limit_size = check_short_utt(self.embed, xs_pad.size(1))
             if short_status:
                 raise TooShortUttError(
```

### Comparing `espnet-202211/espnet2/asr/encoder/conformer_encoder.py` & `espnet-202301/espnet2/asr/encoder/conformer_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 )
 from espnet.nets.pytorch_backend.transformer.positionwise_feed_forward import (
     PositionwiseFeedForward,
 )
 from espnet.nets.pytorch_backend.transformer.repeat import repeat
 from espnet.nets.pytorch_backend.transformer.subsampling import (
     Conv2dSubsampling,
+    Conv2dSubsampling1,
     Conv2dSubsampling2,
     Conv2dSubsampling6,
     Conv2dSubsampling8,
     TooShortUttError,
     check_short_utt,
 )
 
@@ -151,14 +152,21 @@
         elif input_layer == "conv2d":
             self.embed = Conv2dSubsampling(
                 input_size,
                 output_size,
                 dropout_rate,
                 pos_enc_class(output_size, positional_dropout_rate, max_pos_emb_len),
             )
+        elif input_layer == "conv2d1":
+            self.embed = Conv2dSubsampling1(
+                input_size,
+                output_size,
+                dropout_rate,
+                pos_enc_class(output_size, positional_dropout_rate, max_pos_emb_len),
+            )
         elif input_layer == "conv2d2":
             self.embed = Conv2dSubsampling2(
                 input_size,
                 output_size,
                 dropout_rate,
                 pos_enc_class(output_size, positional_dropout_rate, max_pos_emb_len),
             )
@@ -309,14 +317,15 @@
             torch.Tensor: Not to be used now.
 
         """
         masks = (~make_pad_mask(ilens)[:, None, :]).to(xs_pad.device)
 
         if (
             isinstance(self.embed, Conv2dSubsampling)
+            or isinstance(self.embed, Conv2dSubsampling1)
             or isinstance(self.embed, Conv2dSubsampling2)
             or isinstance(self.embed, Conv2dSubsampling6)
             or isinstance(self.embed, Conv2dSubsampling8)
         ):
             short_status, limit_size = check_short_utt(self.embed, xs_pad.size(1))
             if short_status:
                 raise TooShortUttError(
```

### Comparing `espnet-202211/espnet2/asr/encoder/contextual_block_conformer_encoder.py` & `espnet-202301/espnet2/asr/encoder/contextual_block_conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/encoder/contextual_block_transformer_encoder.py` & `espnet-202301/espnet2/asr/encoder/contextual_block_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/encoder/e_branchformer_encoder.py` & `espnet-202301/espnet2/asr/encoder/e_branchformer_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from espnet.nets.pytorch_backend.transformer.layer_norm import LayerNorm
 from espnet.nets.pytorch_backend.transformer.positionwise_feed_forward import (
     PositionwiseFeedForward,
 )
 from espnet.nets.pytorch_backend.transformer.repeat import repeat
 from espnet.nets.pytorch_backend.transformer.subsampling import (
     Conv2dSubsampling,
+    Conv2dSubsampling1,
     Conv2dSubsampling2,
     Conv2dSubsampling6,
     Conv2dSubsampling8,
     TooShortUttError,
     check_short_utt,
 )
 
@@ -248,14 +249,21 @@
         elif input_layer == "conv2d":
             self.embed = Conv2dSubsampling(
                 input_size,
                 output_size,
                 dropout_rate,
                 pos_enc_class(output_size, positional_dropout_rate, max_pos_emb_len),
             )
+        elif input_layer == "conv2d1":
+            self.embed = Conv2dSubsampling1(
+                input_size,
+                output_size,
+                dropout_rate,
+                pos_enc_class(output_size, positional_dropout_rate, max_pos_emb_len),
+            )
         elif input_layer == "conv2d2":
             self.embed = Conv2dSubsampling2(
                 input_size,
                 output_size,
                 dropout_rate,
                 pos_enc_class(output_size, positional_dropout_rate, max_pos_emb_len),
             )
@@ -391,14 +399,15 @@
             torch.Tensor: Not to be used now.
         """
 
         masks = (~make_pad_mask(ilens)[:, None, :]).to(xs_pad.device)
 
         if (
             isinstance(self.embed, Conv2dSubsampling)
+            or isinstance(self.embed, Conv2dSubsampling1)
             or isinstance(self.embed, Conv2dSubsampling2)
             or isinstance(self.embed, Conv2dSubsampling6)
             or isinstance(self.embed, Conv2dSubsampling8)
         ):
             short_status, limit_size = check_short_utt(self.embed, xs_pad.size(1))
             if short_status:
                 raise TooShortUttError(
```

### Comparing `espnet-202211/espnet2/asr/encoder/longformer_encoder.py` & `espnet-202301/espnet2/asr/encoder/longformer_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 )
 from espnet.nets.pytorch_backend.transformer.positionwise_feed_forward import (
     PositionwiseFeedForward,
 )
 from espnet.nets.pytorch_backend.transformer.repeat import repeat
 from espnet.nets.pytorch_backend.transformer.subsampling import (
     Conv2dSubsampling,
+    Conv2dSubsampling1,
     Conv2dSubsampling2,
     Conv2dSubsampling6,
     Conv2dSubsampling8,
     TooShortUttError,
     check_short_utt,
 )
 
@@ -154,14 +155,21 @@
         elif input_layer == "conv2d":
             self.embed = Conv2dSubsampling(
                 input_size,
                 output_size,
                 dropout_rate,
                 pos_enc_class(output_size, positional_dropout_rate),
             )
+        elif input_layer == "conv2d1":
+            self.embed = Conv2dSubsampling1(
+                input_size,
+                output_size,
+                dropout_rate,
+                pos_enc_class(output_size, positional_dropout_rate),
+            )
         elif input_layer == "conv2d2":
             self.embed = Conv2dSubsampling2(
                 input_size,
                 output_size,
                 dropout_rate,
                 pos_enc_class(output_size, positional_dropout_rate),
             )
@@ -300,14 +308,15 @@
             torch.Tensor: Not to be used now.
 
         """
 
         masks = (~make_pad_mask(ilens)[:, None, :]).to(xs_pad.device)
         if (
             isinstance(self.embed, Conv2dSubsampling)
+            or isinstance(self.embed, Conv2dSubsampling1)
             or isinstance(self.embed, Conv2dSubsampling2)
             or isinstance(self.embed, Conv2dSubsampling6)
             or isinstance(self.embed, Conv2dSubsampling8)
         ):
             short_status, limit_size = check_short_utt(self.embed, xs_pad.size(1))
             if short_status:
                 raise TooShortUttError(
```

### Comparing `espnet-202211/espnet2/asr/encoder/rnn_encoder.py` & `espnet-202301/espnet2/asr/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/encoder/transformer_encoder.py` & `espnet-202301/espnet2/asr/encoder/transformer_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 )
 from espnet.nets.pytorch_backend.transformer.positionwise_feed_forward import (
     PositionwiseFeedForward,
 )
 from espnet.nets.pytorch_backend.transformer.repeat import repeat
 from espnet.nets.pytorch_backend.transformer.subsampling import (
     Conv2dSubsampling,
+    Conv2dSubsampling1,
     Conv2dSubsampling2,
     Conv2dSubsampling6,
     Conv2dSubsampling8,
     TooShortUttError,
     check_short_utt,
 )
 
@@ -88,14 +89,16 @@
                 torch.nn.LayerNorm(output_size),
                 torch.nn.Dropout(dropout_rate),
                 torch.nn.ReLU(),
                 pos_enc_class(output_size, positional_dropout_rate),
             )
         elif input_layer == "conv2d":
             self.embed = Conv2dSubsampling(input_size, output_size, dropout_rate)
+        elif input_layer == "conv2d1":
+            self.embed = Conv2dSubsampling1(input_size, output_size, dropout_rate)
         elif input_layer == "conv2d2":
             self.embed = Conv2dSubsampling2(input_size, output_size, dropout_rate)
         elif input_layer == "conv2d6":
             self.embed = Conv2dSubsampling6(input_size, output_size, dropout_rate)
         elif input_layer == "conv2d8":
             self.embed = Conv2dSubsampling8(input_size, output_size, dropout_rate)
         elif input_layer == "embed":
@@ -179,14 +182,15 @@
         """
         masks = (~make_pad_mask(ilens)[:, None, :]).to(xs_pad.device)
 
         if self.embed is None:
             xs_pad = xs_pad
         elif (
             isinstance(self.embed, Conv2dSubsampling)
+            or isinstance(self.embed, Conv2dSubsampling1)
             or isinstance(self.embed, Conv2dSubsampling2)
             or isinstance(self.embed, Conv2dSubsampling6)
             or isinstance(self.embed, Conv2dSubsampling8)
         ):
             short_status, limit_size = check_short_utt(self.embed, xs_pad.size(1))
             if short_status:
                 raise TooShortUttError(
```

### Comparing `espnet-202211/espnet2/asr/encoder/transformer_encoder_multispkr.py` & `espnet-202301/espnet2/asr/encoder/transformer_encoder_multispkr.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 )
 from espnet.nets.pytorch_backend.transformer.positionwise_feed_forward import (
     PositionwiseFeedForward,
 )
 from espnet.nets.pytorch_backend.transformer.repeat import repeat
 from espnet.nets.pytorch_backend.transformer.subsampling import (
     Conv2dSubsampling,
+    Conv2dSubsampling1,
     Conv2dSubsampling2,
     Conv2dSubsampling6,
     Conv2dSubsampling8,
     TooShortUttError,
     check_short_utt,
 )
 
@@ -88,14 +89,16 @@
                 torch.nn.LayerNorm(output_size),
                 torch.nn.Dropout(dropout_rate),
                 torch.nn.ReLU(),
                 pos_enc_class(output_size, positional_dropout_rate),
             )
         elif input_layer == "conv2d":
             self.embed = Conv2dSubsampling(input_size, output_size, dropout_rate)
+        elif input_layer == "conv2d1":
+            self.embed = Conv2dSubsampling1(input_size, output_size, dropout_rate)
         elif input_layer == "conv2d2":
             self.embed = Conv2dSubsampling2(input_size, output_size, dropout_rate)
         elif input_layer == "conv2d6":
             self.embed = Conv2dSubsampling6(input_size, output_size, dropout_rate)
         elif input_layer == "conv2d8":
             self.embed = Conv2dSubsampling8(input_size, output_size, dropout_rate)
         elif input_layer == "embed":
@@ -189,14 +192,15 @@
         Returns:
             position embedded tensor and mask
         """
         masks = (~make_pad_mask(ilens)[:, None, :]).to(xs_pad.device)
 
         if (
             isinstance(self.embed, Conv2dSubsampling)
+            or isinstance(self.embed, Conv2dSubsampling1)
             or isinstance(self.embed, Conv2dSubsampling2)
             or isinstance(self.embed, Conv2dSubsampling6)
             or isinstance(self.embed, Conv2dSubsampling8)
         ):
             short_status, limit_size = check_short_utt(self.embed, xs_pad.size(1))
             if short_status:
                 raise TooShortUttError(
```

### Comparing `espnet-202211/espnet2/asr/encoder/vgg_rnn_encoder.py` & `espnet-202301/espnet2/asr/encoder/vgg_rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/encoder/wav2vec2_encoder.py` & `espnet-202301/espnet2/asr/encoder/wav2vec2_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/espnet_model.py` & `espnet-202301/espnet2/asr/espnet_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,18 @@
         token_list: Union[Tuple[str, ...], List[str]],
         frontend: Optional[AbsFrontend],
         specaug: Optional[AbsSpecAug],
         normalize: Optional[AbsNormalize],
         preencoder: Optional[AbsPreEncoder],
         encoder: AbsEncoder,
         postencoder: Optional[AbsPostEncoder],
-        decoder: AbsDecoder,
+        decoder: Optional[AbsDecoder],
         ctc: CTC,
         joint_network: Optional[torch.nn.Module],
+        aux_ctc: dict = None,
         ctc_weight: float = 0.5,
         interctc_weight: float = 0.0,
         ignore_id: int = -1,
         lsm_weight: float = 0.0,
         length_normalized_loss: bool = False,
         report_cer: bool = True,
         report_wer: bool = True,
@@ -67,27 +68,33 @@
         lang_token_id: int = -1,
     ):
         assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__()
-        self.blank_id = token_list.index(sym_blank)
+        # NOTE (Shih-Lun): else case is for OpenAI Whisper ASR model,
+        #                  which doesn't use <blank> token
+        if sym_blank in token_list:
+            self.blank_id = token_list.index(sym_blank)
+        else:
+            self.blank_id = 0
         if sym_sos in token_list:
             self.sos = token_list.index(sym_sos)
         else:
             self.sos = vocab_size - 1
         if sym_eos in token_list:
             self.eos = token_list.index(sym_eos)
         else:
             self.eos = vocab_size - 1
         self.vocab_size = vocab_size
         self.ignore_id = ignore_id
         self.ctc_weight = ctc_weight
         self.interctc_weight = interctc_weight
+        self.aux_ctc = aux_ctc
         self.token_list = token_list.copy()
 
         self.frontend = frontend
         self.specaug = specaug
         self.normalize = normalize
         self.preencoder = preencoder
         self.postencoder = postencoder
@@ -133,18 +140,20 @@
                         token_list, sym_space, sym_blank, report_cer, report_wer
                     )
         else:
             # we set self.decoder = None in the CTC mode since
             # self.decoder parameters were never used and PyTorch complained
             # and threw an Exception in the multi-GPU experiment.
             # thanks Jeff Farris for pointing out the issue.
-            if ctc_weight == 1.0:
-                self.decoder = None
-            else:
-                self.decoder = decoder
+            if ctc_weight < 1.0:
+                assert (
+                    decoder is not None
+                ), "decoder should not be None when attention is used"
+
+            self.decoder = decoder
 
             self.criterion_att = LabelSmoothingLoss(
                 size=vocab_size,
                 padding_idx=ignore_id,
                 smoothing=lsm_weight,
                 normalize_length=length_normalized_loss,
             )
@@ -157,14 +166,21 @@
         if ctc_weight == 0.0:
             self.ctc = None
         else:
             self.ctc = ctc
 
         self.extract_feats_in_collect_stats = extract_feats_in_collect_stats
 
+        self.is_encoder_whisper = "Whisper" in type(self.encoder).__name__
+
+        if self.is_encoder_whisper:
+            assert (
+                self.frontend is None
+            ), "frontend should be None when using full Whisper model"
+
         if lang_token_id != -1:
             self.lang_token_id = torch.tensor([[lang_token_id]])
         else:
             self.lang_token_id = None
 
     def forward(
         self,
@@ -222,17 +238,39 @@
 
         # Intermediate CTC (optional)
         loss_interctc = 0.0
         if self.interctc_weight != 0.0 and intermediate_outs is not None:
             for layer_idx, intermediate_out in intermediate_outs:
                 # we assume intermediate_out has the same length & padding
                 # as those of encoder_out
-                loss_ic, cer_ic = self._calc_ctc_loss(
-                    intermediate_out, encoder_out_lens, text, text_lengths
-                )
+
+                # use auxillary ctc data if specified
+                loss_ic = None
+                if self.aux_ctc is not None:
+                    idx_key = str(layer_idx)
+                    if idx_key in self.aux_ctc:
+                        aux_data_key = self.aux_ctc[idx_key]
+                        aux_data_tensor = kwargs.get(aux_data_key, None)
+                        aux_data_lengths = kwargs.get(aux_data_key + "_lengths", None)
+
+                        if aux_data_tensor is not None and aux_data_lengths is not None:
+                            loss_ic, cer_ic = self._calc_ctc_loss(
+                                intermediate_out,
+                                encoder_out_lens,
+                                aux_data_tensor,
+                                aux_data_lengths,
+                            )
+                        else:
+                            raise Exception(
+                                "Aux. CTC tasks were specified but no data was found"
+                            )
+                if loss_ic is None:
+                    loss_ic, cer_ic = self._calc_ctc_loss(
+                        intermediate_out, encoder_out_lens, text, text_lengths
+                    )
                 loss_interctc = loss_interctc + loss_ic
 
                 # Collect Intermedaite CTC stats
                 stats["loss_interctc_layer{}".format(layer_idx)] = (
                     loss_ic.detach() if loss_ic is not None else None
                 )
                 stats["cer_interctc_layer{}".format(layer_idx)] = cer_ic
@@ -361,15 +399,18 @@
                 encoder_out, encoder_out_lens
             )
 
         assert encoder_out.size(0) == speech.size(0), (
             encoder_out.size(),
             speech.size(0),
         )
-        if getattr(self.encoder, "selfattention_layer_type", None) != "lf_selfattn":
+        if (
+            getattr(self.encoder, "selfattention_layer_type", None) != "lf_selfattn"
+            and not self.is_encoder_whisper
+        ):
             assert encoder_out.size(-2) <= encoder_out_lens.max(), (
                 encoder_out.size(),
                 encoder_out_lens.max(),
             )
 
         if intermediate_outs is not None:
             return (encoder_out, intermediate_outs), encoder_out_lens
```

### Comparing `espnet-202211/espnet2/asr/frontend/default.py` & `espnet-202301/espnet2/asr/frontend/default.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/frontend/fused.py` & `espnet-202301/espnet2/asr/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/frontend/s3prl.py` & `espnet-202301/espnet2/asr/frontend/s3prl.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     def __init__(
         self,
         fs: Union[int, str] = 16000,
         frontend_conf: Optional[dict] = get_default_kwargs(Frontend),
         download_dir: str = None,
         multilayer_feature: bool = False,
+        layer: int = -1,
     ):
         try:
             import s3prl
             from s3prl.nn import Featurizer, S3PRLUpstream
         except Exception as e:
             print("Error: S3PRL is not properly installed.")
             print("Please install S3PRL: cd ${MAIN_ROOT}/tools && make s3prl.done")
@@ -42,26 +43,37 @@
         if download_dir is not None:
             s3prl.util.download.set_dir(download_dir)
 
         assert frontend_conf.get("upstream", None) in S3PRLUpstream.available_names()
         upstream = S3PRLUpstream(
             frontend_conf.get("upstream"),
             path_or_url=frontend_conf.get("path_or_url", None),
+            normalize=frontend_conf.get("normalize", False),
+            extra_conf=frontend_conf.get("extra_conf", None),
         )
         upstream.eval()
         if getattr(
             upstream, "model", None
         ) is not None and upstream.model.__class__.__name__ in [
             "Wav2Vec2Model",
             "HubertModel",
         ]:
             upstream.model.encoder.layerdrop = 0.0
-        featurizer = Featurizer(upstream)
+
+        if layer != -1:
+            layer_selections = [layer]
+            assert (
+                not multilayer_feature
+            ), "multilayer feature will be deactivated, when specific layer used"
+        else:
+            layer_selections = None
+        featurizer = Featurizer(upstream, layer_selections=layer_selections)
 
         self.multilayer_feature = multilayer_feature
+        self.layer = layer
         self.upstream, self.featurizer = upstream, featurizer
         self.pretrained_params = copy.deepcopy(self.upstream.state_dict())
         self.frontend_type = "s3prl"
         self.hop_length = self.featurizer.downsample_rate
         self.tile_factor = frontend_conf.get("tile_factor", 1)
 
     def _tile_representations(self, feature):
@@ -85,14 +97,19 @@
     def output_size(self) -> int:
         return self.featurizer.output_size
 
     def forward(
         self, input: torch.Tensor, input_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         feats, feats_lens = self.upstream(input, input_lengths)
+        if self.layer != -1:
+            layer = self.layer
+            feats, feats_lens = feats[layer], feats_lens[layer]
+            return feats, feats_lens
+
         if self.multilayer_feature:
             feats, feats_lens = self.featurizer(feats, feats_lens)
         else:
             feats, feats_lens = self.featurizer(feats[-1:], feats_lens[-1:])
 
         if self.tile_factor != 1:
             feats = self._tile_representations(feats)
```

### Comparing `espnet-202211/espnet2/asr/frontend/windowing.py` & `espnet-202301/espnet2/asr/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/layers/cgmlp.py` & `espnet-202301/espnet2/asr/layers/cgmlp.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/layers/fastformer.py` & `espnet-202301/espnet2/asr/layers/fastformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/maskctc_model.py` & `espnet-202301/espnet2/asr/maskctc_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/pit_espnet_model.py` & `espnet-202301/espnet2/asr/pit_espnet_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/postencoder/hugging_face_transformers_postencoder.py` & `espnet-202301/espnet2/asr/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/preencoder/linear.py` & `espnet-202301/espnet2/asr/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/preencoder/sinc.py` & `espnet-202301/espnet2/asr/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/specaug/specaug.py` & `espnet-202301/espnet2/asr/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/transducer/beam_search_transducer.py` & `espnet-202301/espnet2/asr/transducer/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr/transducer/error_calculator.py` & `espnet-202301/espnet2/asr/transducer/error_calculator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/activation.py` & `espnet-202301/espnet2/asr_transducer/activation.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/beam_search_transducer.py` & `espnet-202301/espnet2/asr_transducer/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/decoder/abs_decoder.py` & `espnet-202301/espnet2/asr_transducer/decoder/abs_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/decoder/rnn_decoder.py` & `espnet-202301/espnet2/asr_transducer/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/decoder/stateless_decoder.py` & `espnet-202301/espnet2/asr_transducer/decoder/stateless_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/blocks/branchformer.py` & `espnet-202301/espnet2/asr_transducer/encoder/blocks/branchformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/blocks/conformer.py` & `espnet-202301/espnet2/asr_transducer/encoder/blocks/conformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/blocks/conv1d.py` & `espnet-202301/espnet2/asr_transducer/encoder/blocks/conv1d.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/blocks/conv_input.py` & `espnet-202301/espnet2/asr_transducer/encoder/blocks/conv_input.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/building.py` & `espnet-202301/espnet2/asr_transducer/encoder/building.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/encoder.py` & `espnet-202301/espnet2/asr_transducer/encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/modules/attention.py` & `espnet-202301/espnet2/asr_transducer/encoder/modules/attention.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/modules/convolution.py` & `espnet-202301/espnet2/asr_transducer/encoder/modules/convolution.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/modules/multi_blocks.py` & `espnet-202301/espnet2/asr_transducer/encoder/modules/multi_blocks.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/modules/normalization.py` & `espnet-202301/espnet2/asr_transducer/encoder/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/modules/positional_encoding.py` & `espnet-202301/espnet2/asr_transducer/encoder/modules/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/encoder/validation.py` & `espnet-202301/espnet2/asr_transducer/encoder/validation.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/error_calculator.py` & `espnet-202301/espnet2/asr_transducer/error_calculator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/espnet_transducer_model.py` & `espnet-202301/espnet2/asr_transducer/espnet_transducer_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/joint_network.py` & `espnet-202301/espnet2/asr_transducer/joint_network.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/asr_transducer/utils.py` & `espnet-202301/espnet2/asr_transducer/utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/aggregate_stats_dirs.py` & `espnet-202301/espnet2/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/asr_align.py` & `espnet-202301/espnet2/bin/asr_align.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/asr_inference.py` & `espnet-202301/espnet2/bin/asr_inference.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,32 +7,35 @@
 from typing import Any, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import torch
 import torch.quantization
 from typeguard import check_argument_types, check_return_type
 
+from espnet2.asr.decoder.s4_decoder import S4Decoder
 from espnet2.asr.transducer.beam_search_transducer import BeamSearchTransducer
 from espnet2.asr.transducer.beam_search_transducer import (
     ExtendedHypothesis as ExtTransHypothesis,
 )
 from espnet2.asr.transducer.beam_search_transducer import Hypothesis as TransHypothesis
 from espnet2.fileio.datadir_writer import DatadirWriter
 from espnet2.tasks.asr import ASRTask
 from espnet2.tasks.enh_s2t import EnhS2TTask
 from espnet2.tasks.lm import LMTask
 from espnet2.text.build_tokenizer import build_tokenizer
 from espnet2.text.token_id_converter import TokenIDConverter
+from espnet2.text.whisper_token_id_converter import OpenAIWhisperTokenIDConverter
 from espnet2.torch_utils.device_funcs import to_device
 from espnet2.torch_utils.set_all_random_seed import set_all_random_seed
 from espnet2.utils import config_argparse
 from espnet2.utils.types import str2bool, str2triple_str, str_or_none
 from espnet.nets.batch_beam_search import BatchBeamSearch
 from espnet.nets.batch_beam_search_online_sim import BatchBeamSearchOnlineSim
 from espnet.nets.beam_search import BeamSearch, Hypothesis
+from espnet.nets.beam_search_timesync import BeamSearchTimeSync
 from espnet.nets.pytorch_backend.transformer.subsampling import TooShortUttError
 from espnet.nets.scorer_interface import BatchScorerInterface
 from espnet.nets.scorers.ctc import CTCPrefixScorer
 from espnet.nets.scorers.length_bonus import LengthBonus
 from espnet.utils.cli_utils import get_commandline_args
 
 try:
@@ -82,14 +85,15 @@
         enh_s2t_task: bool = False,
         quantize_asr_model: bool = False,
         quantize_lm: bool = False,
         quantize_modules: List[str] = ["Linear"],
         quantize_dtype: str = "qint8",
         hugging_face_decoder: bool = False,
         hugging_face_decoder_max_length: int = 256,
+        time_sync: bool = False,
         multi_asr: bool = False,
     ):
         assert check_argument_types()
 
         task = ASRTask if not enh_s2t_task else EnhS2TTask
 
         if quantize_asr_model or quantize_lm:
@@ -226,47 +230,68 @@
             weights = dict(
                 decoder=1.0 - ctc_weight,
                 ctc=ctc_weight,
                 lm=lm_weight,
                 ngram=ngram_weight,
                 length_bonus=penalty,
             )
-            beam_search = BeamSearch(
-                beam_size=beam_size,
-                weights=weights,
-                scorers=scorers,
-                sos=asr_model.sos,
-                eos=asr_model.eos,
-                vocab_size=len(token_list),
-                token_list=token_list,
-                pre_beam_score_key=None if ctc_weight == 1.0 else "full",
-            )
 
-            # TODO(karita): make all scorers batchfied
-            if batch_size == 1:
-                non_batch = [
-                    k
-                    for k, v in beam_search.full_scorers.items()
-                    if not isinstance(v, BatchScorerInterface)
-                ]
-                if len(non_batch) == 0:
-                    if streaming:
-                        beam_search.__class__ = BatchBeamSearchOnlineSim
-                        beam_search.set_streaming_config(asr_train_config)
-                        logging.info(
-                            "BatchBeamSearchOnlineSim implementation is selected."
-                        )
-                    else:
-                        beam_search.__class__ = BatchBeamSearch
-                        logging.info("BatchBeamSearch implementation is selected.")
-                else:
-                    logging.warning(
-                        f"As non-batch scorers {non_batch} are found, "
-                        f"fall back to non-batch implementation."
+            if time_sync:
+                if not hasattr(asr_model, "ctc"):
+                    raise NotImplementedError(
+                        "BeamSearchTimeSync without CTC is not supported."
                     )
+                if batch_size != 1:
+                    raise NotImplementedError(
+                        "BeamSearchTimeSync with batching is not yet supported."
+                    )
+                logging.info("BeamSearchTimeSync implementation is selected.")
+
+                scorers["ctc"] = asr_model.ctc
+                beam_search = BeamSearchTimeSync(
+                    beam_size=beam_size,
+                    weights=weights,
+                    scorers=scorers,
+                    sos=asr_model.sos,
+                    token_list=token_list,
+                )
+            else:
+                beam_search = BeamSearch(
+                    beam_size=beam_size,
+                    weights=weights,
+                    scorers=scorers,
+                    sos=asr_model.sos,
+                    eos=asr_model.eos,
+                    vocab_size=len(token_list),
+                    token_list=token_list,
+                    pre_beam_score_key=None if ctc_weight == 1.0 else "full",
+                )
+
+                # TODO(karita): make all scorers batchfied
+                if batch_size == 1:
+                    non_batch = [
+                        k
+                        for k, v in beam_search.full_scorers.items()
+                        if not isinstance(v, BatchScorerInterface)
+                    ]
+                    if len(non_batch) == 0:
+                        if streaming:
+                            beam_search.__class__ = BatchBeamSearchOnlineSim
+                            beam_search.set_streaming_config(asr_train_config)
+                            logging.info(
+                                "BatchBeamSearchOnlineSim implementation is selected."
+                            )
+                        else:
+                            beam_search.__class__ = BatchBeamSearch
+                            logging.info("BatchBeamSearch implementation is selected.")
+                    else:
+                        logging.warning(
+                            f"As non-batch scorers {non_batch} are found, "
+                            f"fall back to non-batch implementation."
+                        )
 
             beam_search.to(device=device, dtype=getattr(torch, dtype)).eval()
             for scorer in scorers.values():
                 if isinstance(scorer, torch.nn.Module):
                     scorer.to(device=device, dtype=getattr(torch, dtype)).eval()
             logging.info(f"Beam_search: {beam_search}")
             logging.info(f"Decoding device={device}, dtype={dtype}")
@@ -275,22 +300,33 @@
         if token_type is None:
             token_type = asr_train_args.token_type
         if bpemodel is None:
             bpemodel = asr_train_args.bpemodel
 
         if token_type is None:
             tokenizer = None
-        elif token_type == "bpe" or token_type == "hugging_face":
+        elif (
+            token_type == "bpe"
+            or token_type == "hugging_face"
+            or "whisper" in token_type
+        ):
             if bpemodel is not None:
                 tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
             else:
                 tokenizer = None
         else:
             tokenizer = build_tokenizer(token_type=token_type)
-        converter = TokenIDConverter(token_list=token_list)
+
+        if bpemodel not in ["whisper_en", "whisper_multilingual"]:
+            converter = TokenIDConverter(token_list=token_list)
+        else:
+            converter = OpenAIWhisperTokenIDConverter(model_type=bpemodel)
+            beam_search.set_hyp_primer(
+                list(converter.tokenizer.sot_sequence_including_notimestamps)
+            )
         logging.info(f"Text tokenizer: {tokenizer}")
 
         self.asr_model = asr_model
         self.asr_train_args = asr_train_args
         self.converter = converter
         self.tokenizer = tokenizer
         self.beam_search = beam_search
@@ -408,14 +444,20 @@
             nbest_hyps = [Hypothesis(yseq=yseq[0])]
             logging.info(
                 "best hypo: "
                 + "".join(self.converter.ids2tokens(nbest_hyps[0].yseq[1:]))
                 + "\n"
             )
         else:
+            if hasattr(self.beam_search.nn_dict, "decoder"):
+                if isinstance(self.beam_search.nn_dict.decoder, S4Decoder):
+                    # Setup: required for S4 autoregressive generation
+                    for module in self.beam_search.nn_dict.decoder.modules():
+                        if hasattr(module, "setup_step"):
+                            module.setup_step()
             nbest_hyps = self.beam_search(
                 x=enc, maxlenratio=self.maxlenratio, minlenratio=self.minlenratio
             )
 
         nbest_hyps = nbest_hyps[: self.nbest]
 
         results = []
@@ -508,14 +550,15 @@
     enh_s2t_task: bool,
     quantize_asr_model: bool,
     quantize_lm: bool,
     quantize_modules: List[str],
     quantize_dtype: str,
     hugging_face_decoder: bool,
     hugging_face_decoder_max_length: int,
+    time_sync: bool,
     multi_asr: bool,
 ):
     assert check_argument_types()
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
@@ -560,14 +603,15 @@
         multi_asr=multi_asr,
         quantize_asr_model=quantize_asr_model,
         quantize_lm=quantize_lm,
         quantize_modules=quantize_modules,
         quantize_dtype=quantize_dtype,
         hugging_face_decoder=hugging_face_decoder,
         hugging_face_decoder_max_length=hugging_face_decoder_max_length,
+        time_sync=time_sync,
     )
     speech2text = Speech2Text.from_pretrained(
         model_tag=model_tag,
         **speech2text_kwargs,
     )
 
     # 3. Build data-iterator
@@ -833,14 +877,20 @@
     group.add_argument(
         "--bpemodel",
         type=str_or_none,
         default=None,
         help="The model path of sentencepiece. "
         "If not given, refers from the training args",
     )
+    group.add_argument(
+        "--time_sync",
+        type=str2bool,
+        default=False,
+        help="Time synchronous beam search.",
+    )
 
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
```

### Comparing `espnet-202211/espnet2/bin/asr_inference_k2.py` & `espnet-202301/espnet2/bin/asr_inference_k2.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/asr_inference_maskctc.py` & `espnet-202301/espnet2/bin/asr_inference_maskctc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/asr_inference_streaming.py` & `espnet-202301/espnet2/bin/asr_inference_streaming.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/asr_transducer_inference.py` & `espnet-202301/espnet2/bin/asr_transducer_inference.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/asr_transducer_train.py` & `espnet-202301/espnet2/bin/asr_transducer_train.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/diar_inference.py` & `espnet-202301/espnet2/bin/diar_inference.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/enh_inference.py` & `espnet-202301/espnet2/bin/enh_inference.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/enh_scoring.py` & `espnet-202301/espnet2/bin/enh_scoring.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/hugging_face_export_vocabulary.py` & `espnet-202301/espnet2/bin/hugging_face_export_vocabulary.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/launch.py` & `espnet-202301/espnet2/bin/launch.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/lm_calc_perplexity.py` & `espnet-202301/espnet2/bin/lm_calc_perplexity.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/mt_inference.py` & `espnet-202301/espnet2/bin/mt_inference.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/pack.py` & `espnet-202301/espnet2/bin/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,20 @@
 
 class EnhS2TPackedContents(PackedContents):
     # These names must be consistent with the argument of inference functions
     files = ["enh_s2t_model_file", "lm_file"]
     yaml_files = ["enh_s2t_train_config", "lm_train_config"]
 
 
+class SSLPackedContents(PackedContents):
+    # These names must be consistent with the argument of inference functions
+    files = ["model_file"]
+    yaml_files = ["train_config"]
+
+
 def add_arguments(parser: argparse.ArgumentParser, contents: Type[PackedContents]):
     parser.add_argument("--outpath", type=str, required=True)
     for key in contents.yaml_files:
         parser.add_argument(f"--{key}", type=str, default=None)
     for key in contents.files:
         parser.add_argument(f"--{key}", type=str, default=None)
     parser.add_argument("--option", type=str, action="append", default=[])
@@ -65,14 +71,15 @@
         ("asr", ASRPackedContents),
         ("st", STPackedContents),
         ("tts", TTSPackedContents),
         ("enh", EnhPackedContents),
         ("diar", DiarPackedContents),
         ("svs", SVSPackedContents),
         ("enh_s2t", EnhS2TPackedContents),
+        ("ssl", SSLPackedContents),
     ]:
         parser_asr = subparsers.add_parser(
             name,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
         add_arguments(parser_asr, contents)
         parser_asr.set_defaults(contents=contents)
```

### Comparing `espnet-202211/espnet2/bin/slu_inference.py` & `espnet-202301/espnet2/bin/slu_inference.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/split_scps.py` & `espnet-202301/espnet2/bin/split_scps.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/st_inference.py` & `espnet-202301/espnet2/bin/st_inference.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/st_inference_streaming.py` & `espnet-202301/espnet2/bin/st_inference_streaming.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/bin/svs_inference.py` & `espnet-202301/espnet2/bin/svs_inference.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import numpy as np
 import soundfile as sf
 import torch
 from typeguard import check_argument_types
 
 from espnet2.fileio.npy_scp import NpyScpWriter
+from espnet2.gan_svs.vits import VITS
 from espnet2.tasks.svs import SVSTask
 from espnet2.torch_utils.device_funcs import to_device
 from espnet2.torch_utils.set_all_random_seed import set_all_random_seed
 from espnet2.utils import config_argparse
 from espnet2.utils.types import str2bool, str2triple_str, str_or_none
 from espnet.utils.cli_utils import get_commandline_args
 
@@ -35,54 +36,68 @@
     """
 
     def __init__(
         self,
         train_config: Optional[Union[Path, str]],
         model_file: Optional[Union[Path, str]] = None,
         use_teacher_forcing: bool = False,
+        noise_scale: float = 0.667,
+        noise_scale_dur: float = 0.8,
         vocoder_config: Union[Path, str] = None,
         vocoder_checkpoint: Union[Path, str] = None,
         dtype: str = "float32",
         device: str = "cpu",
         seed: int = 777,
+        always_fix_seed: bool = False,
+        prefer_normalized_feats: bool = False,
     ):
         assert check_argument_types()
 
+        # setup model
         model, train_args = SVSTask.build_model_from_file(
             train_config, model_file, device
         )
         model.to(dtype=getattr(torch, dtype)).eval()
         self.device = device
         self.dtype = dtype
         self.train_args = train_args
         self.model = model
         self.svs = model.svs
         self.normalize = model.normalize
         self.feats_extract = model.feats_extract
         # self.duration_calculator = DurationCalculator() # TODO(Yuning)
         self.preprocess_fn = SVSTask.build_preprocess_fn(train_args, False)
         self.use_teacher_forcing = use_teacher_forcing
-
+        self.seed = seed
+        self.always_fix_seed = always_fix_seed
         self.vocoder = None
+        self.prefer_normalized_feats = prefer_normalized_feats
         if vocoder_checkpoint is not None:
             vocoder = SVSTask.build_vocoder_from_file(
                 vocoder_config, vocoder_checkpoint, model, device
             )
             if isinstance(vocoder, torch.nn.Module):
                 vocoder.to(dtype=getattr(torch, dtype)).eval()
             self.vocoder = vocoder
 
         logging.info(f"Extractor:\n{self.feats_extract}")
         logging.info(f"Normalizer:\n{self.normalize}")
         logging.info(f"SVS:\n{self.svs}")
+        if self.vocoder is not None:
+            logging.info(f"Vocoder:\n{self.vocoder}")
 
-        decode_config = {}
-        decode_config.update({"use_teacher_forcing": use_teacher_forcing})
-
-        self.decode_config = decode_config
+        # setup decoding config
+        decode_conf = {}
+        decode_conf.update({"use_teacher_forcing": use_teacher_forcing})
+        if isinstance(self.svs, VITS):
+            decode_conf.update(
+                noise_scale=noise_scale,
+                noise_scale_dur=noise_scale_dur,
+            )
+        self.decode_conf = decode_conf
 
     @torch.no_grad()
     def __call__(
         self,
         text: Union[torch.Tensor, np.ndarray],
         singing: Union[torch.Tensor, np.ndarray] = None,
         label: Union[torch.Tensor, np.ndarray] = None,
@@ -126,14 +141,15 @@
             batch.update(midi=midi)
         if beat_phn is not None:
             batch.update(beat_phn=beat_phn)
         if beat_ruled_phn is not None:
             batch.update(beat_ruled_phn=beat_ruled_phn)
         if beat_syb is not None:
             batch.update(beat_syb=beat_syb)
+
         if label_lab is not None:
             batch.update(label_lab=label_lab)
         if label_score is not None:
             batch.update(label_score=label_score)
         if midi_lab is not None:
             batch.update(midi_lab=midi_lab)
         if midi_score is not None:
@@ -158,39 +174,39 @@
             batch.update(spembs=spembs)
         if sids is not None:
             batch.update(sids=sids)
         if lids is not None:
             batch.update(lids=lids)
         batch = to_device(batch, self.device)
 
-        cfg = self.decode_config
+        cfg = self.decode_conf
         if decode_conf is not None:
             cfg = self.decode_conf.copy()
             cfg.update(decode_conf)
+        output_dict = self.model.inference(**batch, **cfg)
 
-        batch = to_device(batch, self.device)
-        outs, outs_denorm, probs, att_ws = self.model.inference(**batch, **cfg)
-
-        if att_ws is not None:
-            duration, focus_rate = self.duration_calculator(att_ws)
+        if output_dict.get("att_ws") is not None:
+            output_dict.update(duration=None, focus_rate=None)
+            # duration, focus_rate = self.duration_calculator(att_ws)
         else:
-            duration, focus_rate = None, None
+            output_dict.update(duration=None, focus_rate=None)
 
-        assert outs.shape[0] == 1
-        outs = outs.squeeze(0)
-        outs_denorm = outs_denorm.squeeze(0)
+        # apply vocoder (mel-to-wav)
         if self.vocoder is not None:
-            if self.vocoder.normalize_before:
-                wav = self.vocoder(outs_denorm)
+            if (
+                self.prefer_normalized_feats
+                or output_dict.get("feat_gen_denorm") is None
+            ):
+                input_feat = output_dict["feat_gen"]
             else:
-                wav = self.vocoder(outs)
-        else:
-            wav = None
+                input_feat = output_dict["feat_gen_denorm"]
+            wav = self.vocoder(input_feat)
+            output_dict.update(wav=wav)
 
-        return wav, outs, outs_denorm, probs, att_ws, duration, focus_rate
+        return output_dict
 
     @property
     def fs(self) -> Optional[int]:
         """Return sampling rate."""
         if hasattr(self.vocoder, "fs"):
             return self.vocoder.fs
         elif hasattr(self.svs, "fs"):
@@ -228,14 +244,16 @@
     num_workers: int,
     log_level: Union[int, str],
     data_path_and_name_and_type: Sequence[Tuple[str, str, str]],
     key_file: Optional[str],
     train_config: Optional[str],
     model_file: Optional[str],
     use_teacher_forcing: bool,
+    noise_scale: float,
+    noise_scale_dur: float,
     allow_variable_data_keys: bool,
     vocoder_config: Optional[str] = None,
     vocoder_checkpoint: Optional[str] = None,
 ):
     """Perform SVS model decoding."""
     assert check_argument_types()
     if batch_size > 1:
@@ -256,14 +274,16 @@
     set_all_random_seed(seed)
 
     # 2. Build model
     singingGenerate = SingingGenerate(
         train_config=train_config,
         model_file=model_file,
         use_teacher_forcing=use_teacher_forcing,
+        noise_scale=noise_scale,
+        noise_scale_dur=noise_scale_dur,
         vocoder_config=vocoder_config,
         vocoder_checkpoint=vocoder_checkpoint,
         dtype=dtype,
         device=device,
     )
 
     # 3. Build data-iterator
@@ -319,108 +339,129 @@
             # because inference() requires 1-seq, not mini-batch.
             batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
 
             logging.info(f"batch: {batch}")
             logging.info(f"keys: {keys}")
 
             start_time = time.perf_counter()
-            (
-                wav,
-                outs,
-                outs_denorm,
-                probs,
-                att_ws,
-                duration,
-                focus_rate,
-            ) = singingGenerate(**batch)
+            output_dict = singingGenerate(**batch)
 
             key = keys[0]
             insize = next(iter(batch.values())).size(0) + 1
-            logging.info(
-                "inference speed = {:.1f} frames / sec.".format(
-                    int(outs.size(0)) / (time.perf_counter() - start_time)
+            if output_dict.get("feat_gen") is not None:
+                # standard text2mel model case
+                feat_gen = output_dict["feat_gen"]
+                logging.info(
+                    "inference speed = {:.1f} frames / sec.".format(
+                        int(feat_gen.size(0)) / (time.perf_counter() - start_time)
+                    )
                 )
-            )
-            logging.info(f"{key} (size:{insize}->{outs.size(0)})")
-
-            norm_writer[key] = outs.cpu().numpy()
-            shape_writer.write(f"{key} " + ",".join(map(str, outs.shape)) + "\n")
+                logging.info(f"{key} (size:{insize}->{feat_gen.size(0)})")
 
-            denorm_writer[key] = outs_denorm.cpu().numpy()
+                norm_writer[key] = output_dict["feat_gen"].cpu().numpy()
+                shape_writer.write(
+                    f"{key} " + ",".join(map(str, output_dict["feat_gen"].shape)) + "\n"
+                )
+                if output_dict.get("feat_gen_denorm") is not None:
+                    denorm_writer[key] = output_dict["feat_gen_denorm"].cpu().numpy()
+            else:
+                # end-to-end text2wav model case
+                wav = output_dict["wav"]
+                logging.info(
+                    "inference speed = {:.1f} points / sec.".format(
+                        int(wav.size(0)) / (time.perf_counter() - start_time)
+                    )
+                )
+                logging.info(f"{key} (size:{insize}->{wav.size(0)})")
 
-            if duration is not None:
+            if output_dict.get("duration") is not None:
                 # Save duration and fucus rates
                 duration_writer.write(
-                    f"{key} " + " ".join(map(str, duration.cpu().numpy())) + "\n"
+                    f"{key} "
+                    + " ".join(map(str, output_dict["duration"].long().cpu().numpy()))
+                    + "\n"
+                )
+
+            if output_dict.get("focus_rate") is not None:
+                focus_rate_writer.write(
+                    f"{key} {float(output_dict['focus_rate']):.5f}\n"
                 )
-                focus_rate_writer.write(f"{key} {float(focus_rate):.5f}\n")
 
+            if output_dict.get("att_w") is not None:
                 # Plot attention weight
-                att_ws = att_ws.cpu().numpy()
+                att_w = output_dict["att_w"].cpu().numpy()
 
-                if att_ws.ndim == 2:
-                    att_ws = att_ws[None][None]
-                elif att_ws.ndim != 4:
-                    raise RuntimeError(f"Must be 2 or 4 dimension: {att_ws.ndim}")
+                if att_w.ndim == 2:
+                    att_w = att_w[None][None]
+                elif att_w.ndim != 4:
+                    raise RuntimeError(f"Must be 2 or 4 dimension: {att_w.ndim}")
 
-                w, h = plt.figaspect(att_ws.shape[0] / att_ws.shape[1])
+                w, h = plt.figaspect(att_w.shape[0] / att_w.shape[1])
                 fig = plt.Figure(
                     figsize=(
-                        w * 1.3 * min(att_ws.shape[0], 2.5),
-                        h * 1.3 * min(att_ws.shape[1], 2.5),
+                        w * 1.3 * min(att_w.shape[0], 2.5),
+                        h * 1.3 * min(att_w.shape[1], 2.5),
                     )
                 )
                 fig.suptitle(f"{key}")
-                axes = fig.subplots(att_ws.shape[0], att_ws.shape[1])
-                if len(att_ws) == 1:
+                axes = fig.subplots(att_w.shape[0], att_w.shape[1])
+                if len(att_w) == 1:
                     axes = [[axes]]
-                for ax, att_w in zip(axes, att_ws):
+                for ax, att_w in zip(axes, att_w):
                     for ax_, att_w_ in zip(ax, att_w):
                         ax_.imshow(att_w_.astype(np.float32), aspect="auto")
                         ax_.set_xlabel("Input")
                         ax_.set_ylabel("Output")
                         ax_.xaxis.set_major_locator(MaxNLocator(integer=True))
                         ax_.yaxis.set_major_locator(MaxNLocator(integer=True))
 
                 fig.set_tight_layout({"rect": [0, 0.03, 1, 0.95]})
                 fig.savefig(output_dir / f"att_ws/{key}.png")
                 fig.clf()
 
-            if probs is not None:
+            if output_dict.get("prob") is not None:
                 # Plot stop token prediction
-                probs = probs.cpu().numpy()
+                prob = output_dict["prob"].cpu().numpy()
 
                 fig = plt.Figure()
                 ax = fig.add_subplot(1, 1, 1)
-                ax.plot(probs)
+                ax.plot(prob)
                 ax.set_title(f"{key}")
                 ax.set_xlabel("Output")
                 ax.set_ylabel("Stop probability")
                 ax.set_ylim(0, 1)
                 ax.grid(which="both")
 
                 fig.set_tight_layout(True)
                 fig.savefig(output_dir / f"probs/{key}.png")
                 fig.clf()
             # TODO(kamo): Write scp
-            if wav is not None:
+            if output_dict.get("wav") is not None:
                 sf.write(
                     f"{output_dir}/wav/{key}.wav",
-                    wav.numpy(),
+                    output_dict["wav"].cpu().numpy(),
                     singingGenerate.fs,
                     "PCM_16",
                 )
 
-    # remove duration related files if attention is not provided
-    if att_ws is None:
+    # remove files if those are not included in output dict
+    if output_dict.get("feat_gen") is None:
+        shutil.rmtree(output_dir / "norm")
+    if output_dict.get("feat_gen_denorm") is None:
+        shutil.rmtree(output_dir / "denorm")
+    if output_dict.get("att_w") is None:
         shutil.rmtree(output_dir / "att_ws")
+    if output_dict.get("duration") is None:
         shutil.rmtree(output_dir / "durations")
+    if output_dict.get("focus_rate") is None:
         shutil.rmtree(output_dir / "focus_rates")
-    if probs is None:
+    if output_dict.get("prob") is None:
         shutil.rmtree(output_dir / "probs")
+    if output_dict.get("wav") is None:
+        shutil.rmtree(output_dir / "wav")
 
 
 def get_parser():
     """Get argument parser."""
 
     parser = config_argparse.ArgumentParser(
         description="SVS Decode",
@@ -506,14 +547,26 @@
     group = parser.add_argument_group("Decoding related")
     group.add_argument(
         "--use_teacher_forcing",
         type=str2bool,
         default=False,
         help="Whether to use teacher forcing",
     )
+    parser.add_argument(
+        "--noise_scale",
+        type=float,
+        default=0.667,
+        help="Noise scale parameter for the flow in vits",
+    )
+    parser.add_argument(
+        "--noise_scale_dur",
+        type=float,
+        default=0.8,
+        help="Noise scale parameter for the stochastic duration predictor in vits",
+    )
 
     group = parser.add_argument_group("Vocoder related")
     group.add_argument(
         "--vocoder_checkpoint",
         default="None",
         type=str_or_none,
         help="checkpoint file to be loaded.",
```

### Comparing `espnet-202211/espnet2/bin/tokenize_text.py` & `espnet-202301/espnet2/bin/tokenize_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 from espnet2.text.cleaner import TextCleaner
 from espnet2.text.phoneme_tokenizer import g2p_choices
 from espnet2.utils.types import str2bool, str_or_none
 from espnet.utils.cli_utils import get_commandline_args
 
 
 def field2slice(field: Optional[str]) -> slice:
-    """Convert field string to slice
+    """Convert field string to slice.
 
     Note that field string accepts 1-based integer.
-
     Examples:
         >>> field2slice("1-")
         slice(0, None, None)
         >>> field2slice("1-3")
         slice(0, 3, None)
         >>> field2slice("-3")
         slice(None, 3, None)
@@ -216,15 +215,23 @@
         type=str2bool,
         default=False,
         help="Remove non-language-symbols from tokens",
     )
     parser.add_argument(
         "--cleaner",
         type=str_or_none,
-        choices=[None, "tacotron", "jaconv", "vietnamese", "korean_cleaner"],
+        choices=[
+            None,
+            "tacotron",
+            "jaconv",
+            "vietnamese",
+            "korean_cleaner",
+            "whisper_en",
+            "whisper_basic",
+        ],
         default=None,
         help="Apply text cleaning",
     )
     parser.add_argument(
         "--g2p",
         type=str_or_none,
         choices=g2p_choices,
```

### Comparing `espnet-202211/espnet2/bin/tts_inference.py` & `espnet-202301/espnet2/bin/tts_inference.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/diar/abs_diar.py` & `espnet-202301/espnet2/diar/abs_diar.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/diar/attractor/rnn_attractor.py` & `espnet-202301/espnet2/diar/attractor/rnn_attractor.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/diar/decoder/linear_decoder.py` & `espnet-202301/espnet2/diar/decoder/linear_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/diar/espnet_model.py` & `espnet-202301/espnet2/diar/espnet_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/diar/label_processor.py` & `espnet-202301/espnet2/diar/label_processor.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/diar/layers/multi_mask.py` & `espnet-202301/espnet2/diar/layers/multi_mask.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/diar/layers/tcn_nomask.py` & `espnet-202301/espnet2/diar/layers/tcn_nomask.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/diar/separator/tcn_separator_nomask.py` & `espnet-202301/espnet2/diar/separator/tcn_separator_nomask.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/abs_enh.py` & `espnet-202301/espnet2/enh/abs_enh.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/decoder/conv_decoder.py` & `espnet-202301/espnet2/enh/decoder/conv_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/decoder/stft_decoder.py` & `espnet-202301/espnet2/enh/decoder/stft_decoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/encoder/conv_encoder.py` & `espnet-202301/espnet2/enh/encoder/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/encoder/stft_encoder.py` & `espnet-202301/espnet2/enh/encoder/stft_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/espnet_enh_s2t_model.py` & `espnet-202301/espnet2/enh/espnet_enh_s2t_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/espnet_model.py` & `espnet-202301/espnet2/enh/espnet_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/beamformer.py` & `espnet-202301/espnet2/enh/layers/beamformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/beamformer_th.py` & `espnet-202301/espnet2/enh/layers/beamformer_th.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/complex_utils.py` & `espnet-202301/espnet2/enh/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/complexnn.py` & `espnet-202301/espnet2/enh/layers/complexnn.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/conv_utils.py` & `espnet-202301/espnet2/enh/layers/conv_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/dc_crn.py` & `espnet-202301/espnet2/enh/layers/dc_crn.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/dnn_beamformer.py` & `espnet-202301/espnet2/enh/layers/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/dnn_wpe.py` & `espnet-202301/espnet2/enh/layers/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/dpmulcat.py` & `espnet-202301/espnet2/enh/layers/dpmulcat.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/dprnn.py` & `espnet-202301/espnet2/enh/layers/dprnn.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/dptnet.py` & `espnet-202301/espnet2/enh/layers/dptnet.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/fasnet.py` & `espnet-202301/espnet2/enh/layers/fasnet.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/ifasnet.py` & `espnet-202301/espnet2/enh/layers/ifasnet.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/mask_estimator.py` & `espnet-202301/espnet2/enh/layers/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/skim.py` & `espnet-202301/espnet2/enh/layers/skim.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/tcndenseunet.py` & `espnet-202301/espnet2/enh/layers/tcndenseunet.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/layers/wpe.py` & `espnet-202301/espnet2/enh/layers/wpe.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/loss/criterions/abs_loss.py` & `espnet-202301/espnet2/enh/loss/criterions/abs_loss.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/loss/criterions/tf_domain.py` & `espnet-202301/espnet2/enh/loss/criterions/tf_domain.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/loss/criterions/time_domain.py` & `espnet-202301/espnet2/enh/loss/criterions/time_domain.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/loss/wrappers/abs_wrapper.py` & `espnet-202301/espnet2/enh/loss/wrappers/abs_wrapper.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/loss/wrappers/dpcl_solver.py` & `espnet-202301/espnet2/enh/loss/wrappers/dpcl_solver.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/loss/wrappers/fixed_order.py` & `espnet-202301/espnet2/enh/loss/wrappers/fixed_order.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/loss/wrappers/mixit_solver.py` & `espnet-202301/espnet2/enh/loss/wrappers/mixit_solver.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/loss/wrappers/multilayer_pit_solver.py` & `espnet-202301/espnet2/enh/loss/wrappers/multilayer_pit_solver.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/loss/wrappers/pit_solver.py` & `espnet-202301/espnet2/enh/loss/wrappers/pit_solver.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/abs_separator.py` & `espnet-202301/espnet2/enh/separator/abs_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/asteroid_models.py` & `espnet-202301/espnet2/enh/separator/asteroid_models.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/conformer_separator.py` & `espnet-202301/espnet2/enh/separator/conformer_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/dan_separator.py` & `espnet-202301/espnet2/enh/separator/dan_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/dc_crn_separator.py` & `espnet-202301/espnet2/enh/separator/dc_crn_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/dccrn_separator.py` & `espnet-202301/espnet2/enh/separator/dccrn_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/dpcl_e2e_separator.py` & `espnet-202301/espnet2/enh/separator/dpcl_e2e_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/dpcl_separator.py` & `espnet-202301/espnet2/enh/separator/dpcl_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/dprnn_separator.py` & `espnet-202301/espnet2/enh/separator/dprnn_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/dptnet_separator.py` & `espnet-202301/espnet2/enh/separator/dptnet_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/fasnet_separator.py` & `espnet-202301/espnet2/enh/separator/fasnet_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/ineube_separator.py` & `espnet-202301/espnet2/enh/separator/ineube_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/neural_beamformer.py` & `espnet-202301/espnet2/enh/separator/neural_beamformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/rnn_separator.py` & `espnet-202301/espnet2/enh/separator/rnn_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/skim_separator.py` & `espnet-202301/espnet2/enh/separator/skim_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/svoice_separator.py` & `espnet-202301/espnet2/enh/separator/svoice_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/tcn_separator.py` & `espnet-202301/espnet2/enh/separator/tcn_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/enh/separator/transformer_separator.py` & `espnet-202301/espnet2/enh/separator/transformer_separator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/fileio/datadir_writer.py` & `espnet-202301/espnet2/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/fileio/npy_scp.py` & `espnet-202301/espnet2/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/fileio/rand_gen_dataset.py` & `espnet-202301/espnet2/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/fileio/rttm.py` & `espnet-202301/espnet2/fileio/rttm.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/fileio/score_scp.py` & `espnet-202301/espnet2/fileio/score_scp.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/fileio/sound_scp.py` & `espnet-202301/espnet2/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/abs_gan_tts.py` & `espnet-202301/espnet2/gan_tts/abs_gan_tts.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/espnet_model.py` & `espnet-202301/espnet2/gan_tts/espnet_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/hifigan/hifigan.py` & `espnet-202301/espnet2/gan_tts/hifigan/hifigan.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/hifigan/loss.py` & `espnet-202301/espnet2/gan_tts/hifigan/loss.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/hifigan/residual_block.py` & `espnet-202301/espnet2/gan_tts/hifigan/residual_block.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/jets/alignments.py` & `espnet-202301/espnet2/gan_tts/jets/alignments.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/jets/generator.py` & `espnet-202301/espnet2/gan_tts/jets/generator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/jets/jets.py` & `espnet-202301/espnet2/gan_tts/jets/jets.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/jets/length_regulator.py` & `espnet-202301/espnet2/gan_tts/jets/length_regulator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/jets/loss.py` & `espnet-202301/espnet2/gan_tts/jets/loss.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/joint/joint_text2wav.py` & `espnet-202301/espnet2/gan_tts/joint/joint_text2wav.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/melgan/melgan.py` & `espnet-202301/espnet2/gan_tts/melgan/melgan.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/melgan/pqmf.py` & `espnet-202301/espnet2/gan_tts/melgan/pqmf.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/melgan/residual_stack.py` & `espnet-202301/espnet2/gan_tts/melgan/residual_stack.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/parallel_wavegan/parallel_wavegan.py` & `espnet-202301/espnet2/gan_tts/parallel_wavegan/parallel_wavegan.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/parallel_wavegan/upsample.py` & `espnet-202301/espnet2/gan_tts/parallel_wavegan/upsample.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/style_melgan/style_melgan.py` & `espnet-202301/espnet2/gan_tts/style_melgan/style_melgan.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/style_melgan/tade_res_block.py` & `espnet-202301/espnet2/gan_tts/style_melgan/tade_res_block.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/utils/get_random_segments.py` & `espnet-202301/espnet2/gan_tts/utils/get_random_segments.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/vits/duration_predictor.py` & `espnet-202301/espnet2/gan_tts/vits/duration_predictor.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/vits/flow.py` & `espnet-202301/espnet2/gan_tts/vits/flow.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/vits/generator.py` & `espnet-202301/espnet2/gan_tts/vits/generator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/vits/loss.py` & `espnet-202301/espnet2/gan_tts/vits/loss.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/vits/monotonic_align/__init__.py` & `espnet-202301/espnet2/gan_tts/vits/monotonic_align/__init__.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/vits/monotonic_align/setup.py` & `espnet-202301/espnet2/gan_tts/vits/monotonic_align/setup.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/vits/posterior_encoder.py` & `espnet-202301/espnet2/gan_tts/vits/posterior_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/vits/residual_coupling.py` & `espnet-202301/espnet2/gan_tts/vits/residual_coupling.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/vits/text_encoder.py` & `espnet-202301/espnet2/gan_tts/vits/text_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/vits/transform.py` & `espnet-202301/espnet2/gan_tts/vits/transform.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/vits/vits.py` & `espnet-202301/espnet2/gan_tts/vits/vits.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/wavenet/residual_block.py` & `espnet-202301/espnet2/gan_tts/wavenet/residual_block.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/gan_tts/wavenet/wavenet.py` & `espnet-202301/espnet2/gan_tts/wavenet/wavenet.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/hubert/espnet_model.py` & `espnet-202301/espnet2/mt/espnet_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,253 +1,281 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-# Thanks to Abdelrahman Mohamed and Wei-Ning Hsu's help in this implementation,
-# Their origial Hubert work is in:
-#     Paper: https://arxiv.org/pdf/2106.07447.pdf
-#     Code in Fairseq: https://github.com/pytorch/fairseq/tree/master/examples/hubert
-
+import logging
 from contextlib import contextmanager
 from typing import Dict, List, Optional, Tuple, Union
 
 import torch
 from packaging.version import parse as V
 from typeguard import check_argument_types
 
+from espnet2.asr.decoder.abs_decoder import AbsDecoder
 from espnet2.asr.encoder.abs_encoder import AbsEncoder
 from espnet2.asr.frontend.abs_frontend import AbsFrontend
+from espnet2.asr.postencoder.abs_postencoder import AbsPostEncoder
 from espnet2.asr.preencoder.abs_preencoder import AbsPreEncoder
-from espnet2.asr.specaug.abs_specaug import AbsSpecAug
-from espnet2.hubert.hubert_loss import HubertPretrainLoss
-from espnet2.layers.abs_normalize import AbsNormalize
 from espnet2.torch_utils.device_funcs import force_gatherable
 from espnet2.train.abs_espnet_model import AbsESPnetModel
-from espnet.nets.e2e_asr_common import ErrorCalculator
+from espnet.nets.e2e_mt_common import ErrorCalculator as MTErrorCalculator
+from espnet.nets.pytorch_backend.nets_utils import th_accuracy
+from espnet.nets.pytorch_backend.transformer.add_sos_eos import add_sos_eos
+from espnet.nets.pytorch_backend.transformer.label_smoothing_loss import (  # noqa: H301
+    LabelSmoothingLoss,
+)
 
 if V(torch.__version__) >= V("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
-class HubertPretrainModel(AbsESPnetModel):
-    """Hubert Pretrain model"""
+class ESPnetMTModel(AbsESPnetModel):
+    """Encoder-Decoder model"""
 
     def __init__(
         self,
         vocab_size: int,
         token_list: Union[Tuple[str, ...], List[str]],
         frontend: Optional[AbsFrontend],
-        specaug: Optional[AbsSpecAug],
-        normalize: Optional[AbsNormalize],
         preencoder: Optional[AbsPreEncoder],
         encoder: AbsEncoder,
+        postencoder: Optional[AbsPostEncoder],
+        decoder: AbsDecoder,
+        src_vocab_size: int = 0,
+        src_token_list: Union[Tuple[str, ...], List[str]] = [],
         ignore_id: int = -1,
         lsm_weight: float = 0.0,
         length_normalized_loss: bool = False,
-        report_cer: bool = False,
-        report_wer: bool = False,
+        report_bleu: bool = True,
         sym_space: str = "<space>",
         sym_blank: str = "<blank>",
-        pred_masked_weight: float = 1.0,
-        pred_nomask_weight: float = 0.0,
-        loss_weights: float = 0.0,
+        extract_feats_in_collect_stats: bool = True,
+        share_decoder_input_output_embed: bool = False,
+        share_encoder_decoder_input_embed: bool = False,
     ):
         assert check_argument_types()
 
         super().__init__()
         # note that eos is the same as sos (equivalent ID)
         self.sos = vocab_size - 1
         self.eos = vocab_size - 1
+        self.src_sos = src_vocab_size - 1 if src_vocab_size else None
+        self.src_eos = src_vocab_size - 1 if src_vocab_size else None
         self.vocab_size = vocab_size
+        self.src_vocab_size = src_vocab_size
         self.ignore_id = ignore_id
         self.token_list = token_list.copy()
 
+        if share_decoder_input_output_embed:
+            if decoder.output_layer is not None:
+                decoder.output_layer.weight = decoder.embed[0].weight
+                logging.info(
+                    "Decoder input embedding and output linear layer are shared"
+                )
+            else:
+                logging.warning(
+                    "Decoder has no output layer, so it cannot be shared "
+                    "with input embedding"
+                )
+
+        if share_encoder_decoder_input_embed:
+            if src_vocab_size == vocab_size:
+                frontend.embed[0].weight = decoder.embed[0].weight
+                logging.info("Encoder and decoder input embeddings are shared")
+            else:
+                logging.warning(
+                    f"src_vocab_size ({src_vocab_size}) does not equal tgt_vocab_size"
+                    f" ({vocab_size}), so the encoder and decoder input embeddings "
+                    "cannot be shared"
+                )
+
         self.frontend = frontend
-        self.specaug = specaug
-        self.normalize = normalize
         self.preencoder = preencoder
+        self.postencoder = postencoder
         self.encoder = encoder
-        self.criterion_att = HubertPretrainLoss(
-            pred_masked_weight,
-            pred_nomask_weight,
-            loss_weights,
-        )
-        self.pred_masked_weight = pred_masked_weight
-        self.pred_nomask_weight = pred_nomask_weight
-        self.loss_weights = loss_weights
-
-        if report_cer or report_wer:
-            self.error_calculator = ErrorCalculator(
-                token_list, sym_space, sym_blank, report_cer, report_wer
+        self.decoder = decoder
+
+        self.criterion_mt = LabelSmoothingLoss(
+            size=vocab_size,
+            padding_idx=ignore_id,
+            smoothing=lsm_weight,
+            normalize_length=length_normalized_loss,
+        )
+
+        # MT error calculator
+        if report_bleu:
+            self.mt_error_calculator = MTErrorCalculator(
+                token_list, sym_space, sym_blank, report_bleu
             )
         else:
-            self.error_calculator = None
+            self.mt_error_calculator = None
+
+        self.extract_feats_in_collect_stats = extract_feats_in_collect_stats
 
     def forward(
         self,
-        speech: torch.Tensor,
-        speech_lengths: torch.Tensor,
         text: torch.Tensor,
         text_lengths: torch.Tensor,
+        src_text: torch.Tensor,
+        src_text_lengths: torch.Tensor,
         **kwargs,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
-        """Frontend + Encoder + Calc loss
+        """Frontend + Encoder + Decoder + Calc loss
 
         Args:
-            speech: (Batch, Length, ...)
-            speech_lengths: (Batch, )
             text: (Batch, Length)
             text_lengths: (Batch,)
+            src_text: (Batch, length)
+            src_text_lengths: (Batch,)
             kwargs: "utt_id" is among the input.
         """
         assert text_lengths.dim() == 1, text_lengths.shape
         # Check that batch_size is unified
         assert (
-            speech.shape[0]
-            == speech_lengths.shape[0]
-            == text.shape[0]
+            text.shape[0]
             == text_lengths.shape[0]
-        ), (speech.shape, speech_lengths.shape, text.shape, text_lengths.shape)
-        batch_size = speech.shape[0]
+            == src_text.shape[0]
+            == src_text_lengths.shape[0]
+        ), (text.shape, text_lengths.shape, src_text.shape, src_text_lengths.shape)
+
+        batch_size = src_text.shape[0]
 
         # for data-parallel
         text = text[:, : text_lengths.max()]
+        src_text = src_text[:, : src_text_lengths.max()]
 
         # 1. Encoder
-        encoder_out = self.encode(speech, speech_lengths, text, text_lengths)
+        encoder_out, encoder_out_lens = self.encode(src_text, src_text_lengths)
 
-        # 2a. Hubert criterion
-        loss, acc_mask, acc_unmask = self._calc_hubert_loss(
-            encoder_out,
+        # 2a. Attention-decoder branch (MT)
+        loss_mt_att, acc_mt_att, bleu_mt_att = self._calc_mt_att_loss(
+            encoder_out, encoder_out_lens, text, text_lengths
         )
 
+        # 3. Loss computation
+        loss = loss_mt_att
+
         stats = dict(
             loss=loss.detach(),
-            acc_mask=acc_mask,
-            acc_unmask=acc_unmask,
-            acc=acc_mask,
+            acc=acc_mt_att,
+            bleu=bleu_mt_att,
         )
 
         # force_gatherable: to-device and to-tensor if scalar for DataParallel
         loss, stats, weight = force_gatherable((loss, stats, batch_size), loss.device)
         return loss, stats, weight
 
     def collect_feats(
         self,
-        speech: torch.Tensor,
-        speech_lengths: torch.Tensor,
         text: torch.Tensor,
         text_lengths: torch.Tensor,
+        src_text: torch.Tensor,
+        src_text_lengths: torch.Tensor,
         **kwargs,
     ) -> Dict[str, torch.Tensor]:
-        feats, feats_lengths = self._extract_feats(speech, speech_lengths)
+        if self.extract_feats_in_collect_stats:
+            feats, feats_lengths = self._extract_feats(src_text, src_text_lengths)
+        else:
+            # Generate dummy stats if extract_feats_in_collect_stats is False
+            logging.warning(
+                "Generating dummy stats for feats and feats_lengths, "
+                "because encoder_conf.extract_feats_in_collect_stats is "
+                f"{self.extract_feats_in_collect_stats}"
+            )
+            feats, feats_lengths = src_text, src_text_lengths
         return {"feats": feats, "feats_lengths": feats_lengths}
 
     def encode(
-        self,
-        speech: torch.Tensor,
-        speech_lengths: torch.Tensor,
-        y_pad: torch.Tensor,
-        y_pad_length: torch.Tensor,
+        self, src_text: torch.Tensor, src_text_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
-        """Frontend + Encoder. Note that this method is used by asr_inference.py
+        """Frontend + Encoder. Note that this method is used by mt_inference.py
 
         Args:
-            speech: (Batch, Length, ...)
-            speech_lengths: (Batch, )
-            y_pad: (Batch, Length, ...)
-            y_pad_length: (Batch, )
+            src_text: (Batch, Length, ...)
+            src_text_lengths: (Batch, )
         """
         with autocast(False):
             # 1. Extract feats
-            feats, feats_lengths = self._extract_feats(speech, speech_lengths)
+            feats, feats_lengths = self._extract_feats(src_text, src_text_lengths)
 
             # 2. Data augmentation
-            if self.specaug is not None and self.training:
-                feats, feats_lengths = self.specaug(feats, feats_lengths)
-
-            # 3. Normalization for feature: e.g. Global-CMVN, Utterance-CMVN
-            if self.normalize is not None:
-                feats, feats_lengths = self.normalize(feats, feats_lengths)
+            # if self.specaug is not None and self.training:
+            #     feats, feats_lengths = self.specaug(feats, feats_lengths)
 
         # Pre-encoder, e.g. used for raw input data
         if self.preencoder is not None:
             feats, feats_lengths = self.preencoder(feats, feats_lengths)
 
         # 4. Forward encoder
         # feats: (Batch, Length, Dim)
         # -> encoder_out: (Batch, Length2, Dim2)
-        encoder_out = self.encoder(feats, feats_lengths, y_pad, y_pad_length)
+        encoder_out, encoder_out_lens, _ = self.encoder(feats, feats_lengths)
 
-        if hasattr(self.encoder, "encoder"):
-            logp_m_list = self.encoder.encoder.get_logits(encoder_out, True)
-            assert self.pred_masked_weight == 0 or len(logp_m_list) > 0
+        # Post-encoder, e.g. NLU
+        if self.postencoder is not None:
+            encoder_out, encoder_out_lens = self.postencoder(
+                encoder_out, encoder_out_lens
+            )
 
-            logp_u_list = self.encoder.encoder.get_logits(encoder_out, False)
-            assert self.pred_nomask_weight == 0 or len(logp_u_list) > 0
+        assert encoder_out.size(0) == src_text.size(0), (
+            encoder_out.size(),
+            src_text.size(0),
+        )
+        assert encoder_out.size(1) <= encoder_out_lens.max(), (
+            encoder_out.size(),
+            encoder_out_lens.max(),
+        )
 
-        return encoder_out
+        return encoder_out, encoder_out_lens
 
     def _extract_feats(
-        self, speech: torch.Tensor, speech_lengths: torch.Tensor
+        self, src_text: torch.Tensor, src_text_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
-        assert speech_lengths.dim() == 1, speech_lengths.shape
+        assert src_text_lengths.dim() == 1, src_text_lengths.shape
 
         # for data-parallel
-        speech = speech[:, : speech_lengths.max()]
+        src_text = src_text[:, : src_text_lengths.max()]
+        src_text, _ = add_sos_eos(src_text, self.src_sos, self.src_eos, self.ignore_id)
+        src_text_lengths = src_text_lengths + 1
 
         if self.frontend is not None:
             # Frontend
-            #  e.g. STFT and Feature extract
-            #       data_loader may send time-domain signal in this case
-            # speech (Batch, NSamples) -> feats: (Batch, NFrames, Dim)
-            feats, feats_lengths = self.frontend(speech, speech_lengths)
+            #  e.g. Embedding Lookup
+            # src_text (Batch, NSamples) -> feats: (Batch, NSamples, Dim)
+            feats, feats_lengths = self.frontend(src_text, src_text_lengths)
         else:
             # No frontend and no feature extract
-            feats, feats_lengths = speech, speech_lengths
+            feats, feats_lengths = src_text, src_text_lengths
         return feats, feats_lengths
 
-    def compute_correct(
+    def _calc_mt_att_loss(
         self,
-        logits,
+        encoder_out: torch.Tensor,
+        encoder_out_lens: torch.Tensor,
+        ys_pad: torch.Tensor,
+        ys_pad_lens: torch.Tensor,
     ):
-        if logits.numel() == 0:
-            return 0, 0
-        else:
-            assert logits.dim() > 1, logits.shape
-            max = logits.argmax(-1) == 0
-            min = logits.argmin(-1) == 0
-            both = max & min
-            corr = max.long().sum().item() - both.long().sum().item()
-            count = max.numel()
-            return corr, count
+        ys_in_pad, ys_out_pad = add_sos_eos(ys_pad, self.sos, self.eos, self.ignore_id)
+        ys_in_lens = ys_pad_lens + 1
 
-    def _calc_hubert_loss(
-        self,
-        encoder_out: Dict[str, torch.Tensor],
-    ):
+        # 1. Forward decoder
+        decoder_out, _ = self.decoder(
+            encoder_out, encoder_out_lens, ys_in_pad, ys_in_lens
+        )
 
-        # 1. Compute attention loss
-        loss_att, logp_m_list, logp_u_list = self.criterion_att(
-            self.encoder.encoder, encoder_out
-        )
-
-        corr_masked, count_masked = 0, 0
-        corr_unmask, count_unmask = 0, 0
-        with torch.no_grad():
-            for i, logp_m in enumerate(logp_m_list):
-                corr_m, count_m = self.compute_correct(logp_m)
-                corr_masked += corr_m
-                count_masked += count_m
-            for i, logp_u in enumerate(logp_u_list):
-                corr_u, count_u = self.compute_correct(logp_u)
-                corr_unmask += corr_u
-                count_unmask += count_u
+        # 2. Compute attention loss
+        loss_att = self.criterion_mt(decoder_out, ys_out_pad)
+        acc_att = th_accuracy(
+            decoder_out.view(-1, self.vocab_size),
+            ys_out_pad,
+            ignore_label=self.ignore_id,
+        )
 
-        acc_att_m = corr_masked / (count_masked + 1e-10)
-        acc_att_u = corr_unmask / (count_unmask + 1e-10)
+        # Compute cer/wer using attention-decoder
+        if self.training or self.mt_error_calculator is None:
+            bleu_att = None
+        else:
+            ys_hat = decoder_out.argmax(dim=-1)
+            bleu_att = self.mt_error_calculator(ys_hat.cpu(), ys_pad.cpu())
 
-        return loss_att, acc_att_m, acc_att_u
+        return loss_att, acc_att, bleu_att
```

### Comparing `espnet-202211/espnet2/hubert/hubert_loss.py` & `espnet-202301/espnet2/hubert/hubert_loss.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/iterators/chunk_iter_factory.py` & `espnet-202301/espnet2/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/iterators/multiple_iter_factory.py` & `espnet-202301/espnet2/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/iterators/sequence_iter_factory.py` & `espnet-202301/espnet2/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/layers/global_mvn.py` & `espnet-202301/espnet2/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/layers/label_aggregation.py` & `espnet-202301/espnet2/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/layers/log_mel.py` & `espnet-202301/espnet2/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/layers/mask_along_axis.py` & `espnet-202301/espnet2/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/layers/sinc_conv.py` & `espnet-202301/espnet2/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/layers/stft.py` & `espnet-202301/espnet2/layers/stft.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
             # use stft_kwargs to flexibly control different PyTorch versions' kwargs
             stft_kwargs = dict(
                 n_fft=self.n_fft,
                 win_length=self.win_length,
                 hop_length=self.hop_length,
                 center=self.center,
                 window=window,
+                pad_mode="reflect",
             )
 
             if window is not None:
                 # pad the given window to n_fft
                 n_pad_left = (self.n_fft - window.shape[0]) // 2
                 n_pad_right = self.n_fft - window.shape[0] - n_pad_left
                 stft_kwargs["window"] = torch.cat(
```

### Comparing `espnet-202211/espnet2/layers/time_warp.py` & `espnet-202301/espnet2/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/layers/utterance_mvn.py` & `espnet-202301/espnet2/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/lm/abs_model.py` & `espnet-202301/espnet2/lm/abs_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/lm/espnet_model.py` & `espnet-202301/espnet2/lm/espnet_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/lm/seq_rnn_lm.py` & `espnet-202301/espnet2/lm/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/lm/transformer_lm.py` & `espnet-202301/espnet2/lm/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/main_funcs/average_nbest_models.py` & `espnet-202301/espnet2/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/main_funcs/calculate_all_attentions.py` & `espnet-202301/espnet2/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/main_funcs/collect_stats.py` & `espnet-202301/espnet2/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/main_funcs/pack_funcs.py` & `espnet-202301/espnet2/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/mt/frontend/embedding.py` & `espnet-202301/espnet2/mt/frontend/embedding.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/optimizers/sgd.py` & `espnet-202301/espnet2/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/samplers/build_batch_sampler.py` & `espnet-202301/espnet2/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/samplers/folded_batch_sampler.py` & `espnet-202301/espnet2/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/samplers/length_batch_sampler.py` & `espnet-202301/espnet2/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/samplers/num_elements_batch_sampler.py` & `espnet-202301/espnet2/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/samplers/sorted_batch_sampler.py` & `espnet-202301/espnet2/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/samplers/unsorted_batch_sampler.py` & `espnet-202301/espnet2/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/schedulers/abs_scheduler.py` & `espnet-202301/espnet2/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/schedulers/noam_lr.py` & `espnet-202301/espnet2/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/schedulers/warmup_lr.py` & `espnet-202301/espnet2/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/schedulers/warmup_step_lr.py` & `espnet-202301/espnet2/schedulers/warmup_step_lr.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/slu/espnet_model.py` & `espnet-202301/espnet2/slu/espnet_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/slu/postdecoder/abs_postdecoder.py` & `espnet-202301/espnet2/slu/postdecoder/abs_postdecoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/slu/postdecoder/hugging_face_transformers_postdecoder.py` & `espnet-202301/espnet2/slu/postdecoder/hugging_face_transformers_postdecoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/slu/postencoder/conformer_postencoder.py` & `espnet-202301/espnet2/slu/postencoder/conformer_postencoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/slu/postencoder/transformer_postencoder.py` & `espnet-202301/espnet2/slu/postencoder/transformer_postencoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/st/espnet_model.py` & `espnet-202301/espnet2/st/espnet_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/svs/abs_svs.py` & `espnet-202301/espnet2/svs/abs_svs.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/svs/espnet_model.py` & `espnet-202301/espnet2/gan_svs/espnet_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,124 +1,80 @@
-# Copyright 2020 Nagoya University (Tomoki Hayashi)
-# Copyright 2021 Carnegie Mellon University (Jiatong Shi)
-# Copyright 2022 Renmin University of China (Yuning Wu)
+# Copyright 2021 Tomoki Hayashi
+# Copyright 2022 Yifeng Yu
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
-"""Singing-voice-synthesis ESPnet model."""
+"""GAN-based Singing-voice-synthesis ESPnet model."""
 
 from contextlib import contextmanager
-from distutils.version import LooseVersion
-from typing import Dict, Optional, Tuple
+from typing import Any, Dict, Optional
 
 import torch
+from packaging.version import parse as V
 from typeguard import check_argument_types
 
+from espnet2.gan_svs.abs_gan_svs import AbsGANSVS
 from espnet2.layers.abs_normalize import AbsNormalize
 from espnet2.layers.inversible_interface import InversibleInterface
-from espnet2.svs.abs_svs import AbsSVS
+from espnet2.svs.espnet_model import cal_ds, cal_ds_syb
 from espnet2.svs.feats_extract.score_feats_extract import (
     FrameScoreFeats,
     SyllableScoreFeats,
 )
-from espnet2.train.abs_espnet_model import AbsESPnetModel
+from espnet2.train.abs_gan_espnet_model import AbsGANESPnetModel
 from espnet2.tts.feats_extract.abs_feats_extract import AbsFeatsExtract
 from espnet.nets.pytorch_backend.nets_utils import pad_list
 
-if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
+if V(torch.__version__) >= V("1.6.0"):
     from torch.cuda.amp import autocast
 else:
-    # Nothing to do if torch<1.6.0
+    # Nothing to do if torch < 1.6.0
     @contextmanager
     def autocast(enabled=True):  # NOQA
         yield
 
 
-def cal_ds(ilen, label, midi, beat, ref_len, ref_label, ref_midi, ref_beat):
-    """Calculate frame expanding length for each label."""
-    ds = []
-    i = 0
-    j = 0
-    while i < ilen:
-        _label = label[i]
-        _midi = midi[i]
-        _beat = beat[i]
-        same = 1
-        i += 1
-        # If adjacent notes are the same, frame counts should be averaged.
-        while i < ilen and label[i] == _label and midi[i] == _midi and beat[i] == _beat:
-            same += 1
-            i += 1
-        # Count for the length
-        cnt = 0
-        while (
-            j < ref_len
-            and ref_label[j] == _label
-            and ref_midi[j] == _midi
-            and ref_beat[j] == _beat
-        ):
-            cnt += 1
-            j += 1
-        # Calculate Average length for same notes
-        ave = int(cnt / same)
-        for k in range(same - 1):
-            ds.append(ave)
-            cnt -= ave
-        ds.append(cnt)
-    assert j == ref_len
-    return ds
-
-
-def cal_ds_syb(ds, phn_cnt):
-    """Calculate frame expanding length for each syllable."""
-    ds_syb = []
-    pos = 0
-    # Sum up phone frames in each syllable
-    for cnt in phn_cnt:
-        d = 0
-        for k in range(pos, pos + cnt):
-            d += ds[k]
-        pos += cnt
-        for k in range(cnt):
-            ds_syb.append(d)
-    return ds_syb
-
-
-class ESPnetSVSModel(AbsESPnetModel):
-    """ESPnet model for singing voice synthesis task."""
+class ESPnetGANSVSModel(AbsGANESPnetModel):
+    """ESPnet model for GAN-based text-to-speech task."""
 
     def __init__(
         self,
         text_extract: Optional[AbsFeatsExtract],
         feats_extract: Optional[AbsFeatsExtract],
         score_feats_extract: Optional[AbsFeatsExtract],
         label_extract: Optional[AbsFeatsExtract],
         pitch_extract: Optional[AbsFeatsExtract],
         tempo_extract: Optional[AbsFeatsExtract],
         beat_extract: Optional[AbsFeatsExtract],
         energy_extract: Optional[AbsFeatsExtract],
         normalize: Optional[AbsNormalize and InversibleInterface],
         pitch_normalize: Optional[AbsNormalize and InversibleInterface],
         energy_normalize: Optional[AbsNormalize and InversibleInterface],
-        svs: AbsSVS,
+        svs: AbsGANSVS,
     ):
-        """Initialize ESPnetSVSModel module."""
+        """Initialize ESPnetGANSVSModel module."""
         assert check_argument_types()
         super().__init__()
         self.text_extract = text_extract
         self.feats_extract = feats_extract
         self.score_feats_extract = score_feats_extract
         self.label_extract = label_extract
         self.pitch_extract = pitch_extract
         self.tempo_extract = tempo_extract
         self.beat_extract = beat_extract
         self.energy_extract = energy_extract
         self.normalize = normalize
         self.pitch_normalize = pitch_normalize
         self.energy_normalize = energy_normalize
         self.svs = svs
+        assert hasattr(
+            svs, "generator"
+        ), "generator module must be registered as svs.generator"
+        assert hasattr(
+            svs, "discriminator"
+        ), "discriminator module must be registered as svs.discriminator"
 
     def forward(
         self,
         text: torch.Tensor,
         text_lengths: torch.Tensor,
         singing: torch.Tensor,
         singing_lengths: torch.Tensor,
@@ -158,18 +114,18 @@
         pitch: Optional[torch.Tensor] = None,
         pitch_lengths: Optional[torch.Tensor] = None,
         energy: Optional[torch.Tensor] = None,
         energy_lengths: Optional[torch.Tensor] = None,
         spembs: Optional[torch.Tensor] = None,
         sids: Optional[torch.Tensor] = None,
         lids: Optional[torch.Tensor] = None,
-        flag_IsValid=False,
+        forward_generator: bool = True,
         **kwargs,
-    ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
-        """Caclualte outputs and return the loss tensor.
+    ) -> Dict[str, Any]:
+        """Return generator or discriminator loss with dict format.
 
         Args:
             text (Tensor): Text index tensor (B, T_text).
             text_lengths (Tensor): Text length tensor (B,).
             singing (Tensor): Singing waveform tensor (B, T_wav).
             singing_lengths (Tensor): Singing length tensor (B,).
             ---- label* is label id sequence ----
@@ -209,31 +165,33 @@
             pitch (Optional[Tensor]): Pitch tensor (B, T_wav). - f0 sequence
             pitch_lengths (Optional[Tensor]): Pitch length tensor (B,).
             energy (Optional[Tensor]): Energy tensor.
             energy_lengths (Optional[Tensor]): Energy length tensor (B,).
             spembs (Optional[Tensor]): Speaker embedding tensor (B, D).
             sids (Optional[Tensor]): Speaker ID tensor (B, 1).
             lids (Optional[Tensor]): Language ID tensor (B, 1).
+            forward_generator (bool): Whether to forward generator.
             kwargs: "utt_id" is among the input.
 
         Returns:
-            Tensor: Loss scalar tensor.
-            Dict[str, float]: Statistics to be monitored.
-            Tensor: Weight tensor to summarize losses.
+            Dict[str, Any]:
+                - loss (Tensor): Loss scalar tensor.
+                - stats (Dict[str, float]): Statistics to be monitored.
+                - weight (Tensor): Weight tensor to summarize losses.
+                - optim_idx (int): Optimizer index (0 for G and 1 for D).
+
         """
         with autocast(False):
             # Extract features
+            feats = None
             if self.feats_extract is not None:
                 feats, feats_lengths = self.feats_extract(
-                    singing, singing_lengths
-                )  # singing to spec feature (frame level)
-            else:
-                # Use precalculated feats (feats_type != raw case)
-                feats, feats_lengths = singing, singing_lengths
-
+                    singing,
+                    singing_lengths,
+                )
             # Extract auxiliary features
             # score : 128 midi pitch
             # tempo : bpm
             # duration :
             #   input-> phone-id seqence
             #   output -> frame level(take mode from window) or syllable level
             ds = None
@@ -415,15 +373,14 @@
                 pitch, pitch_lengths = self.pitch_extract(
                     input=singing,
                     input_lengths=singing_lengths,
                     feats_lengths=feats_lengths,
                     durations=label_lab,
                     durations_lengths=label_lab_lengths,
                 )
-
             if self.energy_extract is not None and energy is None:
                 energy, energy_lengths = self.energy_extract(
                     singing,
                     singing_lengths,
                     feats_lengths=feats_lengths,
                     durations=label_lab,
                     durations_lengths=label_lab_lengths,
@@ -437,24 +394,25 @@
             if self.energy_normalize is not None:
                 energy, energy_lengths = self.energy_normalize(energy, energy_lengths)
 
         # Make batch for svs inputs
         batch = dict(
             text=text,
             text_lengths=text_lengths,
-            feats=feats,
-            feats_lengths=feats_lengths,
-            flag_IsValid=flag_IsValid,
+            forward_generator=forward_generator,
         )
 
+        # Update batch for additional auxiliary inputs
+
         # label
         # NOTE(Yuning): Label can be word, syllable or phoneme,
         # which is determined by annotation file.
         label = dict()
         label_lengths = dict()
+
         if label_lab_after is not None:
             label_lab = label_lab_after.to(dtype=torch.long)
             label.update(lab=label_lab)
             label_lengths.update(lab=label_lab_lengths_after)
         if label_score_after is not None:
             label_score = label_score_after.to(dtype=torch.long)
             label.update(score=label_score)
@@ -518,14 +476,16 @@
 
         if spembs is not None:
             batch.update(spembs=spembs)
         if sids is not None:
             batch.update(sids=sids)
         if lids is not None:
             batch.update(lids=lids)
+        if feats is not None:
+            batch.update(feats=feats, feats_lengths=feats_lengths)
         if self.pitch_extract is not None and pitch is not None:
             batch.update(pitch=pitch, pitch_lengths=pitch_lengths)
         if self.energy_extract is not None and energy is not None:
             batch.update(energy=energy, energy_lengths=energy_lengths)
         if self.svs.require_raw_singing:
             batch.update(singing=singing, singing_lengths=singing_lengths)
         return self.svs(**batch)
@@ -574,15 +534,15 @@
         energy: Optional[torch.Tensor] = None,
         energy_lengths: Optional[torch.Tensor] = None,
         spembs: Optional[torch.Tensor] = None,
         sids: Optional[torch.Tensor] = None,
         lids: Optional[torch.Tensor] = None,
         **kwargs,
     ) -> Dict[str, torch.Tensor]:
-        """Caclualte features and return them as a dict.
+        """Calculate features and return them as a dict.
 
         Args:
             text (Tensor): Text index tensor (B, T_text).
             text_lengths (Tensor): Text length tensor (B,).
             singing (Tensor): Singing waveform tensor (B, T_wav).
             singing_lengths (Tensor): Singing length tensor (B,).
             ---- label* is label id sequence ----
@@ -626,20 +586,20 @@
             spembs (Optional[Tensor]): Speaker embedding tensor (B, D).
             sids (Optional[Tensor]): Speaker ID tensor (B, 1).
             lids (Optional[Tensor]): Language ID tensor (B, 1).
 
         Returns:
             Dict[str, Tensor]: Dict of features.
         """
+        feats = None
         if self.feats_extract is not None:
-            feats, feats_lengths = self.feats_extract(singing, singing_lengths)
-        else:
-            # Use precalculated feats (feats_type != raw case)
-            feats, feats_lengths = singing, singing_lengths
-
+            feats, feats_lengths = self.feats_extract(
+                singing,
+                singing_lengths,
+            )
         if self.score_feats_extract is not None:
             (
                 label_lab_after,
                 label_lab_lengths_after,
                 midi_lab_after,
                 midi_lab_lengths_after,
                 tempo_lab_after,
@@ -690,15 +650,17 @@
                 singing_lengths,
                 feats_lengths=feats_lengths,
                 durations=label_lab,
                 durations_lengths=label_lab_lengths,
             )
 
         # store in dict
-        feats_dict = dict(feats=feats, feats_lengths=feats_lengths)
+        feats_dict = {}
+        if feats is not None:
+            feats_dict.update(feats=feats, feats_lengths=feats_lengths)
         if pitch is not None:
             feats_dict.update(pitch=pitch, pitch_lengths=pitch_lengths)
         if energy is not None:
             feats_dict.update(energy=energy, energy_lengths=energy_lengths)
 
         return feats_dict
 
@@ -788,15 +750,17 @@
         beat_score_phn_lengths = torch.tensor([len(beat_score_phn)])
         assert (
             label_score_lengths == midi_score_lengths
             and label_score_lengths == tempo_score_lengths
             and tempo_score_lengths == beat_score_phn_lengths
         )
 
-        # unsqueeze of singing needed otherwise causing error in STFT dimension
+        # unsqueeze of singing must be here
+        # or it'll cause error in the return dim of STFT
+
         # for data-parallel
         text = text.unsqueeze(0)
 
         label = label.unsqueeze(0)
         midi = midi.unsqueeze(0)
         beat_phn = beat_phn.unsqueeze(0)
         beat_ruled_phn = beat_ruled_phn.unsqueeze(0)
@@ -815,15 +779,15 @@
         beat_score_syb = beat_score_syb.unsqueeze(0)
 
         # Extract auxiliary features
         # score : 128 midi pitch
         # tempo : bpm
         # duration :
         #   input-> phone-id seqence
-        #   output -> frame level or syllable level
+        #   output -> frame level(取众数 from window) or syllable level
         ds = None
         batch_size = text.size(0)
         assert batch_size == 1
         if isinstance(self.score_feats_extract, FrameScoreFeats):
             (
                 label_lab_after,
                 label_lab_lengths_after,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `espnet-202211/espnet2/svs/feats_extract/score_feats_extract.py` & `espnet-202301/espnet2/svs/feats_extract/score_feats_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         fs: Union[int, str] = 22050,
         n_fft: int = 1024,
         win_length: int = 512,
         hop_length: int = 128,
         window: str = "hann",
         center: bool = True,
     ):
+        if win_length is None:
+            win_length = n_fft
         assert check_argument_types()
         super().__init__()
 
         self.fs = fs
         self.n_fft = n_fft
         self.win_length = win_length
         self.hop_length = hop_length
@@ -162,14 +164,16 @@
         fs: Union[int, str] = 22050,
         n_fft: int = 1024,
         win_length: int = 512,
         hop_length: int = 128,
         window: str = "hann",
         center: bool = True,
     ):
+        if win_length is None:
+            win_length = n_fft
         assert check_argument_types()
         super().__init__()
 
         self.fs = fs
         self.n_fft = n_fft
         self.win_length = win_length
         self.hop_length = hop_length
```

### Comparing `espnet-202211/espnet2/svs/naive_rnn/naive_rnn.py` & `espnet-202301/espnet2/svs/naive_rnn/naive_rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,14 +455,15 @@
         tempo: Optional[Dict[str, torch.Tensor]] = None,
         beat: Optional[Dict[str, torch.Tensor]] = None,
         pitch: Optional[torch.Tensor] = None,
         duration: Optional[Dict[str, torch.Tensor]] = None,
         spembs: Optional[torch.Tensor] = None,
         sids: Optional[torch.Tensor] = None,
         lids: Optional[torch.Tensor] = None,
+        use_teacher_forcing: torch.Tensor = False,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Calculate forward propagation.
 
         Args:
             text (LongTensor): Batch of padded character ids (Tmax).
             feats (Tensor): Batch of padded target features (Lmax, odim).
             label (Optional[Dict]): key is "lab" or "score";
@@ -518,15 +519,17 @@
         if self.postnet is None:
             after_outs = before_outs
         else:
             after_outs = before_outs + self.postnet(
                 before_outs.transpose(1, 2)
             ).transpose(1, 2)
 
-        return after_outs, None, None  # outs, probs, att_ws
+        return dict(
+            feat_gen=after_outs[0], prob=None, att_w=None
+        )  # outs, probs, att_ws
 
     def _integrate_with_spk_embed(
         self, hs: torch.Tensor, spembs: torch.Tensor
     ) -> torch.Tensor:
         """Integrate speaker embedding with hidden states.
 
         Args:
```

### Comparing `espnet-202211/espnet2/svs/naive_rnn/naive_rnn_dp.py` & `espnet-202301/espnet2/svs/naive_rnn/naive_rnn_dp.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,14 +457,15 @@
         tempo: Optional[Dict[str, torch.Tensor]] = None,
         beat: Optional[Dict[str, torch.Tensor]] = None,
         pitch: Optional[torch.Tensor] = None,
         duration: Optional[Dict[str, torch.Tensor]] = None,
         spembs: Optional[torch.Tensor] = None,
         sids: Optional[torch.Tensor] = None,
         lids: Optional[torch.Tensor] = None,
+        use_teacher_forcing: torch.Tensor = False,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Calculate forward propagation.
 
         Args:
             text (LongTensor): Batch of padded character ids (Tmax).
             feats (Tensor): Batch of padded target features (Lmax, odim).
             label (Optional[Dict]): key is "lab" or "score";
@@ -533,15 +534,17 @@
         if self.postnet is None:
             after_outs = before_outs
         else:
             after_outs = before_outs + self.postnet(
                 before_outs.transpose(1, 2)
             ).transpose(1, 2)
 
-        return after_outs, None, None  # outs, probs, att_ws
+        return dict(
+            feat_gen=after_outs[0], prob=None, att_w=None
+        )  # outs, probs, att_ws
 
     def _integrate_with_spk_embed(
         self, hs: torch.Tensor, spembs: torch.Tensor
     ) -> torch.Tensor:
         """Integrate speaker embedding with hidden states.
 
         Args:
```

### Comparing `espnet-202211/espnet2/svs/xiaoice/XiaoiceSing.py` & `espnet-202301/espnet2/svs/xiaoice/XiaoiceSing.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tasks/abs_task.py` & `espnet-202301/espnet2/tasks/abs_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from espnet import __version__
 from espnet2.iterators.abs_iter_factory import AbsIterFactory
 from espnet2.iterators.chunk_iter_factory import ChunkIterFactory
 from espnet2.iterators.multiple_iter_factory import MultipleIterFactory
 from espnet2.iterators.sequence_iter_factory import SequenceIterFactory
 from espnet2.main_funcs.collect_stats import collect_stats
+from espnet2.optimizers.optim_groups import configure_optimizer
 from espnet2.optimizers.sgd import SGD
 from espnet2.samplers.build_batch_sampler import BATCH_TYPES, build_batch_sampler
 from espnet2.samplers.unsorted_batch_sampler import UnsortedBatchSampler
 from espnet2.schedulers.noam_lr import NoamLR
 from espnet2.schedulers.warmup_lr import WarmupLR
 from espnet2.schedulers.warmup_step_lr import WarmupStepLR
 from espnet2.torch_utils.load_pretrained_model import load_pretrained_model
@@ -813,14 +814,29 @@
             type=humanfriendly_parse_size_or_none,
             default=None,
             help="The maximum cache size for validation data loader. e.g. 10MB, 20GB. "
             "If None, the 5 percent size of --max_cache_size",
         )
 
         group = parser.add_argument_group("Optimizer related")
+        group.add_argument(
+            "--exclude_weight_decay",
+            type=str2bool,
+            default=False,
+            help="Exclude weight decay in optimizer for model bias, normalization, "
+            "or other special parameters",
+        )
+        group.add_argument(
+            "--exclude_weight_decay_conf",
+            action=NestedDictAction,
+            default=dict(),
+            help="The keyword arguments for configuring weight decay in optimizer. "
+            "e.g., 'bias_weight_decay': False will set zero weight decay for bias "
+            "params. See also espnet2.optimizers.optim_groups.configure_optimizer.",
+        )
         for i in range(1, cls.num_optimizers + 1):
             suf = "" if i == 1 else str(i)
             group.add_argument(
                 f"--optim{suf}",
                 type=lambda x: x.lower(),
                 default="adadelta",
                 choices=list(optim_classes),
@@ -869,15 +885,23 @@
         if args.sharded_ddp:
             if fairscale is None:
                 raise RuntimeError("Requiring fairscale. Do 'pip install fairscale'")
             optim = fairscale.optim.oss.OSS(
                 params=model.parameters(), optim=optim_class, **args.optim_conf
             )
         else:
-            optim = optim_class(model.parameters(), **args.optim_conf)
+            if args.exclude_weight_decay:
+                optim = configure_optimizer(
+                    model,
+                    optim_class,
+                    args.optim_conf,
+                    args.exclude_weight_decay_conf,
+                )
+            else:
+                optim = optim_class(model.parameters(), **args.optim_conf)
 
         optimizers = [optim]
         return optimizers
 
     @classmethod
     def exclude_opts(cls) -> Tuple[str, ...]:
         """The options not to be shown by --print_config"""
```

### Comparing `espnet-202211/espnet2/tasks/asr.py` & `espnet-202301/espnet2/tasks/asr.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,49 +9,54 @@
 from espnet2.asr.ctc import CTC
 from espnet2.asr.decoder.abs_decoder import AbsDecoder
 from espnet2.asr.decoder.hugging_face_transformers_decoder import (  # noqa: H301
     HuggingFaceTransformersDecoder,
 )
 from espnet2.asr.decoder.mlm_decoder import MLMDecoder
 from espnet2.asr.decoder.rnn_decoder import RNNDecoder
+from espnet2.asr.decoder.s4_decoder import S4Decoder
 from espnet2.asr.decoder.transducer_decoder import TransducerDecoder
 from espnet2.asr.decoder.transformer_decoder import (
     DynamicConvolution2DTransformerDecoder,
     DynamicConvolutionTransformerDecoder,
     LightweightConvolution2DTransformerDecoder,
     LightweightConvolutionTransformerDecoder,
     TransformerDecoder,
 )
+from espnet2.asr.decoder.whisper_decoder import OpenAIWhisperDecoder
 from espnet2.asr.encoder.abs_encoder import AbsEncoder
 from espnet2.asr.encoder.branchformer_encoder import BranchformerEncoder
 from espnet2.asr.encoder.conformer_encoder import ConformerEncoder
 from espnet2.asr.encoder.contextual_block_conformer_encoder import (
     ContextualBlockConformerEncoder,
 )
 from espnet2.asr.encoder.contextual_block_transformer_encoder import (
     ContextualBlockTransformerEncoder,
 )
 from espnet2.asr.encoder.e_branchformer_encoder import EBranchformerEncoder
 from espnet2.asr.encoder.hubert_encoder import (
     FairseqHubertEncoder,
     FairseqHubertPretrainEncoder,
+    TorchAudioHuBERTPretrainEncoder,
 )
 from espnet2.asr.encoder.longformer_encoder import LongformerEncoder
 from espnet2.asr.encoder.rnn_encoder import RNNEncoder
 from espnet2.asr.encoder.transformer_encoder import TransformerEncoder
 from espnet2.asr.encoder.transformer_encoder_multispkr import (
     TransformerEncoder as TransformerEncoderMultiSpkr,
 )
 from espnet2.asr.encoder.vgg_rnn_encoder import VGGRNNEncoder
 from espnet2.asr.encoder.wav2vec2_encoder import FairSeqWav2Vec2Encoder
+from espnet2.asr.encoder.whisper_encoder import OpenAIWhisperEncoder
 from espnet2.asr.espnet_model import ESPnetASRModel
 from espnet2.asr.frontend.abs_frontend import AbsFrontend
 from espnet2.asr.frontend.default import DefaultFrontend
 from espnet2.asr.frontend.fused import FusedFrontends
 from espnet2.asr.frontend.s3prl import S3prlFrontend
+from espnet2.asr.frontend.whisper import WhisperFrontend
 from espnet2.asr.frontend.windowing import SlidingWindow
 from espnet2.asr.maskctc_model import MaskCTCModel
 from espnet2.asr.pit_espnet_model import ESPnetASRModel as PITESPnetModel
 from espnet2.asr.postencoder.abs_postencoder import AbsPostEncoder
 from espnet2.asr.postencoder.hugging_face_transformers_postencoder import (
     HuggingFaceTransformersPostEncoder,
 )
@@ -83,14 +88,15 @@
 frontend_choices = ClassChoices(
     name="frontend",
     classes=dict(
         default=DefaultFrontend,
         sliding_window=SlidingWindow,
         s3prl=S3prlFrontend,
         fused=FusedFrontends,
+        whisper=WhisperFrontend,
     ),
     type_check=AbsFrontend,
     default="default",
 )
 specaug_choices = ClassChoices(
     name="specaug",
     classes=dict(
@@ -139,16 +145,18 @@
         contextual_block_transformer=ContextualBlockTransformerEncoder,
         contextual_block_conformer=ContextualBlockConformerEncoder,
         vgg_rnn=VGGRNNEncoder,
         rnn=RNNEncoder,
         wav2vec2=FairSeqWav2Vec2Encoder,
         hubert=FairseqHubertEncoder,
         hubert_pretrain=FairseqHubertPretrainEncoder,
+        torchaudiohubert=TorchAudioHuBERTPretrainEncoder,
         longformer=LongformerEncoder,
         branchformer=BranchformerEncoder,
+        whisper=OpenAIWhisperEncoder,
         e_branchformer=EBranchformerEncoder,
     ),
     type_check=AbsEncoder,
     default="rnn",
 )
 postencoder_choices = ClassChoices(
     name="postencoder",
@@ -166,18 +174,21 @@
         lightweight_conv=LightweightConvolutionTransformerDecoder,
         lightweight_conv2d=LightweightConvolution2DTransformerDecoder,
         dynamic_conv=DynamicConvolutionTransformerDecoder,
         dynamic_conv2d=DynamicConvolution2DTransformerDecoder,
         rnn=RNNDecoder,
         transducer=TransducerDecoder,
         mlm=MLMDecoder,
+        whisper=OpenAIWhisperDecoder,
         hugging_face_transformers=HuggingFaceTransformersDecoder,
+        s4=S4Decoder,
     ),
     type_check=AbsDecoder,
     default="rnn",
+    optional=True,
 )
 preprocessor_choices = ClassChoices(
     "preprocessor",
     classes=dict(
         default=CommonPreprocessor,
         multi=CommonPreprocessor_multi,
     ),
@@ -272,15 +283,23 @@
             default=True,
             help="Apply preprocessing to data or not",
         )
         group.add_argument(
             "--token_type",
             type=str,
             default="bpe",
-            choices=["bpe", "char", "word", "phn", "hugging_face"],
+            choices=[
+                "bpe",
+                "char",
+                "word",
+                "phn",
+                "hugging_face",
+                "whisper_en",
+                "whisper_multilingual",
+            ],
             help="The text will be tokenized " "in the specified level token",
         )
         group.add_argument(
             "--bpemodel",
             type=str_or_none,
             default=None,
             help="The model file of sentencepiece",
@@ -289,15 +308,22 @@
             "--non_linguistic_symbols",
             type=str_or_none,
             help="non_linguistic_symbols file path",
         )
         group.add_argument(
             "--cleaner",
             type=str_or_none,
-            choices=[None, "tacotron", "jaconv", "vietnamese"],
+            choices=[
+                None,
+                "tacotron",
+                "jaconv",
+                "vietnamese",
+                "whisper_en",
+                "whisper_basic",
+            ],
             default=None,
             help="Apply text cleaning",
         )
         group.add_argument(
             "--g2p",
             type=str_or_none,
             choices=g2p_choices,
@@ -343,14 +369,21 @@
         group.add_argument(
             "--short_noise_thres",
             type=float,
             default=0.5,
             help="If len(noise) / len(speech) is smaller than this threshold during "
             "dynamic mixing, a warning will be displayed.",
         )
+        group.add_argument(
+            "--aux_ctc_tasks",
+            type=str,
+            nargs="+",
+            default=[],
+            help="Auxillary tasks to train on using CTC loss. ",
+        )
 
         for class_choices in cls.class_choices_list:
             # Append --<name> and --<name>_conf.
             # e.g. --encoder and --encoder_conf
             class_choices.add_arguments(group)
 
     @classmethod
@@ -402,14 +435,17 @@
                 else "13_15",
                 short_noise_thres=args.short_noise_thres
                 if hasattr(args, "short_noise_thres")
                 else 0.5,
                 speech_volume_normalize=args.speech_volume_normalize
                 if hasattr(args, "rir_scp")
                 else None,
+                aux_task_names=args.aux_ctc_tasks
+                if hasattr(args, "aux_ctc_tasks")
+                else None,
                 **args.preprocessor_conf,
             )
         else:
             retval = None
         assert check_return_type(retval)
         return retval
 
@@ -425,17 +461,19 @@
         return retval
 
     @classmethod
     def optional_data_names(
         cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         MAX_REFERENCE_NUM = 4
-        retval = []
-        retval += ["text_spk{}".format(n) for n in range(2, MAX_REFERENCE_NUM + 1)]
+
+        retval = ["text_spk{}".format(n) for n in range(2, MAX_REFERENCE_NUM + 1)]
         retval = tuple(retval)
+
+        logging.info(f"Optional Data Names: {retval }")
         assert check_return_type(retval)
         return retval
 
     @classmethod
     def build_model(cls, args: argparse.Namespace) -> ESPnetASRModel:
         assert check_argument_types()
         if isinstance(args.token_list, str):
@@ -500,36 +538,39 @@
                 input_size=encoder_output_size, **args.postencoder_conf
             )
             encoder_output_size = postencoder.output_size()
         else:
             postencoder = None
 
         # 5. Decoder
-        decoder_class = decoder_choices.get_class(args.decoder)
-
-        if args.decoder == "transducer":
-            decoder = decoder_class(
-                vocab_size,
-                embed_pad=0,
-                **args.decoder_conf,
-            )
+        if getattr(args, "decoder", None) is not None:
+            decoder_class = decoder_choices.get_class(args.decoder)
 
-            joint_network = JointNetwork(
-                vocab_size,
-                encoder.output_size(),
-                decoder.dunits,
-                **args.joint_net_conf,
-            )
+            if args.decoder == "transducer":
+                decoder = decoder_class(
+                    vocab_size,
+                    embed_pad=0,
+                    **args.decoder_conf,
+                )
+
+                joint_network = JointNetwork(
+                    vocab_size,
+                    encoder.output_size(),
+                    decoder.dunits,
+                    **args.joint_net_conf,
+                )
+            else:
+                decoder = decoder_class(
+                    vocab_size=vocab_size,
+                    encoder_output_size=encoder_output_size,
+                    **args.decoder_conf,
+                )
+                joint_network = None
         else:
-            decoder = decoder_class(
-                vocab_size=vocab_size,
-                encoder_output_size=encoder_output_size,
-                **args.decoder_conf,
-            )
-
+            decoder = None
             joint_network = None
 
         # 6. CTC
         ctc = CTC(
             odim=vocab_size, encoder_output_size=encoder_output_size, **args.ctc_conf
         )
```

### Comparing `espnet-202211/espnet2/tasks/asr_transducer.py` & `espnet-202301/espnet2/tasks/asr_transducer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tasks/diar.py` & `espnet-202301/espnet2/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tasks/enh.py` & `espnet-202301/espnet2/tasks/enh.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tasks/enh_s2t.py` & `espnet-202301/espnet2/tasks/enh_s2t.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tasks/gan_tts.py` & `espnet-202301/espnet2/tasks/gan_tts.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tasks/hubert.py` & `espnet-202301/espnet2/tasks/hubert.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,43 +3,47 @@
 
 # Thanks to Abdelrahman Mohamed and Wei-Ning Hsu's help in this implementation,
 # Their origial Hubert work is in:
 #     Paper: https://arxiv.org/pdf/2106.07447.pdf
 #     Code in Fairseq: https://github.com/pytorch/fairseq/tree/master/examples/hubert
 import argparse
 import logging
-from typing import Callable, Collection, Dict, List, Optional, Tuple
+from typing import Callable, Collection, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from typeguard import check_argument_types, check_return_type
 
 from espnet2.asr.encoder.abs_encoder import AbsEncoder
 from espnet2.asr.encoder.hubert_encoder import (  # noqa: H301
     FairseqHubertPretrainEncoder,
+    TorchAudioHuBERTPretrainEncoder,
 )
 from espnet2.asr.frontend.abs_frontend import AbsFrontend
 from espnet2.asr.frontend.default import DefaultFrontend
 from espnet2.asr.frontend.windowing import SlidingWindow
 from espnet2.asr.preencoder.abs_preencoder import AbsPreEncoder
 from espnet2.asr.preencoder.sinc import LightweightSincConvs
 from espnet2.asr.specaug.abs_specaug import AbsSpecAug
 from espnet2.asr.specaug.specaug import SpecAug
-from espnet2.hubert.espnet_model import HubertPretrainModel
+from espnet2.hubert.espnet_model import (
+    HubertPretrainModel,
+    TorchAudioHubertPretrainModel,
+)
 from espnet2.layers.abs_normalize import AbsNormalize
 from espnet2.layers.global_mvn import GlobalMVN
 from espnet2.layers.utterance_mvn import UtteranceMVN
 from espnet2.tasks.abs_task import AbsTask
 from espnet2.text.phoneme_tokenizer import g2p_choices
 from espnet2.torch_utils.initialize import initialize
+from espnet2.train.abs_espnet_model import AbsESPnetModel
 from espnet2.train.class_choices import ClassChoices
-from espnet2.train.collate_fn import CommonCollateFn
+from espnet2.train.collate_fn import HuBERTCollateFn
 from espnet2.train.preprocessor import CommonPreprocessor
 from espnet2.train.trainer import Trainer
-from espnet2.utils.get_default_kwargs import get_default_kwargs
 from espnet2.utils.nested_dict_action import NestedDictAction
 from espnet2.utils.types import float_or_none, int_or_none, str2bool, str_or_none
 
 frontend_choices = ClassChoices(
     name="frontend",
     classes=dict(default=DefaultFrontend, sliding_window=SlidingWindow),
     type_check=AbsFrontend,
@@ -71,18 +75,28 @@
     default=None,
     optional=True,
 )
 encoder_choices = ClassChoices(
     "encoder",
     classes=dict(
         hubert_pretrain=FairseqHubertPretrainEncoder,
+        torchaudio_hubert=TorchAudioHuBERTPretrainEncoder,
     ),
     type_check=AbsEncoder,
     default="hubert_pretrain",
 )
+model_choices = ClassChoices(
+    "model",
+    classes=dict(
+        fairseq=HubertPretrainModel,
+        torchaudio=TorchAudioHubertPretrainModel,
+    ),
+    type_check=AbsESPnetModel,
+    default="fairseq",
+)
 
 
 class HubertTask(AbsTask):
     # If you need more than one optimizers, change this value
     num_optimizers: int = 1
 
     # Add variable objects configurations
@@ -93,14 +107,16 @@
         specaug_choices,
         # --normalize and --normalize_conf
         normalize_choices,
         # --preencoder and --preencoder_conf
         preencoder_choices,
         # --encoder and --encoder_conf
         encoder_choices,
+        # --model and --model_conf
+        model_choices,
     ]
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def add_task_arguments(cls, parser: argparse.ArgumentParser):
@@ -127,27 +143,33 @@
                 "xavier_uniform",
                 "xavier_normal",
                 "kaiming_uniform",
                 "kaiming_normal",
                 None,
             ],
         )
+        group.add_argument(
+            "--collate_fn_conf",
+            action=NestedDictAction,
+            default=dict(),
+            help="The keyword arguments for collate_fn class.",
+        )
 
         group.add_argument(
             "--input_size",
             type=int_or_none,
             default=None,
             help="The number of input dimension of the feature",
         )
 
         group.add_argument(
-            "--model_conf",
-            action=NestedDictAction,
-            default=get_default_kwargs(HubertPretrainModel),
-            help="The keyword arguments for model class.",
+            "--num_classes",
+            type=int,
+            default=None,
+            help="The number of classes in hubert",
         )
 
         group = parser.add_argument_group(description="Preprocess related")
         group.add_argument(
             "--use_preprocessor",
             type=str2bool,
             default=True,
@@ -235,35 +257,36 @@
         )
         parser.add_argument(
             "--loss_weights",
             type=float,
             default=0.0,
             help="weights for additional loss terms (not first one)",
         )
-        parser.add_argument(
-            "--hubert_dict",
-            type=str,
-            default="./dict.txt",
-            help="word-based target dictionary for Hubert pretraining stage",
-        )
 
         for class_choices in cls.class_choices_list:
             # Append --<name> and --<name>_conf.
             # e.g. --encoder and --encoder_conf
             class_choices.add_arguments(group)
 
     @classmethod
     def build_collate_fn(
         cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
         assert check_argument_types()
-        return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
+        return HuBERTCollateFn(
+            float_pad_value=0.0,
+            int_pad_value=-1,
+            label_downsampling=args.collate_fn_conf.get("label_downsampling", 1),
+            pad=args.collate_fn_conf.get("pad", False),
+            rand_crop=args.collate_fn_conf.get("rand_crop", True),
+            crop_audio=not args.collect_stats,
+        )
 
     @classmethod
     def build_preprocess_fn(
         cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
         assert check_argument_types()
         if args.use_preprocessor:
@@ -315,15 +338,17 @@
         cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
         assert check_return_type(retval)
         return retval
 
     @classmethod
-    def build_model(cls, args: argparse.Namespace) -> HubertPretrainModel:
+    def build_model(
+        cls, args: argparse.Namespace
+    ) -> Union[HubertPretrainModel, TorchAudioHubertPretrainModel]:
         assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
         elif isinstance(args.token_list, (tuple, list)):
@@ -369,21 +394,24 @@
         else:
             preencoder = None
 
         # 4. Encoder
         encoder_class = encoder_choices.get_class(args.encoder)
         encoder = encoder_class(
             input_size=input_size,
-            use_amp=args.use_amp,
-            hubert_dict=args.hubert_dict,
+            num_classes=args.num_classes,
             **args.encoder_conf,
         )
 
         # 8. Build model
-        model = HubertPretrainModel(
+        try:
+            model_class = model_choices.get_class(args.model)
+        except AttributeError:
+            model_class = model_choices.get_class("fairseq")
+        model = model_class(
             vocab_size=vocab_size,
             frontend=frontend,
             specaug=specaug,
             normalize=normalize,
             preencoder=preencoder,
             encoder=encoder,
             token_list=token_list,
```

### Comparing `espnet-202211/espnet2/tasks/lm.py` & `espnet-202301/espnet2/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tasks/mt.py` & `espnet-202301/espnet2/tasks/mt.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tasks/slu.py` & `espnet-202301/espnet2/tasks/slu.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tasks/st.py` & `espnet-202301/espnet2/tasks/st.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tasks/svs.py` & `espnet-202301/espnet2/tasks/svs.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Callable, Collection, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 import yaml
 from typeguard import check_argument_types, check_return_type
 
+from espnet2.gan_svs.vits import VITS
 from espnet2.layers.abs_normalize import AbsNormalize
 from espnet2.layers.global_mvn import GlobalMVN
 from espnet2.svs.abs_svs import AbsSVS
 from espnet2.svs.espnet_model import ESPnetSVSModel
 from espnet2.svs.feats_extract.score_feats_extract import (
     FrameScoreFeats,
     SyllableScoreFeats,
@@ -30,14 +31,15 @@
 from espnet2.train.class_choices import ClassChoices
 from espnet2.train.collate_fn import CommonCollateFn
 from espnet2.train.preprocessor import SVSPreprocessor
 from espnet2.train.trainer import Trainer
 from espnet2.tts.feats_extract.abs_feats_extract import AbsFeatsExtract
 from espnet2.tts.feats_extract.dio import Dio
 from espnet2.tts.feats_extract.energy import Energy
+from espnet2.tts.feats_extract.linear_spectrogram import LinearSpectrogram
 from espnet2.tts.feats_extract.log_mel_fbank import LogMelFbank
 from espnet2.tts.feats_extract.log_spectrogram import LogSpectrogram
 
 # from espnet2.svs.xiaoice.XiaoiceSing import XiaoiceSing_noDP
 # from espnet2.svs.bytesing.bytesing import ByteSing
 from espnet2.tts.utils import ParallelWaveGANPretrainedVocoder
 from espnet2.utils.get_default_kwargs import get_default_kwargs
@@ -45,15 +47,19 @@
 from espnet2.utils.nested_dict_action import NestedDictAction
 from espnet2.utils.types import int_or_none, str2bool, str_or_none
 
 # TODO(Yuning): Add singing augmentation
 
 feats_extractor_choices = ClassChoices(
     "feats_extract",
-    classes=dict(fbank=LogMelFbank, spectrogram=LogSpectrogram),
+    classes=dict(
+        fbank=LogMelFbank,
+        spectrogram=LogSpectrogram,
+        linear_spectrogram=LinearSpectrogram,
+    ),
     type_check=AbsFeatsExtract,
     default="fbank",
 )
 
 score_feats_extractor_choices = ClassChoices(
     "score_feats_extract",
     classes=dict(
@@ -104,14 +110,15 @@
         # transformer=Transformer,
         # glu_transformer=GLU_Transformer,
         # bytesing=ByteSing,
         naive_rnn=NaiveRNN,
         naive_rnn_dp=NaiveRNNDP,
         xiaoice=XiaoiceSing,
         # xiaoice_noDP=XiaoiceSing_noDP,
+        vits=VITS,
         # mlp=MLPSinger,
     ),
     type_check=AbsSVS,
     default="naive_rnn",
 )
 
 
@@ -260,16 +267,15 @@
                 token_type=args.token_type,
                 token_list=args.token_list,
                 bpemodel=args.bpemodel,
                 non_linguistic_symbols=args.non_linguistic_symbols,
                 text_cleaner=args.cleaner,
                 g2p_type=args.g2p,
                 fs=args.fs,
-                time_shift=args.feats_extract_conf["hop_length"]
-                / args.feats_extract_conf["fs"],
+                hop_length=args.feats_extract_conf["hop_length"],
             )
         else:
             retval = None
         # FIXME (jiatong): sometimes checking is not working here
         # assert check_return_type(retval)
         return retval
```

### Comparing `espnet-202211/espnet2/tasks/tts.py` & `espnet-202301/espnet2/tasks/tts.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from espnet2.tts.fastspeech2 import FastSpeech2
 from espnet2.tts.feats_extract.abs_feats_extract import AbsFeatsExtract
 from espnet2.tts.feats_extract.dio import Dio
 from espnet2.tts.feats_extract.energy import Energy
 from espnet2.tts.feats_extract.linear_spectrogram import LinearSpectrogram
 from espnet2.tts.feats_extract.log_mel_fbank import LogMelFbank
 from espnet2.tts.feats_extract.log_spectrogram import LogSpectrogram
+from espnet2.tts.prodiff import ProDiff
 from espnet2.tts.tacotron2 import Tacotron2
 from espnet2.tts.transformer import Transformer
 from espnet2.tts.utils import ParallelWaveGANPretrainedVocoder
 from espnet2.utils.get_default_kwargs import get_default_kwargs
 from espnet2.utils.griffin_lim import Spectrogram2Waveform
 from espnet2.utils.nested_dict_action import NestedDictAction
 from espnet2.utils.types import int_or_none, str2bool, str_or_none
@@ -87,14 +88,15 @@
 tts_choices = ClassChoices(
     "tts",
     classes=dict(
         tacotron2=Tacotron2,
         transformer=Transformer,
         fastspeech=FastSpeech,
         fastspeech2=FastSpeech2,
+        prodiff=ProDiff,
         # NOTE(kan-bayashi): available only for inference
         vits=VITS,
         joint_text2wav=JointText2Wav,
         jets=JETS,
     ),
     type_check=AbsTTS,
     default="tacotron2",
```

### Comparing `espnet-202211/espnet2/text/build_tokenizer.py` & `espnet-202301/espnet2/text/build_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typeguard import check_argument_types
 
 from espnet2.text.abs_tokenizer import AbsTokenizer
 from espnet2.text.char_tokenizer import CharTokenizer
 from espnet2.text.hugging_face_tokenizer import HuggingFaceTokenizer
 from espnet2.text.phoneme_tokenizer import PhonemeTokenizer
 from espnet2.text.sentencepiece_tokenizer import SentencepiecesTokenizer
+from espnet2.text.whisper_tokenizer import OpenAIWhisperTokenizer
 from espnet2.text.word_tokenizer import WordTokenizer
 
 
 def build_tokenizer(
     token_type: str,
     bpemodel: Union[Path, str, Iterable[str]] = None,
     non_linguistic_symbols: Union[Path, str, Iterable[str]] = None,
@@ -64,11 +65,14 @@
         return PhonemeTokenizer(
             g2p_type=g2p_type,
             non_linguistic_symbols=non_linguistic_symbols,
             space_symbol=space_symbol,
             remove_non_linguistic_symbols=remove_non_linguistic_symbols,
         )
 
+    elif "whisper" in token_type:
+        return OpenAIWhisperTokenizer(bpemodel)
+
     else:
         raise ValueError(
             f"token_mode must be one of bpe, word, char or phn: " f"{token_type}"
         )
```

### Comparing `espnet-202211/espnet2/text/char_tokenizer.py` & `espnet-202301/espnet2/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/text/cleaner.py` & `espnet-202301/espnet2/text/cleaner.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 try:
     from vietnamese_cleaner import vietnamese_cleaners
 except ImportError:
     vietnamese_cleaners = None
 
 from espnet2.text.korean_cleaner import KoreanCleaner
 
+try:
+    from whisper.normalizers import BasicTextNormalizer, EnglishTextNormalizer
+except (ImportError, SyntaxError):
+    BasicTextNormalizer = None
+
 
 class TextCleaner:
     """Text cleaner.
 
     Examples:
         >>> cleaner = TextCleaner("tacotron")
         >>> cleaner("(Hello-World);   &  jr. & dr.")
@@ -28,23 +33,33 @@
         if cleaner_types is None:
             self.cleaner_types = []
         elif isinstance(cleaner_types, str):
             self.cleaner_types = [cleaner_types]
         else:
             self.cleaner_types = list(cleaner_types)
 
+        self.whisper_cleaner = None
+        if BasicTextNormalizer is not None:
+            for t in self.cleaner_types:
+                if t == "whisper_en":
+                    self.whisper_cleaner = EnglishTextNormalizer()
+                elif t == "whisper_basic":
+                    self.whisper_cleaner = BasicTextNormalizer()
+
     def __call__(self, text: str) -> str:
         for t in self.cleaner_types:
             if t == "tacotron":
                 text = tacotron_cleaner.cleaners.custom_english_cleaners(text)
             elif t == "jaconv":
                 text = jaconv.normalize(text)
             elif t == "vietnamese":
                 if vietnamese_cleaners is None:
                     raise RuntimeError("Please install underthesea")
                 text = vietnamese_cleaners.vietnamese_cleaner(text)
             elif t == "korean_cleaner":
                 text = KoreanCleaner.normalize_text(text)
+            elif "whisper" in t and self.whisper_cleaner is not None:
+                text = self.whisper_cleaner(text)
             else:
                 raise RuntimeError(f"Not supported: type={t}")
 
         return text
```

### Comparing `espnet-202211/espnet2/text/hugging_face_tokenizer.py` & `espnet-202301/espnet2/text/hugging_face_tokenizer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/text/korean_cleaner.py` & `espnet-202301/espnet2/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/text/phoneme_tokenizer.py` & `espnet-202301/espnet2/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/text/sentencepiece_tokenizer.py` & `espnet-202301/espnet2/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/text/token_id_converter.py` & `espnet-202301/espnet2/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/text/word_tokenizer.py` & `espnet-202301/espnet2/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/torch_utils/add_gradient_noise.py` & `espnet-202301/espnet2/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/torch_utils/device_funcs.py` & `espnet-202301/espnet2/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/torch_utils/forward_adaptor.py` & `espnet-202301/espnet2/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/torch_utils/get_layer_from_string.py` & `espnet-202301/espnet2/torch_utils/get_layer_from_string.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/torch_utils/initialize.py` & `espnet-202301/espnet2/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/torch_utils/load_pretrained_model.py` & `espnet-202301/espnet2/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/torch_utils/model_summary.py` & `espnet-202301/espnet2/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/torch_utils/recursive_op.py` & `espnet-202301/espnet2/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/train/abs_espnet_model.py` & `espnet-202301/espnet2/train/abs_espnet_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/train/abs_gan_espnet_model.py` & `espnet-202301/espnet2/train/abs_gan_espnet_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/train/class_choices.py` & `espnet-202301/espnet2/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/train/dataset.py` & `espnet-202301/espnet2/train/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from espnet2.fileio.npy_scp import NpyScpReader
 from espnet2.fileio.rand_gen_dataset import (
     FloatRandomGenerateDataset,
     IntRandomGenerateDataset,
 )
 from espnet2.fileio.read_text import (
+    RandomTextReader,
     load_num_sequence_text,
     read_2column_text,
     read_label,
 )
 from espnet2.fileio.rttm import RttmReader
 from espnet2.fileio.score_scp import SingingScoreReader
 from espnet2.fileio.sound_scp import SoundScpReader
@@ -292,14 +293,24 @@
         help="Return text as is. The text must be converted to ndarray "
         "by 'preprocess'."
         "\n\n"
         "   utterance_id_A hello world\n"
         "   utterance_id_B foo bar\n"
         "   ...",
     ),
+    "random_text": dict(
+        func=RandomTextReader,
+        kwargs=[],
+        help="Return text as is. The text must be converted to ndarray "
+        "by 'preprocess'."
+        "\n\n"
+        "   hello world\n"
+        "   foo bar\n"
+        "   ...",
+    ),
     "hdf5": dict(
         func=H5FileWrapper,
         kwargs=[],
         help="A HDF5 file which contains arrays at the first level or the second level."
         "   >>> f = h5py.File('file.h5')\n"
         "   >>> array1 = f['utterance_id_A']\n"
         "   >>> array2 = f['utterance_id_B']\n",
```

### Comparing `espnet-202211/espnet2/train/distributed_utils.py` & `espnet-202301/espnet2/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/train/gan_trainer.py` & `espnet-202301/espnet2/train/gan_trainer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/train/iterable_dataset.py` & `espnet-202301/espnet2/train/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/train/preprocessor.py` & `espnet-202301/espnet2/train/preprocessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+import json
 import logging
 import random
+import re
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Collection, Dict, Iterable, List, Union
 
 import numpy as np
 import scipy.signal
 import soundfile
 from typeguard import check_argument_types, check_return_type
 
 from espnet2.text.build_tokenizer import build_tokenizer
 from espnet2.text.cleaner import TextCleaner
 from espnet2.text.token_id_converter import TokenIDConverter
+from espnet2.text.whisper_token_id_converter import OpenAIWhisperTokenIDConverter
 
 
 class AbsPreprocessor(ABC):
     def __init__(self, train: bool):
         self.train = train
 
     @abstractmethod
@@ -135,45 +138,52 @@
         delimiter: str = None,
         rir_scp: str = None,
         rir_apply_prob: float = 1.0,
         noise_scp: str = None,
         noise_apply_prob: float = 1.0,
         noise_db_range: str = "3_10",
         short_noise_thres: float = 0.5,
+        aux_task_names: Collection[str] = None,
         speech_volume_normalize: float = None,
         speech_name: str = "speech",
         text_name: str = "text",
         fs: int = 0,
     ):
         super().__init__(train)
         self.train = train
         self.speech_name = speech_name
         self.text_name = text_name
         self.speech_volume_normalize = speech_volume_normalize
         self.rir_apply_prob = rir_apply_prob
         self.noise_apply_prob = noise_apply_prob
         self.short_noise_thres = short_noise_thres
+        self.aux_task_names = aux_task_names
 
         if token_type is not None:
             if token_list is None:
                 raise ValueError("token_list is required if token_type is not None")
             self.text_cleaner = TextCleaner(text_cleaner)
 
             self.tokenizer = build_tokenizer(
                 token_type=token_type,
                 bpemodel=bpemodel,
                 delimiter=delimiter,
                 space_symbol=space_symbol,
                 non_linguistic_symbols=non_linguistic_symbols,
                 g2p_type=g2p_type,
             )
-            self.token_id_converter = TokenIDConverter(
-                token_list=token_list,
-                unk_symbol=unk_symbol,
-            )
+            if bpemodel not in ["whisper_en", "whisper_multilingual"]:
+                self.token_id_converter = TokenIDConverter(
+                    token_list=token_list,
+                    unk_symbol=unk_symbol,
+                )
+            else:
+                self.token_id_converter = OpenAIWhisperTokenIDConverter(
+                    model_type=bpemodel
+                )
         else:
             self.text_cleaner = None
             self.tokenizer = None
             self.token_id_converter = None
 
         if train and rir_scp is not None:
             self.rirs = []
@@ -194,15 +204,15 @@
                     sps = line.strip().split(None, 1)
                     if len(sps) == 1:
                         self.noises.append(sps[0])
                     else:
                         self.noises.append(sps[1])
             sps = noise_db_range.split("_")
             if len(sps) == 1:
-                self.noise_db_low, self.noise_db_high = float(sps[0])
+                self.noise_db_low = self.noise_db_high = float(sps[0])
             elif len(sps) == 2:
                 self.noise_db_low, self.noise_db_high = float(sps[0]), float(sps[1])
             else:
                 raise ValueError(
                     "Format error: '{noise_db_range}' e.g. -3_4 -> [-3db,4db]"
                 )
         else:
@@ -311,18 +321,28 @@
         return data
 
     def _text_process(
         self, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, np.ndarray]:
         if self.text_name in data and self.tokenizer is not None:
             text = data[self.text_name]
+            if isinstance(text, np.ndarray):
+                return data
             text = self.text_cleaner(text)
             tokens = self.tokenizer.text2tokens(text)
             text_ints = self.token_id_converter.tokens2ids(tokens)
             data[self.text_name] = np.array(text_ints, dtype=np.int64)
+        if self.aux_task_names is not None and self.tokenizer is not None:
+            for name in self.aux_task_names:
+                if name in data:
+                    text = data[name]
+                    text = self.text_cleaner(text)
+                    tokens = self.tokenizer.text2tokens(text)
+                    text_ints = self.token_id_converter.tokens2ids(tokens)
+                    data[name] = np.array(text_ints, dtype=np.int64)
         assert check_return_type(data)
         return data
 
     def __call__(
         self, uid: str, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, np.ndarray]:
         assert check_argument_types()
@@ -429,14 +449,15 @@
         delimiter: str = None,
         rir_scp: str = None,
         rir_apply_prob: float = 1.0,
         noise_scp: str = None,
         noise_apply_prob: float = 1.0,
         noise_db_range: str = "3_10",
         short_noise_thres: float = 0.5,
+        aux_task_names: Collection[str] = None,
         speech_volume_normalize: float = None,
         speech_name: str = "speech",
         text_name: List[str] = ["text"],
         fs: int = 0,
     ):
         super().__init__(
             train=train,
@@ -451,14 +472,15 @@
             delimiter=delimiter,
             rir_scp=rir_scp,
             rir_apply_prob=rir_apply_prob,
             noise_scp=noise_scp,
             noise_apply_prob=noise_apply_prob,
             noise_db_range=noise_db_range,
             short_noise_thres=short_noise_thres,
+            aux_task_names=aux_task_names,
             speech_volume_normalize=speech_volume_normalize,
             speech_name=speech_name,
             fs=fs,
         )
         if isinstance(text_name, str):
             self.text_name = [text_name]
         else:
@@ -470,14 +492,22 @@
         for text_n in self.text_name:
             if text_n in data and self.tokenizer is not None:
                 text = data[text_n]
                 text = self.text_cleaner(text)
                 tokens = self.tokenizer.text2tokens(text)
                 text_ints = self.token_id_converter.tokens2ids(tokens)
                 data[text_n] = np.array(text_ints, dtype=np.int64)
+        if self.aux_task_names is not None and self.tokenizer is not None:
+            for name in self.aux_task_names:
+                if name in data:
+                    text = data[name]
+                    text = self.text_cleaner(text)
+                    tokens = self.tokenizer.text2tokens(text)
+                    text_ints = self.token_id_converter.tokens2ids(tokens)
+                    data[name] = np.array(text_ints, dtype=np.int64)
         assert check_return_type(data)
         return data
 
     def __call__(
         self, uid: str, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, np.ndarray]:
         assert check_argument_types()
@@ -964,15 +994,15 @@
         delimiter: str = None,
         singing_volume_normalize: float = None,
         singing_name: str = "singing",
         text_name: str = "text",
         label_name: str = "label",
         midi_name: str = "score",
         fs: np.int32 = 0,
-        time_shift: np.int32 = 0.0125,
+        hop_length: np.int32 = 256,
         align: list = [
             "singing",
             "label_lab",
             "midi_lab",
             "tempo_lab",
             "beat_lab",
         ],  # TODO(Tao): add to args
@@ -986,18 +1016,19 @@
         super().__init__(train)
         self.train = train
         self.singing_name = singing_name
         self.text_name = text_name
         self.label_name = label_name
         self.midi_name = midi_name
         self.fs = fs
-        self.time_shift = time_shift
+        self.hop_length = hop_length
         self.singing_volume_normalize = singing_volume_normalize
         self.align = align
         self.phn_seg = phn_seg
+        self.time_shift = hop_length / fs
         if token_type is not None:
             if token_list is None:
                 raise ValueError("token_list is required if token_type is not None")
             self.text_cleaner = TextCleaner(text_cleaner)
 
             self.tokenizer = build_tokenizer(
                 token_type=token_type,
@@ -1171,7 +1202,172 @@
         # align frame length with singing
         length = min([len(data[key]) for key in data.keys() if key in self.align])
         for key in self.align:
             if key in data:
                 data[key] = data[key][:length]
 
         return data
+
+
+class TSEPreprocessor(EnhPreprocessor):
+    """Preprocessor for Target Speaker Extraction."""
+
+    def __init__(
+        self,
+        train: bool,
+        train_spk2enroll: str = None,
+        enroll_segment: int = None,
+        load_spk_embedding: bool = False,
+        load_all_speakers: bool = False,
+        # inherited from EnhPreprocessor
+        rir_scp: str = None,
+        rir_apply_prob: float = 1.0,
+        noise_scp: str = None,
+        noise_apply_prob: float = 1.0,
+        noise_db_range: str = "3_10",
+        short_noise_thres: float = 0.5,
+        speech_volume_normalize: float = None,
+        speech_name: str = "speech_mix",
+        speech_ref_name_prefix: str = "speech_ref",
+        noise_ref_name_prefix: str = "noise_ref",
+        dereverb_ref_name_prefix: str = "dereverb_ref",
+        use_reverberant_ref: bool = False,
+        num_spk: int = 1,
+        num_noise_type: int = 1,
+        sample_rate: int = 8000,
+        force_single_channel: bool = False,
+    ):
+        super().__init__(
+            train,
+            rir_scp=rir_scp,
+            rir_apply_prob=rir_apply_prob,
+            noise_scp=noise_scp,
+            noise_apply_prob=noise_apply_prob,
+            noise_db_range=noise_db_range,
+            short_noise_thres=short_noise_thres,
+            speech_volume_normalize=speech_volume_normalize,
+            speech_name=speech_name,
+            speech_ref_name_prefix=speech_ref_name_prefix,
+            noise_ref_name_prefix=noise_ref_name_prefix,
+            dereverb_ref_name_prefix=dereverb_ref_name_prefix,
+            use_reverberant_ref=use_reverberant_ref,
+            num_spk=num_spk,
+            num_noise_type=num_noise_type,
+            sample_rate=sample_rate,
+            force_single_channel=force_single_channel,
+        )
+        # If specified, the enrollment will be chomped to the specified length
+        self.enroll_segment = enroll_segment
+        # If True, the speaker embedding will be loaded instead of enrollment audios
+        self.load_spk_embedding = load_spk_embedding
+        # If False, only one of the speakers in each mixture sample will be loaded
+        self.load_all_speakers = load_all_speakers
+
+        if train:
+            if train_spk2enroll is None:
+                logging.info("Using fixed enrollment for each sample")
+                self.train_spk2enroll = None
+            else:
+                logging.info("Using dynamically sampled enrollment for each sample")
+                with open(train_spk2enroll, "r", encoding="utf-8") as f:
+                    # {spkID: [(uid1, path1), (uid2, path2), ...]}
+                    self.train_spk2enroll = json.load(f)
+        else:
+            self.train_spk2enroll = None
+
+    def _read_audio_segment(self, path, seg_len=None):
+        with soundfile.SoundFile(path) as f:
+            if seg_len is None or f.frames == seg_len:
+                audio = f.read(dtype=np.float32, always_2d=True)
+            elif f.frames < seg_len:
+                offset = np.random.randint(0, seg_len - f.frames)
+                # audio: (Time, Nmic)
+                audio = f.read(dtype=np.float32, always_2d=True)
+                # Repeat audio
+                audio = np.pad(
+                    audio,
+                    [(offset, seg_len - f.frames - offset), (0, 0)],
+                    mode="wrap",
+                )
+            else:
+                offset = np.random.randint(0, f.frames - seg_len)
+                f.seek(offset)
+                # audio: (Time, Nmic)
+                audio = f.read(seg_len, dtype=np.float32, always_2d=True)
+            if len(audio) != seg_len:
+                raise RuntimeError(f"Something wrong: {path}")
+        return audio[:, 0]
+
+    def _speech_process(
+        self, uid: str, data: Dict[str, Union[str, np.ndarray]]
+    ) -> Dict[str, Union[str, np.ndarray]]:
+        assert check_argument_types()
+
+        ref_names = [k for k in data.keys() if re.match(r"speech_ref\d+", k)]
+        num_spk = len(ref_names)
+
+        aux_names = [k for k in data.keys() if re.match(r"enroll_ref\d+", k)]
+        if self.train:
+            assert len(ref_names) == len(aux_names), (len(ref_names), len(aux_names))
+            if not self.load_all_speakers:
+                # only load one target-speaker data
+                spk = np.random.randint(0, num_spk)
+                for i, name in enumerate(ref_names):
+                    if i == 0:
+                        data[name] = data[ref_names[spk]]
+                    else:
+                        data.pop(name)
+                        continue
+
+            for i, name in enumerate(aux_names):
+                if not self.load_all_speakers:
+                    if i == 0:
+                        data[name] = data[aux_names[spk]]
+                    else:
+                        data.pop(name)
+                        continue
+                if self.train_spk2enroll is None:
+                    # normal format in `enroll_spk?.scp`:
+                    # MIXTURE_UID /path/to/enrollment_or_embedding
+                    aux_audio = data[name]
+                else:
+                    # a special format in `enroll_spk?.scp`:
+                    # MIXTURE_UID *UID SPEAKER_ID
+                    assert data[name].startswith("*"), data[name]
+                    cur_uid, spkid = data[name][1:].strip().split(maxsplit=1)
+                    aux_uid, aux_audio = random.choice(self.train_spk2enroll[spkid])
+                    while aux_uid == cur_uid:
+                        aux_uid, aux_audio = random.choice(self.train_spk2enroll[spkid])
+                if getattr(self, "load_spk_embedding", False):
+                    data[name] = np.load(aux_audio)[None, :]  # force 2D
+                elif self.enroll_segment:
+                    data[name] = self._read_audio_segment(
+                        aux_audio, self.enroll_segment
+                    )
+                else:
+                    data[name] = soundfile.read(aux_audio)[0]
+        else:
+            for name in aux_names:
+                if data[name].startswith("*"):
+                    # in case of collecting stats for training data
+                    data[name] = np.zeros(1, dtype=data["speech_mix"].dtype)
+                else:
+                    if getattr(self, "load_spk_embedding", False):
+                        data[name] = np.load(data[name])[None, :]  # force 2D
+                    elif self.enroll_segment:
+                        data[name] = self._read_audio_segment(
+                            data[name], self.enroll_segment
+                        )
+                    else:
+                        data[name] = soundfile.read(data[name])[0]
+
+        assert check_return_type(data)
+        return data
+
+    def __call__(
+        self, uid: str, data: Dict[str, Union[str, np.ndarray]]
+    ) -> Dict[str, np.ndarray]:
+        assert check_argument_types()
+
+        data = super()._speech_process(data)
+        data = self._speech_process(uid, data)
+        return data
```

### Comparing `espnet-202211/espnet2/train/reporter.py` & `espnet-202301/espnet2/train/reporter.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/train/trainer.py` & `espnet-202301/espnet2/train/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,24 @@
 from espnet2.train.reporter import Reporter, SubReporter
 from espnet2.utils.build_dataclass import build_dataclass
 from espnet2.utils.kwargs2args import kwargs2args
 
 if torch.distributed.is_available():
     from torch.distributed import ReduceOp
 
+autocast_args = dict()
 if V(torch.__version__) >= V("1.6.0"):
     from torch.cuda.amp import GradScaler, autocast
+
+    if (
+        V(torch.__version__) >= V("1.10.0")
+        and torch.cuda.is_available()
+        and torch.cuda.is_bf16_supported()
+    ):
+        autocast_args = dict(dtype=torch.bfloat16)
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
     GradScaler = None
@@ -547,15 +555,18 @@
                             del _args
                     else:
                         logging.warning(
                             "model.module is not found (This should be a bug.)"
                         )
                 del _model
 
-            with autocast(scaler is not None):
+            with autocast(
+                scaler is not None,
+                **autocast_args,
+            ):
                 with reporter.measure_time("forward_time"):
                     retval = model(**batch)
 
                     # Note(kamo):
                     # Supporting two patterns for the returned value from the model
                     #   a. dict type
                     if isinstance(retval, dict):
```

### Comparing `espnet-202211/espnet2/tts/abs_tts.py` & `espnet-202301/espnet2/tts/abs_tts.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/espnet_model.py` & `espnet-202301/espnet2/tts/espnet_model.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/fastspeech/fastspeech.py` & `espnet-202301/espnet2/tts/fastspeech/fastspeech.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/fastspeech2/fastspeech2.py` & `espnet-202301/espnet2/tts/fastspeech2/fastspeech2.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/fastspeech2/loss.py` & `espnet-202301/espnet2/tts/fastspeech2/loss.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/fastspeech2/variance_predictor.py` & `espnet-202301/espnet2/tts/fastspeech2/variance_predictor.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/feats_extract/dio.py` & `espnet-202301/espnet2/tts/feats_extract/dio.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/feats_extract/energy.py` & `espnet-202301/espnet2/tts/feats_extract/energy.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/feats_extract/linear_spectrogram.py` & `espnet-202301/espnet2/tts/feats_extract/linear_spectrogram.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/feats_extract/log_mel_fbank.py` & `espnet-202301/espnet2/tts/feats_extract/log_mel_fbank.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/feats_extract/log_spectrogram.py` & `espnet-202301/espnet2/tts/feats_extract/log_spectrogram.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/gst/style_encoder.py` & `espnet-202301/espnet2/tts/gst/style_encoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/tacotron2/tacotron2.py` & `espnet-202301/espnet2/tts/tacotron2/tacotron2.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/transformer/transformer.py` & `espnet-202301/espnet2/tts/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/utils/duration_calculator.py` & `espnet-202301/espnet2/tts/utils/duration_calculator.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/tts/utils/parallel_wavegan_pretrained_vocoder.py` & `espnet-202301/espnet2/tts/utils/parallel_wavegan_pretrained_vocoder.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/utils/build_dataclass.py` & `espnet-202301/espnet2/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/utils/config_argparse.py` & `espnet-202301/espnet2/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/utils/get_default_kwargs.py` & `espnet-202301/espnet2/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/utils/griffin_lim.py` & `espnet-202301/espnet2/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/utils/nested_dict_action.py` & `espnet-202301/espnet2/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/utils/sized_dict.py` & `espnet-202301/espnet2/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/espnet2/utils/types.py` & `espnet-202301/espnet2/utils/types.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/setup.py` & `espnet-202301/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,25 +23,29 @@
         "kaldiio>=2.17.0",
         "torch>=1.3.0",
         "torch_complex",
         "nltk>=3.4.5",
         "numpy",
         # https://github.com/espnet/espnet/runs/6646737793?check_suite_focus=true#step:8:7651
         "protobuf<=3.20.1",
+        "hydra-core",
+        "opt-einsum",
         # ASR
         "sentencepiece",
         "ctc-segmentation>=1.6.6",
         # TTS
         "pyworld>=0.2.10",
         "pypinyin<=0.44.0",
         "espnet_tts_frontend",
         # ENH
         "ci_sdr",
         "pytorch_wpe",
         "fast-bss-eval==0.1.3",
+        # UASR
+        "editdistance",
         # fix CI error due to the use of deprecated functions
         # https://github.com/espnet/espnet/actions/runs/3174416926/jobs/5171182884#step:8:8419
         # https://importlib-metadata.readthedocs.io/en/latest/history.html#v5-0-0
         "importlib-metadata<5.0",
     ],
     # train: The modules invoked when training only.
     "train": [
@@ -63,14 +67,16 @@
         "nnmnkwii",
         "museval>=0.2.1",
         "pystoi>=0.2.2",
         "mir-eval>=0.6",
         "fastdtw",
         "nara_wpe>=0.0.5",
         "sacrebleu>=1.5.1",
+        "praatio>=5.1.1",  # for librispeech phoneme alignment
+        "scikit-learn>=1.0.0",  # for HuBERT kmeans
     ],
     # all: The modules should be optionally installled due to some reason.
     #      Please consider moving them to "install" occasionally
     # NOTE(kamo): The modules in "train" and "recipe" are appended into "all"
     "all": [
         # NOTE(kamo): Append modules requiring specific pytorch version or torch>1.3.0
         "torchaudio",
```

### Comparing `espnet-202211/test/test_asr_init.py` & `espnet-202301/test/test_asr_init.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_asr_quantize.py` & `espnet-202301/test/test_asr_quantize.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_batch_beam_search.py` & `espnet-202301/test/test_batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_beam_search.py` & `espnet-202301/test/test_beam_search.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_cli.py` & `espnet-202301/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_custom_transducer.py` & `espnet-202301/test/test_custom_transducer.py`

 * *Files 0% similar despite different names*

```diff
@@ -624,14 +624,15 @@
         {"mod": {torch.nn.Linear}, "dtype": torch.float16},
         {"mod": {torch.nn.LSTM}, "dtype": torch.qint8},
         {"mod": {torch.nn.LSTM}, "dtype": torch.float16},
         {"mod": {torch.nn.Linear, torch.nn.LSTM}, "dtype": torch.qint8},
         {"mod": {torch.nn.Linear, torch.nn.LSTM}, "dtype": torch.float16},
     ],
 )
+@pytest.mark.execution_timeout(4)
 def test_dynamic_quantization(train_dic, recog_dic, quantize_dic):
     train_args = make_train_args(**train_dic)
     recog_args = make_recog_args(**recog_dic)
 
     model, feats, feats_len, _, _, _ = prepare(train_args)
 
     if not is_torch_1_5_plus and (
```

### Comparing `espnet-202211/test/test_distributed_launch.py` & `espnet-202301/test/test_distributed_launch.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_asr.py` & `espnet-202301/test/test_e2e_asr.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_asr_conformer.py` & `espnet-202301/test/test_e2e_asr_conformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_asr_maskctc.py` & `espnet-202301/test/test_e2e_asr_maskctc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_asr_mulenc.py` & `espnet-202301/test/test_e2e_asr_mulenc.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_asr_transducer.py` & `espnet-202301/test/test_e2e_asr_transducer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_asr_transformer.py` & `espnet-202301/test/test_e2e_asr_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_compatibility.py` & `espnet-202301/test/test_e2e_compatibility.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_mt.py` & `espnet-202301/test/test_e2e_mt.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_mt_transformer.py` & `espnet-202301/test/test_e2e_mt_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_st.py` & `espnet-202301/test/test_e2e_st.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_st_conformer.py` & `espnet-202301/test/test_e2e_st_conformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_st_transformer.py` & `espnet-202301/test/test_e2e_st_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_tts_fastspeech.py` & `espnet-202301/test/test_e2e_tts_fastspeech.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_tts_tacotron2.py` & `espnet-202301/test/test_e2e_tts_tacotron2.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_tts_transformer.py` & `espnet-202301/test/test_e2e_tts_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_vc_tacotron2.py` & `espnet-202301/test/test_e2e_vc_tacotron2.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_e2e_vc_transformer.py` & `espnet-202301/test/test_e2e_vc_transformer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_initialization.py` & `espnet-202301/test/test_initialization.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_io_voxforge.py` & `espnet-202301/test/test_io_voxforge.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_lm.py` & `espnet-202301/test/test_lm.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_loss.py` & `espnet-202301/test/test_loss.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_multi_spkrs.py` & `espnet-202301/test/test_multi_spkrs.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_optimizer.py` & `espnet-202301/test/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_positional_encoding.py` & `espnet-202301/test/test_positional_encoding.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_recog.py` & `espnet-202301/test/test_recog.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_scheduler.py` & `espnet-202301/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_sentencepiece.py` & `espnet-202301/test/test_sentencepiece.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_tensorboard.py` & `espnet-202301/test/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_torch.py` & `espnet-202301/test/test_torch.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_train_dtype.py` & `espnet-202301/test/test_train_dtype.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_transform.py` & `espnet-202301/test/test_transform.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_transformer_decode.py` & `espnet-202301/test/test_transformer_decode.py`

 * *Files identical despite different names*

### Comparing `espnet-202211/test/test_utils.py` & `espnet-202301/test/test_utils.py`

 * *Files identical despite different names*

