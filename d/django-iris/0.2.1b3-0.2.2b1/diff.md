# Comparing `tmp/django-iris-0.2.1b3.tar.gz` & `tmp/django-iris-0.2.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-iris-0.2.1b3.tar", last modified: Thu Apr  6 13:29:44 2023, max compression
+gzip compressed data, was "django-iris-0.2.2b1.tar", last modified: Mon May  1 15:51:13 2023, max compression
```

## Comparing `django-iris-0.2.1b3.tar` & `django-iris-0.2.2b1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:29:44.001900 django-iris-0.2.1b3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-06 13:29:44.001900 django-iris-0.2.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:29:43.993900 django-iris-0.2.1b3/django_iris/
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/django_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/django_iris/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/django_iris/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/django_iris/creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/django_iris/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/django_iris/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/django_iris/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/django_iris/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/django_iris/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/django_iris/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/django_iris/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:29:43.993900 django-iris-0.2.1b3/django_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/django_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/django_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/django_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/django_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:29:43.997900 django-iris-0.2.1b3/intersystems_iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_BufferReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_BufferWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_ConnectionInformation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_ConnectionParameters.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_Constant.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_DBList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_Device.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_GatewayContext.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_GatewayException.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_GatewayUtility.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_IRIS.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_IRISConnection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_IRISEmbedded.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_IRISGlobalNode.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_IRISGlobalNodeView.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_IRISIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_IRISList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_IRISOREF.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_IRISObject.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_IRISReference.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_InStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_LegacyIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_ListItem.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_ListReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_ListWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_LogFileStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_MessageHeader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_OutStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_PrintStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_PythonGateway.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/_SharedMemorySocket.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:29:43.997900 django-iris-0.2.1b3/intersystems_iris/dbapi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/_Column.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    94963 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/_DBAPI.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/_Descriptor.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/_IRISStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/_Parameter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/_ParameterCollection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/_ResultSetRow.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/_SQLType.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:29:44.001900 django-iris-0.2.1b3/intersystems_iris/dbapi/preparser/
--rw-rw-rw-   0 runner    (1001) docker     (123)    78588 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/preparser/_PreParser.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/preparser/_Scanner.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/preparser/_Token.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/preparser/_TokenList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/dbapi/preparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:29:44.001900 django-iris-0.2.1b3/intersystems_iris/pex/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_BusinessHost.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_BusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_BusinessProcess.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_BusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_Common.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_Director.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_IRISBusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_IRISBusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_IRISInboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_IRISOutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_InboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/_OutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/intersystems_iris/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:29:44.001900 django-iris-0.2.1b3/irisnative/
--rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/irisnative/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-06 13:29:43.000000 django-iris-0.2.1b3/irisnative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-06 13:29:44.001900 django-iris-0.2.1b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-06 13:29:26.000000 django-iris-0.2.1b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:51:13.781589 django-iris-0.2.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-01 15:51:13.781589 django-iris-0.2.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:51:13.765589 django-iris-0.2.2b1/django_iris/
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/django_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/django_iris/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/django_iris/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/django_iris/creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/django_iris/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/django_iris/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/django_iris/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/django_iris/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/django_iris/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/django_iris/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/django_iris/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:51:13.769589 django-iris-0.2.2b1/django_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-01 15:51:13.000000 django-iris-0.2.2b1/django_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-01 15:51:13.000000 django-iris-0.2.2b1/django_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-01 15:51:13.000000 django-iris-0.2.2b1/django_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 15:51:13.000000 django-iris-0.2.2b1/django_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:51:13.773589 django-iris-0.2.2b1/intersystems_iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_BufferReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_BufferWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_ConnectionInformation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_ConnectionParameters.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_Constant.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_DBList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_Device.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_GatewayContext.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_GatewayException.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_GatewayUtility.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_IRIS.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_IRISConnection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_IRISEmbedded.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_IRISGlobalNode.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_IRISGlobalNodeView.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_IRISIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_IRISList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_IRISOREF.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_IRISObject.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_IRISReference.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_InStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_LegacyIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_ListItem.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_ListReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_ListWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_LogFileStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_MessageHeader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_OutStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_PrintStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_PythonGateway.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/_SharedMemorySocket.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:51:13.777589 django-iris-0.2.2b1/intersystems_iris/dbapi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/_Column.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    97873 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/_DBAPI.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/_Descriptor.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/_IRISStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4687 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/_Parameter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/_ParameterCollection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/_ResultSetRow.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/_SQLType.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:51:13.777589 django-iris-0.2.2b1/intersystems_iris/dbapi/preparser/
+-rw-rw-rw-   0 runner    (1001) docker     (123)    78828 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/preparser/_PreParser.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/preparser/_Scanner.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/preparser/_Token.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/preparser/_TokenList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/dbapi/preparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:51:13.781589 django-iris-0.2.2b1/intersystems_iris/pex/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_BusinessHost.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_BusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_BusinessProcess.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_BusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_Common.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_Director.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_IRISBusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_IRISBusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_IRISInboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_IRISOutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_InboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/_OutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/intersystems_iris/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:51:13.781589 django-iris-0.2.2b1/irisnative/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/irisnative/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-05-01 15:51:12.000000 django-iris-0.2.2b1/irisnative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-01 15:51:13.781589 django-iris-0.2.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-01 15:50:54.000000 django-iris-0.2.2b1/setup.py
```

### Comparing `django-iris-0.2.1b3/LICENSE` & `django-iris-0.2.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/PKG-INFO` & `django-iris-0.2.2b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iris
-Version: 0.2.1b3
+Version: 0.2.2b1
 Summary: Django backend for InterSystems IRIS
 Home-page: https://github.com/caretdev/django-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/django-iris
 Project-URL: Tracker, https://github.com/caretdev/django-iris/issues
```

### Comparing `django-iris-0.2.1b3/README.md` & `django-iris-0.2.2b1/README.md`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/django_iris/__init__.py` & `django-iris-0.2.2b1/django_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/django_iris/base.py` & `django-iris-0.2.2b1/django_iris/base.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/django_iris/compiler.py` & `django-iris-0.2.2b1/django_iris/compiler.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/django_iris/creation.py` & `django-iris-0.2.2b1/django_iris/creation.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/django_iris/cursor.py` & `django-iris-0.2.2b1/django_iris/cursor.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/django_iris/features.py` & `django-iris-0.2.2b1/django_iris/features.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/django_iris/introspection.py` & `django-iris-0.2.2b1/django_iris/introspection.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/django_iris/operations.py` & `django-iris-0.2.2b1/django_iris/operations.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/django_iris/schema.py` & `django-iris-0.2.2b1/django_iris/schema.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/django_iris/utils.py` & `django-iris-0.2.2b1/django_iris/utils.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/django_iris.egg-info/PKG-INFO` & `django-iris-0.2.2b1/django_iris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iris
-Version: 0.2.1b3
+Version: 0.2.2b1
 Summary: Django backend for InterSystems IRIS
 Home-page: https://github.com/caretdev/django-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/django-iris
 Project-URL: Tracker, https://github.com/caretdev/django-iris/issues
```

### Comparing `django-iris-0.2.1b3/django_iris.egg-info/SOURCES.txt` & `django-iris-0.2.2b1/django_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_BufferWriter.py` & `django-iris-0.2.2b1/intersystems_iris/_BufferWriter.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_ConnectionInformation.py` & `django-iris-0.2.2b1/intersystems_iris/_ConnectionInformation.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_ConnectionParameters.py` & `django-iris-0.2.2b1/intersystems_iris/_ConnectionParameters.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_Constant.py` & `django-iris-0.2.2b1/intersystems_iris/_Constant.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_DBList.py` & `django-iris-0.2.2b1/intersystems_iris/_DBList.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_Device.py` & `django-iris-0.2.2b1/intersystems_iris/_Device.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_GatewayContext.py` & `django-iris-0.2.2b1/intersystems_iris/_GatewayContext.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_GatewayUtility.py` & `django-iris-0.2.2b1/intersystems_iris/_GatewayUtility.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_IRIS.py` & `django-iris-0.2.2b1/intersystems_iris/_IRIS.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_IRISConnection.py` & `django-iris-0.2.2b1/intersystems_iris/_IRISConnection.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_IRISEmbedded.py` & `django-iris-0.2.2b1/intersystems_iris/_IRISEmbedded.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_IRISGlobalNode.py` & `django-iris-0.2.2b1/intersystems_iris/_IRISGlobalNode.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_IRISGlobalNodeView.py` & `django-iris-0.2.2b1/intersystems_iris/_IRISGlobalNodeView.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_IRISIterator.py` & `django-iris-0.2.2b1/intersystems_iris/_IRISIterator.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_IRISList.py` & `django-iris-0.2.2b1/intersystems_iris/_IRISList.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_IRISNative.py` & `django-iris-0.2.2b1/intersystems_iris/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_IRISObject.py` & `django-iris-0.2.2b1/intersystems_iris/_IRISObject.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_IRISReference.py` & `django-iris-0.2.2b1/intersystems_iris/_IRISReference.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_InStream.py` & `django-iris-0.2.2b1/intersystems_iris/_InStream.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_LegacyIterator.py` & `django-iris-0.2.2b1/intersystems_iris/_LegacyIterator.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_ListReader.py` & `django-iris-0.2.2b1/intersystems_iris/_ListReader.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_ListWriter.py` & `django-iris-0.2.2b1/intersystems_iris/_ListWriter.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_LogFileStream.py` & `django-iris-0.2.2b1/intersystems_iris/_LogFileStream.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_MessageHeader.py` & `django-iris-0.2.2b1/intersystems_iris/_MessageHeader.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_OutStream.py` & `django-iris-0.2.2b1/intersystems_iris/_OutStream.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_PrintStream.py` & `django-iris-0.2.2b1/intersystems_iris/_PrintStream.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_PythonGateway.py` & `django-iris-0.2.2b1/intersystems_iris/_PythonGateway.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/_SharedMemorySocket.py` & `django-iris-0.2.2b1/intersystems_iris/_SharedMemorySocket.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/__init__.py` & `django-iris-0.2.2b1/intersystems_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/_Column.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/_Column.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/_DBAPI.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/_DBAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,69 +6,85 @@
 from . import _Message
 import intersystems_iris.dbapi._Parameter
 import intersystems_iris.dbapi._Column
 from ._ResultSetRow import _ResultSetRow
 import intersystems_iris.dbapi._ParameterCollection
 import intersystems_iris.dbapi.preparser._PreParser
 from intersystems_iris.dbapi._Parameter import ParameterMode
-from intersystems_iris.dbapi.preparser._PreParser import StatementType
+from intersystems_iris.dbapi.preparser._PreParser import StatementType, MultiValuesInsert
 from intersystems_iris._IRISConnection import Feature
 from intersystems_iris._InStream import _InStream
-from intersystems_iris.dbapi._IRISStream import (IRISStream, IRISBinaryStream, )
+from intersystems_iris.dbapi._IRISStream import (
+    IRISStream,
+    IRISBinaryStream,
+)
 from ._SQLType import SQLType
 
 from .._IRISNative import connect as native_connect
 from .._IRISEmbedded import _IRISEmbedded
 
+
 def NotImplementedErrorDBAPI(msg=None):
     import traceback
+
     if msg is None:
         traceback.print_stack()
         msg = "Coming soon to an IRIS DB API near you!"
     return NotImplementedError(msg)
 
-def embedded_connect(*args, hostname = None, port = None,  namespace = None, username = None, password = None, **kw):
+
+def embedded_connect(*args, hostname=None, port=None, namespace=None, username=None, password=None, **kw):
     connection = _IRISEmbedded()
-    connection.connect(hostname, port,  namespace, username, password, **kw)
+    connection.connect(hostname, port, namespace, username, password, **kw)
     return connection
 
-def connect(*args, embedded=False, hostname = None, port = None,  namespace = None, username = None, password = None, **kw):
+
+def connect(*args, embedded=False, hostname=None, port=None, namespace=None, username=None, password=None, **kw):
     try:
         if not embedded:
-            return native_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
-        else:
-            return embedded_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
+            return native_connect(
+                *args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw
+            )
+        else:
+            return embedded_connect(
+                *args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw
+            )
     except Exception as e:
-        raise DatabaseError(e)
+        raise OperationalError(e)
+
 
 class ServerReturnType(enum.IntEnum):
     NO_RETURN_VALUE = 0
     IGNORE_RETURN_VALUE = 1
     HAS_RETURN_VALUE = 2
     NULL_RETURN_VALUE = 3
 
+
 class CursorType(enum.IntEnum):
     DEFAULT = 0
     PREPARED = 1
     CALLABLE = 2
 
+
 # api globals, methods, classes, etc.
 # globals
 apilevel = "2.0"
 threadsafety = 0
 paramstyle = "qmark"
 
+
 class _BaseCursor:
     embedded = False
+
     def __init__(self, connection):
         self._connection = connection
-        
+
         self.statement = None
         self._parsed_statement = None
-        
+
         self._columns = None
         self._rowcount = -1
         self.arraysize = 1
 
         self._result_set = None
 
         self._rsrow = None
@@ -100,33 +116,35 @@
 
     def __exit__(self, type, value, traceback):
         self._connection.rollback()
         self.close()
 
     def __iter__(self):
         if self._result_set == None:
-            raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
+            raise InterfaceError(
+                "Either execute has not yet been called, or the previous call of execute did not return a result set"
+            )
         return self
 
     def __next__(self):
         row = self.fetchone()
         if row:
             return row
         raise StopIteration
-    
+
     # non-api methods and classes
     def isClosed(self):
-        return self._closed 
+        return self._closed
 
     def setinputsizes(self, sizes):
         raise NotImplementedErrorDBAPI()
 
-    def setoutputsize(size, column = None):
+    def setoutputsize(size, column=None):
         raise NotImplementedErrorDBAPI()
-    
+
     @property
     def sqlcode(self):
         if self._closed:
             raise InterfaceError("Cursor is closed")
         return 0 if self._sqlcode is None else self._sqlcode
 
     def close(self):
@@ -150,15 +168,15 @@
         self._warehouse_dict = {}
         self._last_row_in_warehouse_dict = -1
         self._warehouse_dict_keys = []
 
         self._params = None
         self._parsed_statement = None
         self._cursor_type = CursorType.DEFAULT
-        self._statementType = StatementType.UPDATE # default
+        self._statementType = StatementType.UPDATE  # default
         self._paramInfo = None
         self.statement = None
         self.statementFeatureOption = Feature.optionNone
         self._statement_id = None
         self._sqlcode = None
         self._current_wire = None
         self._result_set = []
@@ -217,47 +235,63 @@
         return self._rowcount
 
     def execute(self, operation, params=()):
         self._is_alive()
 
         self.statement = operation
         if params and not isinstance(params, list) and not isinstance(params, tuple):
-            params = (params, )
+            params = (params,)
         self.params = params if params is not None else ()
         self._params.set_input_params(self.params)
 
         self._cleanup()
-        self._preparse()
+        try:
+            self._preparse()
+        except MultiValuesInsert as ex:
+            # convert to executemany
+            params = params or ex.params
+            params_count = int(len(params) / ex.rows)
+            new_params = [params[i : i + params_count] for i in range(0, len(params), params_count)]
+            return self.executemany(ex.query, new_params)
+        except Exception:
+            raise
 
         if self._statementType == StatementType.UPDATE:
             self._cursor_type = CursorType.PREPARED
             self._prepare()
         else:
             self._cursor_type = CursorType.DEFAULT
 
         self._execute()
         return self._rowcount
 
     def add_batch(self):
         self._is_alive()
-        
+
         if self._params._array_bound:
             if len(self._params._params_list) > 0:
                 cnt = 0
                 first = True
                 for i in range(self._params._user_parameters_size):
                     i = i + 1
                     cnt = len(self._params._get_user_param(i)._values)
                     if cnt > 1:
                         if first:
                             self._parameter_sets = cnt
                             first = False
                         elif self._parameter_sets != cnt:
-                            raise Exception("Unmatched columnwise parameter values: " + str(self._parameter_sets) 
-                                            +  " rows expected, but found only " + str(cnt) +" in " + str(i) + " parameter!")
+                            raise Exception(
+                                "Unmatched columnwise parameter values: "
+                                + str(self._parameter_sets)
+                                + " rows expected, but found only "
+                                + str(cnt)
+                                + " in "
+                                + str(i)
+                                + " parameter!"
+                            )
                 if self._parameter_sets > 1:
                     return
         self._parameter_sets = self._parameter_sets + 1
 
         for param in self._params._params_list:
             if param.mode != ParameterMode.REPLACED_LITERAL:
                 if len(param._values) != self._parameter_sets:
@@ -282,20 +316,20 @@
         self._is_batch_update = True
 
         self._preparse()
         self._prepare()
 
         for row_num, param_row in enumerate(seq_of_params):
             self.add_batch()
-        
+
         if self._parameter_sets == 0:
             for param in self._params._params_list:
-                if param.value == '?':
+                if param.value == "?":
                     raise ValueError("Missing value")
-            self._prepared_update_execute() # similar to executing a statement w/ literals
+            self._prepared_update_execute()  # similar to executing a statement w/ literals
             return
 
         for param in self._params._params_list:
             mode = param.mode
             if mode == ParameterMode.INPUT_OUTPUT or mode == ParameterMode.OUTPUT:
                 raise ValueError("INOUT/OUT parameters not permitted")
 
@@ -305,19 +339,21 @@
 
     def _process_sqlcode(self, sqlcode, message=None):
         self._sqlcode = sqlcode
         if sqlcode in [0, 100]:
             return
         if abs(sqlcode) in [108, 119, 121, 122]:
             raise IntegrityError(message)
+        if abs(sqlcode) in [1, 12]:
+            raise OperationalError(message)
         raise DatabaseError(message)
 
     def _preparse(self):
         csql = self._connection._pre_preparse_cache.get(self.statement)
-        if csql != None:
+        if csql is not None:
             self._has_return_value = csql._has_return_value
             self._params = copy.deepcopy(csql._params)
             self._params.set_input_params(self.params)
             self._parsed_statement = csql._parsed_statement
             self._statementType = csql._statementType
             self._paramInfo = csql._paramInfo
             return
@@ -336,59 +372,64 @@
             if i == 0:
                 count = len(item) if isinstance(item, list) or isinstance(item, tuple) else 1
             else:
                 curr_count = len(item) if isinstance(item, list) or isinstance(item, tuple) else 1
                 if count != curr_count:
                     raise Exception("Parameter count does not match")
 
-        parser = intersystems_iris.dbapi.preparser._PreParser._PreParser(self._connection._connection_info._delimited_ids, embedded=self.embedded)
+        parser = intersystems_iris.dbapi.preparser._PreParser._PreParser(
+            self._connection._connection_info._delimited_ids, embedded=self.embedded
+        )
         try:
             pOut = parser.PreParse(self.statement, self._params)
+        except MultiValuesInsert:
+            raise
         except Exception as e:
             raise InterfaceError("Error parsing statement '" + self.statement + "':\n" + str(e))
 
         if len(self.params) > 0:
             item = self.params[0]
             if (isinstance(item, list) or isinstance(item, tuple)) and not self._is_batch_update:
                 raise TypeError("Unsupported argument type: " + str(type(item)))
-        
+
         self._parsed_statement = pOut.sResult
         self._statementType = pOut.p_eStmtType
         self._paramInfo = parser.m_ParamInfo
 
-        if self._statementType == StatementType.CALL: 
+        if self._statementType == StatementType.CALL:
             self._has_return_value = ServerReturnType.NO_RETURN_VALUE
-        elif self._statementType == StatementType.CALLWITHRESULT: 
+        elif self._statementType == StatementType.CALLWITHRESULT:
             self._has_return_value = ServerReturnType.HAS_RETURN_VALUE
 
         self._update_parameters()
         self._connection._add_pre_preparse_cache(self.statement, self)
 
     def _prepare(self):
-        notDDL = bool(self._statementType != StatementType.DDL_ALTER_DROP 
-                                  and self._statementType != StatementType.DDL_OTHER)
+        notDDL = bool(
+            self._statementType != StatementType.DDL_ALTER_DROP and self._statementType != StatementType.DDL_OTHER
+        )
 
         if notDDL and self._get_cached_info():
             return
         else:
             self._prepare_new()
 
     def _update_parameters(self):
-        count = self._paramInfo._list_data[0] # self._paramInfo.count()
+        count = self._paramInfo._list_data[0]  # self._paramInfo.count()
         if count == 0:
             return
-        
+
         temp_list_data = self._paramInfo._list_data[1:]
-        param_info_count = int(len(temp_list_data)/2)
+        param_info_count = int(len(temp_list_data) / 2)
         if self._is_batch_update:
             unknown_count = replaced_count = 0
             for item in temp_list_data:
-                if item == 'c':
+                if item == "c":
                     replaced_count = replaced_count + 1
-                elif item == '?':
+                elif item == "?":
                     unknown_count = unknown_count + 1
 
             if len(self.params) > 0:
                 item = self.params[0]
                 param_count = len(item) if isinstance(item, list) or isinstance(item, tuple) else len(self.params)
                 if param_count != unknown_count:
                     raise Exception(f"Parameter mismatch: {param_count}/{unknown_count}")
@@ -405,45 +446,54 @@
                             if i >= len(self.params):
                                 param.mode = ParameterMode.OUTPUT
                             else:
                                 if self.params[i] == None:
                                     param.mode = ParameterMode.OUTPUT
                         i += 1
                 return
-            
+
             if len(temp_list_data) > 0:
                 if count != param_info_count:
                     raise Exception("Parameter mismatch")
 
                 unknown_count = replaced_count = 0
                 for item in temp_list_data:
-                    if item == 'c':
+                    if item == "c":
                         replaced_count = replaced_count + 1
-                    elif item == '?':
+                    elif item == "?":
                         unknown_count = unknown_count + 1
 
                 if unknown_count != len(self.params):
-                    raise Exception(f"Incorrect number of parameters: {unknown_count}/{replaced_count}/{len(self.params)}")
+                    raise Exception(
+                        f"Incorrect number of parameters: {unknown_count}/{replaced_count}/{len(self.params)}"
+                    )
 
     def _is_not_default_or_replaced(self, param):
         mode = param.mode
-        if mode != ParameterMode.REPLACED_LITERAL and mode != ParameterMode.DEFAULT_PARAMETER and mode != ParameterMode.INPUT:
+        if (
+            mode != ParameterMode.REPLACED_LITERAL
+            and mode != ParameterMode.DEFAULT_PARAMETER
+            and mode != ParameterMode.INPUT
+        ):
             raise Exception("Parameters not allowed in Cursor class")
 
     def _validate_parameters(self):
         if self._parameter_list_mismatch_exception and not self._params._has_bound_by_param_name:
             raise Exception("Parameter list mismatch")
         for param in self._params._params_list:
             self._is_not_default_or_replaced(param)
 
     def _validate_prepared_parameters(self):
         if self._parameter_list_mismatch_exception and not self._params._has_bound_by_param_name:
             raise Exception("Parameter list mismatch")
         i = 0
-        if self._has_return_value == ServerReturnType.IGNORE_RETURN_VALUE or self._has_return_value == ServerReturnType.NULL_RETURN_VALUE:
+        if (
+            self._has_return_value == ServerReturnType.IGNORE_RETURN_VALUE
+            or self._has_return_value == ServerReturnType.NULL_RETURN_VALUE
+        ):
             i = 1
         for param in self._params._params_list:
             if i == 1:
                 i = 0
                 continue
             if param.mode == ParameterMode.UNKNOWN:
                 if self._params._has_named_parameters():
@@ -459,22 +509,22 @@
 
         exec_switcher = {
             StatementType.QUERY: self._execute_query,
             StatementType.CALL: self._execute_update,
             StatementType.STMT_USE: self._execute_update,
             StatementType.UPDATE: self._execute_update,
             StatementType.DDL_OTHER: self._execute_update,
-            StatementType.DDL_ALTER_DROP: self._execute_update
+            StatementType.DDL_ALTER_DROP: self._execute_update,
         }
         exec_func = exec_switcher.get(self._statementType, None)
         if exec_func is None:
-            raise NotImplementedErrorDBAPI(f'StatementType {self._statementType.name} not implemented')
+            raise NotImplementedErrorDBAPI(f"StatementType {self._statementType.name} not implemented")
         else:
             return exec_func()
-    
+
     def _prepare_stored_procedure(self):
         if self._get_cached_info():
             self._prepared_stored_procedure_execute()
         pass
 
     def _execute_stored_procedure(self):
         if self._cursor_type == CursorType.DEFAULT:
@@ -513,28 +563,30 @@
             if self._get_cached_info():
                 # found in client side cache - send PQ message
                 self._prepared_query_execute()
             else:
                 # not found in client side cache - send DQ message
                 self._send_direct_query_request()
         else:
-            if (self._statementType != StatementType.QUERY and
-                self._statementType != StatementType.PREPARED_CALL_QUERY and
-                self._statementType != StatementType.DIRECT_CALL_QUERY):
+            if (
+                self._statementType != StatementType.QUERY
+                and self._statementType != StatementType.PREPARED_CALL_QUERY
+                and self._statementType != StatementType.DIRECT_CALL_QUERY
+            ):
                 raise Exception("Not a query")
-            
+
             if self._exec_params != None:
                 self._bind_exec_params()
             self._validate_prepared_parameters()
-            
+
             if self.statementFeatureOption & Feature.optionFastSelect == Feature.optionFastSelect:
                 self._rsrow = _ResultSetRow(self._connection, self._columns, self.maxRowItemCount)
             else:
                 self._rsrow = _ResultSetRow(self._connection, self._columns, 0)
-            
+
             if self._cursor_type == CursorType.CALLABLE or self._statementType == StatementType.PREPARED_CALL_QUERY:
                 self._stored_procedure_query()
                 return
             self._prepared_query_execute()
 
     def _execute_update(self):
         if self._cursor_type == CursorType.DEFAULT:
@@ -554,39 +606,42 @@
 
             if self._statementType == StatementType.CALL:
                 self._execute_stored_procedure()
                 if self._statementType == StatementType.DIRECT_CALL_QUERY:
                     raise Exception("Not an update")
                 return
 
-            notDDL = bool(self._statementType != StatementType.DDL_ALTER_DROP 
-                                      and self._statementType != StatementType.DDL_OTHER)
+            notDDL = bool(
+                self._statementType != StatementType.DDL_ALTER_DROP and self._statementType != StatementType.DDL_OTHER
+            )
 
             if notDDL and self._get_cached_info():
                 # found in client side cache - send PU message
                 self._prepared_update_execute()
             else:
                 # not found in client side cache - send DU message
                 self._send_direct_update_request()
         else:
             if self._statementType == StatementType.QUERY or self._statementType == StatementType.PREPARED_CALL_QUERY:
                 raise Exception("Not an update")
-            
+
             if self._exec_params != None:
                 self._bind_exec_params()
             self._validate_prepared_parameters()
-            
-            if (self._cursor_type == CursorType.CALLABLE or 
-                self._statementType == StatementType.PREPARED_CALL_UPDATE or
-                self._statementType == StatementType.DIRECT_CALL_UPDATE):
+
+            if (
+                self._cursor_type == CursorType.CALLABLE
+                or self._statementType == StatementType.PREPARED_CALL_UPDATE
+                or self._statementType == StatementType.DIRECT_CALL_UPDATE
+            ):
                 self._stored_procedure_update()
                 return
 
             self._prepared_update_execute()
-        
+
     def _query404(self):
         with self._connection._lock:
             self._validate_parameters()
             self._send_direct_query_request()
 
     def _update404(self):
         with self._connection._lock:
@@ -595,41 +650,48 @@
 
     # api properties and methods
     @property
     def description(self):
         if self._columns == None:
             return None
 
-        Column = namedtuple("Column", [
-            'name',
-            'type_code',
-            'display_size',
-            'internal_size',
-            'precision',
-            'scale',
-            'null_ok',
-        ])
+        Column = namedtuple(
+            "Column",
+            [
+                "name",
+                "type_code",
+                "display_size",
+                "internal_size",
+                "precision",
+                "scale",
+                "null_ok",
+            ],
+        )
 
         sequence = []
-        for column in self._columns: sequence.append(Column(
-            column.name,
-            column.type,
-            None,
-            None,
-            column.precision,
-            column.scale,
-            column.nullable,
-        ))
+        for column in self._columns:
+            sequence.append(
+                Column(
+                    column.name,
+                    column.type,
+                    None,
+                    None,
+                    column.precision,
+                    column.scale,
+                    column.nullable,
+                )
+            )
         return tuple(sequence)
-    
+
     # currently doesn't work for queries
     @property
     def rowcount(self):
         return self._rowcount
 
+
 # Cursor class
 class Cursor(_BaseCursor):
     def __init__(self, connection):
         super().__init__(connection)
 
         self._columns = None
         self._rowcount = -1
@@ -642,15 +704,15 @@
         self._result_set = None
 
         self._rsrow = None
         self._rownumber = 0
         self._cursor_ptr = 0
         self._scroll_flag = False
         self._warehouse = list()
-        
+
         self._warehouse_dict = dict()
         self._last_row_in_warehouse_dict = -1
         self._warehouse_dict_keys = list()
 
         self.maxRowItemCount = 0
 
         self._parameter_sets = 0
@@ -673,52 +735,58 @@
 
     def _process_sqlcode(self, sqlcode, message=None):
         if sqlcode in [0, 100]:
             return
         super()._process_sqlcode(sqlcode, self._get_error_info(sqlcode))
 
     def _get_cached_info(self):
-        if not self._connection._preparedCache or not hasattr(self._connection._preparedCache, '__iter__'):
+        if not self._connection._preparedCache or not hasattr(self._connection._preparedCache, "__iter__"):
             return False
         if self._parsed_statement in self._connection._preparedCache:
             self._prepare_cached(self._connection._preparedCache[self._parsed_statement])
             return True
         else:
             return False
 
     def _prepare_cached(self, cached_statement):
         self._statement_id = cached_statement.statement_id
 
         if self._statementType == StatementType.CALL or self._statementType == StatementType.CALLWITHRESULT:
             if len(self._params._params_list) != len(cached_statement._params._params_list):
-                if (self._statementType == StatementType.CALL and
-                    self._has_return_value == 0 and
-                    cached_statement._has_return_value == 1 and
-                    len(self._params._params_list) + 1 == len(cached_statement._params._params_list)):
-                    self._params._params_list.insert(0, intersystems_iris.dbapi._Parameter._Parameter(None, ParameterMode.OUTPUT, 'c'))
+                if (
+                    self._statementType == StatementType.CALL
+                    and self._has_return_value == 0
+                    and cached_statement._has_return_value == 1
+                    and len(self._params._params_list) + 1 == len(cached_statement._params._params_list)
+                ):
+                    self._params._params_list.insert(
+                        0, intersystems_iris.dbapi._Parameter._Parameter(None, ParameterMode.OUTPUT, "c")
+                    )
                 else:
                     if len(self._params._params_list) == 0 or len(self._params._params_list) == 1:
                         self._params._clear()
                     else:
                         return False
-            
+
             if cached_statement._statementType == StatementType.QUERY:
                 self._statementType = StatementType.PREPARED_CALL_QUERY
             else:
                 if cached_statement._statementType == StatementType.UPDATE:
                     self._statementType = StatementType.PREPARED_CALL_UPDATE
                 else:
                     self._statementType = cached_statement._statementType
 
             self._has_return_value = cached_statement._has_return_value
             self._multiple_result_sets = cached_statement.multiple_result_sets
             self._mrs_done = False
 
-            if (not self._multiple_result_sets and 
-                (self._statementType in [StatementType.QUERY, StatementType.PREPARED_CALL_QUERY, StatementType.DIRECT_CALL_QUERY])):
+            if not self._multiple_result_sets and (
+                self._statementType
+                in [StatementType.QUERY, StatementType.PREPARED_CALL_QUERY, StatementType.DIRECT_CALL_QUERY]
+            ):
                 self._columns = []
                 for column in cached_statement.columns:
                     self._columns.append(column.Clone())
 
                 if self.statementFeatureOption & Feature.optionFastSelect == Feature.optionFastSelect:
                     self._rsrow = _ResultSetRow(self._connection, self._columns, cached_statement.maxRowItemCount)
                 else:
@@ -737,27 +805,29 @@
 
         if hasattr(cached_statement, "statementFeatureOption"):
             self.statementFeatureOption = cached_statement.statementFeatureOption
         if hasattr(cached_statement, "maxRowItemCount"):
             self.maxRowItemCount = cached_statement.maxRowItemCount
         if hasattr(cached_statement, "_params"):
             self._params._update_param_info(cached_statement._params)
-    
+
     def _prepare_new(self):
         # send PP message
         with self._connection._lock:
             # message header
             self._statement_id = self._connection._get_new_statement_id()
             self._out_message.wire._write_header(_Message.PREPARE)
-            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
+            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(
+                self._out_message.wire.buffer, self._statement_id
+            )
 
             # message body
-            self._out_message.wire._set(1) # number of statement chunks
-            self._out_message.wire._set(self._parsed_statement) # statement itself
-            self._out_message.wire._set_raw_bytes(self._paramInfo.getBuffer()) # paramInfo (from _PreParser)
+            self._out_message.wire._set(1)  # number of statement chunks
+            self._out_message.wire._set(self._parsed_statement)  # statement itself
+            self._out_message.wire._set_raw_bytes(self._paramInfo.getBuffer())  # paramInfo (from _PreParser)
 
             # send message
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [0])
@@ -785,24 +855,27 @@
         except TypeError:
             raise DatabaseError("Unexpected server response message format")
 
     def _get_error_info(self, sqlcode):
         with self._connection._lock:
             self._out_message.wire._write_header(_Message.GET_SERVER_ERROR)
             self._out_message.wire._set(sqlcode)
-            
+
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             self._in_message._read_message_sql(sequence_number)
             return self._in_message.wire._get()
 
     def _check_statement_feature(self, wire):
         self.statementFeatureOption = wire._get()
-        if self.statementFeatureOption == Feature.optionFastSelect or self.statementFeatureOption == Feature.optionFastInsert:
+        if (
+            self.statementFeatureOption == Feature.optionFastSelect
+            or self.statementFeatureOption == Feature.optionFastInsert
+        ):
             self.maxRowItemCount = wire._get()
         else:
             self.maxRowItemCount = 0
 
     def _get_column_info(self, wire):
         self._columns = []
         count = wire._get()
@@ -815,23 +888,41 @@
             label = wire._get()
             tableName = wire._get()
             schema = wire._get()
             catalog = wire._get()
             if catalog == 0:
                 catalog = None
             additionalData = wire._get().encode()
-            slotPosition = wire._get() if self.statementFeatureOption & Feature.optionFastSelect == Feature.optionFastSelect else i + 1
-            self._columns.append(intersystems_iris.dbapi._Column._Column(name, type, precision, scale, nullable, label, tableName, schema, catalog, additionalData, slotPosition))
+            slotPosition = (
+                wire._get()
+                if self.statementFeatureOption & Feature.optionFastSelect == Feature.optionFastSelect
+                else i + 1
+            )
+            self._columns.append(
+                intersystems_iris.dbapi._Column._Column(
+                    name,
+                    type,
+                    precision,
+                    scale,
+                    nullable,
+                    label,
+                    tableName,
+                    schema,
+                    catalog,
+                    additionalData,
+                    slotPosition,
+                )
+            )
 
     def _get_parameter_info(self, wire):
         count = wire._get()
         if count != len(self._params._params_list):
             raise Exception("Invalid number of parameters")
         self._read_parameter_data(wire, count, False)
-        
+
         addToCache = bool(wire._get())
         return addToCache
 
     def _read_parameter_data(self, wire, count, is_stored_procedure):
         if count != len(self._params._params_list):
             raise Exception("Invalid number of parameters")
         with self._connection._lock:
@@ -847,15 +938,15 @@
                 param.type = wire._get()
                 param.precision = wire._get()
                 param.scale = wire._get()
                 param.nullable = wire._get()
 
                 if self.statementFeatureOption & Feature.optionFastInsert == Feature.optionFastInsert:
                     param.slotPosition = wire._get()
-                    self.rowOfDefaultValues = wire._get() # needs to be processed
+                    self.rowOfDefaultValues = wire._get()  # needs to be processed
                 else:
                     param.slotPosition = i + r
 
                 if is_stored_procedure:
                     param.name = wire._get()
                     wire._get()
 
@@ -864,15 +955,14 @@
 
     def _execute_update(self):
         super()._execute_update()
 
         if self._parameter_sets == 0 and not self._multiple_result_sets:
             self._rowcount = self._in_message.wire._get()
 
-
     class prepared_statement(intersystems_iris._IRISConnection.CachedSQL):
         def __init__(self, cursor):
             if not isinstance(cursor, Cursor):
                 raise TypeError("cursor must be a Cursor")
 
             super().__init__(cursor)
             self.statement = cursor._parsed_statement
@@ -892,16 +982,16 @@
 
     def _cache_prepared_statement(self):
         self._connection._cache_prepared_statement(self.prepared_statement(self))
 
     def _write_parameters(self):
         sets = self._parameter_sets or 1
 
-        self._out_message.wire._set(sets) # nParamSets
-        self._out_message.wire._set(len(self._params._params_list)) # nParams
+        self._out_message.wire._set(sets)  # nParamSets
+        self._out_message.wire._set(len(self._params._params_list))  # nParams
         for i in range(sets):
             param_index = 0
             param_counter = i
             for param in self._params._params_list:
                 mode = param.mode
                 if mode == ParameterMode.REPLACED_LITERAL:
                     self._out_message.wire._set_parameter(param)
@@ -922,20 +1012,22 @@
                     raise Exception("Missing value")
 
     def _prepared_query_execute(self):
         # send PQ message
         with self._connection._lock:
             # message header
             self._out_message.wire._write_header(_Message.PREPARED_QUERY_EXECUTE)
-            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
+            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(
+                self._out_message.wire.buffer, self._statement_id
+            )
 
             # message body
             self._write_parameters()
-            self._out_message.wire._set(0) # query timeout
-            self._out_message.wire._set(0) # maxRows (0 = all rows)
+            self._out_message.wire._set(0)  # query timeout
+            self._out_message.wire._set(0)  # maxRows (0 = all rows)
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, _InStream.FETCH_DATA, [404, 100])
@@ -944,31 +1036,33 @@
             if self._sqlcode == 404:
                 return
             self._process_sqlcode(self._sqlcode)
 
         self._current_wire = self._in_message.wire
         self._result_set = [self._current_wire]
         self._rs_index = 0
-        
+
         self._rowcount = -1
 
     def _send_direct_stored_procedure_request(self):
         # self._has_return_value = ServerReturnType.NO_RETURN_VALUE
         # send DS message
         with self._connection._lock:
             # message header
             self._statement_id = self._connection._get_new_statement_id()
             self._out_message.wire._write_header(_Message.DIRECT_STORED_PROCEDURE)
-            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
+            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(
+                self._out_message.wire.buffer, self._statement_id
+            )
 
             # message body
-            self._out_message.wire._set(self._parsed_statement) # statement itself
-            self._out_message.wire._set(0) # resultSetType != ResultSet.TYPE_SCROLL_INSENSITIVE
-            self._out_message.wire._set(0) # query timeout
-            self._out_message.wire._set(0) # maxRows (0 = all rows)
+            self._out_message.wire._set(self._parsed_statement)  # statement itself
+            self._out_message.wire._set(0)  # resultSetType != ResultSet.TYPE_SCROLL_INSENSITIVE
+            self._out_message.wire._set(0)  # query timeout
+            self._out_message.wire._set(0)  # maxRows (0 = all rows)
             self._write_stored_procedure_parameters()
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             try:
@@ -981,45 +1075,52 @@
                 self._process_stored_procedure_metadata(self._in_message.wire, True)
                 if self._multiple_result_sets:
                     # todo
                     return
 
                 self._cache_prepared_statement()
 
-                if self._statementType in [StatementType.UPDATE, StatementType.DIRECT_CALL_UPDATE, StatementType.PREPARED_CALL_UPDATE]:
+                if self._statementType in [
+                    StatementType.UPDATE,
+                    StatementType.DIRECT_CALL_UPDATE,
+                    StatementType.PREPARED_CALL_UPDATE,
+                ]:
                     return False
 
             except IndexError:
                 raise DatabaseError("Server response message terminated prematurely")
             except TypeError:
                 raise DatabaseError("Unexpected server response message format")
-    
+
     def _prepared_stored_procedure_execute(self):
         # send SU message
         with self._connection._lock:
             # message header
             self._out_message.wire._write_header(_Message.PREPARED_UPDATE_EXECUTE)
-            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
-
+            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(
+                self._out_message.wire.buffer, self._statement_id
+            )
 
     def _send_direct_query_request(self):
         # send DQ message
         with self._connection._lock:
             # message header
             self._statement_id = self._connection._get_new_statement_id()
             self._out_message.wire._write_header(_Message.DIRECT_QUERY)
-            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
+            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(
+                self._out_message.wire.buffer, self._statement_id
+            )
 
             # message body
-            self._out_message.wire._set(1) # number of statement chunks
-            self._out_message.wire._set(self._parsed_statement) # statement itself
-            self._out_message.wire._set_raw_bytes(self._paramInfo.getBuffer()) # paramInfo (from _PreParser)
+            self._out_message.wire._set(1)  # number of statement chunks
+            self._out_message.wire._set(self._parsed_statement)  # statement itself
+            self._out_message.wire._set_raw_bytes(self._paramInfo.getBuffer())  # paramInfo (from _PreParser)
             self._write_parameters()
-            self._out_message.wire._set(0) # query timeout
-            self._out_message.wire._set(0) # maxRows (0 = all rows)
+            self._out_message.wire._set(0)  # query timeout
+            self._out_message.wire._set(0)  # maxRows (0 = all rows)
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             try:
                 # retrieve metadata
@@ -1045,32 +1146,34 @@
                 raise DatabaseError("Server response message terminated prematurely")
             except TypeError:
                 raise DatabaseError("Unexpected server response message format")
 
         self._current_wire = self._in_message.wire
         self._result_set = [self._current_wire]
         self._rs_index = 0
-        
+
         self._rowcount = -1
         if self.statementFeatureOption & Feature.optionFastSelect == Feature.optionFastSelect:
             self._rsrow = _ResultSetRow(self._connection, self._columns, self.maxRowItemCount)
         else:
             self._rsrow = _ResultSetRow(self._connection, self._columns, 0)
-        
+
     def _prepared_update_execute(self):
         # send PU message
         with self._connection._lock:
             # message header
             self._out_message.wire._write_header(_Message.PREPARED_UPDATE_EXECUTE)
-            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
+            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(
+                self._out_message.wire.buffer, self._statement_id
+            )
 
             # message body
             self._lastrowid = None
-            self._out_message.wire._set(-1) # autoGeneratedKeyColumn
-            self._out_message.wire._set(0) # statement timeout always 0 for non-queries
+            self._out_message.wire._set(-1)  # autoGeneratedKeyColumn
+            self._out_message.wire._set(0)  # statement timeout always 0 for non-queries
             self._write_parameters()
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
@@ -1083,58 +1186,64 @@
 
     def _send_direct_update_request(self):
         # send DU message
         with self._connection._lock:
             self._statement_id = self._connection._get_new_statement_id()
             # message header
             self._out_message.wire._write_header(_Message.DIRECT_UPDATE)
-            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
+            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(
+                self._out_message.wire.buffer, self._statement_id
+            )
 
             # message body
             self._lastrowid = None
-            self._out_message.wire._set(1) # number of statement chunks
-            self._out_message.wire._set(self._parsed_statement) # statement itself
-            self._out_message.wire._set_raw_bytes(self._paramInfo.getBuffer()) # paramInfo (from _PreParser)
-            self._out_message.wire._set(-1) # autoGeneratedKeyColumn
-            self._out_message.wire._set(0) # statement timeout always 0 for non-queries
+            self._out_message.wire._set(1)  # number of statement chunks
+            self._out_message.wire._set(self._parsed_statement)  # statement itself
+            self._out_message.wire._set_raw_bytes(self._paramInfo.getBuffer())  # paramInfo (from _PreParser)
+            self._out_message.wire._set(-1)  # autoGeneratedKeyColumn
+            self._out_message.wire._set(0)  # statement timeout always 0 for non-queries
             self._write_parameters()
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             try:
                 # retrieve response
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 self._sqlcode = self._in_message.wire.header._get_function_code()
                 self._process_sqlcode(self._sqlcode)
 
                 addToCache = self._get_parameter_info(self._in_message.wire)
-                
-                notDDL = bool(self._statementType != StatementType.DDL_ALTER_DROP 
-                                  and self._statementType != StatementType.DDL_OTHER)
+
+                notDDL = bool(
+                    self._statementType != StatementType.DDL_ALTER_DROP
+                    and self._statementType != StatementType.DDL_OTHER
+                )
                 if notDDL and addToCache:
                     self._cache_prepared_statement()
 
             except IndexError:
                 raise DatabaseError("Server response message terminated prematurely")
             except TypeError:
                 raise DatabaseError("Unexpected server response message format")
 
     def _prepare_stored_procedure(self):
         with self._connection._lock:
             # message header
             self._statement_id = self._connection._get_new_statement_id()
             self._out_message.wire._write_header(_Message.PREPARE_STORED_PROCEDURE)
-            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
+            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(
+                self._out_message.wire.buffer, self._statement_id
+            )
 
             # message body
-            #self._out_message.wire._set(1) # number of statement chunks
-            self._out_message.wire._set(self._parsed_statement) # statement itself
-            
+            # self._out_message.wire._set(1) # number of statement chunks
+            self._out_message.wire._set(self._parsed_statement)  # statement itself
+
             # send message
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [0])
             sqlcode = self._in_message.wire.header._get_function_code()
@@ -1205,19 +1314,28 @@
             if server_has_return:
                 self._has_return_value = ServerReturnType.IGNORE_RETURN_VALUE
         elif size == count:
             if server_has_return and self._has_return_value == ServerReturnType.HAS_RETURN_VALUE:
                 self._has_return_value = ServerReturnType.HAS_RETURN_VALUE
             elif not server_has_return and self._has_return_value == ServerReturnType.NO_RETURN_VALUE:
                 self._has_return_value = ServerReturnType.NO_RETURN_VALUE
-            elif (size == 1 and count == 1 
-                  and (self._params._params_list[0].mode == ParameterMode.DEFAULT_PARAMETER 
-                       and self._has_return_value == ServerReturnType.NO_RETURN_VALUE and server_has_return) 
-                  or (self._params._params_list[0].mode == ParameterMode.UNKNOWN 
-                      and self._has_return_value == ServerReturnType.IGNORE_RETURN_VALUE and server_has_return)):
+            elif (
+                size == 1
+                and count == 1
+                and (
+                    self._params._params_list[0].mode == ParameterMode.DEFAULT_PARAMETER
+                    and self._has_return_value == ServerReturnType.NO_RETURN_VALUE
+                    and server_has_return
+                )
+                or (
+                    self._params._params_list[0].mode == ParameterMode.UNKNOWN
+                    and self._has_return_value == ServerReturnType.IGNORE_RETURN_VALUE
+                    and server_has_return
+                )
+            ):
                 self._params._params_list.pop(0)
                 self._params._params_list.insert(0, intersystems_iris.dbapi._Parameter._Parameter())
                 self._has_return_value = ServerReturnType.IGNORE_RETURN_VALUE
             else:
                 wire._move_to_end()
                 return False
         elif size == count + 1:
@@ -1241,25 +1359,29 @@
                 wire._move_to_end()
                 return False
         elif size == count - 1:
             if server_has_return and self._has_return_value == ServerReturnType.NO_RETURN_VALUE:
                 self._params._params_list.insert(0, intersystems_iris.dbapi._Parameter._Parameter())
                 self._has_return_value = ServerReturnType.IGNORE_RETURN_VALUE
             else:
-                self._params._params_list.append(intersystems_iris.dbapi._Parameter._Parameter(ParameterMode.DEFAULT_PARAMETER, 'c'))
+                self._params._params_list.append(
+                    intersystems_iris.dbapi._Parameter._Parameter(ParameterMode.DEFAULT_PARAMETER, "c")
+                )
         else:
             self._parameter_list_mismatch_exception = True
             if server_has_return and self._has_return_value == ServerReturnType.NO_RETURN_VALUE:
                 self._has_return_value = ServerReturnType.IGNORE_RETURN_VALUE
                 param = intersystems_iris.dbapi._Parameter._Parameter()
                 param.mode = ParameterMode.OUTPUT
                 self._params._params_list.insert(0, param)
                 size = size + 1
             while size < count:
-                self._params._params_list.append(intersystems_iris.dbapi._Parameter._Parameter(ParameterMode.DEFAULT_PARAMETER, 'c'))
+                self._params._params_list.append(
+                    intersystems_iris.dbapi._Parameter._Parameter(ParameterMode.DEFAULT_PARAMETER, "c")
+                )
                 size = size + 1
         self._read_parameter_data(wire, count, True)
         return True
 
     def _bind_exec_params(self):
         for param in self._params._params_list:
             exec_param = self._get_exec_param_by_name(param.name)
@@ -1283,20 +1405,22 @@
         self._exec_params._has_bound_by_param_name = True
         return self._exec_params._params_list[self._exec_params._param_names.get(name.upper())]
 
     def _stored_procedure_update(self):
         with self._connection._lock:
             # message header
             self._out_message.wire._write_header(_Message.STORED_PROCEDURE_UPDATE_EXECUTE)
-            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
+            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(
+                self._out_message.wire.buffer, self._statement_id
+            )
 
             # message body
-            self._out_message.wire._set(0) # isStatic should always be 0 for non-queries
-            self._out_message.wire._set(0) # query timeout
-            self._out_message.wire._set(0) # maxRows (0 = all rows)
+            self._out_message.wire._set(0)  # isStatic should always be 0 for non-queries
+            self._out_message.wire._set(0)  # query timeout
+            self._out_message.wire._set(0)  # maxRows (0 = all rows)
             self._write_stored_procedure_parameters()
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
@@ -1312,20 +1436,22 @@
     def _stored_procedure_query(self):
         if self._multiple_result_sets:
             self._execute_multiple_result_sets(False)
             return
         with self._connection._lock:
             # message header
             self._out_message.wire._write_header(_Message.STORED_PROCEDURE_QUERY_EXECUTE)
-            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
+            intersystems_iris._MessageHeader._MessageHeader._set_statement_id(
+                self._out_message.wire.buffer, self._statement_id
+            )
 
             # message body
-            self._out_message.wire._set(0) # ResultSet.TYPE_SCROLL_INSENSITIVE
-            self._out_message.wire._set(0) # query timeout
-            self._out_message.wire._set(0) # maxRows (0 = all rows)
+            self._out_message.wire._set(0)  # ResultSet.TYPE_SCROLL_INSENSITIVE
+            self._out_message.wire._set(0)  # query timeout
+            self._out_message.wire._set(0)  # maxRows (0 = all rows)
             self._write_stored_procedure_parameters()
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
@@ -1350,16 +1476,16 @@
 
     def _execute_multiple_result_sets(self, validate):
         self._fetch_done = False
         if validate:
             self._validate_parameters()
         with self._connection._lock:
             self._out_message.wire._write_header(_Message.EXECUTE_MULTIPLE_RESULT_SETS)
-            self._out_message.wire._set(0) # resultSetType != ResultSet.TYPE_SCROLL_INSENSITIVE
-            self._out_message.wire._set(0) # query timeout
+            self._out_message.wire._set(0)  # resultSetType != ResultSet.TYPE_SCROLL_INSENSITIVE
+            self._out_message.wire._set(0)  # query timeout
             self._write_stored_procedure_parameters()
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             if self.statementFeatureOption & Feature.optionFastSelect == Feature.optionFastSelect:
@@ -1374,23 +1500,23 @@
             self._get_output_parameters(self._in_message.wire)
 
             self._current_wire = self._in_message.wire
             self._result_set = [self._current_wire]
             self._rs_index = 0
 
             results = self._in_message.wire._get()
-            if results >= 0 :
+            if results >= 0:
                 self._update_cnt = results
                 return False
             elif results == -1:
                 return True
             elif results == -2:
                 self._update_cnt = -1
                 self._mrs_done = True
-                #self._rsrow._is_after_last = True
+                # self._rsrow._is_after_last = True
                 return False
             else:
                 raise Exception("Invalid result type value")
 
     def _write_stored_procedure_parameters(self):
         i = 0
         if self._parameter_sets != 0:
@@ -1431,25 +1557,31 @@
         i = 0
         if self._has_return_value == ServerReturnType.NULL_RETURN_VALUE:
             i += 1
         for param in self._params._params_list:
             if i == 1:
                 i = 0
                 continue
-            if param.mode == ParameterMode.INPUT_OUTPUT or param.mode == ParameterMode.OUTPUT or param.mode == ParameterMode.RETURN_VALUE:
+            if (
+                param.mode == ParameterMode.INPUT_OUTPUT
+                or param.mode == ParameterMode.OUTPUT
+                or param.mode == ParameterMode.RETURN_VALUE
+            ):
                 wire._next_unless_undefined()
             else:
                 wire._next()
         if self._has_return_value == ServerReturnType.NULL_RETURN_VALUE:
             self._output_parameter_list = wire._get_output_parameter_list(beg, True)
             self._has_return_value = ServerReturnType.HAS_RETURN_VALUE
         else:
             self._output_parameter_list = wire._get_output_parameter_list(beg, False)
         if self._statementType not in [StatementType.DIRECT_CALL_UPDATE]:
-            self._params._prep_list_index(False, self._output_parameter_list) # fast select not supported for stored procedures
+            self._params._prep_list_index(
+                False, self._output_parameter_list
+            )  # fast select not supported for stored procedures
         return
 
     def _handle_error_504(self, error):
         if error == 404:
             self._query404()
             return
         self._handle_error_100(error)
@@ -1460,15 +1592,19 @@
             pass
         else:
             pass
 
     def stored_results(self):
         if self._closed:
             raise InterfaceError("Cursor is closed")
-        if self._statementType not in [StatementType.QUERY, StatementType.DIRECT_CALL_QUERY, StatementType.PREPARED_CALL_QUERY]:
+        if self._statementType not in [
+            StatementType.QUERY,
+            StatementType.DIRECT_CALL_QUERY,
+            StatementType.PREPARED_CALL_QUERY,
+        ]:
             return None
         # getResultSet()
         if self._multiple_result_sets:
             if self._rsrow == None and self._rowcount == -1:
                 return None
             if self._mrs_done:
                 return None
@@ -1488,38 +1624,43 @@
             return True
         else:
             # getMoreResults()
             if self._closed:
                 raise InterfaceError("Cursor is closed")
             if self._connection == None or self._connection.isClosed():
                 raise InterfaceError("Connection not open")
-            if (self._mrs_done or not self._multiple_result_sets or 
-                (self._statementType != StatementType.PREPARED_CALL_QUERY and 
-                 self._statementType != StatementType.DIRECT_CALL_QUERY and
-                 self._statementType != StatementType.CALL and
-                 self._statementType != StatementType.CALLWITHRESULT and
-                 not (self._statementType == StatementType.QUERY and self._cursor_type == CursorType.CALLABLE))):
+            if (
+                self._mrs_done
+                or not self._multiple_result_sets
+                or (
+                    self._statementType != StatementType.PREPARED_CALL_QUERY
+                    and self._statementType != StatementType.DIRECT_CALL_QUERY
+                    and self._statementType != StatementType.CALL
+                    and self._statementType != StatementType.CALLWITHRESULT
+                    and not (self._statementType == StatementType.QUERY and self._cursor_type == CursorType.CALLABLE)
+                )
+            ):
                 return False
             with self._connection._lock:
                 self._out_message.wire._write_header(_Message.GET_MORE_RESULTS)
-                self._out_message.wire._set(1) # current = CLOSE_CURRENT_RESULT
+                self._out_message.wire._set(1)  # current = CLOSE_CURRENT_RESULT
 
                 # send
                 sequence_number = self._connection._get_new_sequence_number()
                 self._out_message._send(sequence_number)
 
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 sqlcode = self._in_message.wire.header._get_function_code()
 
                 self._current_wire = self._in_message.wire
                 self._result_set = [self._current_wire]
                 self._rs_index = 0
 
                 results = self._in_message.wire._get()
-                if results >= 0 :
+                if results >= 0:
                     self._update_cnt = results
                     return False
                 elif results == -1:
                     self._rsrow = None
                     self._get_column_info(self._in_message.wire)
                     if self.statementFeatureOption & Feature.optionFastSelect == Feature.optionFastSelect:
                         self._rsrow = _ResultSetRow(self._connection, self._columns, self.maxRowItemCount)
@@ -1539,19 +1680,19 @@
                 else:
                     raise Exception("Invalid result type value")
         return
 
     def _get_result_set(self, oref):
         if oref == None:
             return None
-        
+
         with self._connection._lock:
             self._out_message.wire._write_header(_Message.GET_RESULT_SET_OBJECT)
             self._out_message.wire._set(oref)
-            self._out_message.wire._set(0) # IRISResultSet.GET_RESULT_SET_OBJECT_INIT
+            self._out_message.wire._set(0)  # IRISResultSet.GET_RESULT_SET_OBJECT_INIT
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             error = self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
@@ -1569,24 +1710,24 @@
         self.statement = procname
         if len(params) == 1 and (isinstance(params[0], tuple) or isinstance(params[0], list)):
             self.params = self.params[0]
         else:
             self.params = params
 
         self._params.set_input_params(self.params)
-        
+
         self._cursor_type = CursorType.CALLABLE
         self._cleanup()
         self._preparse()
         self._stored_results = []
-        
+
         if not self._get_cached_info():
             self._prepare_stored_procedure()
 
-        #execute() in IrisPreparedStatement
+        # execute() in IrisPreparedStatement
         if self._multiple_result_sets:
             return self._execute_multiple_result_sets(True)
         if self._statementType == StatementType.QUERY or self._statementType == StatementType.PREPARED_CALL_QUERY:
             self._execute_query()
             self._rowcount = -1
             if self._fetch_done and self._in_message.wire.header._get_message_length() == 0:
                 return
@@ -1599,29 +1740,29 @@
 
     def _process_return_values(self):
         return_args = []
         for i, param in enumerate(self._params._params_list):
             if param.mode in [ParameterMode.RETURN_VALUE, ParameterMode.OUTPUT, ParameterMode.INPUT]:
                 offset = self._params._get_user_list_offset(i + 1)
                 val = self._output_parameter_list._get_at_offset(offset)
-                if param.type == -51: # RESULT_SET_TYPE
+                if param.type == -51:  # RESULT_SET_TYPE
                     self._get_result_set(val)
                     self.nextset()
                     return_args.append(self._stored_results[0])
                 else:
-                    if val == '\x01': # Either represents the number 1 or a null/None value
+                    if val == "\x01":  # Either represents the number 1 or a null/None value
                         # maybe move this to _grab_ascii_string in DBList?
                         off = self._output_parameter_list.list_item.data_offset
                         buf = self._output_parameter_list.list_item.buffer
                         if buf[off] == 1 and buf[off - 1] == 1 and buf[off - 2] == 3:
                             return_args.append(None)
                     else:
                         return_args.append(val)
         if len(return_args) > 0:
-            if any(i != None for i in return_args): 
+            if any(i != None for i in return_args):
                 return return_args
             else:
                 return
         else:
             return
 
     @property
@@ -1632,28 +1773,28 @@
         if self._closed:
             return None
         if self._connection == None or self._connection.isClosed():
             return None
 
         if self._statementType is not StatementType.UPDATE:
             return None
-        
+
         # In multivalue inserts it returns the first inserted value, not the last one
         # with self._connection._lock:
         #     self._out_message.wire._write_header(_Message.GET_AUTO_GENERATED_KEYS)
         #     sequence_number = self._connection._get_new_sequence_number()
         #     self._out_message._send(sequence_number)
         #     self._in_message._read_message_sql(sequence_number)
         #     self._sqlcode = self._in_message.wire.header._get_function_code()
         #     if self._sqlcode != 100:
         #         raise DatabaseError(self._get_error_info(self._sqlcode))
         #     self._get_column_info(self._in_message.wire)
         #     self._lastrowid = self._in_message.wire._get()
 
-        self.execute('SELECT LAST_IDENTITY()')
+        self.execute("SELECT LAST_IDENTITY()")
         self._lastrowid = self.fetchone()[0]
         return self._lastrowid
 
     def _cleanup(self):
         super()._cleanup()
         if self._rsrow != None:
             self._rsrow = None
@@ -1692,15 +1833,15 @@
         self._warehouse_dict = {}
         self._last_row_in_warehouse_dict = -1
         self._warehouse_dict_keys = []
 
         self._params = None
         self._parsed_statement = None
         self._cursor_type = CursorType.DEFAULT
-        self._statementType = StatementType.UPDATE # default
+        self._statementType = StatementType.UPDATE  # default
         self._paramInfo = None
         self.statement = None
         self.statementFeatureOption = Feature.optionNone
         self._statement_id = None
         self._sqlcode = None
         self._current_wire = None
         self._result_set = []
@@ -1722,23 +1863,23 @@
         super().executemany(operation, seq_of_params)
         self._rowcount = 0
         for i in range(len(self.params)):
             self._rowcount += self._in_message.wire._get()
         return self._rowcount
 
     def scroll(self, value, mode):
-        if mode == None or mode == '':
-            mode = 'relative'
+        if mode == None or mode == "":
+            mode = "relative"
         mode = mode.lower()
-        if mode != 'absolute' and mode != 'relative':
+        if mode != "absolute" and mode != "relative":
             raise ValueError("This mode is not supported - use 'relative' or 'absolute'.")
 
         # Backward Scrolling
         if value < 0:
-            if mode == 'relative':
+            if mode == "relative":
                 self._rownumber = self._cursor_ptr + value - 1
             else:
                 raise ValueError("Negative values with absolute scrolling are not allowed.")
             self._cursor_ptr = self._rownumber + 1
             if self._rs_index == 0:
                 return self._warehouse[self._rownumber]
             else:
@@ -1749,21 +1890,21 @@
                         rows_available = self._last_row_in_warehouse_dict
                     else:
                         rows_available = self._last_row_in_warehouse_dict + len(self._warehouse)
                     if self._rownumber <= rows_available:
                         return self._warehouse[self._rownumber - self._last_row_in_warehouse_dict - 1]
         # Forward Scrolling
         else:
-            if mode == 'absolute':
+            if mode == "absolute":
                 self._cursor_ptr = 0
             self._scroll_flag = True
             self._rownumber = self._cursor_ptr + value - 1
             if self._rs_index == 0:
                 if self._rownumber >= len(self._warehouse):
-                    if mode == 'absolute':
+                    if mode == "absolute":
                         self._cursor_ptr = len(self._warehouse)
                     return self.fetchone()
                 else:
                     self._scroll_flag = False
                     self._cursor_ptr = self._rownumber + 1
                     return self._warehouse[self._rownumber]
             else:
@@ -1777,15 +1918,15 @@
                     else:
                         rows_available = self._last_row_in_warehouse_dict + len(self._warehouse)
                     if self._rownumber <= rows_available:
                         self._scroll_flag = False
                         self._cursor_ptr = self._rownumber + 1
                         return self._warehouse[self._rownumber - self._last_row_in_warehouse_dict - 1]
                     else:
-                        if mode == 'absolute':
+                        if mode == "absolute":
                             self._cursor_ptr = rows_available + 1
                         return self.fetchone()
 
     def _retrieve_from_warehouse(self, value):
         for idx, (key, val) in enumerate(self._warehouse_dict.items()):
             if value <= key:
                 if idx != 0:
@@ -1793,15 +1934,17 @@
                     return val[value - prev_key - 1]
                 return val[value]
 
     def _switch_buffer(self):
         if self._sqlcode == 0:
             with self._connection._lock:
                 self._out_message.wire._write_header(_Message.FETCH_DATA)
-                intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
+                intersystems_iris._MessageHeader._MessageHeader._set_statement_id(
+                    self._out_message.wire.buffer, self._statement_id
+                )
 
                 sequence_number = self._connection._get_new_sequence_number()
                 self._out_message._send(sequence_number)
 
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 self._sqlcode = self._in_message.wire.header._get_function_code()
                 self._process_sqlcode(self._sqlcode)
@@ -1827,15 +1970,15 @@
 
     def fetchone_helper(self):
         row_indexing = True
         if self.statementFeatureOption & Feature.optionFastSelect == Feature.optionFastSelect:
             list_item = self._current_wire.list_item
             buffer = list_item.buffer
             length = list_item.list_buffer_end
-                
+
             if self._rsrow._new_buffer:
                 prev_offset = list_item.next_offset
                 self._rsrow._new_buffer = False
             else:
                 prev_offset = self._rsrow._offsets._length
 
             if prev_offset < length:
@@ -1844,18 +1987,18 @@
                 else:
                     if self._rsrow._new_buffer:
                         list_item.buffer = buffer
                     list_item.next_offset = prev_offset
                 intersystems_iris._DBList._DBList._get_list_element(list_item)
                 length = list_item.next_offset
                 prev_offset = list_item.data_offset
-                if list_item.data_length == 0: #
+                if list_item.data_length == 0:  #
                     for j in range(self._rsrow.colCount):
                         rowItems[j] = -1
-                    self._rsrow._offsets = self._rsrow.update(rowItems) # ???
+                    self._rsrow._offsets = self._rsrow.update(rowItems)  # ???
                     return True
             else:
                 if self._rsrow.rowItems != None:
                     self._rsrow.rowItems[-1] = 0
                 return False
 
             self._rsrow._last_list_item = list_item
@@ -1874,18 +2017,20 @@
                 return
 
             if self._rsrow.rowItems[-1] >= self._current_wire.list_item.list_buffer_end:
                 self._switch_buffer()
 
         self._cursor_ptr += 1
         return row_indexing
-            
+
     def fetchone(self):
         if self._result_set == None:
-            raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
+            raise InterfaceError(
+                "Either execute has not yet been called, or the previous call of execute did not return a result set"
+            )
 
         if self._current_wire == None and self._cursor_ptr > self._last_row_in_warehouse_dict:
             return None
 
         retval = None
         if self._rs_index == 0:
             if self._cursor_ptr < len(self._warehouse):
@@ -1916,17 +2061,19 @@
                     retval = self._rsrow._offsets
 
         if retval is None:
             return retval
         return retval.as_tuple()
         # return tuple(retval[:])
 
-    def fetchmany(self, size = None):
+    def fetchmany(self, size=None):
         if self._result_set == None:
-            raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
+            raise InterfaceError(
+                "Either execute has not yet been called, or the previous call of execute did not return a result set"
+            )
 
         if self._current_wire == None:
             if self._cursor_ptr > self._last_row_in_warehouse_dict:
                 return []
             if size is None:
                 size = self.arraysize
             if self._rs_index == 0:
@@ -1946,30 +2093,32 @@
                     row = self._retrieve_from_warehouse(self._cursor_ptr)
                     rows.append(row[:])
                     if self._cursor_ptr + 1 > self._last_row_in_warehouse_dict:
                         self._cursor_ptr += 1
                         break
                     self._cursor_ptr += 1
                 return rows
-        
+
         if size is None:
             size = self.arraysize
 
         rows = []
         for i in range(size):
             row = self.fetchone()
             if row is None:
                 break
             rows.append(row)
         return rows
 
     def fetchall(self):
         if self._result_set == None:
-            raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
-        
+            raise InterfaceError(
+                "Either execute has not yet been called, or the previous call of execute did not return a result set"
+            )
+
         if self._current_wire == None:
             if self._cursor_ptr > self._last_row_in_warehouse_dict:
                 return []
             if self._rs_index == 0:
                 if self._cursor_ptr < len(self._warehouse):
                     rows = []
                     while 1:
@@ -1986,58 +2135,60 @@
                     row = self._retrieve_from_warehouse(self._cursor_ptr)
                     rows.append(row[:])
                     if self._cursor_ptr + 1 > self._last_row_in_warehouse_dict:
                         self._cursor_ptr += 1
                         break
                     self._cursor_ptr += 1
                 return rows
-        
+
         rows = []
         while self._current_wire is not None:
             row = self.fetchone()
-            if not row: break
+            if not row:
+                break
             rows.append(row)
-        
+
         return rows
 
+
 class EmbdeddedCursor(_BaseCursor):
     embedded = True
     _result_set = None
 
     def __init__(self, connection: _IRISEmbedded) -> None:
         super().__init__(connection)
         self._sql = connection.iris.sql
         self._iris = connection.iris
         self._closed = False
-        
+
         # $System.SQL.SetSelectMode(1 /* ODBC */)
         # $System.SQL.Util.SetOption("SelectMode", 1 /* ODBC */)
         connection.iris.system.SQL.SetSelectMode(1)
 
     def _get_cached_info(self):
         return False
 
-    def _get_parameters(self, params_set = 0):
+    def _get_parameters(self, params_set=0):
         params = self._params.collect(params_set)
         # None = '', '' = b'\x00'
         _conv = {
-            type(None): lambda v: '',
-            str: lambda v: v or b'\x00',
+            type(None): lambda v: "",
+            str: lambda v: v or b"\x00",
             decimal.Decimal: lambda v: float(v),
         }
         params = [_conv[type(v)](v) if type(v) in _conv else v for v in params]
         return params
 
     def _get_column_info(self):
         self._columns = []
         if self._result_set is None:
             return
-        
+
         metadata = self._result_set.ResultSet._GetMetadata()
-        count = metadata.columnCount if metadata != '' and metadata is not None else 0
+        count = metadata.columnCount if metadata != "" and metadata is not None else 0
         for i in range(count):
             slotPosition = i + 1
             _column_info = metadata.columns.GetAt(slotPosition)
             name = _column_info.colName
             odbctype = _column_info.ODBCType
             if _column_info.scale in SQLType.__members__:
                 # There is a bug on IRIS side, when it may return incorrectly when it passed that way NUMERIC(?, ?)
@@ -2061,15 +2212,29 @@
                 _column_info.isAliased,
                 _column_info.isExpression,
                 _column_info.isHidden,
                 _column_info.isIdentity,
                 _column_info.isKeyColumn,
                 _column_info.isRowId,
             ]
-            self._columns.append(intersystems_iris.dbapi._Column._Column(name, odbctype, precision, scale, nullable, label, tableName, schema, catalog, additionalData, slotPosition))
+            self._columns.append(
+                intersystems_iris.dbapi._Column._Column(
+                    name,
+                    odbctype,
+                    precision,
+                    scale,
+                    nullable,
+                    label,
+                    tableName,
+                    schema,
+                    catalog,
+                    additionalData,
+                    slotPosition,
+                )
+            )
 
     @property
     def lastrowid(self):
         return self._lastrowid
 
     def _prepare_new(self):
         statement = self._parsed_statement
@@ -2151,16 +2316,16 @@
                 message = ex.message
             self._process_sqlcode(sqlcode, message)
 
     def _send_direct_stored_procedure_request(self):
         sqlproc = self._parsed_statement
         self._rowcount = 0
         params = self._get_parameters()
-        params_marks = ', '.join(['?'] * len(params))
-        statement = f'CALL {sqlproc} ({params_marks})'
+        params_marks = ", ".join(["?"] * len(params))
+        statement = f"CALL {sqlproc} ({params_marks})"
 
         sqlcode = 0
         message = None
         try:
             self._result_set = self._sql.exec(statement, *params)
             self._rowcount = self._result_set.ResultSet._ROWCOUNT
             self._get_column_info()
@@ -2168,75 +2333,85 @@
             sqlcode = ex.sqlcode
             message = ex.message
         self._process_sqlcode(sqlcode, message)
 
     @property
     def rowcount(self):
         return self._rowcount
-        
+
     def fetchone(self):
         if self._result_set == None:
-            raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
-        
+            raise InterfaceError(
+                "Either execute has not yet been called, or the previous call of execute did not return a result set"
+            )
+
         try:
             values = self._result_set.__next__()
         except:
             return None
 
-        values = [None if v == '' else '' if v == '\x00' else v for v in values]
-        row = namedtuple('Row', [col.name for col in self._columns], rename=True)
+        values = [None if v == "" else "" if v == "\x00" else v for v in values]
+        row = namedtuple("Row", [col.name for col in self._columns], rename=True)
 
         _types = {
             SQLType.BIGINT: int,
             SQLType.BINARY: bytes,
             SQLType.BIT: bool,
+            SQLType.FLOAT: float,
+            SQLType.NUMERIC: decimal.Decimal,
             SQLType.INTEGER: int,
             SQLType.VARCHAR: str,
             SQLType.LONGVARBINARY: IRISBinaryStream,
             SQLType.LONGVARCHAR: IRISStream,
         }
-        
+
         if self._columns:
             for _column in self._columns:
                 value = values[_column.slotPosition - 1]
 
                 ctype = _column.type
                 value_type = _types[ctype] if ctype in _types else None
                 try:
-                    if type(value) == float:
-                        value = decimal.Decimal(str(value))
-                    elif not _column.tableName and not _column.schema:
-                        pass
+                    if not _column.tableName and not _column.schema:
+                        if type(value) == float:
+                            value = decimal.Decimal(str(value))
                     elif value is None or value_type is None:
                         pass
+                    elif value_type is decimal.Decimal:
+                        value = decimal.Decimal(str(value))
                     elif issubclass(value_type, IRISStream):
                         stream = value_type(self._connection, value, embedded=True)
                         value = stream.fetch()
                     elif not isinstance(value, value_type):
                         value = value_type(value)
                 except Exception as ex:
                     raise ex
                     pass
                 values[_column.slotPosition - 1] = value
         return row(*values)
 
     def fetchall(self):
         if self._result_set == None:
-            raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
+            raise InterfaceError(
+                "Either execute has not yet been called, or the previous call of execute did not return a result set"
+            )
 
         rows = []
         while True:
             row = self.fetchone()
-            if not row: break
+            if not row:
+                break
             rows.append(row)
         return rows
-    
-    def fetchmany(self, size = None):
+
+    def fetchmany(self, size=None):
         if self._result_set == None:
-            raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
+            raise InterfaceError(
+                "Either execute has not yet been called, or the previous call of execute did not return a result set"
+            )
 
         if size is None:
             size = self.arraysize
 
         rows = []
         for i in range(size):
             row = self.fetchone()
@@ -2249,65 +2424,81 @@
         raise NotImplementedErrorDBAPI()
 
 
 # Type Objects
 def Date(year, month, day):
     raise NotImplementedErrorDBAPI()
 
+
 def Time(hour, minutes, second):
     raise NotImplementedErrorDBAPI()
 
+
 def Timestamp(year, month, day, hour, minute, second):
     raise NotImplementedErrorDBAPI()
 
+
 def DateFromTicks(ticks):
     raise NotImplementedErrorDBAPI()
 
+
 def TimeFromTicks(ticks):
     raise NotImplementedErrorDBAPI()
 
+
 def TimestampFromTicks(ticks):
     raise NotImplementedErrorDBAPI()
 
+
 # def Binary(string):
 #     return string
 
 # Type definitions.
 Binary = bytes
 
 STRING = str
 BINARY = bytes
 NUMBER = float
 ROWID = str
 
 # still needs type singletons (?)
 
+
 # Exception architecture
 class Error(Exception):
     pass
 
+
 class Warning(Exception):
-     pass
+    pass
+
 
 class InterfaceError(Error):
     pass
 
+
 class DatabaseError(Error):
     pass
 
+
 class InternalError(DatabaseError):
     pass
 
+
 class OperationalError(DatabaseError):
     pass
 
+
 class ProgrammingError(DatabaseError):
     pass
 
+
 class IntegrityError(DatabaseError):
     pass
 
+
 class DataError(DatabaseError):
     pass
 
+
 class NotSupportedError(DatabaseError):
     pass
```

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/_Descriptor.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/_Descriptor.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/_IRISStream.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/_IRISStream.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/_Message.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/_Message.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/_Parameter.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/_Parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,21 +83,16 @@
             int: lambda v : v,
             float: lambda v : v,
             decimal.Decimal: lambda v : v,
         }
         func = _set_switcher[type(self.__value)] if type(self.__value) in _set_switcher else (lambda v : str(v))
         value = func(self.__value)
         if self.mode == ParameterMode.REPLACED_LITERAL:
-            try:
+            if isinstance(value, str) and value.isdigit():
                 value = int(value)
-            except:
-                try:
-                    value = float(value)
-                except:
-                    pass
         return value
 
     def _copy_cached_info(self, desc, copy_replaced):
         self.type = desc.type
         self.precision = desc.precision
         self.scale = desc.scale
         self.nullable = desc.nullable
```

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/_ParameterCollection.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/_ParameterCollection.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/_ResultSetRow.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/_ResultSetRow.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/_SQLType.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/_SQLType.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/preparser/_PreParser.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/preparser/_PreParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,23 @@
 import intersystems_iris.dbapi.preparser._Token
 import intersystems_iris.dbapi.preparser._TokenList
 import intersystems_iris.dbapi.preparser._Scanner
 from intersystems_iris.dbapi._Parameter import ParameterMode
 from intersystems_iris.dbapi.preparser._Token import TOKEN
 from intersystems_iris.dbapi.preparser._Scanner import ParseToken
 
+class MultiValuesInsert(Exception):
+
+    def __init__(self, *args: object, query: str, rows: int, params=None) -> None:
+        super().__init__(*args)
+        self.query = query
+        self.rows = rows
+        self.params = params
+    
+
 # May want to move to its own file eventually
 # SQL Statement Types
 class StatementType(enum.IntEnum):
     UPDATE = 0
     QUERY = 1
     CALL = 2
     SYNC_COMMIT = 3
@@ -540,56 +549,56 @@
             new_query += _query(False)
             
             return found, new_query
         except:
             return False, query
         
     def InsertMultiValues(self, query):
-        try:
-            new_query = ''
-            values_list = []
-
-            tokens = self.m_Tokens.GetEnumerator()
-            while tokens.MoveNext() and not tokens.Current().UpperEquals("INSERT"):
-                new_query += tokens.Current().Lexeme + ' '
-            if not tokens.MoveNext() or not tokens.Current().UpperEquals("INTO"):
-                return False, query
-            new_query += 'INSERT INTO '
-            while tokens.MoveNext() and not tokens.Current().UpperEquals("VALUES"):
-                new_query += tokens.Current().Lexeme + ' '
+        new_query = ''
+        values_list = []
 
-            values = ''
-            while tokens.MoveNext():
-                assert tokens.Current().TokenType is TOKEN.OPEN_PAREN
-                open_parens = 1
-                while tokens.MoveNext() or open_parens > 0:
-                    token = tokens.Current()
-                    if token.TokenType is TOKEN.OPEN_PAREN:
-                        open_parens += 1
-                    elif token.TokenType is TOKEN.CLOSE_PAREN:
-                        open_parens -= 1
-                    if open_parens == 0:
-                        break
-                    values += token.Lexeme
-                    values += ' '
-                values_list.append(values)
-                values = ''
-                if not tokens.MoveNext() or tokens.Current().TokenType is not TOKEN.COMMA:
+        tokens = self.m_Tokens.GetEnumerator()
+        while tokens.MoveNext() and not tokens.Current().UpperEquals("INSERT"):
+            new_query += tokens.Current().Lexeme + ' '
+        if not tokens.MoveNext() or not tokens.Current().UpperEquals("INTO"):
+            return False, query
+        new_query += 'INSERT INTO '
+        while tokens.MoveNext() and not tokens.Current().UpperEquals("VALUES"):
+            new_query += tokens.Current().Lexeme + ' '
+
+        values = ''
+        params = []
+        while tokens.MoveNext():
+            assert tokens.Current().TokenType is TOKEN.OPEN_PAREN
+            open_parens = 1
+            while tokens.MoveNext() or open_parens > 0:
+                token = tokens.Current()
+                if token.TokenType is TOKEN.OPEN_PAREN:
+                    open_parens += 1
+                elif token.TokenType is TOKEN.CLOSE_PAREN:
+                    open_parens -= 1
+                if open_parens == 0:
                     break
-            
-            if len(values_list) <= 1:
-                return False, query
-
-            new_query += ' SELECT '
-            new_query += ' UNION ALL SELECT '.join(values_list)
-
-            return True, new_query
-        except:
+                if token.TokenType is TOKEN.CONSTANT:
+                    values += '?'
+                    params += [token.Lexeme] 
+                else:    
+                    values += token.Lexeme
+                values += ' '
+            values_list.append(values)
+            values = ''
+            if not tokens.MoveNext() or tokens.Current().TokenType is not TOKEN.COMMA:
+                break
+        
+        if len(values_list) <= 1:
             return False, query
 
+        new_query += f" VALUES ({values_list[0]})"
+        raise MultiValuesInsert(query=new_query, rows=len(values_list), params=params)
+
     #  Parse a statement
     def Tokenize(self, p_strInput):
         #  Get a scanner on the sql string
         self.m_Scanner = intersystems_iris.dbapi.preparser._Scanner._Scanner(p_strInput)
         #  Create a new token list
         self.m_Tokens = intersystems_iris.dbapi.preparser._TokenList._TokenList()
         #  Scan the input string and break into tokens
```

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/preparser/_Scanner.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/preparser/_Scanner.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/preparser/_Token.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/preparser/_Token.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/dbapi/preparser/_TokenList.py` & `django-iris-0.2.2b1/intersystems_iris/dbapi/preparser/_TokenList.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/pex/_BusinessHost.py` & `django-iris-0.2.2b1/intersystems_iris/pex/_BusinessHost.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/pex/_BusinessOperation.py` & `django-iris-0.2.2b1/intersystems_iris/pex/_BusinessOperation.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/pex/_BusinessProcess.py` & `django-iris-0.2.2b1/intersystems_iris/pex/_BusinessProcess.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/pex/_BusinessService.py` & `django-iris-0.2.2b1/intersystems_iris/pex/_BusinessService.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/pex/_Common.py` & `django-iris-0.2.2b1/intersystems_iris/pex/_Common.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/pex/_Director.py` & `django-iris-0.2.2b1/intersystems_iris/pex/_Director.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/pex/_IRISBusinessService.py` & `django-iris-0.2.2b1/intersystems_iris/pex/_IRISBusinessService.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/pex/_IRISOutboundAdapter.py` & `django-iris-0.2.2b1/intersystems_iris/pex/_IRISOutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/pex/_InboundAdapter.py` & `django-iris-0.2.2b1/intersystems_iris/pex/_InboundAdapter.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/pex/_OutboundAdapter.py` & `django-iris-0.2.2b1/intersystems_iris/pex/_OutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/intersystems_iris/pex/__init__.py` & `django-iris-0.2.2b1/intersystems_iris/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/irisnative/_IRISNative.py` & `django-iris-0.2.2b1/irisnative/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.1b3/setup.cfg` & `django-iris-0.2.2b1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-iris
-version = 0.2.1b3
+version = 0.2.2b1
 url = https://github.com/caretdev/django-iris
 maintainer = CaretDev
 maintainer_email = dmitry@caretdev.com
 license = MIT
 description = Django backend for InterSystems IRIS
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `django-iris-0.2.1b3/setup.py` & `django-iris-0.2.2b1/setup.py`

 * *Files identical despite different names*

