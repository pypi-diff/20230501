# Comparing `tmp/dbus-client-gen-0.5.tar.gz` & `tmp/dbus-client-gen-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbus-client-gen-0.5.tar", last modified: Tue Dec  8 15:42:46 2020, max compression
+gzip compressed data, was "dbus-client-gen-0.5.1.tar", last modified: Mon May  1 19:11:52 2023, max compression
```

## Comparing `dbus-client-gen-0.5.tar` & `dbus-client-gen-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-08 15:42:46.000000 dbus-client-gen-0.5/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4721 2020-12-08 15:42:46.000000 dbus-client-gen-0.5/PKG-INFO
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3253 2020-08-10 16:44:40.000000 dbus-client-gen-0.5/README.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       38 2020-12-08 15:42:46.000000 dbus-client-gen-0.5/setup.cfg
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1512 2020-10-28 21:05:55.000000 dbus-client-gen-0.5/setup.py
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-08 15:42:46.000000 dbus-client-gen-0.5/src/
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-08 15:42:46.000000 dbus-client-gen-0.5/src/dbus_client_gen/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      690 2020-08-08 01:05:20.000000 dbus-client-gen-0.5/src/dbus_client_gen/__init__.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4619 2020-10-28 21:05:55.000000 dbus-client-gen-0.5/src/dbus_client_gen/_errors.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4480 2020-08-10 16:44:40.000000 dbus-client-gen-0.5/src/dbus_client_gen/_managed_objects.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5536 2020-08-10 16:44:40.000000 dbus-client-gen-0.5/src/dbus_client_gen/_managed_objects_queries.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      314 2020-12-08 15:31:18.000000 dbus-client-gen-0.5/src/dbus_client_gen/_version.py
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2020-12-08 15:42:46.000000 dbus-client-gen-0.5/src/dbus_client_gen.egg-info/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4721 2020-12-08 15:42:46.000000 dbus-client-gen-0.5/src/dbus_client_gen.egg-info/PKG-INFO
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      384 2020-12-08 15:42:46.000000 dbus-client-gen-0.5/src/dbus_client_gen.egg-info/SOURCES.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        1 2020-12-08 15:42:46.000000 dbus-client-gen-0.5/src/dbus_client_gen.egg-info/dependency_links.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       16 2020-12-08 15:42:46.000000 dbus-client-gen-0.5/src/dbus_client_gen.egg-info/top_level.txt
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-01 19:11:52.023308 dbus-client-gen-0.5.1/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)    16726 2021-06-03 20:53:05.000000 dbus-client-gen-0.5.1/LICENSE
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)     4081 2023-05-01 19:11:52.023308 dbus-client-gen-0.5.1/PKG-INFO
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     3253 2021-06-03 20:53:05.000000 dbus-client-gen-0.5.1/README.rst
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)       81 2023-05-01 02:55:36.000000 dbus-client-gen-0.5.1/pyproject.toml
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      899 2023-05-01 19:11:52.024308 dbus-client-gen-0.5.1/setup.cfg
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      105 2023-05-01 02:55:36.000000 dbus-client-gen-0.5.1/setup.py
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-01 19:11:52.021308 dbus-client-gen-0.5.1/src/
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-01 19:11:52.023308 dbus-client-gen-0.5.1/src/dbus_client_gen/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      724 2023-05-01 17:16:26.000000 dbus-client-gen-0.5.1/src/dbus_client_gen/__init__.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     4619 2021-06-03 20:53:05.000000 dbus-client-gen-0.5.1/src/dbus_client_gen/_errors.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     4480 2023-05-01 17:13:22.000000 dbus-client-gen-0.5.1/src/dbus_client_gen/_managed_objects.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     5552 2022-05-25 04:03:29.000000 dbus-client-gen-0.5.1/src/dbus_client_gen/_managed_objects_queries.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)      316 2023-05-01 19:01:59.000000 dbus-client-gen-0.5.1/src/dbus_client_gen/_version.py
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-01 19:11:52.023308 dbus-client-gen-0.5.1/src/dbus_client_gen.egg-info/
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)     4081 2023-05-01 19:11:52.000000 dbus-client-gen-0.5.1/src/dbus_client_gen.egg-info/PKG-INFO
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)      460 2023-05-01 19:11:52.000000 dbus-client-gen-0.5.1/src/dbus_client_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)        1 2023-05-01 19:11:52.000000 dbus-client-gen-0.5.1/src/dbus_client_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 mulhern   (1000) mulhern   (1000)       16 2023-05-01 19:11:52.000000 dbus-client-gen-0.5.1/src/dbus_client_gen.egg-info/top_level.txt
+drwxr-xr-x   0 mulhern   (1000) mulhern   (1000)        0 2023-05-01 19:11:52.023308 dbus-client-gen-0.5.1/tests/
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     1929 2023-05-01 18:56:16.000000 dbus-client-gen-0.5.1/tests/test_deterministic.py
+-rw-rw----   0 mulhern   (1000) mulhern   (1000)     4400 2021-08-27 18:10:36.000000 dbus-client-gen-0.5.1/tests/test_hypothesis.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dbus-client-gen-0.5/PKG-INFO` & `dbus-client-gen-0.5.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,101 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dbus-client-gen
-Version: 0.5
+Version: 0.5.1
 Summary: generates classes and methods useful to a D-Bus client
 Home-page: https://github.com/mulkieran/dbus-client-gen
 Author: Anne Mulhern
 Author-email: amulhern@redhat.com
-License: MPL 2.0
-Description: A Python Library for Generating D-Bus Client Code
-        =================================================
-        
-        Introduction
-        ------------
-        This library contains a few methods that consume an XML specification of
-        a D-Bus interface and return classes or functions that may be useful in
-        constructing a python D-Bus client. The XML specification has the
-        format of the data returned by the Introspect() method of the Introspectable
-        interface.
-        
-        Methods
-        -------
-        
-        managed_object_class
-        ^^^^^^^^^^^^^^^^^^^^
-          This function consumes the spec for a single interface and returns a class
-          which constructs objects which wrap the table for a particular object in the
-          format returned by the GetManagedObjects() method of the ObjectManager
-          interface. Each object has an instance method for each property of the
-          interface.
-        
-        mo_query_builder
-        ^^^^^^^^^^^^^^^^^
-          This function consumes the spec for a single interface and returns a function
-          which implements a query on the whole object returned by a GetManagedObjects()
-          call. The query function takes two arguments: the GetManagedObjects() object
-          and a dict of key/value pairs. The query function generates pairs of the
-          object path and corresponding table which match all the key/value pairs in
-          the table.
-        
-        
-        Errors
-        ------
-        This library exports the exception type  DbusClientError and all its subtypes.
-        It constitutes a bug if an error of any other type is propagated during class
-        generation or when the methods of the class are executed.
-        
-        The following shows the error heirarchy. Entries after the dash indicate
-        additional fields beyond the message which the exception contains. Only leaves
-        of the error class heirarchy are constructed directly.
-        
-        
-        DbusClientError
-        
-            * DbusClientGenerationError
-              This exception is raised if an error occurs while generating a method.
-              Such an exception would result from introspection data which lacked the
-              necessary attributes or entries.
-        
-            * DbusClientRuntimeError - interface name
-              This exception is raised if there is an error while the generated method
-              is executing.
-        
-                - DbusClientMissingInterfaceError
-                  This exception is raisded if when constructing a managed object it
-                  turns out that its argument does not have an entry for the
-                  expected interface.
-        
-                - DbusClientMissingPropertyError - property name
-                  This exception is raised if when reading a value for a managed
-                  object it turns out that the value corresponding to that property
-                  is not available.
-        
-                - DbusClientMissingSearchPropertiesError - too many fields to list here
-                  This exception is raised if when traversing a GetManagedObjects()
-                  result the keys used by the query have no corresponding values in the
-                  result.
-        
-                - DbusClientUnknownSearchPropertiesError -- too many fields to list here
-                  This exception is raised if the search properties specified can not
-                  be found in the specified interface.
-        
-        
-        Packaging
-        ---------
-        Downstream packagers, if incorporating testing into their packaging, are
-        encouraged to use only the tests in the test_deterministic.py module, to
-        avoid testing failures that may arise due to the non-deterministic behavior
-        of Hypothesis tests.
-        
+License: MPL-2.0
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+A Python Library for Generating D-Bus Client Code
+=================================================
+
+Introduction
+------------
+This library contains a few methods that consume an XML specification of
+a D-Bus interface and return classes or functions that may be useful in
+constructing a python D-Bus client. The XML specification has the
+format of the data returned by the Introspect() method of the Introspectable
+interface.
+
+Methods
+-------
+
+managed_object_class
+^^^^^^^^^^^^^^^^^^^^
+  This function consumes the spec for a single interface and returns a class
+  which constructs objects which wrap the table for a particular object in the
+  format returned by the GetManagedObjects() method of the ObjectManager
+  interface. Each object has an instance method for each property of the
+  interface.
+
+mo_query_builder
+^^^^^^^^^^^^^^^^^
+  This function consumes the spec for a single interface and returns a function
+  which implements a query on the whole object returned by a GetManagedObjects()
+  call. The query function takes two arguments: the GetManagedObjects() object
+  and a dict of key/value pairs. The query function generates pairs of the
+  object path and corresponding table which match all the key/value pairs in
+  the table.
+
+
+Errors
+------
+This library exports the exception type  DbusClientError and all its subtypes.
+It constitutes a bug if an error of any other type is propagated during class
+generation or when the methods of the class are executed.
+
+The following shows the error heirarchy. Entries after the dash indicate
+additional fields beyond the message which the exception contains. Only leaves
+of the error class heirarchy are constructed directly.
+
+
+DbusClientError
+
+    * DbusClientGenerationError
+      This exception is raised if an error occurs while generating a method.
+      Such an exception would result from introspection data which lacked the
+      necessary attributes or entries.
+
+    * DbusClientRuntimeError - interface name
+      This exception is raised if there is an error while the generated method
+      is executing.
+
+        - DbusClientMissingInterfaceError
+          This exception is raisded if when constructing a managed object it
+          turns out that its argument does not have an entry for the
+          expected interface.
+
+        - DbusClientMissingPropertyError - property name
+          This exception is raised if when reading a value for a managed
+          object it turns out that the value corresponding to that property
+          is not available.
+
+        - DbusClientMissingSearchPropertiesError - too many fields to list here
+          This exception is raised if when traversing a GetManagedObjects()
+          result the keys used by the query have no corresponding values in the
+          result.
+
+        - DbusClientUnknownSearchPropertiesError -- too many fields to list here
+          This exception is raised if the search properties specified can not
+          be found in the specified interface.
+
+
+Packaging
+---------
+Downstream packagers, if incorporating testing into their packaging, are
+encouraged to use only the tests in the test_deterministic.py module, to
+avoid testing failures that may arise due to the non-deterministic behavior
+of Hypothesis tests.
```

### Comparing `dbus-client-gen-0.5/README.rst` & `dbus-client-gen-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `dbus-client-gen-0.5/src/dbus_client_gen/__init__.py` & `dbus-client-gen-0.5.1/src/dbus_client_gen/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,7 +14,8 @@
     DbusClientRuntimeError,
     DbusClientSearchConditionError,
     DbusClientUniqueResultError,
     DbusClientUnknownSearchPropertiesError,
 )
 from ._managed_objects import managed_object_class
 from ._managed_objects_queries import GMOQuery, mo_query_builder
+from ._version import __version__
```

### Comparing `dbus-client-gen-0.5/src/dbus_client_gen/_errors.py` & `dbus-client-gen-0.5.1/src/dbus_client_gen/_errors.py`

 * *Files identical despite different names*

### Comparing `dbus-client-gen-0.5/src/dbus_client_gen/_managed_objects.py` & `dbus-client-gen-0.5.1/src/dbus_client_gen/_managed_objects.py`

 * *Files identical despite different names*

### Comparing `dbus-client-gen-0.5/src/dbus_client_gen/_managed_objects_queries.py` & `dbus-client-gen-0.5.1/src/dbus_client_gen/_managed_objects_queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,16 +87,17 @@
             if self._filter_func(data)
         )
 
         if self._require_unique:
             list_result = list(result)
             if len(list_result) != 1:
                 raise DbusClientUniqueResultError(
-                    "No unique match found for interface %s and properties %s, found %s"
-                    % (self._interface_name, self._props, list_result),
+                    f"No unique match found for interface "
+                    f"{self._interface_name} and properties {self._props}, "
+                    f"found {list_result}",
                     self._interface_name,
                     self._props,
                     list_result,
                 )
             result = (x for x in list_result)
 
         return result
@@ -136,15 +137,15 @@
 
         :param props: a specification of properties to restrict values
         :type props: dict of str * object or NoneType
         :returns: an appropriately constructed GMOQuery object
         :rtype: GMOQuery
 
         """
-        props = dict() if props is None else props
+        props = {} if props is None else props
 
         if not frozenset(props.keys()) <= property_names:
             fmt_str = (
                 "These properties in the specified query are unknown to "
                 'interface "%s": %s'
             )
             unknown_properties = ", ".join(
```

### Comparing `dbus-client-gen-0.5/src/dbus_client_gen.egg-info/PKG-INFO` & `dbus-client-gen-0.5.1/src/dbus_client_gen.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,101 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dbus-client-gen
-Version: 0.5
+Version: 0.5.1
 Summary: generates classes and methods useful to a D-Bus client
 Home-page: https://github.com/mulkieran/dbus-client-gen
 Author: Anne Mulhern
 Author-email: amulhern@redhat.com
-License: MPL 2.0
-Description: A Python Library for Generating D-Bus Client Code
-        =================================================
-        
-        Introduction
-        ------------
-        This library contains a few methods that consume an XML specification of
-        a D-Bus interface and return classes or functions that may be useful in
-        constructing a python D-Bus client. The XML specification has the
-        format of the data returned by the Introspect() method of the Introspectable
-        interface.
-        
-        Methods
-        -------
-        
-        managed_object_class
-        ^^^^^^^^^^^^^^^^^^^^
-          This function consumes the spec for a single interface and returns a class
-          which constructs objects which wrap the table for a particular object in the
-          format returned by the GetManagedObjects() method of the ObjectManager
-          interface. Each object has an instance method for each property of the
-          interface.
-        
-        mo_query_builder
-        ^^^^^^^^^^^^^^^^^
-          This function consumes the spec for a single interface and returns a function
-          which implements a query on the whole object returned by a GetManagedObjects()
-          call. The query function takes two arguments: the GetManagedObjects() object
-          and a dict of key/value pairs. The query function generates pairs of the
-          object path and corresponding table which match all the key/value pairs in
-          the table.
-        
-        
-        Errors
-        ------
-        This library exports the exception type  DbusClientError and all its subtypes.
-        It constitutes a bug if an error of any other type is propagated during class
-        generation or when the methods of the class are executed.
-        
-        The following shows the error heirarchy. Entries after the dash indicate
-        additional fields beyond the message which the exception contains. Only leaves
-        of the error class heirarchy are constructed directly.
-        
-        
-        DbusClientError
-        
-            * DbusClientGenerationError
-              This exception is raised if an error occurs while generating a method.
-              Such an exception would result from introspection data which lacked the
-              necessary attributes or entries.
-        
-            * DbusClientRuntimeError - interface name
-              This exception is raised if there is an error while the generated method
-              is executing.
-        
-                - DbusClientMissingInterfaceError
-                  This exception is raisded if when constructing a managed object it
-                  turns out that its argument does not have an entry for the
-                  expected interface.
-        
-                - DbusClientMissingPropertyError - property name
-                  This exception is raised if when reading a value for a managed
-                  object it turns out that the value corresponding to that property
-                  is not available.
-        
-                - DbusClientMissingSearchPropertiesError - too many fields to list here
-                  This exception is raised if when traversing a GetManagedObjects()
-                  result the keys used by the query have no corresponding values in the
-                  result.
-        
-                - DbusClientUnknownSearchPropertiesError -- too many fields to list here
-                  This exception is raised if the search properties specified can not
-                  be found in the specified interface.
-        
-        
-        Packaging
-        ---------
-        Downstream packagers, if incorporating testing into their packaging, are
-        encouraged to use only the tests in the test_deterministic.py module, to
-        avoid testing failures that may arise due to the non-deterministic behavior
-        of Hypothesis tests.
-        
+License: MPL-2.0
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+A Python Library for Generating D-Bus Client Code
+=================================================
+
+Introduction
+------------
+This library contains a few methods that consume an XML specification of
+a D-Bus interface and return classes or functions that may be useful in
+constructing a python D-Bus client. The XML specification has the
+format of the data returned by the Introspect() method of the Introspectable
+interface.
+
+Methods
+-------
+
+managed_object_class
+^^^^^^^^^^^^^^^^^^^^
+  This function consumes the spec for a single interface and returns a class
+  which constructs objects which wrap the table for a particular object in the
+  format returned by the GetManagedObjects() method of the ObjectManager
+  interface. Each object has an instance method for each property of the
+  interface.
+
+mo_query_builder
+^^^^^^^^^^^^^^^^^
+  This function consumes the spec for a single interface and returns a function
+  which implements a query on the whole object returned by a GetManagedObjects()
+  call. The query function takes two arguments: the GetManagedObjects() object
+  and a dict of key/value pairs. The query function generates pairs of the
+  object path and corresponding table which match all the key/value pairs in
+  the table.
+
+
+Errors
+------
+This library exports the exception type  DbusClientError and all its subtypes.
+It constitutes a bug if an error of any other type is propagated during class
+generation or when the methods of the class are executed.
+
+The following shows the error heirarchy. Entries after the dash indicate
+additional fields beyond the message which the exception contains. Only leaves
+of the error class heirarchy are constructed directly.
+
+
+DbusClientError
+
+    * DbusClientGenerationError
+      This exception is raised if an error occurs while generating a method.
+      Such an exception would result from introspection data which lacked the
+      necessary attributes or entries.
+
+    * DbusClientRuntimeError - interface name
+      This exception is raised if there is an error while the generated method
+      is executing.
+
+        - DbusClientMissingInterfaceError
+          This exception is raisded if when constructing a managed object it
+          turns out that its argument does not have an entry for the
+          expected interface.
+
+        - DbusClientMissingPropertyError - property name
+          This exception is raised if when reading a value for a managed
+          object it turns out that the value corresponding to that property
+          is not available.
+
+        - DbusClientMissingSearchPropertiesError - too many fields to list here
+          This exception is raised if when traversing a GetManagedObjects()
+          result the keys used by the query have no corresponding values in the
+          result.
+
+        - DbusClientUnknownSearchPropertiesError -- too many fields to list here
+          This exception is raised if the search properties specified can not
+          be found in the specified interface.
+
+
+Packaging
+---------
+Downstream packagers, if incorporating testing into their packaging, are
+encouraged to use only the tests in the test_deterministic.py module, to
+avoid testing failures that may arise due to the non-deterministic behavior
+of Hypothesis tests.
```

