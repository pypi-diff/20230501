# Comparing `tmp/pytrex-0.9.2-py3-none-any.whl.zip` & `tmp/pytrex-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 41857 bytes, number of entries: 21
+Zip file size: 41934 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat      140 b- defN 22-Nov-06 09:12 pytrex/__init__.py
 -rw-rw-rw-  2.0 fat     4152 b- defN 22-Nov-06 09:12 pytrex/common.py
 -rw-rw-rw-  2.0 fat     5218 b- defN 22-Nov-06 09:12 pytrex/text_opts.py
--rw-rw-rw-  2.0 fat     8193 b- defN 23-Apr-14 06:35 pytrex/trex_app.py
+-rw-rw-rw-  2.0 fat     8193 b- defN 23-May-01 10:57 pytrex/trex_app.py
 -rw-rw-rw-  2.0 fat     3849 b- defN 22-Nov-06 09:12 pytrex/trex_capture.py
--rw-rw-rw-  2.0 fat     1581 b- defN 23-Apr-14 06:35 pytrex/trex_object.py
--rw-rw-rw-  2.0 fat    11960 b- defN 23-Apr-14 06:35 pytrex/trex_port.py
--rw-rw-rw-  2.0 fat     2864 b- defN 23-Apr-14 06:35 pytrex/trex_statistics_view.py
--rw-rw-rw-  2.0 fat    64578 b- defN 23-Apr-14 06:35 pytrex/trex_stl_packet_builder_scapy.py
--rw-rw-rw-  2.0 fat    12179 b- defN 23-Apr-14 06:35 pytrex/trex_stream.py
+-rw-rw-rw-  2.0 fat     1581 b- defN 23-May-01 10:57 pytrex/trex_object.py
+-rw-rw-rw-  2.0 fat    11960 b- defN 23-May-01 10:57 pytrex/trex_port.py
+-rw-rw-rw-  2.0 fat     2864 b- defN 23-May-01 10:57 pytrex/trex_statistics_view.py
+-rw-rw-rw-  2.0 fat    64578 b- defN 23-May-01 10:57 pytrex/trex_stl_packet_builder_scapy.py
+-rw-rw-rw-  2.0 fat    12288 b- defN 23-May-01 10:57 pytrex/trex_stream.py
 -rw-rw-rw-  2.0 fat     1012 b- defN 22-Nov-06 09:12 pytrex/zipmsg.py
 -rw-rw-rw-  2.0 fat      112 b- defN 22-Nov-06 09:12 pytrex/api/__init__.py
 -rw-rw-rw-  2.0 fat    10736 b- defN 22-Nov-06 09:12 pytrex/api/trex_event.py
 -rw-rw-rw-  2.0 fat    12057 b- defN 22-Nov-06 09:12 pytrex/api/trex_stl_async_client.py
 -rw-rw-rw-  2.0 fat     7093 b- defN 22-Nov-06 09:12 pytrex/api/trex_stl_conn.py
 -rw-rw-rw-  2.0 fat     7798 b- defN 22-Nov-06 09:12 pytrex/api/trex_stl_jsonrpc_client.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-06 09:12 pytrex/api/trex_stl_types.py
--rw-rw-rw-  2.0 fat     1207 b- defN 23-Apr-14 13:55 pytrex-0.9.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-14 13:55 pytrex-0.9.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-14 13:55 pytrex-0.9.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1674 b- defN 23-Apr-14 13:55 pytrex-0.9.2.dist-info/RECORD
-21 files, 156502 bytes uncompressed, 39167 bytes compressed:  75.0%
+-rw-rw-rw-  2.0 fat     1352 b- defN 23-May-01 10:58 pytrex-0.9.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-01 10:58 pytrex-0.9.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-May-01 10:58 pytrex-0.9.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1674 b- defN 23-May-01 10:58 pytrex-0.9.3.dist-info/RECORD
+21 files, 156756 bytes uncompressed, 39244 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: pytrex/api/trex_stl_jsonrpc_client.py
 Comment: 
 
 Filename: pytrex/api/trex_stl_types.py
 Comment: 
 
-Filename: pytrex-0.9.2.dist-info/METADATA
+Filename: pytrex-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: pytrex-0.9.2.dist-info/WHEEL
+Filename: pytrex-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: pytrex-0.9.2.dist-info/top_level.txt
+Filename: pytrex-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pytrex-0.9.2.dist-info/RECORD
+Filename: pytrex-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytrex/trex_stream.py

```diff
@@ -267,17 +267,17 @@
             dump = scapy_b.to_pkt_dump()
         else:
             print("Nothing to dump")
         return dump
 
 
 class TrexYamlLoader:
-    def __init__(self, port, yaml_file: Path) -> None:
+    def __init__(self, port, profile_path: Path) -> None:
         self.port = port
-        self.yaml_file = yaml_file
+        self.profile_path = profile_path
 
     def __parse_packet(
         self, stream: TrexStream, packet_dict: dict, mac_src_override_by_pkt: int, mac_dst_override_mode: int
     ) -> None:
         pkt_str = base64.b64decode(packet_dict["binary"])
         builder = STLPktBuilder(pkt_buffer=pkt_str)
         stream.set_packet(builder, mac_src_override_by_pkt, mac_dst_override_mode)
@@ -293,23 +293,23 @@
             attributes["packets"] = mode_obj.get("total_pkts", 1)
         elif tx_type == TrexTxType.multi_burst:
             attributes["packets"] = mode_obj.get("pkts_per_burst", 1)
             attributes["ibg"] = mode_obj.get("ibg", 0.0)
             attributes["count"] = mode_obj.get("count", 2)
         stream.set_tx_type(tx_type, **attributes)
 
-    def __parse_flow_stats(self, stream, flow_stats_obj):
+    def __parse_flow_stats(self, stream: TrexStream, flow_stats_obj: dict) -> None:
         if not flow_stats_obj.get("enabled"):
             stream.set_flow_stats(TrexFlowStatsType.none)
-        stream.set_flow_stats(TrexFlowStatsType[flow_stats_obj.get("rule_type")], flow_stats_obj.get("stream_id"))
+        stream.set_flow_stats(TrexFlowStatsType[flow_stats_obj.get("rule_type", "none")], flow_stats_obj.get("stream_id"))
 
     def __parse_stream(self, yaml_object: dict) -> TrexStream:
         # create the stream
-        s_obj = yaml_object["stream"]
-        stream = self.port.add_stream(name=yaml_object.get("name"))
+        s_obj = yaml_object["stream"] if "stream" in yaml_object else yaml_object
+        stream = self.port.add_stream(name=yaml_object.get("name", f"stream-{len(self.port.streams)}"))
 
         stream.config(
             enabled=s_obj.get("enabled", True),
             self_start=s_obj.get("self_start", True),
             isg=s_obj.get("isg", 0.0),
             action_count=s_obj.get("action_count", 0),
         )
@@ -334,12 +334,11 @@
         if "vm" in s_obj:
             stream.fields["vm"].update(s_obj["vm"])
 
         return stream
 
     def parse(self) -> list:
         """Read YAML and pass it down to stream object."""
-        with open(self.yaml_file, "r") as f:
-            yaml_str = f.read()
-            objects = yaml.safe_load(yaml_str)
+        with open(self.profile_path, "r") as yaml_file:
+            objects = yaml.safe_load(yaml_file.read())
         streams = [self.__parse_stream(obj) for obj in objects]
         return streams
```

## Comparing `pytrex-0.9.2.dist-info/METADATA` & `pytrex-0.9.3.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrex
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python OO API package to manage TRex traffic generator stateless traffic generator
 Home-page: https://github.com/shmir/PyTRex
 Author: Yoram Shamir
 Author-email: yoram@ignissoft.com
 License: Apache Software License
 Keywords: cisco,trex,l2l3,tg,traffic generator,test automation,automation api
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,10 +22,11 @@
 Requires-Dist: pyzmq
 
 ## Python OO API for Cisco TRex.
 
 The package was tested with TRex version 2.61.
 
 ### TRex Resources
-- https://trex-tgn.cisco.com/trex/doc/trex_manual.html
-- https://trex-tgn.cisco.com/trex/doc/trex_rpc_server_spec.html
-- https://trex-tgn.cisco.com/trex/doc/cp_stl_docs/
+- [TRex](https://trex-tgn.cisco.com/trex/doc/trex_manual.html)
+- [TRex Stateless support](https://trex-tgn.cisco.com/trex/doc/trex_stateless.html)
+- [The TRex RPC Server](https://trex-tgn.cisco.com/trex/doc/trex_rpc_server_spec.html)
+- [TRex Stateless Python API](https://trex-tgn.cisco.com/trex/doc/cp_stl_docs/)
```

## Comparing `pytrex-0.9.2.dist-info/RECORD` & `pytrex-0.9.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 pytrex/text_opts.py,sha256=nhRQOqDWkVzrKAx2v9jpG3noQf3jWvMz6jlXImdMit0,5218
 pytrex/trex_app.py,sha256=pbGB-qAfGglBDtWWko6EmzKyJp9f3QzRrBOk89o6UMo,8193
 pytrex/trex_capture.py,sha256=Ag9swtJMvbgHQtF0m10GNSxCY3mwVYioH1VK22PB4oI,3849
 pytrex/trex_object.py,sha256=QE4zHDN2ECb960su2EH4LIZjNdHW9t3LZ6zrlzpPjPU,1581
 pytrex/trex_port.py,sha256=ic3W5MxLDrKjlbJ2oRUUu6_HMjNk10Mz9FE6ued0owg,11960
 pytrex/trex_statistics_view.py,sha256=zXl6FIRvmCgOdvi9fVffHrIlacLU93_rFpXqsEcKmfk,2864
 pytrex/trex_stl_packet_builder_scapy.py,sha256=DqSQMvvp5oEBioY0JRH6jyXMmU1T0Oyg2UwtmzxaVh4,64578
-pytrex/trex_stream.py,sha256=lMmhxma3l2dRs8qhVXQkWycY1WYPGWPRR5wk6OtA1gM,12179
+pytrex/trex_stream.py,sha256=yp5_XjAY5Z_qEGXb71PMNI39Sia8MibuvVWvnxDC_zg,12288
 pytrex/zipmsg.py,sha256=CAjh03lTAJHAhV3cMZXVpJc1aGi09OOFUcmc5umyV8g,1012
 pytrex/api/__init__.py,sha256=tXyqchlqi1Bos01i_DLOtmfYIUVRBON3pnnZI4EOtfM,112
 pytrex/api/trex_event.py,sha256=wBTKc7toWr3NQas39I4Dy5ND43_w8FbQnYPvPiMSRLI,10736
 pytrex/api/trex_stl_async_client.py,sha256=SDxjJop43HB8ZkF-6uU7jYh70Twf8wV6QjNFMWwxfZg,12057
 pytrex/api/trex_stl_conn.py,sha256=7-IQbSlwPG-CQQboAYxFqWtTw6XyUhU5gek44IynEBs,7093
 pytrex/api/trex_stl_jsonrpc_client.py,sha256=ImCGnWtyYafDeG-MqiPu0WSIO0aAovR5WmhQ5VP5vhI,7798
 pytrex/api/trex_stl_types.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pytrex-0.9.2.dist-info/METADATA,sha256=aaGOzlpwDI9OwBBxzG75bzO53VZOWXU-haBqUs2cwmk,1207
-pytrex-0.9.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pytrex-0.9.2.dist-info/top_level.txt,sha256=FCMTg-MWQsmCI5N09Xu716ZJeffUX90fX2ELlwaHR3w,7
-pytrex-0.9.2.dist-info/RECORD,,
+pytrex-0.9.3.dist-info/METADATA,sha256=KA56ZbPy0N9SSJ6gYXpZkmCxMQDPJuFycGX8-spIopE,1352
+pytrex-0.9.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pytrex-0.9.3.dist-info/top_level.txt,sha256=FCMTg-MWQsmCI5N09Xu716ZJeffUX90fX2ELlwaHR3w,7
+pytrex-0.9.3.dist-info/RECORD,,
```

