# Comparing `tmp/krbjack-1.0.1.tar.gz` & `tmp/krbjack-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krbjack-1.0.1.tar", max compression
+gzip compressed data, was "krbjack-1.0.2.tar", max compression
```

## Comparing `krbjack-1.0.1.tar` & `krbjack-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-04-16 10:50:40.975309 krbjack-1.0.1/krbjack/__init__.py
--rw-r--r--   0        0        0     4844 2023-04-20 21:06:41.754965 krbjack-1.0.1/krbjack/__main__.py
--rw-r--r--   0        0        0     3349 2023-04-16 10:50:33.382821 krbjack-1.0.1/krbjack/custompipes.py
--rw-r--r--   0        0        0    10478 2023-04-20 20:56:42.382098 krbjack-1.0.1/krbjack/krbjacker.py
--rw-r--r--   0        0        0        0 2023-04-16 10:50:53.310403 krbjack-1.0.1/krbjack/modules/__init__.py
--rw-r--r--   0        0        0     7373 2023-04-20 21:12:00.797143 krbjack-1.0.1/krbjack/modules/psexec.py
--rw-r--r--   0        0        0     1784 2023-04-16 10:50:46.295130 krbjack-1.0.1/krbjack/modules/utils.py
--rw-r--r--   0        0        0     6012 2023-04-26 16:00:54.249740 krbjack-1.0.1/krbjack/tcpforward.py
--rw-r--r--   0        0        0     1485 2023-04-16 10:50:21.132287 krbjack-1.0.1/krbjack/utils.py
--rw-r--r--   0        0        0      446 2023-04-16 10:50:04.426169 krbjack-1.0.1/LICENSE
--rw-r--r--   0        0        0      649 2023-04-26 16:01:35.796435 krbjack-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8900 2023-04-26 16:01:13.917585 krbjack-1.0.1/README.md
--rw-r--r--   0        0        0     9763 1970-01-01 00:00:00.000000 krbjack-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-16 10:50:40.975309 krbjack-1.0.2/krbjack/__init__.py
+-rw-r--r--   0        0        0     4844 2023-04-20 21:06:41.754965 krbjack-1.0.2/krbjack/__main__.py
+-rw-r--r--   0        0        0     3349 2023-04-16 10:50:33.382821 krbjack-1.0.2/krbjack/custompipes.py
+-rw-r--r--   0        0        0    10478 2023-04-20 20:56:42.382098 krbjack-1.0.2/krbjack/krbjacker.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:50:53.310403 krbjack-1.0.2/krbjack/modules/__init__.py
+-rw-r--r--   0        0        0     7373 2023-04-20 21:12:00.797143 krbjack-1.0.2/krbjack/modules/psexec.py
+-rw-r--r--   0        0        0     1784 2023-04-16 10:50:46.295130 krbjack-1.0.2/krbjack/modules/utils.py
+-rw-r--r--   0        0        0     6012 2023-05-01 14:46:37.582796 krbjack-1.0.2/krbjack/tcpforward.py
+-rw-r--r--   0        0        0     1485 2023-04-16 10:50:21.132287 krbjack-1.0.2/krbjack/utils.py
+-rw-r--r--   0        0        0      446 2023-04-16 10:50:04.426169 krbjack-1.0.2/LICENSE
+-rw-r--r--   0        0        0      649 2023-05-01 14:46:52.197256 krbjack-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9014 2023-05-01 14:43:55.625654 krbjack-1.0.2/README.md
+-rw-r--r--   0        0        0     9877 1970-01-01 00:00:00.000000 krbjack-1.0.2/PKG-INFO
```

### Comparing `krbjack-1.0.1/krbjack/__main__.py` & `krbjack-1.0.2/krbjack/__main__.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.1/krbjack/custompipes.py` & `krbjack-1.0.2/krbjack/custompipes.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.1/krbjack/krbjacker.py` & `krbjack-1.0.2/krbjack/krbjacker.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.1/krbjack/modules/psexec.py` & `krbjack-1.0.2/krbjack/modules/psexec.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.1/krbjack/modules/utils.py` & `krbjack-1.0.2/krbjack/modules/utils.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.1/krbjack/tcpforward.py` & `krbjack-1.0.2/krbjack/tcpforward.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.1/krbjack/utils.py` & `krbjack-1.0.2/krbjack/utils.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.1/pyproject.toml` & `krbjack-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krbjack"
-version = "1.0.1"
+version = "1.0.2"
 description = "Kerberos AP-REQ hijacking tool with DNS unsecure updates abuse."
 authors = ["Virgile Jarry <virgile@mailbox.org>"]
 readme = "README.md"
 license = "Beerware"
 homepage = "https://github.com/almandin/krbjack"
 repository = "https://github.com/almandin/krbjack"
 documentation = "https://github.com/almandin/krbjack/README.md"
```

### Comparing `krbjack-1.0.1/README.md` & `krbjack-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 This tool can be used to abuse the dangerous `ZONE_UPDATE_UNSECURE` flag on DNS main domain zone in an Active Directory. This flag when set allows anyone unauthenticated to update, add and remove DNS records anonymously. It is quite common to see it during engagements as it is required to get some DHCP servers working with non-windows based systems, to get them update their own records. Even though this flag is extremely dangerous, I've never seen any tool to ease its exploitation. What I wanted to build is a mean to perform Man-in-the-Middle based on this dangerous flag, grab credentials and use them directly to own systems or the entire active directory services (though multiple tools can be used together to perform ntlm relay for example).
 
 The benefit from using this technique of man in the middle is that it goes through routers, as the "official" DNS records are poisonned. If proper routing is set (and if no firewall rule prevents it), someone on another broadcast domain can be targeted (unlike ARP poisoning which only works on you broadcast domain).
 
 Moreover I made the choice to perform fully functionnal AP_REQ hijacking to allow compromission of systems using kerberos instead of NetNTLM.
 
+![image](https://user-images.githubusercontent.com/9830129/235469315-a77c5875-393e-40db-8301-e006013cc98f.png)
+
+
 # Install
 
 ```bash
 sudo python -m pip install krbjack
 ```
 
 You do need to install the tool with root rights as it will need to be runnable by root to listen to privileged ports. Alternatively you can have fun with virtual envs. Alternatively you can download this repo and use `poetry` to install it.
@@ -65,8 +68,8 @@
 - https://googleprojectzero.blogspot.com/2021/10/windows-exploitation-tricks-relaying.html
 
 Impacket :
 - https://github.com/fortra/impacket
 
 # Disclaimer
 
-This tooling is made only for legal penetration testing and not for any other use. I am not responsible for how it is used by anyone or if it is used to penetrate systems without permission or proper contractual agreements. It is provided as is and without warranty of any sort.
+This tooling is made only for legal penetration testing and not for any other use. I am not responsible for how it is used by anyone or if it is used to penetrate systems without permission or proper contractual agreements. It is provided as is and without warranty of any sort.
```

### Comparing `krbjack-1.0.1/PKG-INFO` & `krbjack-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krbjack
-Version: 1.0.1
+Version: 1.0.2
 Summary: Kerberos AP-REQ hijacking tool with DNS unsecure updates abuse.
 Home-page: https://github.com/almandin/krbjack
 License: Beerware
 Author: Virgile Jarry
 Author-email: virgile@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -24,14 +24,17 @@
 
 This tool can be used to abuse the dangerous `ZONE_UPDATE_UNSECURE` flag on DNS main domain zone in an Active Directory. This flag when set allows anyone unauthenticated to update, add and remove DNS records anonymously. It is quite common to see it during engagements as it is required to get some DHCP servers working with non-windows based systems, to get them update their own records. Even though this flag is extremely dangerous, I've never seen any tool to ease its exploitation. What I wanted to build is a mean to perform Man-in-the-Middle based on this dangerous flag, grab credentials and use them directly to own systems or the entire active directory services (though multiple tools can be used together to perform ntlm relay for example).
 
 The benefit from using this technique of man in the middle is that it goes through routers, as the "official" DNS records are poisonned. If proper routing is set (and if no firewall rule prevents it), someone on another broadcast domain can be targeted (unlike ARP poisoning which only works on you broadcast domain).
 
 Moreover I made the choice to perform fully functionnal AP_REQ hijacking to allow compromission of systems using kerberos instead of NetNTLM.
 
+![image](https://user-images.githubusercontent.com/9830129/235469315-a77c5875-393e-40db-8301-e006013cc98f.png)
+
+
 # Install
 
 ```bash
 sudo python -m pip install krbjack
 ```
 
 You do need to install the tool with root rights as it will need to be runnable by root to listen to privileged ports. Alternatively you can have fun with virtual envs. Alternatively you can download this repo and use `poetry` to install it.
@@ -88,7 +91,8 @@
 
 Impacket :
 - https://github.com/fortra/impacket
 
 # Disclaimer
 
 This tooling is made only for legal penetration testing and not for any other use. I am not responsible for how it is used by anyone or if it is used to penetrate systems without permission or proper contractual agreements. It is provided as is and without warranty of any sort.
+
```

