# Comparing `tmp/didcomm-0.3.1.tar.gz` & `tmp/didcomm-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "didcomm-0.3.1.tar", max compression
+gzip compressed data, was "didcomm-0.3.2.tar", max compression
```

## Comparing `didcomm-0.3.1.tar` & `didcomm-0.3.2.tar`

### file list

```diff
@@ -1,47 +1,46 @@
--rw-r--r--   0        0        0    11357 2022-10-20 06:05:50.812286 didcomm-0.3.1/LICENSE
--rw-r--r--   0        0        0     6646 2022-10-20 06:05:50.812286 didcomm-0.3.1/README.md
--rw-r--r--   0        0        0       22 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/common/__init__.py
--rw-r--r--   0        0        0     1630 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/common/algorithms.py
--rw-r--r--   0        0        0      449 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/common/resolvers.py
--rw-r--r--   0        0        0     2885 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/common/types.py
--rw-r--r--   0        0        0      285 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/common/utils.py
--rw-r--r--   0        0        0      133 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/__init__.py
--rw-r--r--   0        0        0     3726 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/anoncrypt.py
--rw-r--r--   0        0        0     4669 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/authcrypt.py
--rw-r--r--   0        0        0      534 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/converters.py
--rw-r--r--   0        0        0      210 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/defaults.py
--rw-r--r--   0        0        0     4927 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/from_prior.py
--rw-r--r--   0        0        0        0 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/keys/__init__.py
--rw-r--r--   0        0        0     3790 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/keys/anoncrypt_keys_selector.py
--rw-r--r--   0        0        0     4831 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/keys/authcrypt_keys_selector.py
--rw-r--r--   0        0        0      611 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/keys/forward_next_keys_selector.py
--rw-r--r--   0        0        0     2691 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/keys/sign_keys_selector.py
--rw-r--r--   0        0        0      824 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/serialization.py
--rw-r--r--   0        0        0     2093 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/sign.py
--rw-r--r--   0        0        0     2114 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/types.py
--rw-r--r--   0        0        0    14433 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/utils.py
--rw-r--r--   0        0        0     3082 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/validation.py
--rw-r--r--   0        0        0     3019 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/core/validators.py
--rw-r--r--   0        0        0        0 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/did_doc/__init__.py
--rw-r--r--   0        0        0     4982 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/did_doc/did_doc.py
--rw-r--r--   0        0        0     1566 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/did_doc/did_resolver.py
--rw-r--r--   0        0        0      429 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/did_doc/did_resolver_in_memory.py
--rw-r--r--   0        0        0     1711 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/errors.py
--rw-r--r--   0        0        0    13440 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/message.py
--rw-r--r--   0        0        0    15760 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/pack_encrypted.py
--rw-r--r--   0        0        0     2813 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/pack_plaintext.py
--rw-r--r--   0        0        0     4115 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/pack_signed.py
--rw-r--r--   0        0        0        0 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/protocols/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/protocols/routing/__init__.py
--rw-r--r--   0        0        0    11829 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/protocols/routing/forward.py
--rw-r--r--   0        0        0        0 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/secrets/__init__.py
--rw-r--r--   0        0        0     1749 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/secrets/secrets_resolver.py
--rw-r--r--   0        0        0     1353 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/secrets/secrets_resolver_demo.py
--rw-r--r--   0        0        0      330 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/secrets/secrets_resolver_editable.py
--rw-r--r--   0        0        0      552 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/secrets/secrets_resolver_in_memory.py
--rw-r--r--   0        0        0     2087 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/secrets/secrets_util.py
--rw-r--r--   0        0        0     8707 2022-10-20 06:05:50.812286 didcomm-0.3.1/didcomm/unpack.py
--rw-r--r--   0        0        0     1127 2022-10-20 06:05:50.812286 didcomm-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7746 1970-01-01 00:00:00.000000 didcomm-0.3.1/setup.py
--rw-r--r--   0        0        0     7758 1970-01-01 00:00:00.000000 didcomm-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-01 08:05:38.458193 didcomm-0.3.2/LICENSE
+-rw-r--r--   0        0        0     7066 2023-05-01 08:05:38.458193 didcomm-0.3.2/README.md
+-rw-r--r--   0        0        0     3051 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/common/__init__.py
+-rw-r--r--   0        0        0     1630 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/common/algorithms.py
+-rw-r--r--   0        0        0      449 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/common/resolvers.py
+-rw-r--r--   0        0        0     3060 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/common/types.py
+-rw-r--r--   0        0        0      285 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/common/utils.py
+-rw-r--r--   0        0        0      133 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/__init__.py
+-rw-r--r--   0        0        0     3726 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/anoncrypt.py
+-rw-r--r--   0        0        0     4669 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/authcrypt.py
+-rw-r--r--   0        0        0      534 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/converters.py
+-rw-r--r--   0        0        0      210 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/defaults.py
+-rw-r--r--   0        0        0     4998 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/from_prior.py
+-rw-r--r--   0        0        0        0 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/keys/__init__.py
+-rw-r--r--   0        0        0     3809 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/keys/anoncrypt_keys_selector.py
+-rw-r--r--   0        0        0     4801 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/keys/authcrypt_keys_selector.py
+-rw-r--r--   0        0        0      634 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/keys/forward_next_keys_selector.py
+-rw-r--r--   0        0        0     2671 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/keys/sign_keys_selector.py
+-rw-r--r--   0        0        0      824 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/serialization.py
+-rw-r--r--   0        0        0     2093 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/sign.py
+-rw-r--r--   0        0        0     2114 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/types.py
+-rw-r--r--   0        0        0    13854 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/utils.py
+-rw-r--r--   0        0        0     3141 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/validation.py
+-rw-r--r--   0        0        0     3691 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/core/validators.py
+-rw-r--r--   0        0        0        0 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/did_doc/__init__.py
+-rw-r--r--   0        0        0     1265 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/did_doc/did_doc.py
+-rw-r--r--   0        0        0     1566 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/did_doc/did_resolver.py
+-rw-r--r--   0        0        0      428 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/did_doc/did_resolver_in_memory.py
+-rw-r--r--   0        0        0     1711 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/errors.py
+-rw-r--r--   0        0        0    14512 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/message.py
+-rw-r--r--   0        0        0    15863 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/pack_encrypted.py
+-rw-r--r--   0        0        0     2888 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/pack_plaintext.py
+-rw-r--r--   0        0        0     4191 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/pack_signed.py
+-rw-r--r--   0        0        0        0 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/protocols/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/protocols/routing/__init__.py
+-rw-r--r--   0        0        0    11591 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/protocols/routing/forward.py
+-rw-r--r--   0        0        0        0 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/secrets/__init__.py
+-rw-r--r--   0        0        0     1749 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/secrets/secrets_resolver.py
+-rw-r--r--   0        0        0     1353 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/secrets/secrets_resolver_demo.py
+-rw-r--r--   0        0        0      330 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/secrets/secrets_resolver_editable.py
+-rw-r--r--   0        0        0      552 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/secrets/secrets_resolver_in_memory.py
+-rw-r--r--   0        0        0     2087 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/secrets/secrets_util.py
+-rw-r--r--   0        0        0     9093 2023-05-01 08:05:38.458193 didcomm-0.3.2/didcomm/unpack.py
+-rw-r--r--   0        0        0     1128 2023-05-01 08:05:38.458193 didcomm-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8216 1970-01-01 00:00:00.000000 didcomm-0.3.2/PKG-INFO
```

### Comparing `didcomm-0.3.1/LICENSE` & `didcomm-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/README.md` & `didcomm-0.3.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -70,42 +70,74 @@
 
 See `pack_encrypted` documentation for more details.
 
 **Authentication encryption** example (most common case):
 
 ```
 # ALICE
-message = Message(body={"aaa": 1, "bbb": 2},
-                  id="1234567890", type="my-protocol/1.0",
-                  frm=ALICE_DID, to=[BOB_DID])
-pack_result = await pack_encrypted(message=message, frm=ALICE_DID, to=BOB_DID)
+message = Message(
+    body={"aaa": 1, "bbb": 2},
+    id="1234567890",
+    type="my-protocol/1.0",
+    frm=ALICE_DID,
+    to=[BOB_DID],
+)
+pack_result = await pack_encrypted(
+    resolvers_config=resolvers_config_alice,
+    message=message,
+    frm=ALICE_DID,
+    to=BOB_DID,
+    pack_config=PackEncryptedConfig(),
+)
 packed_msg = pack_result.packed_msg
 print(f"Sending ${packed_msg} to ${pack_result.service_metadata.service_endpoint}")
 
 # BOB
-unpack_result = await unpack(packed_msg)
+unpack_result = await unpack(resolvers_config_bob, packed_msg)
 print(f"Got ${unpack_result.message} message")
 ```
 
 **Anonymous encryption** example:
 
 ```
-message = Message(body={"aaa": 1, "bbb": 2},
-                  id="1234567890", type="my-protocol/1.0",
-                  frm=ALICE_DID, to=[BOB_DID])
-pack_result = await pack_encrypted(message=message, to=BOB_DID)
+message = Message(
+    body={"aaa": 1, "bbb": 2},
+    id="1234567890",
+    type="my-protocol/1.0",
+    frm=ALICE_DID,
+    to=[BOB_DID],
+)
+
+pack_result = await pack_encrypted(
+    resolvers_config=resolvers_config_alice,
+    message=message,
+    to=BOB_DID,
+    pack_config=PackEncryptedConfig(),
+)
 ```
 
 **Encryption with non-repudiation** example:
 
 ```
-message = Message(body={"aaa": 1, "bbb": 2},
-                  id="1234567890", type="my-protocol/1.0",
-                  frm=ALICE_DID, to=[BOB_DID])
-pack_result = await pack_encrypted(message=message, frm=ALICE_DID, to=BOB_DID, sign_frm=ALICE_DID)
+message = Message(
+    body={"aaa": 1, "bbb": 2},
+    id="1234567890",
+    type="my-protocol/1.0",
+    frm=ALICE_DID,
+    to=[BOB_DID],
+)
+
+pack_result = await pack_encrypted(
+    resolvers_config=resolvers_config_alice,
+    message=message,
+    frm=ALICE_DID,
+    sign_frm=ALICE_DID,
+    to=BOB_DID,
+    pack_config=PackEncryptedConfig(),
+)
 ```
 
 ### 2. Build an unencrypted but Signed DIDComm message
 
 Signed messages are only necessary when
 - the origin of plaintext must be provable to third parties
 - or the sender can’t be proven to the recipient by authenticated encryption because the recipient is not known in advance (e.g., in a
@@ -114,46 +146,58 @@
 Adding a signature when one is not needed can degrade rather than enhance security because it
 relinquishes the sender’s ability to speak off the record.
 
 See `pack_signed` documentation for more details.
 
 ```
 # ALICE
-message = Message(body={"aaa": 1, "bbb": 2},
-                  id="1234567890", type="my-protocol/1.0",
-                  frm=ALICE_DID, to=[BOB_DID])
-packed_msg = await pack_signed(message=message, sign_frm=ALICE_DID)
+message = Message(
+    body={"aaa": 1, "bbb": 2},
+    id="1234567890",
+    type="my-protocol/1.0",
+    frm=ALICE_DID,
+    to=[BOB_DID],
+)
+pack_result = await pack_signed(
+    resolvers_config=resolvers_config_alice,
+    message=message,
+    sign_frm=ALICE_DID
+)
 packed_msg = pack_result.packed_msg
 print(f"Publishing ${packed_msg}")
 
 # BOB
-unpack_result = await unpack(packed_msg)
+unpack_result = await unpack(resolvers_config_bob, packed_msg)
 print(f"Got ${unpack_result.message} message signed as ${unpack_result.metadata.signed_message}")
 ```
 
 ### 3. Build a Plaintext DIDComm message
 
 A DIDComm message in its plaintext form that 
 - is not packaged into any protective envelope
 - lacks confidentiality and integrity guarantees
 - repudiable
 
 They are therefore not normally transported across security boundaries. 
 
 ```
 # ALICE
-message = Message(body={"aaa": 1, "bbb": 2},
-                  id="1234567890", type="my-protocol/1.0",
-                  frm=ALICE_DID, to=[BOB_DID])
-packed_msg = await pack_plaintext(message)
-print(f"Publishing ${packed_msg}")
+message = Message(
+    body={"aaa": 1, "bbb": 2},
+    id="1234567890",
+    type="my-protocol/1.0",
+    frm=ALICE_DID,
+    to=[BOB_DID],
+)
+pack_result = await pack_plaintext(resolvers_config=resolvers_config_alice, message)
+print(f"Publishing ${pack_result.packed_msg}")
 
 # BOB
-unpack_result = await unpack(packed_msg)
-print(f"Got ${unpack_result.plaintext} message")
+unpack_result = await unpack(resolvers_config_bob, pack_result.packed_msg)
+print(f"Got ${unpack_result.message} message")
 ```
 
 ## Contribution
 PRs are welcome!
 
 The following CI checks are run against every PR:
 - all tests must pass
```

### Comparing `didcomm-0.3.1/didcomm/common/algorithms.py` & `didcomm-0.3.2/didcomm/common/algorithms.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/common/types.py` & `didcomm-0.3.2/didcomm/common/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import Dict, Any, Union, List
+from pydid.did import DID, DIDUrl
 
 JSON_OBJ = Dict[str, Any]
-JSON_VALUE = Union[None, str, int, bool, float, JSON_OBJ, List[Any]]
+JSON_VALUE = Union[type(None), str, int, bool, float, Dict, List]
 JSON = str
 JWK = JSON
 JWT = JSON
 JWS = JSON
-DID = str
-DID_URL = str
+DID_URL = DIDUrl
 DID_OR_DID_URL = Union[DID, DID_URL]
 
 
-class VerificationMethodType(Enum):
-    JSON_WEB_KEY_2020 = 1
-    X25519_KEY_AGREEMENT_KEY_2019 = 2
-    ED25519_VERIFICATION_KEY_2018 = 3
-    X25519_KEY_AGREEMENT_KEY_2020 = 4
-    ED25519_VERIFICATION_KEY_2020 = 5
-    # ECDSA_SECP_256K1_VERIFICATION_KEY_2019 = 6 - not supported now
-    OTHER = 1000
+class VerificationMethodType:
+    JSON_WEB_KEY_2020 = "JsonWebKey2020"
+    X25519_KEY_AGREEMENT_KEY_2019 = "X25519KeyAgreementKey2019"
+    ED25519_VERIFICATION_KEY_2018 = "Ed25519VerificationKey2018"
+    X25519_KEY_AGREEMENT_KEY_2020 = "X25519KeyAgreementKey2020"
+    ED25519_VERIFICATION_KEY_2020 = "Ed25519VerificationKey2020"
+    # ECDSA_SECP_256K1_VERIFICATION_KEY_2019 = "EcdsaSecp256k1VerificationKey2019" - not supported now
+    OTHER = "Other"
 
 
 class VerificationMaterialFormat(Enum):
     JWK = 1
     BASE58 = 2
     MULTIBASE = 3
     OTHER = 1000
@@ -61,15 +61,14 @@
 
 
 class DIDCommMessageProtocolTypes(Enum):
     FORWARD = "https://didcomm.org/routing/2.0/forward"
 
 
 class JOSEFields:
-
     # JOSE Header fields as defined in JWS and JWE specs
     # (RFCs 7515, 7516, 7518, 7519, 7797, 8225, 8555)
     # https://www.iana.org/assignments/jose/jose.xhtml#web-signature-encryption-header-parameters
     JOSE_ALG = "alg"
     JOSE_JKU = "jku"
     JOSE_JWK = "jwk"
     JOSE_KID = "kid"
```

### Comparing `didcomm-0.3.1/didcomm/core/anoncrypt.py` & `didcomm-0.3.2/didcomm/core/anoncrypt.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/core/authcrypt.py` & `didcomm-0.3.2/didcomm/core/authcrypt.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/core/converters.py` & `didcomm-0.3.2/didcomm/core/converters.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/core/from_prior.py` & `didcomm-0.3.2/didcomm/core/from_prior.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 from authlib.common.encoding import to_unicode, to_bytes, json_loads, urlsafe_b64decode
 from authlib.jose import jwt
 from authlib.jose.errors import BadSignatureError
 
 from didcomm.common.resolvers import ResolversConfig
 from didcomm.common.types import DID_URL
 from didcomm.core.keys.sign_keys_selector import find_signing_key, find_verification_key
-from didcomm.core.utils import extract_key, extract_sign_alg, is_did_url, get_did
+from didcomm.core.utils import (
+    extract_key,
+    extract_sign_alg,
+    is_did_with_uri_fragment,
+    get_did,
+)
 from didcomm.errors import (
     MalformedMessageError,
     MalformedMessageCode,
     DIDCommValueError,
 )
 
 
@@ -117,16 +122,16 @@
 
 
 def __extract_from_prior_kid(from_prior_jwt: str) -> DID_URL:
     try:
         from_prior_jwt = to_bytes(from_prior_jwt)
         protected_segment = from_prior_jwt.split(b".")[0]
         protected = json_loads(urlsafe_b64decode(protected_segment).decode("utf-8"))
-        if not is_did_url(protected.get("kid")):
+        if not is_did_with_uri_fragment(protected.get("kid")):
             raise DIDCommValueError(
-                f"from_prior `kid` value is not a valid DID URL: {protected.get('kid')}"
+                f"from_prior `kid` value is not a valid DID URL containing a fragment: {protected.get('kid')}"
             )
         return protected["kid"]
     except Exception as exc:
         raise MalformedMessageError(
             MalformedMessageCode.INVALID_MESSAGE, "from_prior value is invalid"
         ) from exc
```

### Comparing `didcomm-0.3.1/didcomm/core/keys/anoncrypt_keys_selector.py` & `didcomm-0.3.2/didcomm/core/keys/anoncrypt_keys_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 async def _find_anoncrypt_pack_recipient_public_keys_by_kid(
     to_did: DID, to_kid: DID_URL, resolvers_config: ResolversConfig
 ) -> List[VerificationMethod]:
     did_doc = await resolvers_config.did_resolver.resolve(to_did)
     if did_doc is None:
         raise DIDDocNotResolvedError(to_did)
 
-    if to_kid not in did_doc.key_agreement_kids:
+    if not did_doc.key_agreement or to_kid not in did_doc.key_agreement:
         raise DIDUrlNotFoundError(
             f"DID URL `{to_kid}` is not found in keyAgreement verification relationships of DID `{to_did}`"
         )
 
     verification_method = did_doc.get_verification_method(to_kid)
     if verification_method is None:
         raise DIDUrlNotFoundError(f"Verification method `{to_kid}` is not found")
@@ -74,15 +74,15 @@
 async def _find_anoncrypt_pack_recipient_public_keys_by_did(
     to_did: DID, resolvers_config: ResolversConfig
 ) -> List[VerificationMethod]:
     did_doc = await resolvers_config.did_resolver.resolve(to_did)
     if did_doc is None:
         raise DIDDocNotResolvedError(to_did)
 
-    kids = did_doc.key_agreement_kids
+    kids = did_doc.key_agreement
     if not kids:
         raise DIDUrlNotFoundError(
             f"No keyAgreement verification relationships are found for DID `{to_did}`"
         )
 
     # return only verification methods having the same type as the first one
     first_verification_method = did_doc.get_verification_method(kids[0])
```

### Comparing `didcomm-0.3.1/didcomm/core/keys/authcrypt_keys_selector.py` & `didcomm-0.3.2/didcomm/core/keys/authcrypt_keys_selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,34 +34,34 @@
     frm_did, frm_kid = get_did_and_optionally_kid(frm_did_or_kid)
     to_did, to_kid = get_did_and_optionally_kid(to_did_or_kid)
 
     if frm_kid is None:
         sender_did_doc = await resolvers_config.did_resolver.resolve(frm_did)
         if sender_did_doc is None:
             raise DIDDocNotResolvedError(frm_did)
-        if not sender_did_doc.key_agreement_kids:
+        if not sender_did_doc.key_agreement:
             raise DIDUrlNotFoundError(
                 f"No keyAgreement verification relationships are found for DID `{frm_did}`"
             )
-        sender_kids = sender_did_doc.key_agreement_kids
+        sender_kids = sender_did_doc.key_agreement
     else:
         sender_kids = [frm_kid]
 
     recipient_did_doc = await resolvers_config.did_resolver.resolve(to_did)
     if recipient_did_doc is None:
         raise DIDDocNotResolvedError(to_did)
 
     if to_kid is None:
-        if not recipient_did_doc.key_agreement_kids:
+        if not recipient_did_doc.key_agreement:
             raise DIDUrlNotFoundError(
                 f"No keyAgreement verification relationships are found for DID `{to_did}`"
             )
-        recipient_kids = recipient_did_doc.key_agreement_kids
+        recipient_kids = recipient_did_doc.key_agreement
     else:
-        if to_kid not in recipient_did_doc.key_agreement_kids:
+        if to_kid not in recipient_did_doc.key_agreement:
             raise DIDUrlNotFoundError(
                 f"DID URL `{to_kid}` is not found in keyAgreement verification relationships of DID `{to_did}`"
             )
         recipient_kids = [to_kid]
 
     secret_found = False
     for skid in sender_kids:
@@ -100,15 +100,15 @@
             f"No secrets are found in secrets resolver for DID URLs: {to_kids}"
         )
 
     frm_did = get_did(frm_kid)
     sender_did_doc = await resolvers_config.did_resolver.resolve(frm_did)
     if sender_did_doc is None:
         raise DIDDocNotResolvedError(frm_did)
-    if not sender_did_doc.key_agreement_kids:
+    if not sender_did_doc.key_agreement:
         raise DIDUrlNotFoundError(
             f"No keyAgreement verification relationships are found for DID `{frm_did}`"
         )
     sender_verification_method = sender_did_doc.get_verification_method(frm_kid)
     if sender_verification_method is None:
         raise DIDUrlNotFoundError(f"Verification method `{frm_kid}` is not found")
```

### Comparing `didcomm-0.3.1/didcomm/core/keys/sign_keys_selector.py` & `didcomm-0.3.2/didcomm/core/keys/sign_keys_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ) -> VerificationMethod:
     did = get_did(frm_kid)
 
     did_doc = await resolvers_config.did_resolver.resolve(did)
     if did_doc is None:
         raise DIDDocNotResolvedError(did)
 
-    if frm_kid not in did_doc.authentication_kids:
+    if frm_kid not in did_doc.authentication:
         raise DIDUrlNotFoundError(
             f"DID URL `{frm_kid}` is not found in authentication verification relationships of DID `{did}`"
         )
 
     verification_method = did_doc.get_verification_method(frm_kid)
     if verification_method is None:
         raise DIDUrlNotFoundError(f"Verification method `{frm_kid}` is not found")
@@ -56,25 +56,25 @@
 async def _find_signing_key_by_did(
     frm_did: DID_OR_DID_URL, resolvers_config: ResolversConfig
 ) -> Secret:
     did_doc = await resolvers_config.did_resolver.resolve(frm_did)
     if did_doc is None:
         raise DIDDocNotResolvedError(frm_did)
 
-    if not did_doc.authentication_kids:
+    if not did_doc.authentication:
         raise DIDUrlNotFoundError(
             f"No authentication verification relationships are found for DID `{frm_did}`"
         )
 
     secret_ids = await resolvers_config.secrets_resolver.get_keys(
-        did_doc.authentication_kids
+        did_doc.authentication
     )
     if not secret_ids:
         raise SecretNotFoundError(
-            f"No secrets are found in secrets resolver for DID URLs: {did_doc.authentication_kids}"
+            f"No secrets are found in secrets resolver for DID URLs: {did_doc.authentication}"
         )
 
     kid = secret_ids[0]
     secret = await resolvers_config.secrets_resolver.get_key(kid)
     if secret is None:
         raise SecretNotFoundError(f"Secret `{kid}` is not found in secrets resolver")
```

### Comparing `didcomm-0.3.1/didcomm/core/serialization.py` & `didcomm-0.3.2/didcomm/core/serialization.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/core/sign.py` & `didcomm-0.3.2/didcomm/core/sign.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/core/types.py` & `didcomm-0.3.2/didcomm/core/types.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/core/utils.py` & `didcomm-0.3.2/didcomm/core/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,33 +41,24 @@
     return res
 
 
 def extract_key(
     method: Union[VerificationMethod, Secret], align_kid=False
 ) -> AsymmetricKey:
     if isinstance(method, VerificationMethod):
-        return _extract_key_from_verifciation_method(method, align_kid)
+        return _extract_key_from_verification_method(method, align_kid)
     else:
         return _extract_key_from_secret(method, align_kid)
 
 
-def _extract_key_from_verifciation_method(
+def _extract_key_from_verification_method(
     verification_method: VerificationMethod, align_kid
 ) -> AsymmetricKey:
     if verification_method.type == VerificationMethodType.JSON_WEB_KEY_2020:
-        if (
-            verification_method.verification_material.format
-            != VerificationMaterialFormat.JWK
-        ):
-            raise DIDCommValueError(
-                f"Verification material format {verification_method.verification_material.format} "
-                f"is not supported for verification method type {verification_method.type}"
-            )
-
-        jwk = json_str_to_dict(verification_method.verification_material.value)
+        jwk = verification_method.public_key_jwk
 
         if align_kid:
             jwk["kid"] = verification_method.id
 
         if jwk["kty"] == "EC":
             return ECKey.import_key(jwk)
         elif jwk["kty"] == "OKP":
@@ -75,24 +66,15 @@
         else:
             raise DIDCommValueError(f"JWK key type {jwk['kty']} is not supported")
 
     elif verification_method.type in [
         VerificationMethodType.X25519_KEY_AGREEMENT_KEY_2019,
         VerificationMethodType.ED25519_VERIFICATION_KEY_2018,
     ]:
-        if (
-            verification_method.verification_material.format
-            != VerificationMaterialFormat.BASE58
-        ):
-            raise DIDCommValueError(
-                f"Verification material format {verification_method.verification_material.format} "
-                f"is not supported for verification method type {verification_method.type}"
-            )
-
-        raw_value = base58.b58decode(verification_method.verification_material.value)
+        raw_value = base58.b58decode(verification_method.public_key_base58)
         base64url_value = urlsafe_b64encode(raw_value)
 
         jwk = {
             "kty": "OKP",
             "crv": "X25519"
             if verification_method.type
             == VerificationMethodType.X25519_KEY_AGREEMENT_KEY_2019
@@ -105,32 +87,23 @@
 
         return OKPKey.import_key(jwk)
 
     elif verification_method.type in [
         VerificationMethodType.X25519_KEY_AGREEMENT_KEY_2020,
         VerificationMethodType.ED25519_VERIFICATION_KEY_2020,
     ]:
-        if (
-            verification_method.verification_material.format
-            != VerificationMaterialFormat.MULTIBASE
-        ):
-            raise DIDCommValueError(
-                f"Verification material format {verification_method.verification_material.format} "
-                f"is not supported for verification method type {verification_method.type}"
-            )
-
         # Currently only base58btc encoding is supported in scope of multibase support
-        if verification_method.verification_material.value.startswith("z"):
+        if verification_method.public_key_multibase.startswith("z"):
             prefixed_raw_value = base58.b58decode(
-                verification_method.verification_material.value[1:]
+                verification_method.public_key_multibase[1:]
             )
         else:
             raise DIDCommValueError(
                 f"Multibase keys containing internally Base58 values only are currently supported "
-                f"but got the value: {verification_method.verification_material.value}"
+                f"but got the value: {verification_method.public_key_multibase}"
             )
 
         codec, raw_value = _from_multicodec(prefixed_raw_value)
 
         expected_codec = (
             _Codec.X25519_PUB
             if verification_method.type
@@ -302,21 +275,23 @@
 
     prefix = varint.encode(prefix_int)
     return codec, value[len(prefix) :]
 
 
 def extract_sign_alg(method: Union[VerificationMethod, Secret]) -> SignAlg:
     if method.type == VerificationMethodType.JSON_WEB_KEY_2020:
-        if method.verification_material.format != VerificationMaterialFormat.JWK:
-            raise DIDCommValueError(
-                f"Verification material format {method.verification_material.format} "
-                f"is not supported for verification method type {method.type}"
-            )
-
-        jwk = json_str_to_dict(method.verification_material.value)
+        if isinstance(method, Secret):
+            if method.verification_material.format != VerificationMaterialFormat.JWK:
+                raise DIDCommValueError(
+                    f"Verification material format {method.verification_material.format} "
+                    f"is not supported for verification method type {method.type}"
+                )
+            jwk = json_str_to_dict(method.verification_material.value)
+        else:
+            jwk = method.public_key_jwk  # instance of VerificationMethod
 
         if jwk["kty"] == "EC" and jwk["crv"] == "P-256":
             return SignAlg.ES256
         elif jwk["kty"] == "EC" and jwk["crv"] == "secp256k1":
             return SignAlg.ES256K
         elif jwk["kty"] == "OKP" and jwk["crv"] == "Ed25519":
             return SignAlg.ED25519
@@ -349,62 +324,84 @@
     if isinstance(v, (str, DID)):
         parts = str(v).split(":")
         return len(parts) >= 3 and parts[0] == "did" and all(parts)
     return False
 
 
 # TODO TEST
-def is_did_url(v: Any) -> bool:
+def is_did_with_uri_fragment(v: Any) -> bool:
     # TODO
     #   - consider other presentations (e.g bytes)
     #   - verifications for after-did parts
     #     (https://www.w3.org/TR/did-core/#did-url-syntax)
     if isinstance(v, (str, DID_URL)):
         before, sep, after = str(v).partition("#")  # always 3-tuple
         return sep and after and is_did(before)
     return False
 
 
 # TODO TEST
 def is_did_or_did_url(v: Any) -> bool:
-    return is_did(v) or is_did_url(v)
+    return is_did(v) or is_did_with_uri_fragment(v)
 
 
 def get_did(did_or_did_url: DID_OR_DID_URL) -> DID:
     return did_or_did_url.partition("#")[0]
 
 
 def get_did_and_optionally_kid(did_or_kid: DID_OR_DID_URL) -> (DID, Optional[DID_URL]):
-    if is_did_url(did_or_kid):
+    if is_did_with_uri_fragment(did_or_kid):
         did = get_did(did_or_kid)
         kid = did_or_kid
     else:
         did = did_or_kid
         kid = None
     return did, kid
 
 
+class _Crv(Enum):
+    ED25519 = "Ed25519"
+    X25519 = "X25519"
+
+
+def _get_crv_for_verification_method(
+    key: Union[VerificationMethod, Secret],
+) -> Optional[str]:
+    if key.type in {
+        VerificationMethodType.ED25519_VERIFICATION_KEY_2020,
+        VerificationMethodType.ED25519_VERIFICATION_KEY_2018,
+    }:
+        return _Crv.ED25519.value
+    elif key.type in {
+        VerificationMethodType.X25519_KEY_AGREEMENT_KEY_2020,
+        VerificationMethodType.X25519_KEY_AGREEMENT_KEY_2019,
+    }:
+        return _Crv.X25519.value
+    elif key.type is VerificationMethodType.JSON_WEB_KEY_2020:
+        jwk = (
+            json_str_to_dict(key.verification_material.value)
+            if isinstance(key, Secret)
+            else key.public_key_jwk
+        )
+        return jwk["crv"]
+    else:
+        return None
+
+
 def are_keys_compatible(
     method1: Union[Secret, VerificationMethod], method2: VerificationMethod
 ) -> bool:
-    if method1.type == method2.type and (
-        method1.verification_material.format == method2.verification_material.format
-    ):
-        if method1.verification_material.format == VerificationMaterialFormat.JWK:
-            private_jwk = json_str_to_dict(method1.verification_material.value)
-            public_jwk = json_str_to_dict(method2.verification_material.value)
-            return (
-                private_jwk["kty"] == public_jwk["kty"]
-                and private_jwk["crv"] == public_jwk["crv"]
-            )
-        else:
-            return True
-    else:
+    crv_1 = _get_crv_for_verification_method(method1)
+    crv_2 = _get_crv_for_verification_method(method2)
+
+    if crv_1 is None or crv_2 is None:
         return False
 
+    return crv_1 == crv_2
+
 
 def parse_base64url_encoded_json(base64url):
     return json_str_to_dict(to_unicode(urlsafe_b64decode(to_bytes(base64url))))
 
 
 def get_jwe_alg(jwe: dict) -> Optional[str]:
     if "protected" not in jwe:
```

### Comparing `didcomm-0.3.1/didcomm/core/validation.py` & `didcomm-0.3.2/didcomm/core/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from authlib.common.encoding import to_bytes, urlsafe_b64decode, to_unicode
 
-from didcomm.core.utils import is_did_url, parse_base64url_encoded_json, calculate_apv
+from didcomm.core.utils import (
+    is_did_with_uri_fragment,
+    parse_base64url_encoded_json,
+    calculate_apv,
+)
 from didcomm.errors import MalformedMessageError, MalformedMessageCode
 
 
 def validate_jws(msg: dict):
     if (
         "signatures" not in msg
         or not msg["signatures"]
@@ -34,28 +38,28 @@
 def validate_authcrypt_jwe(msg: dict):
     # 1. Validate recipient unprotected header
     if "recipients" not in msg:
         raise MalformedMessageError(MalformedMessageCode.INVALID_MESSAGE)
     for r in msg["recipients"]:
         if "header" not in r or "kid" not in r["header"]:
             raise MalformedMessageError(MalformedMessageCode.INVALID_MESSAGE)
-        if not is_did_url(r["header"]["kid"]):
+        if not is_did_with_uri_fragment(r["header"]["kid"]):
             raise MalformedMessageError(MalformedMessageCode.INVALID_MESSAGE)
 
     # 2. Decode protected header
     protected_header = _get_protected_header(msg)
 
     # 3. Check apu
     if "apu" not in protected_header:
         raise MalformedMessageError(MalformedMessageCode.INVALID_MESSAGE)
     try:
         apu = to_unicode(urlsafe_b64decode(to_bytes(protected_header["apu"])))
     except Exception as exc:
         raise MalformedMessageError(MalformedMessageCode.INVALID_MESSAGE) from exc
-    if not is_did_url(apu):
+    if not is_did_with_uri_fragment(apu):
         raise MalformedMessageError(MalformedMessageCode.INVALID_MESSAGE)
 
     # 4. Check skid
     if "skid" in protected_header and protected_header["skid"] != apu:
         raise MalformedMessageError(MalformedMessageCode.INVALID_MESSAGE)
 
     # 5. Check apv
```

### Comparing `didcomm-0.3.1/didcomm/core/validators.py` & `didcomm-0.3.2/didcomm/core/validators.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,50 +2,72 @@
 from typing import Callable, Any, Optional
 from packaging.specifiers import SpecifierSet
 from urllib.parse import urlparse
 from pathlib import Path
 
 from didcomm.errors import DIDCommValueError
 from didcomm.core.types import DIDCOMM_ORG_DOMAIN
-from didcomm.core.utils import is_did, is_did_url, is_did_or_did_url
+from didcomm.core.utils import is_did, is_did_with_uri_fragment, is_did_or_did_url
 
 
 # TODO TEST
 def _attr_validator_wrapper(attr_validator):
     def _f(instance, attribute, value):
         try:
             attr_validator(instance, attribute, value)
         except Exception as exc:
             raise DIDCommValueError(str(exc)) from exc
 
     return _f
 
 
+def validator__optional(validator: Callable) -> Callable:
+    return _attr_validator_wrapper(attr.validators.optional(validator))
+
+
 # TODO TEST
 def validator__instance_of(classinfo) -> Callable:
     return _attr_validator_wrapper(attr.validators.instance_of(classinfo))
 
 
+def validator__and_(*validators: Callable):
+    return _attr_validator_wrapper(attr.validators.and_(*validators))
+
+
 # TODO TEST
 def validator__in_(options) -> Callable:
     return _attr_validator_wrapper(attr.validators.in_(options))
 
 
+def validator__not_in_(options) -> Callable:
+    return _attr_validator_wrapper(attr.validators.not_(attr.validators.in_(options)))
+
+
 # TODO TEST
 def validator__deep_iterable(member_validator: Callable, iterable_validator=None):
     return _attr_validator_wrapper(
         attr.validators.deep_iterable(member_validator, iterable_validator)
     )
 
 
 # TODO TEST
+def validator__deep_mapping(
+    key_validator: Callable,
+    value_validator: Callable,
+    mapping_validator: Callable = None,
+):
+    return _attr_validator_wrapper(
+        attr.validators.deep_mapping(key_validator, value_validator, mapping_validator)
+    )
+
+
+# TODO TEST
 def validator__didcomm_protocol_mturi(
     p_name: str, p_version_specifier: SpecifierSet, p_msg_t: str
 ) -> Callable:
-
     # TODO strict check as per
     #      https://github.com/hyperledger/aries-rfcs/blob/main/concepts/0003-protocols/README.md#mturi
     def _f(instance, attribute, value):
         parsed = urlparse(value)
         path = Path(parsed.path)
 
         if not (
@@ -80,21 +102,23 @@
         except Exception as cause:
             raise DIDCommValueError(exc_msg) from cause
 
     return _f
 
 
 # TODO TEST
-def validator__did(instance, attribute, value) -> None:
-    validator__check_f(is_did, "is not a did")(instance, attribute, value)
+def validator__did() -> Callable:
+    return validator__check_f(is_did, "is not a did")
 
 
 # TODO TEST
 def validator__did_url(instance, attribute, value) -> None:
-    validator__check_f(is_did_url, "is not a did url")(instance, attribute, value)
+    validator__check_f(is_did_with_uri_fragment, "is not a did url with a fragment")(
+        instance, attribute, value
+    )
 
 
 # TODO TEST
 def validator__did_or_did_url(instance, attribute, value) -> None:
     validator__check_f(is_did_or_did_url, "is neither a did nor a did url")(
         instance, attribute, value
     )
```

### Comparing `didcomm-0.3.1/didcomm/did_doc/did_resolver.py` & `didcomm-0.3.2/didcomm/did_doc/did_resolver.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/errors.py` & `didcomm-0.3.2/didcomm/errors.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/pack_encrypted.py` & `didcomm-0.3.2/didcomm/pack_encrypted.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
-from typing import Optional, List
+from typing import Optional, List, Union
 
 from didcomm.common.algorithms import AuthCryptAlg, AnonCryptAlg
 from didcomm.common.resolvers import ResolversConfig
 from didcomm.common.types import JSON, JSON_OBJ, DID_OR_DID_URL, DID_URL
 from didcomm.core.anoncrypt import anoncrypt, find_keys_and_anoncrypt
 from didcomm.core.authcrypt import find_keys_and_authcrypt
 from didcomm.core.defaults import DEF_ENC_ALG_AUTH, DEF_ENC_ALG_ANON
 from didcomm.core.serialization import dict_to_json
 from didcomm.core.sign import sign
 from didcomm.core.types import EncryptResult, SignResult, DIDCommGeneratorType
 from didcomm.core.utils import get_did, is_did, didcomm_id_generator_default
 from didcomm.did_doc.did_doc import DIDCommService
 from didcomm.errors import DIDCommValueError
 from didcomm.core.from_prior import pack_from_prior_in_place
-from didcomm.message import Message, Header
+from didcomm.message import Message, Headers
 from didcomm.protocols.routing.forward import (
     wrap_in_forward,
     resolve_did_services_chain,
     ForwardPackResult,
 )
 
 logger = logging.getLogger(__name__)
 
 
 async def pack_encrypted(
     resolvers_config: ResolversConfig,
-    message: Message,
+    message: Union[Message, JSON_OBJ],
     to: DID_OR_DID_URL,
     frm: Optional[DID_OR_DID_URL] = None,
     sign_frm: Optional[DID_OR_DID_URL] = None,
     pack_config: Optional[PackEncryptedConfig] = None,
     pack_params: Optional[PackEncryptedParameters] = None,
 ) -> PackEncryptedResult:
     """
@@ -105,34 +105,34 @@
              and an optional service metadata with an endpoint to be used to transport the packed message.
     :rtype: PackEncryptedResult
     """
 
     pack_config = pack_config or PackEncryptedConfig()
     pack_params = pack_params or PackEncryptedParameters()
 
+    if isinstance(message, Message):
+        message = message.as_dict()
+
     # 1. validate message
     __validate(message, to, frm, sign_frm)
 
-    # 2. message as dict
-    msg_as_dict = message.as_dict()
-
     # 3. Pack from_prior in place
     from_prior_issuer_kid = await pack_from_prior_in_place(
-        msg_as_dict,
+        message,
         resolvers_config,
         pack_params.from_prior_issuer_kid,
     )
 
     # 4. sign if needed
-    sign_res = await __sign_if_needed(resolvers_config, msg_as_dict, sign_frm)
+    sign_res = await __sign_if_needed(resolvers_config, message, sign_frm)
 
     # 5. encrypt
     encrypt_res = await __encrypt(
         resolvers_config,
-        msg=sign_res.msg if sign_res else msg_as_dict,
+        msg=sign_res.msg if sign_res else message,
         to=to,
         frm=frm,
         pack_config=pack_config,
     )
 
     # 6. protected sender ID if needed
     encrypt_res_protected = __protected_sender_id_if_needed(encrypt_res, pack_config)
@@ -257,24 +257,24 @@
             for forward messages ``id`` generation, ``didcomm_id_generator_default``
             is used by default
         from_prior_issuer_kid (DID_URL): If from_prior is specified in the source message,
             this field can explicitly specify which key to use for signing from_prior
             in the packed message
     """
 
-    forward_headers: Optional[Header] = None
+    forward_headers: Optional[Headers] = None
     forward_service_id: Optional[str] = None
     forward_didcomm_id_generator: Optional[
         DIDCommGeneratorType
     ] = didcomm_id_generator_default
     from_prior_issuer_kid: Optional[DID_URL] = None
 
 
 def __validate(
-    message: Message,
+    message: JSON_OBJ,
     to: DID_OR_DID_URL,
     frm: Optional[DID_OR_DID_URL] = None,
     sign_frm: Optional[DID_OR_DID_URL] = None,
 ):
     if not is_did(to):
         raise DIDCommValueError(f"`to` value is not a valid DID of DID URL: {to}")
 
@@ -282,25 +282,27 @@
         raise DIDCommValueError(f"`from` value is not a valid DID of DID URL: {frm}")
 
     if sign_frm is not None and not is_did(sign_frm):
         raise DIDCommValueError(
             f"`sign_from` value is not a valid DID of DID URL: {sign_frm}"
         )
 
-    if message.to is not None and not isinstance(message.to, List):
-        raise DIDCommValueError(f"`message.to` value is not a list: {message.to}")
+    message_to = message.get("to")
+    if message_to is not None and not isinstance(message_to, List):
+        raise DIDCommValueError(f"message `to` value is not a list: {message_to}")
 
-    if message.to is not None and get_did(to) not in message.to:
+    if message_to is not None and get_did(to) not in message_to:
         raise DIDCommValueError(
-            f"`message.to` value {message.to} does not contain `to` value's DID {get_did(to)}"
+            f"message `to` value {message_to} does not contain `to` value's DID {get_did(to)}"
         )
 
-    if frm is not None and message.frm is not None and get_did(frm) != message.frm:
+    message_from = message.get("from")
+    if frm is not None and message_from is not None and get_did(frm) != message_from:
         raise DIDCommValueError(
-            f"`message.from` value {message.frm} is not equal to `from` value's DID {get_did(frm)}"
+            f"message `from` value {message_from} is not equal to `from` value's DID {get_did(frm)}"
         )
 
 
 async def __sign_if_needed(
     resolvers_config: ResolversConfig,
     msg: dict,
     sign_frm: Optional[DID_OR_DID_URL] = None,
@@ -340,15 +342,14 @@
     resolvers_config: ResolversConfig,
     packed_msg: JSON_OBJ,
     to: DID_OR_DID_URL,
     did_services_chain: List[DIDCommService],
     pack_config: PackEncryptedConfig,
     pack_params: PackEncryptedParameters,
 ) -> Optional[ForwardPackResult]:
-
     if not pack_config.forward:
         logger.debug("forward is turned off")
         return None
 
     # build routing keys them using recipient service information
     if not did_services_chain:
         logger.debug("No service endpoint found: skipping forward wrapping")
```

### Comparing `didcomm-0.3.1/didcomm/pack_plaintext.py` & `didcomm-0.3.2/didcomm/pack_plaintext.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Optional
+from typing import Optional, Union
 
 from didcomm.common.resolvers import ResolversConfig
-from didcomm.common.types import JSON, DID_URL
+from didcomm.common.types import JSON, DID_URL, JSON_OBJ
 from didcomm.core.serialization import dict_to_json
 from didcomm.core.from_prior import pack_from_prior_in_place
 from didcomm.message import Message
 
 
 async def pack_plaintext(
     resolvers_config: ResolversConfig,
-    message: Message,
+    message: Union[Message, JSON_OBJ],
     pack_params: Optional[PackPlaintextParameters] = None,
 ) -> PackPlaintextResult:
     """
     Produces `DIDComm Plaintext Messages`
     https://identity.foundation/didcomm-messaging/spec/#didcomm-plaintext-messages.
 
     A DIDComm message in its plaintext form that
@@ -37,15 +37,16 @@
     :raises DIDNotResolvedError: If a DID or DID URL (key ID) can not be resolved or not found
     :raises SecretNotResolvedError: If there is no secret for the given DID or DID URL (key ID)
 
     :return: PackPlaintextResult
     """
     pack_params = pack_params or PackPlaintextParameters()
 
-    message = message.as_dict()
+    if isinstance(message, Message):
+        message = message.as_dict()
 
     from_prior_issuer_kid = await pack_from_prior_in_place(
         message,
         resolvers_config,
         pack_params.from_prior_issuer_kid,
     )
```

### Comparing `didcomm-0.3.1/didcomm/pack_signed.py` & `didcomm-0.3.2/didcomm/pack_signed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Optional
+from typing import Optional, Union
 
 from didcomm.common.resolvers import ResolversConfig
-from didcomm.common.types import JSON, DID_OR_DID_URL, DID_URL
+from didcomm.common.types import JSON, DID_OR_DID_URL, DID_URL, JSON_OBJ
 from didcomm.core.serialization import dict_to_json
 from didcomm.core.sign import sign
 from didcomm.core.utils import is_did
 from didcomm.errors import DIDCommValueError
 from didcomm.core.from_prior import pack_from_prior_in_place
 from didcomm.message import Message
 
 
 async def pack_signed(
     resolvers_config: ResolversConfig,
-    message: Message,
+    message: Union[Message, JSON_OBJ],
     sign_frm: DID_OR_DID_URL,
     pack_params: Optional[PackSignedParameters] = None,
 ) -> PackSignedResult:
     """
     Produces `DIDComm Signed Message`
     https://identity.foundation/didcomm-messaging/spec/#didcomm-signed-message.
 
@@ -51,15 +51,17 @@
     :raises DIDCommValueError: If invalid input is provided.
 
     :return: PackSignedResult
     """
     pack_params = pack_params or PackSignedParameters()
 
     __validate(sign_frm)
-    message = message.as_dict()
+
+    if isinstance(message, Message):
+        message = message.as_dict()
 
     from_prior_issuer_kid = await pack_from_prior_in_place(
         message,
         resolvers_config,
         pack_params.from_prior_issuer_kid,
     )
```

### Comparing `didcomm-0.3.1/didcomm/protocols/routing/forward.py` & `didcomm-0.3.2/didcomm/protocols/routing/forward.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from copy import deepcopy
 
 import logging
 import attr
 from dataclasses import dataclass
-from typing import List, Union, Optional, Callable, Dict
+from typing import List, Union, Optional, Dict
 from packaging.specifiers import SpecifierSet
 from enum import Enum
 
 from didcomm.errors import (
     MalformedMessageError,
     MalformedMessageCode,
     DIDDocNotResolvedError,
@@ -20,18 +20,17 @@
     DID_OR_DID_URL,
     JSON_OBJ,
     DID_URL,
     DIDCommMessageProtocolTypes,
 )
 from didcomm.common.resolvers import ResolversConfig
 from didcomm.common.algorithms import AnonCryptAlg
-from didcomm.message import GenericMessage, Header, Attachment, AttachmentDataJson
+from didcomm.message import GenericMessage, Headers, Attachment, AttachmentDataJson
 from didcomm.core.types import EncryptResult, DIDCommGeneratorType, DIDCOMM_ORG_DOMAIN
 from didcomm.core.defaults import DEF_ENC_ALG_ANON
-from didcomm.core.converters import converter__didcomm_id
 from didcomm.core.validators import (
     validator__instance_of,
     validator__didcomm_protocol_mturi,
     validator__did_or_did_url,
 )
 from didcomm.core.serialization import (
     json_str_to_dict,
@@ -66,20 +65,14 @@
     next: DID_OR_DID_URL = attr.ib(
         validator=validator__did_or_did_url,
     )
 
 
 @attr.s(auto_attribs=True)
 class ForwardMessage(GenericMessage[ForwardBody]):
-    # if not specified would be auto-generated
-    id: Optional[Union[str, Callable]] = attr.ib(
-        converter=converter__didcomm_id,
-        validator=validator__instance_of(str),
-        default=None,
-    )
     type: Optional[str] = attr.ib(
         validator=[
             validator__instance_of(str),
             validator__didcomm_protocol_mturi(
                 ROUTING_PROTOCOL_NAME,
                 ROUTING_PROTOCOL_VER_COMPATIBILITY,
                 ROUTING_PROTOCOL_MSG_TYPES.FORWARD.value,
@@ -132,16 +125,15 @@
     forward_msg: ForwardMessage
     forwarded_msg: JSON_OBJ
     forwarded_msg_encrypted_to: Optional[List[DID_URL]] = None
 
 
 async def find_did_service(
     resolvers_config: ResolversConfig, to: DID_OR_DID_URL, service_id: str = None
-) -> DIDCommService:
-
+) -> Optional[DIDCommService]:
     to_did = get_did(to)
     did_doc = await resolvers_config.did_resolver.resolve(to_did)
 
     if did_doc is None:
         raise DIDDocNotResolvedError(to_did)
 
     if service_id:
@@ -159,27 +151,27 @@
         return did_service
     else:
         # Find the first service accepting `didcomm/v2` profile because the spec states:
         # > Entries SHOULD be specified in order of receiver preference,
         # > but any endpoint MAY be selected by the sender, typically
         # > by protocol availability or preference.
         # https://identity.foundation/didcomm-messaging/spec/#multiple-endpoints
-        for did_service in did_doc.didcomm_services:
-            if PROFILE_DIDCOMM_V2 in did_service.accept:
-                return did_service
+        if did_doc.service:
+            for did_service in did_doc.service:
+                if PROFILE_DIDCOMM_V2 in did_service.accept:
+                    return did_service
         return None
 
 
 async def resolve_did_services_chain(
     resolvers_config: ResolversConfig,
     to: DID_OR_DID_URL,
     service_id: str = None,
     did_recursion=False,
 ) -> List[DIDCommService]:
-
     res = []
 
     to_did_service = await find_did_service(resolvers_config, to, service_id)
     if to_did_service is None:
         return res
 
     service_uri = to_did_service.service_endpoint
@@ -214,30 +206,30 @@
 
 async def wrap_in_forward(
     resolvers_config: ResolversConfig,
     packed_msg: JSON_OBJ,
     to: DID_OR_DID_URL,
     routing_keys: List[DID_OR_DID_URL],
     enc_alg_anon: Optional[AnonCryptAlg] = DEF_ENC_ALG_ANON,
-    headers: Optional[Header] = None,
+    headers: Optional[Headers] = None,
     didcomm_id_generator: Optional[DIDCommGeneratorType] = None,
 ) -> Optional[ForwardPackResult]:
     """
     Resolves recipient DID DOC Service and Builds Forward envelops if needed.
 
     Wraps the given packed DIDComm message in Forward messages for every routing key.
 
     :param resolvers_config: secrets and DIDDoc resolvers
     :param packed_msg: the message to be wrapped in Forward messages
     :param to: recipient's DID (DID URL)
     :param routing_keys: list of routing keys
-    :param enc_alg_anon (AnonCryptAlg): The encryption algorithm to be used for
+    :param enc_alg_anon: (AnonCryptAlg), The encryption algorithm to be used for
         anonymous encryption (anon_crypt).
     :param headers: optional headers for Forward message
-    :param didcomm_id_generator (Callable): optional callable to use
+    :param didcomm_id_generator: (Callable), optional callable to use
         for forward messages ``id`` generation, ``didcomm_id_generator_default``
         is used by default
 
     :raises DIDDocNotResolvedError: If a DID can not be resolved to a DID Doc.
     :raises DIDUrlNotFoundError: If a DID URL (for example a key ID) is not found within a DID Doc
     :raises SecretNotFoundError: If there is no secret for the given DID or DID URL (key ID)
```

### Comparing `didcomm-0.3.1/didcomm/secrets/secrets_resolver.py` & `didcomm-0.3.2/didcomm/secrets/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/secrets/secrets_resolver_demo.py` & `didcomm-0.3.2/didcomm/secrets/secrets_resolver_demo.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/secrets/secrets_resolver_in_memory.py` & `didcomm-0.3.2/didcomm/secrets/secrets_resolver_in_memory.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/secrets/secrets_util.py` & `didcomm-0.3.2/didcomm/secrets/secrets_util.py`

 * *Files identical despite different names*

### Comparing `didcomm-0.3.1/didcomm/unpack.py` & `didcomm-0.3.2/didcomm/unpack.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Optional, List, Union
+from typing import Any, Callable, Optional, List, Union
 
 from authlib.common.encoding import to_unicode
 
 from didcomm.common.algorithms import AnonCryptAlg, AuthCryptAlg, SignAlg
 from didcomm.common.resolvers import ResolversConfig
 from didcomm.common.types import JWS, JSON, JSON_OBJ, DID_URL
 from didcomm.core.anoncrypt import unpack_anoncrypt, is_anoncrypted
@@ -23,21 +23,23 @@
 from didcomm.protocols.routing.forward import is_forward, ForwardMessage
 
 
 async def unpack(
     resolvers_config: ResolversConfig,
     packed_msg: Union[JSON, JSON_OBJ],
     unpack_config: Optional[UnpackConfig] = None,
+    deserializer: Callable[[JSON_OBJ], Any] = Message.from_dict,
 ) -> UnpackResult:
     """
     Unpacks the packed DIDComm message by doing decryption and verifying the signatures.
 
     :param resolvers_config: secrets and DIDDoc resolvers
     :param packed_msg: packed DIDComm message as JSON string of JSON_OBJ to be unpacked
     :param unpack_config: configuration for unpack. Default parameters are used if not specified.
+    :param deserializer: callable taking a json object and deserializes to desired message type. If not specified, defaults to returning a dictionary.
 
     :raises DIDDocNotResolvedError: If a DID can not be resolved to a DID Doc.
     :raises DIDUrlNotFoundError: If a DID URL (for example a key ID) is not found within a DID Doc
     :raises SecretNotFoundError: If there is no secret for the given DID or DID URL (key ID)
     :raises MalformedMessageError: if the message is invalid (can not be decrypted, signature is invalid, the message is invalid, etc.)
 
     :return: the message, metadata, and optionally a JWS if the message has been signed.
@@ -57,22 +59,25 @@
     metadata = Metadata(
         encrypted=False,
         authenticated=False,
         non_repudiation=False,
         anonymous_sender=False,
     )
 
-    return await _do_unpack(resolvers_config, packed_msg, unpack_config, metadata)
+    return await _do_unpack(
+        resolvers_config, packed_msg, unpack_config, metadata, deserializer
+    )
 
 
 async def _do_unpack(
     resolvers_config: ResolversConfig,
     packed_msg: JSON_OBJ,
     unpack_config: UnpackConfig,
     metadata: Metadata,
+    deserializer: Callable[[JSON_OBJ], Any],
 ) -> UnpackResult:
     msg = dict_to_json_bytes(packed_msg)
     msg_as_dict = packed_msg
 
     if is_anoncrypted(msg_as_dict):
         unwrap_anoncrypt_result = await unpack_anoncrypt(
             msg_as_dict,
@@ -88,15 +93,19 @@
         metadata.enc_alg_anon = unwrap_anoncrypt_result.alg
 
         if unpack_config.unwrap_re_wrapping_forward and is_forward(msg_as_dict):
             fwd_msg = ForwardMessage.from_json(msg)
             if await has_keys_for_forward_next(fwd_msg.body.next, resolvers_config):
                 metadata.re_wrapped_in_forward = True
                 return await _do_unpack(
-                    resolvers_config, fwd_msg.forwarded_msg, unpack_config, metadata
+                    resolvers_config,
+                    fwd_msg.forwarded_msg,
+                    unpack_config,
+                    metadata,
+                    deserializer,
                 )
 
     if is_authcrypted(msg_as_dict):
         unwrap_authcrypt_result = await unpack_authcrypt(
             msg_as_dict,
             resolvers_config,
             decrypt_by_all_keys=unpack_config.expect_decrypt_by_all_keys,
@@ -124,30 +133,30 @@
     if msg_as_dict.get("from_prior") is not None:
         metadata.from_prior_jwt = msg_as_dict["from_prior"]
     from_prior_issuer_kid = await unpack_from_prior_in_place(
         msg_as_dict, resolvers_config
     )
     metadata.from_prior_issuer_kid = from_prior_issuer_kid
 
-    message = Message.from_dict(msg_as_dict)
+    message = deserializer(msg_as_dict)
 
     return UnpackResult(message=message, metadata=metadata)
 
 
 @dataclass(frozen=True)
 class UnpackResult:
     """
     Result of unpack operation.
 
     Attributes:
-        message (Message): unpacked message consisting of headers and application/protocol specific data (body)
+        message (Any): unpacked message consisting of headers and application/protocol specific data (body)
         metadata (Metadata): metadata with details about the packed messaged. Can be used for MTC (message trust context) analysis.
     """
 
-    message: Message
+    message: Any
     metadata: Metadata
 
 
 @dataclass
 class Metadata:
     """
     Metadata with details about the packed messaged. Can be used for MTC (message trust context) analysis.
```

### Comparing `didcomm-0.3.1/pyproject.toml` & `didcomm-0.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "didcomm"
-version = "0.3.1"
+version = "0.3.2"
 description = "Basic DIDComm v2 support in python"
 authors = ["SICPA <DLCHOpenSourceContrib@sicpa.com>", "Daniel Bluhm <dbluhm@pm.me>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/sicpa-dlab/didcomm-python"
 repository = "https://github.com/sicpa-dlab/didcomm-python"
 classifiers = [
@@ -20,26 +20,26 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 Authlib = "^1.1.0"
 pycryptodomex = "~=3.10"
 base58 = "~=2.1"
 varint = "~=1.0.2"
-attrs = "~=21.2"
-packaging = "~=21.0"
+attrs = "~=22.2"
+packaging = "~=23.0"
+pydid = "~=0.3.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
-pytest-asyncio = "^0.19.0"
-pytest-xdist = "^2.5.0"
+pytest-asyncio = "^0.20.0"
+pytest-xdist = "^3.2.0"
 flake8 = "^5.0.4"
-black = "^22.10.0"
+black = "^23.1.0"
 pytest-mock = "^3.10.0"
-mock = "^4.0.3"
-tox = "^3.26.0"
+mock = "^5.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 mock_use_standalone_module = true
```

### Comparing `didcomm-0.3.1/setup.py` & `didcomm-0.3.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,234 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['didcomm',
- 'didcomm.common',
- 'didcomm.core',
- 'didcomm.core.keys',
- 'didcomm.did_doc',
- 'didcomm.protocols',
- 'didcomm.protocols.routing',
- 'didcomm.secrets']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Authlib>=1.1.0,<2.0.0',
- 'attrs>=21.2,<22.0',
- 'base58>=2.1,<3.0',
- 'packaging>=21.0,<22.0',
- 'pycryptodomex>=3.10,<4.0',
- 'varint>=1.0.2,<1.1.0']
-
-setup_kwargs = {
-    'name': 'didcomm',
-    'version': '0.3.1',
-    'description': 'Basic DIDComm v2 support in python',
-    'long_description': '# DIDComm Python\n\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Unit Tests](https://github.com/sicpa-dlab/didcomm-python/workflows/verify/badge.svg)](https://github.com/sicpa-dlab/didcomm-python/actions/workflows/verify.yml)\n[![Python Package](https://img.shields.io/pypi/v/didcomm)](https://pypi.org/project/didcomm/)\n\nBasic [DIDComm v2](https://identity.foundation/didcomm-messaging/spec) support in Python.\n\n## Installation\n```\npip install didcomm\n```\n\n## DIDComm + peerdid Demo\nSee https://github.com/sicpa-dlab/didcomm-demo.\n\n## Assumptions and Limitations\n- Python >= 3.7.\n- In order to use the library, `SecretsResolver` and `DIDResolver` interfaces must be implemented on the application level. \n  Implementation of that interfaces is out of DIDComm library scope.  \n  - Verification materials are expected in JWK, Base58 and Multibase (internally Base58 only) formats.\n    - In Base58 and Multibase formats, keys using only X25519 and Ed25519 curves are supported.\n    - For private keys in Base58 and Multibase formats, the verification material value contains both private and public parts (concatenated bytes).\n    - In Multibase format, bytes of the verification material value is prefixed with the corresponding Multicodec code.\n  - Key IDs (kids) used in `SecretsResolver` must match the corresponding key IDs from DID Doc verification methods.\n  - Key IDs (kids) in DID Doc verification methods and secrets must be a full [DID Fragment](https://www.w3.org/TR/did-core/#fragment), that is `did#key-id`.\n  - Verification methods referencing another DID Document are not supported (see [Referring to Verification Methods](https://www.w3.org/TR/did-core/#referring-to-verification-methods)).\n- The following curves and algorithms are supported:\n  - Encryption:\n     - Curves: X25519, P-384, P-256, P-521\n     - Content encryption algorithms: \n       - XC20P (to be used with ECDH-ES only, default for anoncrypt),\n       - A256GCM (to be used with ECDH-ES only),\n       - A256CBC-HS512 (default for authcrypt)\n     - Key wrapping algorithms: ECDH-ES+A256KW, ECDH-1PU+A256KW\n  - Signing:\n    - Curves: Ed25519, Secp256k1, P-256\n    - Algorithms: EdDSA (with crv=Ed25519), ES256, ES256K\n- Forward protocol is implemented and used by default.\n- DID rotation (`fromPrior` field) is supported.\n- DIDComm has been implemented under the following [Assumptions](https://hackmd.io/i3gLqgHQR2ihVFV5euyhqg)   \n\n\n## Examples\n\nSee [demo scripts](tests/demo) for details.\n\nA general usage of the API is the following:\n- Sender Side:\n  - Build a `Message` (plaintext, payload).\n  - Convert a message to a DIDComm Message for further transporting by calling one of the following:\n     - `pack_encrypted` to build an Encrypted DIDComm message\n     - `pack_signed` to build a Signed DIDComm message\n     - `pack_plaintext` to build a Plaintext DIDComm message\n- Receiver side:\n  - Call `unpack` on receiver side that will decrypt the message, verify signature if needed\n  and return a `Message` for further processing on the application level.\n\n### 1. Build an Encrypted DIDComm message for the given recipient\n\nThis is the most common DIDComm message to be used in most of the applications.\n\nA DIDComm encrypted message is an encrypted JWM (JSON Web Messages) that \n- hides its content from all but authorized recipients\n- (optionally) discloses and proves the sender to only those recipients\n- provides message integrity guarantees\n\nIt is important in privacy-preserving routing. It is what normally moves over network transports in DIDComm\napplications, and is the safest format for storing DIDComm data at rest.\n\nSee `pack_encrypted` documentation for more details.\n\n**Authentication encryption** example (most common case):\n\n```\n# ALICE\nmessage = Message(body={"aaa": 1, "bbb": 2},\n                  id="1234567890", type="my-protocol/1.0",\n                  frm=ALICE_DID, to=[BOB_DID])\npack_result = await pack_encrypted(message=message, frm=ALICE_DID, to=BOB_DID)\npacked_msg = pack_result.packed_msg\nprint(f"Sending ${packed_msg} to ${pack_result.service_metadata.service_endpoint}")\n\n# BOB\nunpack_result = await unpack(packed_msg)\nprint(f"Got ${unpack_result.message} message")\n```\n\n**Anonymous encryption** example:\n\n```\nmessage = Message(body={"aaa": 1, "bbb": 2},\n                  id="1234567890", type="my-protocol/1.0",\n                  frm=ALICE_DID, to=[BOB_DID])\npack_result = await pack_encrypted(message=message, to=BOB_DID)\n```\n\n**Encryption with non-repudiation** example:\n\n```\nmessage = Message(body={"aaa": 1, "bbb": 2},\n                  id="1234567890", type="my-protocol/1.0",\n                  frm=ALICE_DID, to=[BOB_DID])\npack_result = await pack_encrypted(message=message, frm=ALICE_DID, to=BOB_DID, sign_frm=ALICE_DID)\n```\n\n### 2. Build an unencrypted but Signed DIDComm message\n\nSigned messages are only necessary when\n- the origin of plaintext must be provable to third parties\n- or the sender can’t be proven to the recipient by authenticated encryption because the recipient is not known in advance (e.g., in a\nbroadcast scenario).\n \nAdding a signature when one is not needed can degrade rather than enhance security because it\nrelinquishes the sender’s ability to speak off the record.\n\nSee `pack_signed` documentation for more details.\n\n```\n# ALICE\nmessage = Message(body={"aaa": 1, "bbb": 2},\n                  id="1234567890", type="my-protocol/1.0",\n                  frm=ALICE_DID, to=[BOB_DID])\npacked_msg = await pack_signed(message=message, sign_frm=ALICE_DID)\npacked_msg = pack_result.packed_msg\nprint(f"Publishing ${packed_msg}")\n\n# BOB\nunpack_result = await unpack(packed_msg)\nprint(f"Got ${unpack_result.message} message signed as ${unpack_result.metadata.signed_message}")\n```\n\n### 3. Build a Plaintext DIDComm message\n\nA DIDComm message in its plaintext form that \n- is not packaged into any protective envelope\n- lacks confidentiality and integrity guarantees\n- repudiable\n\nThey are therefore not normally transported across security boundaries. \n\n```\n# ALICE\nmessage = Message(body={"aaa": 1, "bbb": 2},\n                  id="1234567890", type="my-protocol/1.0",\n                  frm=ALICE_DID, to=[BOB_DID])\npacked_msg = await pack_plaintext(message)\nprint(f"Publishing ${packed_msg}")\n\n# BOB\nunpack_result = await unpack(packed_msg)\nprint(f"Got ${unpack_result.plaintext} message")\n```\n\n## Contribution\nPRs are welcome!\n\nThe following CI checks are run against every PR:\n- all tests must pass\n- [flake8](https://github.com/PyCQA/flake8) checks must pass\n- code must be formatted by [Black](https://github.com/psf/black)',
-    'author': 'SICPA',
-    'author_email': 'DLCHOpenSourceContrib@sicpa.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/sicpa-dlab/didcomm-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: didcomm
+Version: 0.3.2
+Summary: Basic DIDComm v2 support in python
+Home-page: https://github.com/sicpa-dlab/didcomm-python
+License: Apache-2.0
+Author: SICPA
+Author-email: DLCHOpenSourceContrib@sicpa.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Requires-Dist: Authlib (>=1.1.0,<2.0.0)
+Requires-Dist: attrs (>=22.2,<23.0)
+Requires-Dist: base58 (>=2.1,<3.0)
+Requires-Dist: packaging (>=23.0,<24.0)
+Requires-Dist: pycryptodomex (>=3.10,<4.0)
+Requires-Dist: pydid (>=0.3.7,<0.4.0)
+Requires-Dist: varint (>=1.0.2,<1.1.0)
+Project-URL: Repository, https://github.com/sicpa-dlab/didcomm-python
+Description-Content-Type: text/markdown
+
+# DIDComm Python
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Unit Tests](https://github.com/sicpa-dlab/didcomm-python/workflows/verify/badge.svg)](https://github.com/sicpa-dlab/didcomm-python/actions/workflows/verify.yml)
+[![Python Package](https://img.shields.io/pypi/v/didcomm)](https://pypi.org/project/didcomm/)
+
+Basic [DIDComm v2](https://identity.foundation/didcomm-messaging/spec) support in Python.
+
+## Installation
+```
+pip install didcomm
+```
+
+## DIDComm + peerdid Demo
+See https://github.com/sicpa-dlab/didcomm-demo.
+
+## Assumptions and Limitations
+- Python >= 3.7.
+- In order to use the library, `SecretsResolver` and `DIDResolver` interfaces must be implemented on the application level. 
+  Implementation of that interfaces is out of DIDComm library scope.  
+  - Verification materials are expected in JWK, Base58 and Multibase (internally Base58 only) formats.
+    - In Base58 and Multibase formats, keys using only X25519 and Ed25519 curves are supported.
+    - For private keys in Base58 and Multibase formats, the verification material value contains both private and public parts (concatenated bytes).
+    - In Multibase format, bytes of the verification material value is prefixed with the corresponding Multicodec code.
+  - Key IDs (kids) used in `SecretsResolver` must match the corresponding key IDs from DID Doc verification methods.
+  - Key IDs (kids) in DID Doc verification methods and secrets must be a full [DID Fragment](https://www.w3.org/TR/did-core/#fragment), that is `did#key-id`.
+  - Verification methods referencing another DID Document are not supported (see [Referring to Verification Methods](https://www.w3.org/TR/did-core/#referring-to-verification-methods)).
+- The following curves and algorithms are supported:
+  - Encryption:
+     - Curves: X25519, P-384, P-256, P-521
+     - Content encryption algorithms: 
+       - XC20P (to be used with ECDH-ES only, default for anoncrypt),
+       - A256GCM (to be used with ECDH-ES only),
+       - A256CBC-HS512 (default for authcrypt)
+     - Key wrapping algorithms: ECDH-ES+A256KW, ECDH-1PU+A256KW
+  - Signing:
+    - Curves: Ed25519, Secp256k1, P-256
+    - Algorithms: EdDSA (with crv=Ed25519), ES256, ES256K
+- Forward protocol is implemented and used by default.
+- DID rotation (`fromPrior` field) is supported.
+- DIDComm has been implemented under the following [Assumptions](https://hackmd.io/i3gLqgHQR2ihVFV5euyhqg)   
+
+
+## Examples
+
+See [demo scripts](tests/demo) for details.
+
+A general usage of the API is the following:
+- Sender Side:
+  - Build a `Message` (plaintext, payload).
+  - Convert a message to a DIDComm Message for further transporting by calling one of the following:
+     - `pack_encrypted` to build an Encrypted DIDComm message
+     - `pack_signed` to build a Signed DIDComm message
+     - `pack_plaintext` to build a Plaintext DIDComm message
+- Receiver side:
+  - Call `unpack` on receiver side that will decrypt the message, verify signature if needed
+  and return a `Message` for further processing on the application level.
+
+### 1. Build an Encrypted DIDComm message for the given recipient
+
+This is the most common DIDComm message to be used in most of the applications.
+
+A DIDComm encrypted message is an encrypted JWM (JSON Web Messages) that 
+- hides its content from all but authorized recipients
+- (optionally) discloses and proves the sender to only those recipients
+- provides message integrity guarantees
+
+It is important in privacy-preserving routing. It is what normally moves over network transports in DIDComm
+applications, and is the safest format for storing DIDComm data at rest.
+
+See `pack_encrypted` documentation for more details.
+
+**Authentication encryption** example (most common case):
+
+```
+# ALICE
+message = Message(
+    body={"aaa": 1, "bbb": 2},
+    id="1234567890",
+    type="my-protocol/1.0",
+    frm=ALICE_DID,
+    to=[BOB_DID],
+)
+pack_result = await pack_encrypted(
+    resolvers_config=resolvers_config_alice,
+    message=message,
+    frm=ALICE_DID,
+    to=BOB_DID,
+    pack_config=PackEncryptedConfig(),
+)
+packed_msg = pack_result.packed_msg
+print(f"Sending ${packed_msg} to ${pack_result.service_metadata.service_endpoint}")
+
+# BOB
+unpack_result = await unpack(resolvers_config_bob, packed_msg)
+print(f"Got ${unpack_result.message} message")
+```
+
+**Anonymous encryption** example:
+
+```
+message = Message(
+    body={"aaa": 1, "bbb": 2},
+    id="1234567890",
+    type="my-protocol/1.0",
+    frm=ALICE_DID,
+    to=[BOB_DID],
+)
+
+pack_result = await pack_encrypted(
+    resolvers_config=resolvers_config_alice,
+    message=message,
+    to=BOB_DID,
+    pack_config=PackEncryptedConfig(),
+)
+```
+
+**Encryption with non-repudiation** example:
+
+```
+message = Message(
+    body={"aaa": 1, "bbb": 2},
+    id="1234567890",
+    type="my-protocol/1.0",
+    frm=ALICE_DID,
+    to=[BOB_DID],
+)
+
+pack_result = await pack_encrypted(
+    resolvers_config=resolvers_config_alice,
+    message=message,
+    frm=ALICE_DID,
+    sign_frm=ALICE_DID,
+    to=BOB_DID,
+    pack_config=PackEncryptedConfig(),
+)
+```
+
+### 2. Build an unencrypted but Signed DIDComm message
+
+Signed messages are only necessary when
+- the origin of plaintext must be provable to third parties
+- or the sender can’t be proven to the recipient by authenticated encryption because the recipient is not known in advance (e.g., in a
+broadcast scenario).
+ 
+Adding a signature when one is not needed can degrade rather than enhance security because it
+relinquishes the sender’s ability to speak off the record.
+
+See `pack_signed` documentation for more details.
+
+```
+# ALICE
+message = Message(
+    body={"aaa": 1, "bbb": 2},
+    id="1234567890",
+    type="my-protocol/1.0",
+    frm=ALICE_DID,
+    to=[BOB_DID],
+)
+pack_result = await pack_signed(
+    resolvers_config=resolvers_config_alice,
+    message=message,
+    sign_frm=ALICE_DID
+)
+packed_msg = pack_result.packed_msg
+print(f"Publishing ${packed_msg}")
+
+# BOB
+unpack_result = await unpack(resolvers_config_bob, packed_msg)
+print(f"Got ${unpack_result.message} message signed as ${unpack_result.metadata.signed_message}")
+```
+
+### 3. Build a Plaintext DIDComm message
+
+A DIDComm message in its plaintext form that 
+- is not packaged into any protective envelope
+- lacks confidentiality and integrity guarantees
+- repudiable
+
+They are therefore not normally transported across security boundaries. 
+
+```
+# ALICE
+message = Message(
+    body={"aaa": 1, "bbb": 2},
+    id="1234567890",
+    type="my-protocol/1.0",
+    frm=ALICE_DID,
+    to=[BOB_DID],
+)
+pack_result = await pack_plaintext(resolvers_config=resolvers_config_alice, message)
+print(f"Publishing ${pack_result.packed_msg}")
+
+# BOB
+unpack_result = await unpack(resolvers_config_bob, pack_result.packed_msg)
+print(f"Got ${unpack_result.message} message")
+```
+
+## Contribution
+PRs are welcome!
+
+The following CI checks are run against every PR:
+- all tests must pass
+- [flake8](https://github.com/PyCQA/flake8) checks must pass
+- code must be formatted by [Black](https://github.com/psf/black)
```

