# Comparing `tmp/ondewo-s2t-client-5.2.0.tar.gz` & `tmp/ondewo-s2t-client-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-s2t-client-5.2.0.tar", last modified: Tue Jan 24 17:42:32 2023, max compression
+gzip compressed data, was "ondewo-s2t-client-5.3.0.tar", last modified: Mon May  1 18:24:42 2023, max compression
```

## Comparing `ondewo-s2t-client-5.2.0.tar` & `ondewo-s2t-client-5.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 17:42:32.480737 ondewo-s2t-client-5.2.0/
--rw-r--r--   0 root         (0) root         (0)     6574 2023-01-24 17:42:32.480737 ondewo-s2t-client-5.2.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6020 2023-01-24 17:42:11.000000 ondewo-s2t-client-5.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 17:42:32.479737 ondewo-s2t-client-5.2.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2023-01-24 17:42:11.000000 ondewo-s2t-client-5.2.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 17:42:32.479737 ondewo-s2t-client-5.2.0/ondewo/s2t/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 17:42:11.000000 ondewo-s2t-client-5.2.0/ondewo/s2t/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 17:42:32.480737 ondewo-s2t-client-5.2.0/ondewo/s2t/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 17:42:11.000000 ondewo-s2t-client-5.2.0/ondewo/s2t/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      756 2023-01-24 17:42:11.000000 ondewo-s2t-client-5.2.0/ondewo/s2t/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      262 2023-01-24 17:42:11.000000 ondewo-s2t-client-5.2.0/ondewo/s2t/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 17:42:32.480737 ondewo-s2t-client-5.2.0/ondewo/s2t/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 17:42:11.000000 ondewo-s2t-client-5.2.0/ondewo/s2t/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3514 2023-01-24 17:42:11.000000 ondewo-s2t-client-5.2.0/ondewo/s2t/client/services/speech_to_text.py
--rw-rw-r--   0 root         (0) root         (0)      265 2023-01-24 17:42:11.000000 ondewo-s2t-client-5.2.0/ondewo/s2t/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    35895 2023-01-24 17:42:16.000000 ondewo-s2t-client-5.2.0/ondewo/s2t/speech_to_text_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    27764 2023-01-24 17:42:16.000000 ondewo-s2t-client-5.2.0/ondewo/s2t/speech_to_text_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 17:42:32.480737 ondewo-s2t-client-5.2.0/ondewo_s2t_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6574 2023-01-24 17:42:32.000000 ondewo-s2t-client-5.2.0/ondewo_s2t_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      562 2023-01-24 17:42:32.000000 ondewo-s2t-client-5.2.0/ondewo_s2t_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-24 17:42:32.000000 ondewo-s2t-client-5.2.0/ondewo_s2t_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-01-24 17:42:32.000000 ondewo-s2t-client-5.2.0/ondewo_s2t_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-01-24 17:42:32.000000 ondewo-s2t-client-5.2.0/ondewo_s2t_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2023-01-24 17:42:32.480737 ondewo-s2t-client-5.2.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      946 2023-01-24 17:42:20.000000 ondewo-s2t-client-5.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:24:42.564346 ondewo-s2t-client-5.3.0/
+-rw-r--r--   0 root         (0) root         (0)     6574 2023-05-01 18:24:42.564346 ondewo-s2t-client-5.3.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6020 2023-05-01 18:24:18.000000 ondewo-s2t-client-5.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:24:42.563346 ondewo-s2t-client-5.3.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-05-01 18:24:18.000000 ondewo-s2t-client-5.3.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:24:42.563346 ondewo-s2t-client-5.3.0/ondewo/s2t/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-01 18:24:18.000000 ondewo-s2t-client-5.3.0/ondewo/s2t/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:24:42.563346 ondewo-s2t-client-5.3.0/ondewo/s2t/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-01 18:24:18.000000 ondewo-s2t-client-5.3.0/ondewo/s2t/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      756 2023-05-01 18:24:18.000000 ondewo-s2t-client-5.3.0/ondewo/s2t/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      262 2023-05-01 18:24:18.000000 ondewo-s2t-client-5.3.0/ondewo/s2t/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:24:42.563346 ondewo-s2t-client-5.3.0/ondewo/s2t/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-01 18:24:18.000000 ondewo-s2t-client-5.3.0/ondewo/s2t/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3514 2023-05-01 18:24:18.000000 ondewo-s2t-client-5.3.0/ondewo/s2t/client/services/speech_to_text.py
+-rw-rw-r--   0 root         (0) root         (0)      265 2023-05-01 18:24:18.000000 ondewo-s2t-client-5.3.0/ondewo/s2t/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    36634 2023-05-01 18:24:27.000000 ondewo-s2t-client-5.3.0/ondewo/s2t/speech_to_text_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    27703 2023-05-01 18:24:27.000000 ondewo-s2t-client-5.3.0/ondewo/s2t/speech_to_text_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:24:42.564346 ondewo-s2t-client-5.3.0/ondewo_s2t_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6574 2023-05-01 18:24:42.000000 ondewo-s2t-client-5.3.0/ondewo_s2t_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      562 2023-05-01 18:24:42.000000 ondewo-s2t-client-5.3.0/ondewo_s2t_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 18:24:42.000000 ondewo-s2t-client-5.3.0/ondewo_s2t_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-01 18:24:42.000000 ondewo-s2t-client-5.3.0/ondewo_s2t_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-01 18:24:42.000000 ondewo-s2t-client-5.3.0/ondewo_s2t_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-05-01 18:24:42.564346 ondewo-s2t-client-5.3.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1094 2023-05-01 18:24:31.000000 ondewo-s2t-client-5.3.0/setup.py
```

### Comparing `ondewo-s2t-client-5.2.0/PKG-INFO` & `ondewo-s2t-client-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-s2t-client
-Version: 5.2.0
+Version: 5.3.0
 Summary: exposes the ondewo-s2t-grpc-server endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-s2t-client-python
 Author: ONDEWO GbmH
 Author-email: info@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-s2t-client Version: 5.2.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-s2t-client Version: 5.3.0 Summary: exposes
 the ondewo-s2t-grpc-server endpoints in a user-friendly way Home-page: https://
 github.com/ondewo/ondewo-s2t-client-python Author: ONDEWO GbmH Author-email:
 info@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha Classifier: Topic :: Software
 Development :: Libraries Requires-Python: >=2.7, !=3.0.1 Description-Content-
 Type: text/markdown
```

### Comparing `ondewo-s2t-client-5.2.0/README.md` & `ondewo-s2t-client-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-s2t-client-5.2.0/ondewo/s2t/client/client.py` & `ondewo-s2t-client-5.3.0/ondewo/s2t/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-s2t-client-5.2.0/ondewo/s2t/client/services/speech_to_text.py` & `ondewo-s2t-client-5.3.0/ondewo/s2t/client/services/speech_to_text.py`

 * *Files identical despite different names*

### Comparing `ondewo-s2t-client-5.2.0/ondewo/s2t/speech_to_text_pb2.py` & `ondewo-s2t-client-5.3.0/ondewo/s2t/speech_to_text_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,23 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fondewo/s2t/speech-to-text.proto\x12\nondewo.s2t\x1a\x1bgoogle/protobuf/empty.proto\"\x9a\x04\n\x17TranscribeRequestConfig\x12\x17\n\x0fs2t_pipeline_id\x18\x01 \x01(\t\x12&\n\x08\x64\x65\x63oding\x18\x02 \x01(\x0e\x32\x14.ondewo.s2t.Decoding\x12\x1d\n\x13language_model_name\x18\x03 \x01(\tH\x00\x12<\n\x0fpost_processing\x18\x04 \x01(\x0b\x32!.ondewo.s2t.PostProcessingOptionsH\x01\x12\x44\n\x13utterance_detection\x18\x05 \x01(\x0b\x32%.ondewo.s2t.UtteranceDetectionOptionsH\x02\x12(\n\x08pyannote\x18\x06 \x01(\x0b\x32\x14.ondewo.s2t.PyannoteH\x03\x12(\n\x08matchbox\x18\x07 \x01(\x0b\x32\x14.ondewo.s2t.MatchboxH\x03\x12@\n\x0ereturn_options\x18\x08 \x01(\x0b\x32&.ondewo.s2t.TranscriptionReturnOptionsH\x04\x42\x1b\n\x19oneof_language_model_nameB\x17\n\x15oneof_post_processingB\x1b\n\x19oneof_utterance_detectionB\x1a\n\x18voice_activity_detectionB\x16\n\x14oneof_return_options\"\xba\x01\n\x1aTranscriptionReturnOptions\x12\x1e\n\x16return_start_of_speech\x18\x01 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x02 \x01(\x08\x12)\n!return_alternative_transcriptions\x18\x03 \x01(\x08\x12\x1f\n\x17return_confidence_score\x18\x04 \x01(\x08\x12\x1a\n\x12return_word_timing\x18\x08 \x01(\x08\"\xbf\x01\n\x19UtteranceDetectionOptions\x12\x1e\n\x14transcribe_not_final\x18\x01 \x01(\x08H\x00\x12$\n\x1cstart_of_utterance_threshold\x18\x02 \x01(\x02\x12\"\n\x1a\x65nd_of_utterance_threshold\x18\x03 \x01(\x02\x12\x1a\n\x12next_chunk_timeout\x18\x04 \x01(\x02\x42\x1c\n\x1aoneof_transcribe_not_final\"s\n\x15PostProcessingOptions\x12\x1b\n\x13spelling_correction\x18\x01 \x01(\x08\x12\x11\n\tnormalize\x18\x02 \x01(\x08\x12*\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\"\x8e\x01\n\x17TranscribeStreamRequest\x12\x13\n\x0b\x61udio_chunk\x18\x01 \x01(\x0c\x12\x15\n\rend_of_stream\x18\x02 \x01(\x08\x12\x33\n\x06\x63onfig\x18\x03 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\x12\x12\n\nmute_audio\x18\x04 \x01(\x08\"@\n\rTranscription\x12\x15\n\rtranscription\x18\x01 \x01(\t\x12\x18\n\x10\x63onfidence_score\x18\x02 \x01(\x02\"\x83\x02\n\x18TranscribeStreamResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12\r\n\x05\x66inal\x18\x03 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x04 \x01(\x08\x12\r\n\x05\x61udio\x18\x05 \x01(\x0c\x12\x17\n\x0futterance_start\x18\x06 \x01(\x08\x12\x12\n\naudio_uuid\x18\x07 \x01(\t\x12\x35\n\x06\x63onfig\x18\x08 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfigH\x00\x42\x0e\n\x0coneof_config\"`\n\x15TranscribeFileRequest\x12\x12\n\naudio_file\x18\x01 \x01(\x0c\x12\x33\n\x06\x63onfig\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\"\x9a\x01\n\x16TranscribeFileResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12+\n\x0bword_timing\x18\x03 \x03(\x0b\x32\x16.ondewo.s2t.WordTiming\x12\x12\n\naudio_uuid\x18\x04 \x01(\t\"6\n\nWordTiming\x12\x0c\n\x04word\x18\x01 \x01(\t\x12\r\n\x05\x62\x65gin\x18\x02 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x05\"\x1b\n\rS2tPipelineId\x12\n\n\x02id\x18\x01 \x01(\t\"o\n\x17ListS2tPipelinesRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x0f\n\x07\x64omains\x18\x03 \x03(\t\x12\x17\n\x0fregistered_only\x18\x04 \x01(\x08\"S\n\x18ListS2tPipelinesResponse\x12\x37\n\x10pipeline_configs\x18\x01 \x03(\x0b\x32\x1d.ondewo.s2t.Speech2TextConfig\"C\n\x17ListS2tLanguagesRequest\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\"-\n\x18ListS2tLanguagesResponse\x12\x11\n\tlanguages\x18\x01 \x03(\t\"C\n\x15ListS2tDomainsRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\")\n\x16ListS2tDomainsResponse\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\",\n\x19S2TGetServiceInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"\xe5\x02\n\x11Speech2TextConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12/\n\x0b\x64\x65scription\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.S2TDescription\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\x12+\n\tinference\x18\x04 \x01(\x0b\x32\x18.ondewo.s2t.S2TInference\x12\x35\n\x10streaming_server\x18\x05 \x01(\x0b\x32\x1b.ondewo.s2t.StreamingServer\x12\x44\n\x18voice_activity_detection\x18\x06 \x01(\x0b\x32\".ondewo.s2t.VoiceActivityDetection\x12\x33\n\x0fpost_processing\x18\x07 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\x12$\n\x07logging\x18\x08 \x01(\x0b\x32\x13.ondewo.s2t.Logging\"\\\n\x0eS2TDescription\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x16\n\x0epipeline_owner\x18\x02 \x01(\t\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x10\n\x08\x63omments\x18\x04 \x01(\t\"x\n\x0cS2TInference\x12\x33\n\x0f\x61\x63oustic_models\x18\x01 \x01(\x0b\x32\x1a.ondewo.s2t.AcousticModels\x12\x33\n\x0flanguage_models\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.LanguageModels\"\xb1\x02\n\x0e\x41\x63ousticModels\x12\x0c\n\x04type\x18\x01 \x01(\t\x12(\n\tquartznet\x18\x02 \x01(\x0b\x32\x15.ondewo.s2t.Quartznet\x12\x35\n\x10quartznet_triton\x18\x03 \x01(\x0b\x32\x1b.ondewo.s2t.QuartznetTriton\x12$\n\x07wav2vec\x18\x04 \x01(\x0b\x32\x13.ondewo.s2t.Wav2Vec\x12\x31\n\x0ewav2vec_triton\x18\x05 \x01(\x0b\x32\x19.ondewo.s2t.Wav2VecTriton\x12$\n\x07whisper\x18\x06 \x01(\x0b\x32\x13.ondewo.s2t.Whisper\x12\x31\n\x0ewhisper_triton\x18\x07 \x01(\x0b\x32\x19.ondewo.s2t.WhisperTriton\"@\n\x07Whisper\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\x12\x10\n\x08language\x18\x03 \x01(\t\"~\n\rWhisperTriton\x12\x16\n\x0eprocessor_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1c\n\x14triton_model_version\x18\x03 \x01(\t\x12\x1c\n\x14\x63heck_status_timeout\x18\x04 \x01(\x03\".\n\x07Wav2Vec\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\"~\n\rWav2VecTriton\x12\x16\n\x0eprocessor_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1c\n\x14triton_model_version\x18\x03 \x01(\t\x12\x1c\n\x14\x63heck_status_timeout\x18\x04 \x01(\x03\"\x94\x01\n\tQuartznet\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x11\n\tload_type\x18\x02 \x01(\t\x12%\n\x08pt_files\x18\x03 \x01(\x0b\x32\x13.ondewo.s2t.PtFiles\x12\'\n\tckpt_file\x18\x04 \x01(\x0b\x32\x14.ondewo.s2t.CkptFile\x12\x0f\n\x07use_gpu\x18\x05 \x01(\x08\"%\n\x07PtFiles\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0c\n\x04step\x18\x02 \x01(\t\"\x18\n\x08\x43kptFile\x12\x0c\n\x04path\x18\x01 \x01(\t\"P\n\x0fQuartznetTriton\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x12\n\ntriton_url\x18\x02 \x01(\t\x12\x14\n\x0ctriton_model\x18\x03 \x01(\t\"\x88\x01\n\x0eLanguageModels\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tbeam_size\x18\x02 \x01(\x03\x12\x12\n\ndefault_lm\x18\x03 \x01(\t\x12 \n\x18\x62\x65\x61m_search_scorer_alpha\x18\x04 \x01(\x02\x12\x1f\n\x17\x62\x65\x61m_search_scorer_beta\x18\x05 \x01(\x02\"\x91\x01\n\x0fStreamingServer\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x03\x12\x14\n\x0coutput_style\x18\x03 \x01(\t\x12L\n\x1cstreaming_speech_recognition\x18\x04 \x01(\x0b\x32&.ondewo.s2t.StreamingSpeechRecognition\"\xee\x01\n\x1aStreamingSpeechRecognition\x12\x1c\n\x14transcribe_not_final\x18\x01 \x01(\x08\x12\x17\n\x0f\x64\x65\x63oding_method\x18\x02 \x01(\t\x12\x15\n\rsampling_rate\x18\x03 \x01(\x03\x12\x1c\n\x14min_audio_chunk_size\x18\x04 \x01(\x03\x12$\n\x1cstart_of_utterance_threshold\x18\x05 \x01(\x02\x12\"\n\x1a\x65nd_of_utterance_threshold\x18\x06 \x01(\x02\x12\x1a\n\x12next_chunk_timeout\x18\x07 \x01(\x02\"\x8f\x01\n\x16VoiceActivityDetection\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\t\x12\x15\n\rsampling_rate\x18\x02 \x01(\x03\x12&\n\x08pyannote\x18\x03 \x01(\x0b\x32\x14.ondewo.s2t.Pyannote\x12&\n\x08matchbox\x18\x04 \x01(\x0b\x32\x14.ondewo.s2t.Matchbox\"\xb0\x01\n\x08Pyannote\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x16\n\x0emin_audio_size\x18\x02 \x01(\x03\x12\x0e\n\x06offset\x18\x03 \x01(\x02\x12\r\n\x05onset\x18\x04 \x01(\x02\x12\x13\n\tlog_scale\x18\x05 \x01(\x08H\x00\x12\x18\n\x10min_duration_off\x18\x06 \x01(\x02\x12\x17\n\x0fmin_duration_on\x18\x07 \x01(\x02\x42\x11\n\x0foneof_log_scale\"L\n\x08Matchbox\x12\x14\n\x0cmodel_config\x18\x01 \x01(\t\x12\x14\n\x0c\x65ncoder_path\x18\x02 \x01(\t\x12\x14\n\x0c\x64\x65\x63oder_path\x18\x03 \x01(\t\"W\n\x0ePostProcessing\x12\x10\n\x08pipeline\x18\x01 \x03(\t\x12\x33\n\x0fpost_processors\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessors\"n\n\x0ePostProcessors\x12\'\n\tsym_spell\x18\x01 \x01(\x0b\x32\x14.ondewo.s2t.SymSpell\x12\x33\n\rnormalization\x18\x02 \x01(\x0b\x32\x1c.ondewo.s2t.S2TNormalization\"Z\n\x08SymSpell\x12\x11\n\tdict_path\x18\x01 \x01(\t\x12$\n\x1cmax_dictionary_edit_distance\x18\x02 \x01(\x03\x12\x15\n\rprefix_length\x18\x03 \x01(\x03\"$\n\x10S2TNormalization\x12\x10\n\x08language\x18\x01 \x01(\t\"%\n\x07Logging\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"+\n\x1cListS2tLanguageModelsRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"C\n\x17LanguageModelPipelineId\x12\x13\n\x0bpipeline_id\x18\x01 \x01(\t\x12\x13\n\x0bmodel_names\x18\x02 \x03(\t\"]\n\x1dListS2tLanguageModelsResponse\x12<\n\x0flm_pipeline_ids\x18\x01 \x03(\x0b\x32#.ondewo.s2t.LanguageModelPipelineId\"=\n\x1e\x43reateUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"=\n\x1e\x44\x65leteUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"U\n!AddDataToUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\x13\n\x0bzipped_data\x18\x02 \x01(\x0c\"K\n\x1dTrainUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\x03*M\n\x08\x44\x65\x63oding\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06GREEDY\x10\x01\x12\x17\n\x13\x42\x45\x41M_SEARCH_WITH_LM\x10\x02\x12\x0f\n\x0b\x42\x45\x41M_SEARCH\x10\x03\x32\xec\n\n\x0bSpeech2Text\x12Y\n\x0eTranscribeFile\x12!.ondewo.s2t.TranscribeFileRequest\x1a\".ondewo.s2t.TranscribeFileResponse\"\x00\x12\x63\n\x10TranscribeStream\x12#.ondewo.s2t.TranscribeStreamRequest\x1a$.ondewo.s2t.TranscribeStreamResponse\"\x00(\x01\x30\x01\x12L\n\x0eGetS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x1d.ondewo.s2t.Speech2TextConfig\"\x00\x12O\n\x11\x43reateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x19.ondewo.s2t.S2tPipelineId\"\x00\x12H\n\x11\x44\x65leteS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x11UpdateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x10ListS2tPipelines\x12#.ondewo.s2t.ListS2tPipelinesRequest\x1a$.ondewo.s2t.ListS2tPipelinesResponse\"\x00\x12_\n\x10ListS2tLanguages\x12#.ondewo.s2t.ListS2tLanguagesRequest\x1a$.ondewo.s2t.ListS2tLanguagesResponse\"\x00\x12Y\n\x0eListS2tDomains\x12!.ondewo.s2t.ListS2tDomainsRequest\x1a\".ondewo.s2t.ListS2tDomainsResponse\"\x00\x12Q\n\x0eGetServiceInfo\x12\x16.google.protobuf.Empty\x1a%.ondewo.s2t.S2TGetServiceInfoResponse\"\x00\x12n\n\x15ListS2tLanguageModels\x12(.ondewo.s2t.ListS2tLanguageModelsRequest\x1a).ondewo.s2t.ListS2tLanguageModelsResponse\"\x00\x12_\n\x17\x43reateUserLanguageModel\x12*.ondewo.s2t.CreateUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x17\x44\x65leteUserLanguageModel\x12*.ondewo.s2t.DeleteUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x65\n\x1a\x41\x64\x64\x44\x61taToUserLanguageModel\x12-.ondewo.s2t.AddDataToUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12]\n\x16TrainUserLanguageModel\x12).ondewo.s2t.TrainUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fondewo/s2t/speech-to-text.proto\x12\nondewo.s2t\x1a\x1bgoogle/protobuf/empty.proto\"\x9a\x04\n\x17TranscribeRequestConfig\x12\x17\n\x0fs2t_pipeline_id\x18\x01 \x01(\t\x12&\n\x08\x64\x65\x63oding\x18\x02 \x01(\x0e\x32\x14.ondewo.s2t.Decoding\x12\x1d\n\x13language_model_name\x18\x03 \x01(\tH\x00\x12<\n\x0fpost_processing\x18\x04 \x01(\x0b\x32!.ondewo.s2t.PostProcessingOptionsH\x01\x12\x44\n\x13utterance_detection\x18\x05 \x01(\x0b\x32%.ondewo.s2t.UtteranceDetectionOptionsH\x02\x12(\n\x08pyannote\x18\x06 \x01(\x0b\x32\x14.ondewo.s2t.PyannoteH\x03\x12(\n\x08matchbox\x18\x07 \x01(\x0b\x32\x14.ondewo.s2t.MatchboxH\x03\x12@\n\x0ereturn_options\x18\x08 \x01(\x0b\x32&.ondewo.s2t.TranscriptionReturnOptionsH\x04\x42\x1b\n\x19oneof_language_model_nameB\x17\n\x15oneof_post_processingB\x1b\n\x19oneof_utterance_detectionB\x1a\n\x18voice_activity_detectionB\x16\n\x14oneof_return_options\"\xaf\x02\n\x1aTranscriptionReturnOptions\x12\x1e\n\x16return_start_of_speech\x18\x01 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x02 \x01(\x08\x12\x1f\n\x17return_confidence_score\x18\x03 \x01(\x08\x12)\n!return_alternative_transcriptions\x18\x04 \x01(\x08\x12,\n$return_alternative_transcriptions_nr\x18\x05 \x01(\x05\x12 \n\x18return_alternative_words\x18\x06 \x01(\x08\x12#\n\x1breturn_alternative_words_nr\x18\x07 \x01(\x05\x12\x1a\n\x12return_word_timing\x18\x08 \x01(\x08\"\xbf\x01\n\x19UtteranceDetectionOptions\x12\x1e\n\x14transcribe_not_final\x18\x01 \x01(\x08H\x00\x12$\n\x1cstart_of_utterance_threshold\x18\x02 \x01(\x02\x12\"\n\x1a\x65nd_of_utterance_threshold\x18\x03 \x01(\x02\x12\x1a\n\x12next_chunk_timeout\x18\x04 \x01(\x02\x42\x1c\n\x1aoneof_transcribe_not_final\"s\n\x15PostProcessingOptions\x12\x1b\n\x13spelling_correction\x18\x01 \x01(\x08\x12\x11\n\tnormalize\x18\x02 \x01(\x08\x12*\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\"\x8e\x01\n\x17TranscribeStreamRequest\x12\x13\n\x0b\x61udio_chunk\x18\x01 \x01(\x0c\x12\x15\n\rend_of_stream\x18\x02 \x01(\x08\x12\x33\n\x06\x63onfig\x18\x03 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\x12\x12\n\nmute_audio\x18\x04 \x01(\x08\"@\n\rTranscription\x12\x15\n\rtranscription\x18\x01 \x01(\t\x12\x18\n\x10\x63onfidence_score\x18\x02 \x01(\x02\"\x83\x02\n\x18TranscribeStreamResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12\r\n\x05\x66inal\x18\x03 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x04 \x01(\x08\x12\r\n\x05\x61udio\x18\x05 \x01(\x0c\x12\x17\n\x0futterance_start\x18\x06 \x01(\x08\x12\x12\n\naudio_uuid\x18\x07 \x01(\t\x12\x35\n\x06\x63onfig\x18\x08 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfigH\x00\x42\x0e\n\x0coneof_config\"`\n\x15TranscribeFileRequest\x12\x12\n\naudio_file\x18\x01 \x01(\x0c\x12\x33\n\x06\x63onfig\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\"\x9a\x01\n\x16TranscribeFileResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12+\n\x0bword_timing\x18\x03 \x03(\x0b\x32\x16.ondewo.s2t.WordTiming\x12\x12\n\naudio_uuid\x18\x04 \x01(\t\"6\n\nWordTiming\x12\x0c\n\x04word\x18\x01 \x01(\t\x12\r\n\x05\x62\x65gin\x18\x02 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x05\"\x1b\n\rS2tPipelineId\x12\n\n\x02id\x18\x01 \x01(\t\"o\n\x17ListS2tPipelinesRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x0f\n\x07\x64omains\x18\x03 \x03(\t\x12\x17\n\x0fregistered_only\x18\x04 \x01(\x08\"S\n\x18ListS2tPipelinesResponse\x12\x37\n\x10pipeline_configs\x18\x01 \x03(\x0b\x32\x1d.ondewo.s2t.Speech2TextConfig\"C\n\x17ListS2tLanguagesRequest\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\"-\n\x18ListS2tLanguagesResponse\x12\x11\n\tlanguages\x18\x01 \x03(\t\"C\n\x15ListS2tDomainsRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\")\n\x16ListS2tDomainsResponse\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\",\n\x19S2TGetServiceInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"\xe5\x02\n\x11Speech2TextConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12/\n\x0b\x64\x65scription\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.S2TDescription\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\x12+\n\tinference\x18\x04 \x01(\x0b\x32\x18.ondewo.s2t.S2TInference\x12\x35\n\x10streaming_server\x18\x05 \x01(\x0b\x32\x1b.ondewo.s2t.StreamingServer\x12\x44\n\x18voice_activity_detection\x18\x06 \x01(\x0b\x32\".ondewo.s2t.VoiceActivityDetection\x12\x33\n\x0fpost_processing\x18\x07 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\x12$\n\x07logging\x18\x08 \x01(\x0b\x32\x13.ondewo.s2t.Logging\"\\\n\x0eS2TDescription\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x16\n\x0epipeline_owner\x18\x02 \x01(\t\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x10\n\x08\x63omments\x18\x04 \x01(\t\"\xb1\x01\n\x0cS2TInference\x12\x33\n\x0f\x61\x63oustic_models\x18\x01 \x01(\x0b\x32\x1a.ondewo.s2t.AcousticModels\x12\x33\n\x0flanguage_models\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.LanguageModels\x12\x37\n\x11inference_backend\x18\x03 \x01(\x0e\x32\x1c.ondewo.s2t.InferenceBackend\"\xb1\x02\n\x0e\x41\x63ousticModels\x12\x0c\n\x04type\x18\x01 \x01(\t\x12(\n\tquartznet\x18\x02 \x01(\x0b\x32\x15.ondewo.s2t.Quartznet\x12\x35\n\x10quartznet_triton\x18\x03 \x01(\x0b\x32\x1b.ondewo.s2t.QuartznetTriton\x12$\n\x07wav2vec\x18\x04 \x01(\x0b\x32\x13.ondewo.s2t.Wav2Vec\x12\x31\n\x0ewav2vec_triton\x18\x05 \x01(\x0b\x32\x19.ondewo.s2t.Wav2VecTriton\x12$\n\x07whisper\x18\x06 \x01(\x0b\x32\x13.ondewo.s2t.Whisper\x12\x31\n\x0ewhisper_triton\x18\x07 \x01(\x0b\x32\x19.ondewo.s2t.WhisperTriton\"@\n\x07Whisper\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\x12\x10\n\x08language\x18\x03 \x01(\t\"~\n\rWhisperTriton\x12\x16\n\x0eprocessor_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1c\n\x14triton_model_version\x18\x03 \x01(\t\x12\x1c\n\x14\x63heck_status_timeout\x18\x04 \x01(\x03\".\n\x07Wav2Vec\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\"~\n\rWav2VecTriton\x12\x16\n\x0eprocessor_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1c\n\x14triton_model_version\x18\x03 \x01(\t\x12\x1c\n\x14\x63heck_status_timeout\x18\x04 \x01(\x03\"\x94\x01\n\tQuartznet\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x11\n\tload_type\x18\x02 \x01(\t\x12%\n\x08pt_files\x18\x03 \x01(\x0b\x32\x13.ondewo.s2t.PtFiles\x12\'\n\tckpt_file\x18\x04 \x01(\x0b\x32\x14.ondewo.s2t.CkptFile\x12\x0f\n\x07use_gpu\x18\x05 \x01(\x08\"%\n\x07PtFiles\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0c\n\x04step\x18\x02 \x01(\t\"\x18\n\x08\x43kptFile\x12\x0c\n\x04path\x18\x01 \x01(\t\"P\n\x0fQuartznetTriton\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x12\n\ntriton_url\x18\x02 \x01(\t\x12\x14\n\x0ctriton_model\x18\x03 \x01(\t\"\x88\x01\n\x0eLanguageModels\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tbeam_size\x18\x02 \x01(\x03\x12\x12\n\ndefault_lm\x18\x03 \x01(\t\x12 \n\x18\x62\x65\x61m_search_scorer_alpha\x18\x04 \x01(\x02\x12\x1f\n\x17\x62\x65\x61m_search_scorer_beta\x18\x05 \x01(\x02\"\x91\x01\n\x0fStreamingServer\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x03\x12\x14\n\x0coutput_style\x18\x03 \x01(\t\x12L\n\x1cstreaming_speech_recognition\x18\x04 \x01(\x0b\x32&.ondewo.s2t.StreamingSpeechRecognition\"\xee\x01\n\x1aStreamingSpeechRecognition\x12\x1c\n\x14transcribe_not_final\x18\x01 \x01(\x08\x12\x17\n\x0f\x64\x65\x63oding_method\x18\x02 \x01(\t\x12\x15\n\rsampling_rate\x18\x03 \x01(\x03\x12\x1c\n\x14min_audio_chunk_size\x18\x04 \x01(\x03\x12$\n\x1cstart_of_utterance_threshold\x18\x05 \x01(\x02\x12\"\n\x1a\x65nd_of_utterance_threshold\x18\x06 \x01(\x02\x12\x1a\n\x12next_chunk_timeout\x18\x07 \x01(\x02\"\x8f\x01\n\x16VoiceActivityDetection\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\t\x12\x15\n\rsampling_rate\x18\x02 \x01(\x03\x12&\n\x08pyannote\x18\x03 \x01(\x0b\x32\x14.ondewo.s2t.Pyannote\x12&\n\x08matchbox\x18\x04 \x01(\x0b\x32\x14.ondewo.s2t.Matchbox\"\xb0\x01\n\x08Pyannote\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x16\n\x0emin_audio_size\x18\x02 \x01(\x03\x12\x0e\n\x06offset\x18\x03 \x01(\x02\x12\r\n\x05onset\x18\x04 \x01(\x02\x12\x13\n\tlog_scale\x18\x05 \x01(\x08H\x00\x12\x18\n\x10min_duration_off\x18\x06 \x01(\x02\x12\x17\n\x0fmin_duration_on\x18\x07 \x01(\x02\x42\x11\n\x0foneof_log_scale\"L\n\x08Matchbox\x12\x14\n\x0cmodel_config\x18\x01 \x01(\t\x12\x14\n\x0c\x65ncoder_path\x18\x02 \x01(\t\x12\x14\n\x0c\x64\x65\x63oder_path\x18\x03 \x01(\t\"W\n\x0ePostProcessing\x12\x10\n\x08pipeline\x18\x01 \x03(\t\x12\x33\n\x0fpost_processors\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessors\"n\n\x0ePostProcessors\x12\'\n\tsym_spell\x18\x01 \x01(\x0b\x32\x14.ondewo.s2t.SymSpell\x12\x33\n\rnormalization\x18\x02 \x01(\x0b\x32\x1c.ondewo.s2t.S2TNormalization\"Z\n\x08SymSpell\x12\x11\n\tdict_path\x18\x01 \x01(\t\x12$\n\x1cmax_dictionary_edit_distance\x18\x02 \x01(\x03\x12\x15\n\rprefix_length\x18\x03 \x01(\x03\"$\n\x10S2TNormalization\x12\x10\n\x08language\x18\x01 \x01(\t\"%\n\x07Logging\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"+\n\x1cListS2tLanguageModelsRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"C\n\x17LanguageModelPipelineId\x12\x13\n\x0bpipeline_id\x18\x01 \x01(\t\x12\x13\n\x0bmodel_names\x18\x02 \x03(\t\"]\n\x1dListS2tLanguageModelsResponse\x12<\n\x0flm_pipeline_ids\x18\x01 \x03(\x0b\x32#.ondewo.s2t.LanguageModelPipelineId\"=\n\x1e\x43reateUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"=\n\x1e\x44\x65leteUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"U\n!AddDataToUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\x13\n\x0bzipped_data\x18\x02 \x01(\x0c\"K\n\x1dTrainUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\x03*l\n\x10InferenceBackend\x12\x1d\n\x19INFERENCE_BACKEND_UNKNOWN\x10\x00\x12\x1d\n\x19INFERENCE_BACKEND_PYTORCH\x10\x01\x12\x1a\n\x16INFERENCE_BACKEND_FLAX\x10\x02*M\n\x08\x44\x65\x63oding\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06GREEDY\x10\x01\x12\x17\n\x13\x42\x45\x41M_SEARCH_WITH_LM\x10\x02\x12\x0f\n\x0b\x42\x45\x41M_SEARCH\x10\x03\x32\xec\n\n\x0bSpeech2Text\x12Y\n\x0eTranscribeFile\x12!.ondewo.s2t.TranscribeFileRequest\x1a\".ondewo.s2t.TranscribeFileResponse\"\x00\x12\x63\n\x10TranscribeStream\x12#.ondewo.s2t.TranscribeStreamRequest\x1a$.ondewo.s2t.TranscribeStreamResponse\"\x00(\x01\x30\x01\x12L\n\x0eGetS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x1d.ondewo.s2t.Speech2TextConfig\"\x00\x12O\n\x11\x43reateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x19.ondewo.s2t.S2tPipelineId\"\x00\x12H\n\x11\x44\x65leteS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x11UpdateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x10ListS2tPipelines\x12#.ondewo.s2t.ListS2tPipelinesRequest\x1a$.ondewo.s2t.ListS2tPipelinesResponse\"\x00\x12_\n\x10ListS2tLanguages\x12#.ondewo.s2t.ListS2tLanguagesRequest\x1a$.ondewo.s2t.ListS2tLanguagesResponse\"\x00\x12Y\n\x0eListS2tDomains\x12!.ondewo.s2t.ListS2tDomainsRequest\x1a\".ondewo.s2t.ListS2tDomainsResponse\"\x00\x12Q\n\x0eGetServiceInfo\x12\x16.google.protobuf.Empty\x1a%.ondewo.s2t.S2TGetServiceInfoResponse\"\x00\x12n\n\x15ListS2tLanguageModels\x12(.ondewo.s2t.ListS2tLanguageModelsRequest\x1a).ondewo.s2t.ListS2tLanguageModelsResponse\"\x00\x12_\n\x17\x43reateUserLanguageModel\x12*.ondewo.s2t.CreateUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x17\x44\x65leteUserLanguageModel\x12*.ondewo.s2t.DeleteUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x65\n\x1a\x41\x64\x64\x44\x61taToUserLanguageModel\x12-.ondewo.s2t.AddDataToUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12]\n\x16TrainUserLanguageModel\x12).ondewo.s2t.TrainUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
 
+_INFERENCEBACKEND = DESCRIPTOR.enum_types_by_name['InferenceBackend']
+InferenceBackend = enum_type_wrapper.EnumTypeWrapper(_INFERENCEBACKEND)
 _DECODING = DESCRIPTOR.enum_types_by_name['Decoding']
 Decoding = enum_type_wrapper.EnumTypeWrapper(_DECODING)
+INFERENCE_BACKEND_UNKNOWN = 0
+INFERENCE_BACKEND_PYTORCH = 1
+INFERENCE_BACKEND_FLAX = 2
 DEFAULT = 0
 GREEDY = 1
 BEAM_SEARCH_WITH_LM = 2
 BEAM_SEARCH = 3
 
 
 _TRANSCRIBEREQUESTCONFIG = DESCRIPTOR.message_types_by_name['TranscribeRequestConfig']
@@ -410,108 +415,110 @@
   })
 _sym_db.RegisterMessage(TrainUserLanguageModelRequest)
 
 _SPEECH2TEXT = DESCRIPTOR.services_by_name['Speech2Text']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _DECODING._serialized_start=5754
-  _DECODING._serialized_end=5831
+  _INFERENCEBACKEND._serialized_start=5929
+  _INFERENCEBACKEND._serialized_end=6037
+  _DECODING._serialized_start=6039
+  _DECODING._serialized_end=6116
   _TRANSCRIBEREQUESTCONFIG._serialized_start=77
   _TRANSCRIBEREQUESTCONFIG._serialized_end=615
   _TRANSCRIPTIONRETURNOPTIONS._serialized_start=618
-  _TRANSCRIPTIONRETURNOPTIONS._serialized_end=804
-  _UTTERANCEDETECTIONOPTIONS._serialized_start=807
-  _UTTERANCEDETECTIONOPTIONS._serialized_end=998
-  _POSTPROCESSINGOPTIONS._serialized_start=1000
-  _POSTPROCESSINGOPTIONS._serialized_end=1115
-  _TRANSCRIBESTREAMREQUEST._serialized_start=1118
-  _TRANSCRIBESTREAMREQUEST._serialized_end=1260
-  _TRANSCRIPTION._serialized_start=1262
-  _TRANSCRIPTION._serialized_end=1326
-  _TRANSCRIBESTREAMRESPONSE._serialized_start=1329
-  _TRANSCRIBESTREAMRESPONSE._serialized_end=1588
-  _TRANSCRIBEFILEREQUEST._serialized_start=1590
-  _TRANSCRIBEFILEREQUEST._serialized_end=1686
-  _TRANSCRIBEFILERESPONSE._serialized_start=1689
-  _TRANSCRIBEFILERESPONSE._serialized_end=1843
-  _WORDTIMING._serialized_start=1845
-  _WORDTIMING._serialized_end=1899
-  _S2TPIPELINEID._serialized_start=1901
-  _S2TPIPELINEID._serialized_end=1928
-  _LISTS2TPIPELINESREQUEST._serialized_start=1930
-  _LISTS2TPIPELINESREQUEST._serialized_end=2041
-  _LISTS2TPIPELINESRESPONSE._serialized_start=2043
-  _LISTS2TPIPELINESRESPONSE._serialized_end=2126
-  _LISTS2TLANGUAGESREQUEST._serialized_start=2128
-  _LISTS2TLANGUAGESREQUEST._serialized_end=2195
-  _LISTS2TLANGUAGESRESPONSE._serialized_start=2197
-  _LISTS2TLANGUAGESRESPONSE._serialized_end=2242
-  _LISTS2TDOMAINSREQUEST._serialized_start=2244
-  _LISTS2TDOMAINSREQUEST._serialized_end=2311
-  _LISTS2TDOMAINSRESPONSE._serialized_start=2313
-  _LISTS2TDOMAINSRESPONSE._serialized_end=2354
-  _S2TGETSERVICEINFORESPONSE._serialized_start=2356
-  _S2TGETSERVICEINFORESPONSE._serialized_end=2400
-  _SPEECH2TEXTCONFIG._serialized_start=2403
-  _SPEECH2TEXTCONFIG._serialized_end=2760
-  _S2TDESCRIPTION._serialized_start=2762
-  _S2TDESCRIPTION._serialized_end=2854
-  _S2TINFERENCE._serialized_start=2856
-  _S2TINFERENCE._serialized_end=2976
-  _ACOUSTICMODELS._serialized_start=2979
-  _ACOUSTICMODELS._serialized_end=3284
-  _WHISPER._serialized_start=3286
-  _WHISPER._serialized_end=3350
-  _WHISPERTRITON._serialized_start=3352
-  _WHISPERTRITON._serialized_end=3478
-  _WAV2VEC._serialized_start=3480
-  _WAV2VEC._serialized_end=3526
-  _WAV2VECTRITON._serialized_start=3528
-  _WAV2VECTRITON._serialized_end=3654
-  _QUARTZNET._serialized_start=3657
-  _QUARTZNET._serialized_end=3805
-  _PTFILES._serialized_start=3807
-  _PTFILES._serialized_end=3844
-  _CKPTFILE._serialized_start=3846
-  _CKPTFILE._serialized_end=3870
-  _QUARTZNETTRITON._serialized_start=3872
-  _QUARTZNETTRITON._serialized_end=3952
-  _LANGUAGEMODELS._serialized_start=3955
-  _LANGUAGEMODELS._serialized_end=4091
-  _STREAMINGSERVER._serialized_start=4094
-  _STREAMINGSERVER._serialized_end=4239
-  _STREAMINGSPEECHRECOGNITION._serialized_start=4242
-  _STREAMINGSPEECHRECOGNITION._serialized_end=4480
-  _VOICEACTIVITYDETECTION._serialized_start=4483
-  _VOICEACTIVITYDETECTION._serialized_end=4626
-  _PYANNOTE._serialized_start=4629
-  _PYANNOTE._serialized_end=4805
-  _MATCHBOX._serialized_start=4807
-  _MATCHBOX._serialized_end=4883
-  _POSTPROCESSING._serialized_start=4885
-  _POSTPROCESSING._serialized_end=4972
-  _POSTPROCESSORS._serialized_start=4974
-  _POSTPROCESSORS._serialized_end=5084
-  _SYMSPELL._serialized_start=5086
-  _SYMSPELL._serialized_end=5176
-  _S2TNORMALIZATION._serialized_start=5178
-  _S2TNORMALIZATION._serialized_end=5214
-  _LOGGING._serialized_start=5216
-  _LOGGING._serialized_end=5253
-  _LISTS2TLANGUAGEMODELSREQUEST._serialized_start=5255
-  _LISTS2TLANGUAGEMODELSREQUEST._serialized_end=5298
-  _LANGUAGEMODELPIPELINEID._serialized_start=5300
-  _LANGUAGEMODELPIPELINEID._serialized_end=5367
-  _LISTS2TLANGUAGEMODELSRESPONSE._serialized_start=5369
-  _LISTS2TLANGUAGEMODELSRESPONSE._serialized_end=5462
-  _CREATEUSERLANGUAGEMODELREQUEST._serialized_start=5464
-  _CREATEUSERLANGUAGEMODELREQUEST._serialized_end=5525
-  _DELETEUSERLANGUAGEMODELREQUEST._serialized_start=5527
-  _DELETEUSERLANGUAGEMODELREQUEST._serialized_end=5588
-  _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_start=5590
-  _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_end=5675
-  _TRAINUSERLANGUAGEMODELREQUEST._serialized_start=5677
-  _TRAINUSERLANGUAGEMODELREQUEST._serialized_end=5752
-  _SPEECH2TEXT._serialized_start=5834
-  _SPEECH2TEXT._serialized_end=7222
+  _TRANSCRIPTIONRETURNOPTIONS._serialized_end=921
+  _UTTERANCEDETECTIONOPTIONS._serialized_start=924
+  _UTTERANCEDETECTIONOPTIONS._serialized_end=1115
+  _POSTPROCESSINGOPTIONS._serialized_start=1117
+  _POSTPROCESSINGOPTIONS._serialized_end=1232
+  _TRANSCRIBESTREAMREQUEST._serialized_start=1235
+  _TRANSCRIBESTREAMREQUEST._serialized_end=1377
+  _TRANSCRIPTION._serialized_start=1379
+  _TRANSCRIPTION._serialized_end=1443
+  _TRANSCRIBESTREAMRESPONSE._serialized_start=1446
+  _TRANSCRIBESTREAMRESPONSE._serialized_end=1705
+  _TRANSCRIBEFILEREQUEST._serialized_start=1707
+  _TRANSCRIBEFILEREQUEST._serialized_end=1803
+  _TRANSCRIBEFILERESPONSE._serialized_start=1806
+  _TRANSCRIBEFILERESPONSE._serialized_end=1960
+  _WORDTIMING._serialized_start=1962
+  _WORDTIMING._serialized_end=2016
+  _S2TPIPELINEID._serialized_start=2018
+  _S2TPIPELINEID._serialized_end=2045
+  _LISTS2TPIPELINESREQUEST._serialized_start=2047
+  _LISTS2TPIPELINESREQUEST._serialized_end=2158
+  _LISTS2TPIPELINESRESPONSE._serialized_start=2160
+  _LISTS2TPIPELINESRESPONSE._serialized_end=2243
+  _LISTS2TLANGUAGESREQUEST._serialized_start=2245
+  _LISTS2TLANGUAGESREQUEST._serialized_end=2312
+  _LISTS2TLANGUAGESRESPONSE._serialized_start=2314
+  _LISTS2TLANGUAGESRESPONSE._serialized_end=2359
+  _LISTS2TDOMAINSREQUEST._serialized_start=2361
+  _LISTS2TDOMAINSREQUEST._serialized_end=2428
+  _LISTS2TDOMAINSRESPONSE._serialized_start=2430
+  _LISTS2TDOMAINSRESPONSE._serialized_end=2471
+  _S2TGETSERVICEINFORESPONSE._serialized_start=2473
+  _S2TGETSERVICEINFORESPONSE._serialized_end=2517
+  _SPEECH2TEXTCONFIG._serialized_start=2520
+  _SPEECH2TEXTCONFIG._serialized_end=2877
+  _S2TDESCRIPTION._serialized_start=2879
+  _S2TDESCRIPTION._serialized_end=2971
+  _S2TINFERENCE._serialized_start=2974
+  _S2TINFERENCE._serialized_end=3151
+  _ACOUSTICMODELS._serialized_start=3154
+  _ACOUSTICMODELS._serialized_end=3459
+  _WHISPER._serialized_start=3461
+  _WHISPER._serialized_end=3525
+  _WHISPERTRITON._serialized_start=3527
+  _WHISPERTRITON._serialized_end=3653
+  _WAV2VEC._serialized_start=3655
+  _WAV2VEC._serialized_end=3701
+  _WAV2VECTRITON._serialized_start=3703
+  _WAV2VECTRITON._serialized_end=3829
+  _QUARTZNET._serialized_start=3832
+  _QUARTZNET._serialized_end=3980
+  _PTFILES._serialized_start=3982
+  _PTFILES._serialized_end=4019
+  _CKPTFILE._serialized_start=4021
+  _CKPTFILE._serialized_end=4045
+  _QUARTZNETTRITON._serialized_start=4047
+  _QUARTZNETTRITON._serialized_end=4127
+  _LANGUAGEMODELS._serialized_start=4130
+  _LANGUAGEMODELS._serialized_end=4266
+  _STREAMINGSERVER._serialized_start=4269
+  _STREAMINGSERVER._serialized_end=4414
+  _STREAMINGSPEECHRECOGNITION._serialized_start=4417
+  _STREAMINGSPEECHRECOGNITION._serialized_end=4655
+  _VOICEACTIVITYDETECTION._serialized_start=4658
+  _VOICEACTIVITYDETECTION._serialized_end=4801
+  _PYANNOTE._serialized_start=4804
+  _PYANNOTE._serialized_end=4980
+  _MATCHBOX._serialized_start=4982
+  _MATCHBOX._serialized_end=5058
+  _POSTPROCESSING._serialized_start=5060
+  _POSTPROCESSING._serialized_end=5147
+  _POSTPROCESSORS._serialized_start=5149
+  _POSTPROCESSORS._serialized_end=5259
+  _SYMSPELL._serialized_start=5261
+  _SYMSPELL._serialized_end=5351
+  _S2TNORMALIZATION._serialized_start=5353
+  _S2TNORMALIZATION._serialized_end=5389
+  _LOGGING._serialized_start=5391
+  _LOGGING._serialized_end=5428
+  _LISTS2TLANGUAGEMODELSREQUEST._serialized_start=5430
+  _LISTS2TLANGUAGEMODELSREQUEST._serialized_end=5473
+  _LANGUAGEMODELPIPELINEID._serialized_start=5475
+  _LANGUAGEMODELPIPELINEID._serialized_end=5542
+  _LISTS2TLANGUAGEMODELSRESPONSE._serialized_start=5544
+  _LISTS2TLANGUAGEMODELSRESPONSE._serialized_end=5637
+  _CREATEUSERLANGUAGEMODELREQUEST._serialized_start=5639
+  _CREATEUSERLANGUAGEMODELREQUEST._serialized_end=5700
+  _DELETEUSERLANGUAGEMODELREQUEST._serialized_start=5702
+  _DELETEUSERLANGUAGEMODELREQUEST._serialized_end=5763
+  _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_start=5765
+  _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_end=5850
+  _TRAINUSERLANGUAGEMODELREQUEST._serialized_start=5852
+  _TRAINUSERLANGUAGEMODELREQUEST._serialized_end=5927
+  _SPEECH2TEXT._serialized_start=6119
+  _SPEECH2TEXT._serialized_end=7507
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-s2t-client-5.2.0/ondewo/s2t/speech_to_text_pb2_grpc.py` & `ondewo-s2t-client-5.3.0/ondewo/s2t/speech_to_text_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import grpc
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from ondewo.s2t import speech_to_text_pb2 as ondewo_dot_s2t_dot_speech__to__text__pb2
 
 
 class Speech2TextStub(object):
-    """endpoints of speech-to-text service
+    """Speech-to-text service
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -90,19 +90,20 @@
                 '/ondewo.s2t.Speech2Text/TrainUserLanguageModel',
                 request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.TrainUserLanguageModelRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
 
 
 class Speech2TextServicer(object):
-    """endpoints of speech-to-text service
+    """Speech-to-text service
     """
 
     def TranscribeFile(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Transcribes an audio file
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def TranscribeStream(self, request_iterator, context):
         """Transcribes an audio stream.
         """
@@ -287,15 +288,15 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'ondewo.s2t.Speech2Text', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Speech2Text(object):
-    """endpoints of speech-to-text service
+    """Speech-to-text service
     """
 
     @staticmethod
     def TranscribeFile(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `ondewo-s2t-client-5.2.0/ondewo_s2t_client.egg-info/PKG-INFO` & `ondewo-s2t-client-5.3.0/ondewo_s2t_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-s2t-client
-Version: 5.2.0
+Version: 5.3.0
 Summary: exposes the ondewo-s2t-grpc-server endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-s2t-client-python
 Author: ONDEWO GbmH
 Author-email: info@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-s2t-client Version: 5.2.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-s2t-client Version: 5.3.0 Summary: exposes
 the ondewo-s2t-grpc-server endpoints in a user-friendly way Home-page: https://
 github.com/ondewo/ondewo-s2t-client-python Author: ONDEWO GbmH Author-email:
 info@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha Classifier: Topic :: Software
 Development :: Libraries Requires-Python: >=2.7, !=3.0.1 Description-Content-
 Type: text/markdown
```

### Comparing `ondewo-s2t-client-5.2.0/ondewo_s2t_client.egg-info/SOURCES.txt` & `ondewo-s2t-client-5.3.0/ondewo_s2t_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ondewo-s2t-client-5.2.0/setup.py` & `ondewo-s2t-client-5.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-import setuptools
+from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
-setuptools.setup(
+setup(
     name="ondewo-s2t-client",
-    version='5.2.0',
+    version='5.3.0',
     author="ONDEWO GbmH",
     author_email="info@ondewo.com",
     description="exposes the ondewo-s2t-grpc-server endpoints in a user-friendly way",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ondewo/ondewo-s2t-client-python',
     packages=[
-        np for np in filter(lambda n: n.startswith("ondewo.") or n == "ondewo", setuptools.find_packages())
+        np
+        for np in filter(
+            lambda n: n.startswith('ondewo.') or n == 'ondewo',
+            find_packages()
+        )
     ],
+    include_package_data=True,
+    package_data={
+        'ondewo.s2t': ['py.typed', '*.pyi'],
+    },
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
         'Development Status :: 3 - Alpha',
         'Topic :: Software Development :: Libraries',
     ],
     python_requires=">=2.7, !=3.0.1",
```

